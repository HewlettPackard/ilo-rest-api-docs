# iSCSI Software Initiator Configuration

# Introduction
   The iSCSI Software Initiator allows you to configure an iSCSI target device to be used as a boot source. The BIOS current configuration object contains a link to a separate resource of type `HpiSCSISoftwareInitiator`. The BIOS current configuration resource and the iSCSI Software Initiator current configuration resources are read-only. To change iSCSI settings, you need to follow another link to the Settings resource, which allows PUT and PATCH operations.

The iSCSI target configurations are represented in an `iSCSIBootSources` property, that is an array of objects, each containing the settings for a single target. The size of the array represents the total number of iSCSI boot sources that can be configured at the same time. Many mutable properties exist, including `iSCSIBootAttemptInstance`, which can be set to a unique integer in the range [1, N], where N is the boot sources array size. By default, this instance number is 0 for all objects, indicating that the object should be ignored when configuring iSCSI.

Each object also contains two read-only properties—`StructuredBootString` and `UEFIDevicePath`, which are only populated after the target has been successfully configured as a boot source. More information about each property is available in the corresponding schema. The iSCSI initiator name is represented by the `iSCSIInitiatorName` property.

An additional read-only property, `iSCSINicSources`, is only shown in the iSCSI current configuration resource. This property is an array of strings representing the possible NIC instances that can be used as targets for iSCSI boot configuration. To confirm which NIC device each string corresponds to, it is recommended to cross-reference two other resources.


* A resource of type `HpBiosMapping` can be found through a `Mappings` link in the BIOS
current configurations resource. Within its `BiosPciSettingsMappings` property is an
array of mappings between BIOS-specific device strings (such as the `NIC` source string)
and a `CorrelatableID` string that can be used to refer to the same device in non-BIOS
contexts.
* A collection of `HpServerPciDevices` may be found through a PCIDevices link in the
`ComputerSystem` resource. To find the specific PCI device corresponding to the NIC instance, you can 
search for the `CorrelatableID` that usually matches a
`UEFIDevicePath.` Once you find the `HpServerPciDevice` resource, you have access
to all the human-readable properties useful for describing a NIC source.

Changing the `iSCSIBootSources` and `iSCSIInitiatorName` settings can be done through
`PATCH` operations, very similar to how `HpBios` settings are changed. However, whereas all BIOS
settings are located in a single flat object, iSCSI settings are nested into arrays and sub-objects.
When doing a `PATCH` operation, use empty objects (`{}`) in place of those boot source objects
that you do not want to alter.

The following example covers a situation where you have configured two iSCSI boot sources,
and you would like to edit some existing settings, and add a third source.

1. Iterate through `/redfish/v1/Systems` and choose a member `ComputerSystem.` Find a
child resource of type `HpiSCSISoftwareInitiator` that allows PATCH operations.
  * `{ilo-address}/redfish/v1/Systems/1/BIOS/iSCSI/Settings`
2. Inspect the existing `iSCSIBootSources` array. You need to inspect the
`iSCSIBootAttemptInstance` property of each object to find the boot sources you are
prefer to change.

3. Create a new JSON object with the `iSCSIBootSources` property.
  *  Use an empty object in the position of instance 1 to indicate that it should not be modified.
Use an object in the position of instance 2 containing the properties that should be
modified—all omitted properties remain unmodified.
  * To add a new boot source, find any position of instance 0 and replace it with an object
containing all the new settings, and most importantly, a new unique value of
`iSCSIBootAttemptInstance.`

4. Change the iSCSI software initiator settings.
  * `PATCH {ilo-address}/redfish/v1/Systems/1/BIOS/iSCSI/Settings` 

# Scalable Persistent Memory Configuration


### HPE Scalable Persistent Memory has two resources within the RESTful API tree:
- **Current settings resource (read-only) : redfish/v1/systems/1/bios/hpescalablepmem**
    - Contains current Persistent Memory and Drive configuration data present in the system<br/><br/>
