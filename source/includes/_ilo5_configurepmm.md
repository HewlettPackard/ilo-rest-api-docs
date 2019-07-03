# HPE Persistent Memory Configuration

Configuration of HPE Persistent Memory featuring Intel Optane persistent memory modules (PMM) uses the Redfish MemoryChunk, MemoryDomain, and TaskService to manage goal configurations. Please note that the HPE RESTful Interface tool v2.5.0 provides commands for inventory and configuration of PMMs. The new HPE Persistent Memory Management Utility provides a graphical experience for managing PMMs. Both tools use the iLO RESTful API, but add a layer of abstraction for the user.

## Concepts and Terms

|Term|Definition|
|---|---|
| Interleave Set | A group of Memory Regions that are interleaved together. Represented by a MemoryChunk in Redfish. |
| Memory Chunk | A Memory Chunk is a group of one or more regions. The chunk represents an interleave set. Memory Domains and Chunks will ONLY be reported for Persistent Regions. Volatile Regions will be treated just like DIMMs with no such data reported. |
| Memory Domain | Memory Domains are used to indicate to the client which Memory (DIMMs) can be grouped together in Memory Chunks to form interleave sets or otherwise grouped together.  Informational only, not configurable. |
| Memory Region | A region is a portion of a DIMM of a specific size and mode. A DIMM can have one or more regions. Regions can be the same or different mode on a DIMM.  |
| Namespace | For PMM, this is a device made available in filesystem (OS) source. |


## Overview

To create a MemoryChunk and Regions required, POST a MemoryChunk to the MemoryChunkCollection in a specific MemoryDomain. In the POST, list the DIMMs that should be included in MemorySet for the MemoryChunk, based on the `InterleavableMemorySets` in the MemoryDomain. All DIMMs on the socket related to the MemoryDomain must be configured in a MemoryChunk in order for the configuration to succeed.

To delete a MemoryChunk, DELETE the MemoryChunk from the MemoryChunkCollection. Deleting a MemoryChunk will result in the corresponding memory region being set to volatile memory.

POST will only be supported for persistent Memory Chunks. Remaining capacity will be configured as volatile. Only persistent Memory Chunks will be reported in the system, since volatile interleaving is not reported for standard DIMMs.

Only one Interleaved MemoryChunk is supported, and that Interleaved MemoryChunk must include all DIMMs on that socket. This matches what is specified in the MemoryDomain's `InterleavableMemorySets`. If several POST requests are issued to configure multiple Interleaved MemoryChunks on a socket, iLO will reject the POST. iLO ensures all CPU installed PMMs are included in the memory set for a POST that is creating an interleaved Memory Chunk. This also checks for duplicate DIMM entries.

#### Memory Population Violations
If the memory population rules are violated, then configuration through the iLO RESTful API is not supported. Configuration may fail or have unexpected results.

### MemoryChunk POST properties
- `AddressRangeType`: required
- `MemoryChunkSizeMiB`: optional, default value is 0. Maximum is the sum total of the CapacityMiB of each Memory in the `InterleaveSets`. Specify this or `MemoryChunkSizePercentage`, but not both. In order to create the PMM goal configuration, sizes will be converted to a percentage. During this conversion, the size may change slightly.
- `IsMirrorEnabled`: optional, default value is false
- `IsSpare`: optional, default is false.
- `InterleaveSets`: required. Must match one of the `InterleavableMemorySets` in the corresponding MemoryDomain.  If `InterleaveSet` is empty, all possible Memory in the Memory Domain will be included in the Memory Chunk by default. BIOS will use best interleaving.
- `Oem.Hpe.MemoryChunkSizePercentage`: optional, default value is 0. Specify this or `MemoryChunkSizeMiB`, but not both. `MemoryChunkSizePercentage` is recommended.

**Note**: The values specified by `MemoryChunkSizeMiB` or `MemoryChunkSizePercentage` must be the same across all POST requests on a given socket (Memory Domain).

#### Example MemoryChunk POST 
The example below is a POST body for creating a MemoryChunk using the `MemoryChunkSizePercentage` property. The PMMs on processor 1 in slots 6 and 7 will be interleaved and provisioned to 50% persistent memory (App Direct) mode. The remaining 50% is set to volatile (memory) mode.

> POST /redfish/v1/Systems/1/MemoryDomains/PROC1MemoryDomain/MemoryChunks/


```json
{ 
    "AddressRangeType": "PMEM",
    "Oem": {
       "Hpe": {
          "MemoryChunkSizePercentage": 50
       }    
    },
    "InterleaveSets": [
       {
          "Memory" : { "@odata.id": "/redfish/v1/Systems/1/Memory/proc1dimm6/"}
       },
       {
          "Memory" : { "@odata.id": "/redfish/v1/Systems/1/Memory/proc1dimm7/"}
       }
    ]
} 
```

