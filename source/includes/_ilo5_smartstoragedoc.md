# SmartStorage configuration

## Introduction
HPE ProLiant Gen10 servers with SmartStorage array controllers now provide a way to manage the array controllers using the REST API.  This is in addition to the existing SmartStorage inventory and status REST API resources.

SmartStorage adds two new resources to the API per controller:
* Current array controller configuration (read only)
* Pending array controller configuration (modifiable with HTTP PATCH)

This is very similar to the way BIOS is configured.

The resource sub-tree is linked into the ComputerSystem resource:

> GET /redfish/v1/systems/{item}/

```json
{
  "Oem": {
    "Hpe": {
      "SmartStorageConfig": {
        "@odata.id": "/redfish/v1/systems/{item}/smartstorageconfig/"
      }
    }
  }
}
```

This URI is the GET-only current configuration.  This resource links to the pending configuration.  The `@odata.type` is `SmartStorageConfig.v2_0_0.SmartStorageConfig`

An example of the SmartStorageConfig resource:

```json
{
    "@Redfish.Settings": {
        "@odata.type": "#Settings.v1_0_0.Settings",
        "ETag": "",
        "Messages": [
            {
                "MessageId": "Base.1.0.Success"
            }
        ],
        "SettingsObject": {
            "@odata.id": "/redfish/v1/systems/1/smartstorageconfig/settings/"
        },
        "Time": ""
    },
    "@odata.context": "/redfish/v1/$metadata#SmartStorageConfig.SmartStorageConfig",
    "@odata.etag": "W/\"5C73F2701BE5B6B6B665E028E718BAB2\"",
    "@odata.id": "/redfish/v1/systems/1/smartstorageconfig/",
    "@odata.type": "#SmartStorageConfig.v2_0_0.SmartStorageConfig",
    "CurrentParallelSurfaceScanCount": 1,
    "DataGuard": "Strict",
    "DegradedPerformanceOptimization": "Disabled",
    "DriveWriteCache": "Disabled",
    "ElevatorSort": "Enabled",
    "EncryptionConfiguration": "None",
    "EncryptionEULA": null,
    "ExpandPriority": "Medium",
    "FlexibleLatencySchedulerSetting": "Default",
    "Id": "smartstorageconfig",
    "InconsistencyRepairPolicy": "Disabled",
    "Location": "Slot UNKNOWN",
    "LocationFormat": "PCISlot",
    "LogicalDrives": [
        {
            "Accelerator": "ControllerCache",
            "BlockSizeBytes": 512,
            "CapacityBlocks": 1953459632,
            "CapacityGiB": 931,
            "DataDrives": [
                "P1I:3:1"
            ],
            "DriveLocationFormat": "ControllerPort:Box:Bay",
            "LegacyBootPriority": "None",
            "LogicalDriveName": "Logical Drive 0",
            "LogicalDriveNumber": 1,
            "ParityGroupCount": 0,
            "Raid": "Raid0",
            "SpareDrives": [],
            "SpareRebuildMode": null,
            "StripSizeBytes": 262144,
            "StripeSizeBytes": 262144,
            "VolumeUniqueIdentifier": "600508B1001CAC3093F52C735D6DE038"
        }
    ],
    "MonitorAndPerformanceAnalysisDelaySeconds": 60,
    "NoBatteryWriteCache": "Disabled",
    "Oem": {
        "Hpe": {
            "@odata.type": "#HpeBiosExt.v2_0_0.HpeBiosExt",
            "SettingsObject": {
                "UnmodifiedETag": "W/\"1D348072E79A999999DDFE0BCB960774\""
            }
        }
    },
    "PhysicalDrives": [
        {
            "LegacyBootPriority": "None",
            "Location": "P1I:3:1",
            "LocationFormat": "ControllerPort:Box:Bay"
        }
    ],
    "Ports": [
        {
            "OperatingModeAfterReboot": "Mixed",
            "PortIndex": 0
        },
        {
            "OperatingModeAfterReboot": "Mixed",
            "PortIndex": 1
        }
    ],
    "PowerModeAfterReboot": "MaxPerformance",
    "PredictiveSpareRebuild": "Disabled",
    "QueueDepth": "Automatic",
    "ReadCachePercent": 100,
    "RebuildPriority": "RapidLow",
    "SurfaceScanAnalysisDelaySeconds": 3,
    "SurfaceScanAnalysisPriority": "Idle",
    "SurvivalPowerMode": "Enabled",
    "WriteCacheBypassThresholdKiB": 1040
}
```

## Update controller configuration
The controller configuration is accurate after boot, before any online changes are administered via SSA.
A live version of this data is available in iLO-data/smartstorage/.