- **Pending settings resource (read/write) : redfish/v1/systems/1/bios/hpescalablepmem/settings**
    - Writable resource used to configure Persistent Memory settings
    - Modifable properties:<br/> 
        - "FeatureEnabled" - Enable/disable the Scalable Persistent Memory feature<br/>
        - "StorageInitialize" - Reinitialize drives on the next boot<br/>
        - "ConfigurationRestoration" - Restore the Logical NVDIMM-N configuration contained on the storage devices<br/>
        - "Processor1LogicalNvdimm1SizeGiB" - Memory size in Gibibytes allocated for processor 1 logical NVDIMM 1<br/>
        - "Processor1LogicalNvdimm2SizeGiB" - Memory size in Gibibytes allocated for processor 1 logical NVDIMM 2<br/>
        - "Processor2LogicalNvdimm1SizeGiB" - Memory size in Gibibytes allocated for processor 2 logical NVDIMM 1<br/>
        - "Processor2LogicalNvdimm2SizeGiB" - Memory size in Gibibytes allocated for processor 2 logical NVDIMM 2<br/>
        - "Processor3LogicalNvdimm1SizeGiB" - Memory size in Gibibytes allocated for processor 3 logical NVDIMM 1<br/>
        - "Processor3LogicalNvdimm2SizeGiB" - Memory size in Gibibytes allocated for processor 3 logical NVDIMM 2<br/>
        - "Processor4LogicalNvdimm1SizeGiB" - Memory size in Gibibytes allocated for processor 4 logical NVDIMM 1<br/>
        - "Processor4LogicalNvdimm2SizeGiB" - Memory size in Gibibytes allocated for processor 5 logical NVDIMM 2<br/>         