## Configuration Tasks
Since the POST and DELETE modifications to the MemoryChunks are applied on system reboot, iLO will create a Task for each request. The Tasks are managed by the TaskService. On success, the POST and DELETE responses will include information about the corresponding Task. All the staged Tasks will be provided to BIOS on reboot. BIOS will process all the Tasks, in order, to create new Goal Configurations for each impacted PMMs. If Goal Configurations cannot be created, then ALL of the Tasks will fail, and the Task status will report the reason for the failure. PATCH to the MemoryChunk is not supported, so reconfiguration of existing configurations must first DELETE the existing MemoryChunks before creating a new configuration.

Example response to a MemoryChunk POST:

> Status: 202 Accepted

```json
{
    "@odata.context": "/redfish/v1/$metadata#Task.Task",
    "@odata.etag": "W/\"D793BCE6\"",
    "@odata.id": "/redfish/v1/TaskService/Tasks/1545/",
    "@odata.type": "#Task.v1_3_0.Task",
    "Id": "1545",
    "Description": "iLO Task",
    "Messages": [
        {}
    ],
    "Name": "Task 1545",
    "Payload": {
        "HttpOperation": "POST",
        "JsonBody": "{\"AddressRangeType\":\"PMEM\",\"InterleaveSets\":[{\"Memory\":{\"@odata.id\":\"/redfish/v1/Systems/1/Memory/proc1dimm6/\"}},{\"Memory\":{\"@odata.id\":\"/redfish/v1/Systems/1/Memory/proc1dimm7/\"}}],\"Oem\":{\"Hpe\":{\"MemoryChunkSizePercentage\":100}}}",
        "TargetUri": "/redfish/v1/Systems/1/MemoryDomains/PROC1MemoryDomain/MemoryChunks/"
    },
    "StartTime": "2019-03-06T16:18:50Z",
    "TaskMonitor": "/redfish/v1/TaskService/TaskMonitors/1545/",
    "TaskState": "New"
}
```

### POST and Task limits
iLO will limit the total number of Tasks to a minimum of 192. 

## Configuration Sequencing
The intent of configuration will only be inferred from the sequence in which the requests are made. As such, any DELETE requests must precede any POST requests relating to MemoryDomains on the same socket. A DELETE request and a POST request may be performed in the same reboot, as long as they follow this rule.

## Example 1: Reconfigure to Change Interleaving

**Start**: Example configuration is two PMMs, A1 and A2, of 16 GiB each on a single socket on the same memory controller. There are two existing MemoryChunks, MC1 and MC2, for 100% persistent memory non-interleaved.

**Goal**: Reconfigure these two PMMs to be 100% persistent memory interleaved.

**Solution**: The client would first issue a DELETE request on MC1 and a separate DELETE request on MC2. This would create two New Tasks in the 
TaskService. The client would then issue a POST request on the MemoryDomain's Memory Chunk Collection. The POST body includes DIMMs A1 and A2 in the corresponding `InterleaveSets` with an 
`Oem.Hpe.MemoryChunkSizePercentage` of 100% or a `MemoryChunkSizeMiB` of 32GiB. This would result in three New Tasks in the TaskService queue to be consumed on 
reboot. See details steps below:

Step 1. Delete MC1

> DELETE `/redfish/v1/Systems/1/MemoryDomains/PROC1MemoryDomain/MemoryChunks/MC1`

Step 2. Delete MC2

> DELETE `/redfish/v1/Systems/1/MemoryDomains/PROC1MemoryDomain/MemoryChunks/MC2`

Step 3. Create new configuration: **Option 1** using MemoryChunkSizePercentage

> POST `/redfish/v1/Systems/1/MemoryDomains/PROC1MemoryDomain/MemoryChunks`

```json
   {
       "AddressRangeType": "PMEM",
       "Oem": {
           "Hpe": {
               "MemoryChunkSizePercentage": 100
           }
       },
       "InterleaveSets": [
          {
               "Memory": {
                   "@odata.id": "/redfish/v1/Systems/1/Memory/A1/"
            }
           },
           {
               "Memory": {
                   "@odata.id": "/redfish/v1/Systems/1/Memory/A2/"
               }
           }
       ]
   }
```

Step 4. Create new configuration: **Option 2** using MemoryChunkSizeMiB

> POST `/redfish/v1/Systems/1/MemoryDomains/PROC1MemoryDomain/MemoryChunks`