> PATCH /redfish/v1/Systems/{item}/smartstorageconfig/settings/

```json
{
    "DataGuard": "Strict",
    "ExpandPriority": "High",
    "RebuildPriority": "High",
    "ReadCachePercent": 20
}
``` 


## View logical drive inventory
The logical drive inventory is accurate after boot, before any online changes are administered via SSA.
A live version of this data is available in iLO-data/smartstorage/.

> GET /redfish/v1/Systems/{item}/smartstorageconfig/

```json
{
   "LocationFormat": "PCISlot",
   "DataGuard": "Strict",
   "Location": "Slot 1",
   "BootVolumePrimary": "600508B1001C406C193B03A644CDF6C2",
   "BootVolumeSecondary": "00000000000000000000000000000000",
   "LogicalDrives": [
        {
            "LogicalDriveNumber": 1,
            "Status": {
                "State": "Enabled",
                "HealthRollup": "OK",
                "Health": "OK"
            },
            "VolumeUniqueIdentifier": "600508B1001C406C193B03A644CDF6C2",
            "LegacyBootPriority": "Primary",
            "CapacityGiB": 558,
            "CapacityBlocks": 1171743324,
            "Raid": "Raid0",
            "StripSizeBytes": 262144,
            "StripeSizeBytes": 524288,
            "Accelerator": "None",
            "LogicalDriveName": "A4119B335001438020C7EA30\u0002\u00012B8F",
            "DriveLocationFormat": "ControllerPort:Box:Bay",
            "DataDrives": [
                "1I:1:1",
                "1I:1:2"
            ],
            "SpareDrives": []
        }
    ]
}
``` 


## Create logical drives


> PUT /redfish/v1/Systems/{item}/smartstorageconfig/settings/

```json
{
    "LogicalDrives": [
       {
          "CapacityGiB": 558,
          "Raid": "Raid0",
          "StripSizeBytes": 262144,
          "LogicalDriveName": "MyLD",
          "DataDrives": [
                "1I:1:1",
                "1I:1:2"
          ],
          "SpareDrives": [
                "1I:1:3"
          ],
          "Accelerator": "ControllerCache" 
       }
    ]
}
```


> PUT /redfish/v1/Systems/{item}/smartstorageconfig/settings/

```json
{
    "LogicalDrives": [
       {
          "LogicalDriveName": "MyLD",      
          "Raid": "Raid5", 
          "DataDrives": {
             "DataDriveCount": 4,
             "DataDriveMediaType": "HDD",
             "DataDriveInterfaceType": "SAS", 
             "DataDriveMinimumSizeGiB": 1000
          }
       }
    ]
}
``` 


## Delete logical drives

There are two ways to delete logical drives.  The first enables you to remove specific logical drives by Volume Unique Identifier.  The second can be used to remove all logical drives.

The `Actions` property is not present by default in the resource but must be added with an HTTPS PUT operation.

**NOTE:  that the `Actions` property here is under the specific logical drive you wish to delete.**

> PUT /redfish/v1/Systems/{item}/SmartStorageConfig/Settings/

```json
{
   "LogicalDrives": [
      {
         "Actions": [{"Action": "LogicalDriveDelete"}],
         "VolumeUniqueIdentifier": "600123459AF45456664443"
      }
    ],
    "DataGuard": "Permissive"
}
```

> PATCH /redfish/v1/Systems/{item}/SmartStorageConfig/Settings/

```json
{
    "LogicalDrives": [],
    "DataGuard": "Disabled"
}
```

A system reboot is required for the Smart Storage firmware to validate and perform any requested changes.  The result of the operations will be available in the current configuration resource at `/redfish/v1/Systems/{item}/SmartStorageConfig/` (the parent resource of the settings resource.)

### DataGuard rules 

+ When DataGuard is set to Disabled, logical drives are deleted if they are omitted or if the delete action is specified.
+ When DataGuard is set to Permissive, logical drives are deleted if the delete action is specified. Omitted logical drives are not deleted.
+ When DataGuard is set to Strict, in any case, logical drives are not deleted. If a logical drive is omitted or a delete action is found on a logical drive, the request returns an error. 

## Sanitize drives
Physical drive erase:

> PATCH /redfish/v1/systems/{item}/smartstorageconfig/settings/

```json
{
    "Actions": [
        {
            "Action": "PhysicalDriveErase",
            "ErasePattern": "SanitizeRestrictedBlockErase",
            "PhysicalDriveList": [
                "1I:1:1",
                "1I:1:2"
            ]
        }
    ],
    "DataGuard": "Disabled"
}

```

Sanitize is a long running operation and the drive is not available (for RAID config) until sanitize is complete. The status can be checked from the iLO/SmartStorage data.