## View Scalable Persistent Memory settings
    GET /redfish/v1/Systems/1/bios/hpescalablepmem/
    
    {
    "@odata.context": "/redfish/v1/$metadata#HpeScalablePmem.HpeScalablePmem",
    "@odata.etag": "W/\"64BB3A2CBEF02B2B2B91DB834BAE934E\"",
    "@odata.id": "/redfish/v1/systems/1/bios/hpescalablepmem/settings/",
    "@odata.type": "#HpeScalablePmem.v1_0_0.HpeScalablePmem",
    "Attributes": {
        "AllocationUnitSizeGiB": 1,
        "BackupState": "Completed",
        "CT1": 0,
        "CT2": 100,
        "CT3": 100,
        "CT4": 0,
        "ConfigurationRestoration": false,
        "DT": 300,
        "DriveSizeOverheadMB": 20,
        "FeatureEnabled": true,
        "FeatureNotSupportedReasons": {
            "OemDisabled": false,
            "OtherNvdimmTechnologyEnabled": false,
            "UnsupportedPlatform": false
        },
        "FeatureSupported": true,
        "FunctionalityDisabledReason": {
            "MemorySubsystemProblem": false,
            "PowerSubsystemProblem": false,
            "StorageSubsystemProblem": false
        },
        "FunctionalityEnabled": true,
        "MW": 1600,
        "MaximumDriveCount": 12,
        "MaximumNumberOfSpannedLogicalNvdimmRegions": 2,
        "MaximumRegionsPerDomain": 2,
        "MinimumRegionSizeGiB": 1,
        "PS": 4,
        "PW": 340,
        "Policy": {
            "ConfigRequiresStorageInit": true,
            "SameModelNVMe": true,
            "SameSizeNVMe": true
        },
        "Processor1LogicalNvdimm1SizeGiB": 20,
        "Processor1LogicalNvdimm2SizeGiB": 0,
        "Processor1ScalablePmemAvailableGiB": 24,
        "Processor2LogicalNvdimm1SizeGiB": 0,
        "Processor2LogicalNvdimm2SizeGiB": 0,
        "Processor2ScalablePmemAvailableGiB": 48,
        "Processor3LogicalNvdimm1SizeGiB": 0,
        "Processor3LogicalNvdimm2SizeGiB": 0,
        "Processor3ScalablePmemAvailableGiB": 0,
        "Processor4LogicalNvdimm1SizeGiB": 0,
        "Processor4LogicalNvdimm2SizeGiB": 0,
        "Processor4ScalablePmemAvailableGiB": 0,
        "SpannedLogicalNvdimm1AvailableMemoryGiB": 72,
        "SpannedLogicalNvdimm1SizeGiB": 25,
        "SpannedLogicalNvdimm2AvailableMemoryGiB": 0,
        "SpannedLogicalNvdimm2SizeGiB": 0,
        "StorageInitialize": false,
        "SupportedDrives": [
            {
                "DW": 16,
                "DriveSizeGB": 400,
                "NVMeId": "8086_MO0400KEFHN_CVFT6092002X400GGN",
                "SettingName": "NVMeDriveBox2Bay1",
                "WP": 1000
            },
            {
                "DW": 16,
                "DriveSizeGB": 400,
                "NVMeId": "8086_MO0400KEFHN_CVFT543400A2400GGN",
                "SettingName": "NVMeDriveBox2Bay3",
                "WP": 1000
            },
            {
                "DW": 16,
                "DriveSizeGB": 400,
                "NVMeId": "8086_MO0400KEFHN_CVFT60920040400GGN",
                "SettingName": "NVMeDriveBox2Bay5",
                "WP": 1000
            },
            {
                "DW": 16,
                "DriveSizeGB": 800,
                "NVMeId": "8086_MO0800KEFHP_CVFT5414002B800HGN",
                "SettingName": "NVMeDriveBox2Bay8",
                "WP": 1700
            }
        ],
        "T1": 1,
        "T2": 40,
        "T3": 259,
        "T4": 0,
        "TW": 2704,
        "TheoreticalPMemMaxGiB": 117,
        "TheoreticalPmemMaxPerDomainGiB": {
            "Processor1": 57,
            "Processor2": 60,
            "Processor3": 0,
            "Processor4": 0,
            "SpannedLogicalNvdimm1": 117,
            "SpannedLogicalNvdimm2": 0
        },
        "ValidationVersion": 1
    },
    "Id": "settings",
    "Name": "Scalable Persistent Memory Current Settings"
    }


## Enabling Scalable Persistent Memory
The Scalable Persistent Memory feature must be enabled before any configuration is allowed. 
    
    PATCH /redfish/v1/Systems/1/bios/hpescalablepmem/settings/

    {
        "FeatureEnabled": true
    }

## Configuring NVMe Drives for Persistent Memory
The NVMe drive configuration properties are found in the /bios/ REST resource.<br/> 
NVMe drive properties are displayed with its Box Bay configuration as shown below. <br/>
Valid drive configurations : "Nvme" or "ScalablePMEM".<br/>

    PATCH /redfish/v1/Systems/1/bios/settings/

    {
        "NVMeDriveBox2Bay1": "ScalablePMEM",
        "NVMeDriveBox2Bay3": "ScalablePMEM",
        "NVMeDriveBox2Bay5": "Nvme",
        "NVMeDriveBox2Bay8": "Nvme"
    }
    
## Sanitize NVMe Drives
    PATCH /redfish/v1/Systems/1/bios/hpescalablepmem/settings/

    {
        "StorageInitialize": true
    }
    
## Restore NVMe Drives
    PATCH /redfish/v1/Systems/1/bios/hpescalablepmem/settings/

    {
        "ConfigurationRestoration": true
    }    
    
## Creating Logical NVDIMM regions
Example: Create a 100 GiB logical NVDIMM on processor 1 
    
    PATCH /redfish/v1/Systems/1/bios/hpescalablepmem/settings/

    {
        "Processor1LogicalNvdimm1SizeGiB": 100
    }    