```json
   {
       "AddressRangeType": "PMEM",
       "MemoryChunkSizeMiB": 32768,
       "InterleaveSets": [
          {
               "Memory": {
                   "@odata.id": "/redfish/v1/Systems/1/Memory/A1/"
            }
           },
           {
               "Memory": {
                   "@odata.id": "/redfish/v1/Systems/1/Memory/A2/"
               }
           }
       ]
   }
```

Step 5. Reboot system to apply changes staged in iLO as Tasks.

## Example 2: Reconfigure to change Memory Provisioning on Two-Socket System

**Start**: Example configuration is two PMMs, A1 and A2, of 16GiB each on a single socket on the same memory controller. There are two existing MemoryChunks, MC1 and MC2, for 100% persistent memory non-interleaved. Also, two PMMs, B1 and B2, of 16GiB each on a single socket (separate than A1 and A2) on the same memory controller with two existing MemoryChunks, MC3 and MC4, for 100% persistent memory non-interleaved.

**Goal**: Reconfigure these four PMMs to be 50% persistent memory non-interleaved. The remaining 50% is volatile (memory mode).

**Solution**: The client would first issue separate DELETE requests on MC1, MC2, MC3, and MC4. This would create four New Tasks in the TaskService. The client would then issue a POST request on the Memroy Chunk Collection of the MemoryDomain corresponding to A1 with A1 in the corresponding `InterleaveSets` and an `Oem.Hpe.MemoryChunkSizePercentage` of 50% or a `MemoryChunkSizeMiB` of 16GiB. The client would repeat this POST request on the MemoryDomains corresponding to A2, B1, and B2 with each of those respective DIMMs in their own `InterleaveSets`. This would result in eight New Tasks in the TaskService queue that would be consumed on reboot. See detailed steps below:

Step 1. Delete MC1

> DELETE `/redfish/v1/Systems/1/MemoryDomains/PROC1MemoryDomain/MemoryChunks/MC1`

Step 2. Delete MC2

> DELETE `/redfish/v1/Systems/1/MemoryDomains/PROC1MemoryDomain/MemoryChunks/MC2`

Step 3. Delete MC3

> DELETE `/redfish/v1/Systems/1/MemoryDomains/PROC2MemoryDomain/MemoryChunks/MC3`

Step 4. Delete MC4

> DELETE `/redfish/v1/Systems/1/MemoryDomains/PROC2MemoryDomain/MemoryChunks/MC4`

Step 5. Create new configuration using MemoryChunkSizePercentage for A1.

> POST `/redfish/v1/Systems/1/MemoryDomains/PROC1MemoryDomain/MemoryChunks`

```json
   {
       "AddressRangeType": "PMEM",
       "Oem": {
           "Hpe": {
               "MemoryChunkSizePercentage": 50
           }
       },
       "InterleaveSets": [
            {
               "Memory": {
                   "@odata.id": "/redfish/v1/Systems/1/Memory/A1/"
               }
           }
       ]
   }
```

Step 6. Create new configuration using MemoryChunkSizePercentage for A2.

> POST `/redfish/v1/Systems/1/MemoryDomains/PROC1MemoryDomain/MemoryChunks`

```json
   {
       "AddressRangeType": "PMEM",
       "Oem": {
           "Hpe": {
               "MemoryChunkSizePercentage": 50
           }
       },
       "InterleaveSets": [
            {
               "Memory": {
                   "@odata.id": "/redfish/v1/Systems/1/Memory/A2/"
               }
           }
       ]
   }
```

Step 7. Create new configuration using MemoryChunkSizePercentage for B1.

> POST `/redfish/v1/Systems/1/MemoryDomains/PROC2MemoryDomain/MemoryChunks`

```json
   {
       "AddressRangeType": "PMEM",
       "Oem": {
           "Hpe": {
               "MemoryChunkSizePercentage": 50
           }
       },
       "InterleaveSets": [
            {
               "Memory": {
                   "@odata.id": "/redfish/v1/Systems/1/Memory/B1/"
               }
           }
       ]
   }
```

Step 8. Create new configuration using MemoryChunkSizePercentage for B2.

> POST `/redfish/v1/Systems/1/MemoryDomains/PROC2MemoryDomain/MemoryChunks`

```json
   {
       "AddressRangeType": "PMEM",
       "Oem": {
           "Hpe": {
               "MemoryChunkSizePercentage": 50
           }
       },
       "InterleaveSets": [
            {
               "Memory": {
                   "@odata.id": "/redfish/v1/Systems/1/Memory/B2/"
               }
           }
       ]
   }
```

Step 9. Reboot system to apply changes staged in iLO as Tasks.
