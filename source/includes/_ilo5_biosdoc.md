# BIOS Defaults and Passwords

Actions are POST operations to perform a specific request, such as a system reset or a password change.
Actions are completely different from actions in iLO 4. The Bios resource has 2 actions:

## Reset BIOS Settings 

UEFI BIOS Supports a new POST action to reset settings.
      
```json
"Actions": {
  "#Bios.ResetBios": {
    "target": "/redfish/v1/Systems/1/Bios/Settings/Actions/Bios.ResetBios"
  }
}
```
> The body of the POST should contain

```json
{
  "ResetType" : "default"      
} 
```
> or

```json
{  
  "ResetType" : "default.user"
} 
```

## Change BIOS password  

UEFI BIOS supports a new POST action to change the BIOS password.

```json
"Actions": {
  "#Bios.ChangePassword": {
    "target": "/redfish/v1/Systems/1/Bios/Settings/Actions/Bios.ChangePassword"
  }
}
```

> The body of the action should contain:

```json
{
  "PasswordName": "Administrator | User",
  "OldPassword" : "OldPasswordText",
  "NewPassword" : "NewPasswordText"
}
```

The target link is where the body of the action should be posted.

# iSCSI Software Initiator Configuration

## Introduction
   The iSCSI Software Initiator allows you to configure an iSCSI target device to be used as a boot source. The BIOS current configuration object contains a link to a separate resource of type `HpeiSCSISoftwareInitiator`. The BIOS current configuration resource and the iSCSI Software Initiator current configuration resources are read-only. To change iSCSI settings, you need to follow another link to the Settings resource, which allows PUT and PATCH operations.

The iSCSI target configurations are represented in an `iSCSISources` property, that is an array of objects, each containing the settings for a single target. The size of the array represents the total number of iSCSI boot sources that can be configured at the same time. Many mutable properties exist, including `iSCSIAttemptInstance`, which can be set to a unique integer in the range [1, N], where N is the boot sources array size. By default, this instance number is 0 for all objects, indicating that the object should be ignored when configuring iSCSI.

Each object also contains two read-only properties—`StructuredBootString` and `UEFIDevicePath`, which are only populated after the target has been successfully configured as a boot source. More information about each property is available in the corresponding schema. The iSCSI initiator name is represented by the `iSCSIInitiatorName` property.

An additional read-only property, `iSCSINicSources`, is only shown in the iSCSI current configuration resource. This property is an array of strings representing the possible NIC instances that can be used as targets for iSCSI boot configuration. To confirm which NIC device each string corresponds to, it is recommended to cross-reference two other resources.


* A resource of type `HpeBiosMapping` can be found through a `Mappings` link in the BIOS
current configurations resource. Within its `BiosPciSettingsMappings` property is an
array of mappings between BIOS-specific device strings (such as the `NIC` source string)
and a `CorrelatableID` string that can be used to refer to the same device in non-BIOS
contexts.
* A collection of `HpeServerPciDevices` may be found through a PCIDevices link in the
`ComputerSystem` resource. To find the specific PCI device corresponding to the NIC instance, you can 
search for the `CorrelatableID` that usually matches a
`UEFIDevicePath.` Once you find the `HpeServerPciDevice` resource, you have access
to all the human-readable properties useful for describing a NIC source.

Changing the `iSCSISources` and `iSCSIInitiatorName` settings can be done through
`PATCH` operations, very similar to how `HpeBios` settings are changed. However, whereas all BIOS
settings are located in a single flat object, iSCSI settings are nested into arrays and sub-objects.
When doing a `PATCH` operation, use empty objects (`{}`) in place of those boot source objects
that you do not want to alter.

The following example covers a situation where you have configured two iSCSI boot sources,
and you would like to edit some existing settings, and add a third source.

1. Iterate through `/redfish/v1/Systems` and choose a member `ComputerSystem.` Find a
child resource of type `HpeiSCSISoftwareInitiator` that allows PATCH operations.
  * `{ilo-address}/redfish/v1/Systems/1/BIOS/iSCSI/Settings`
2. Inspect the existing `iSCSISources` array. You need to inspect the
`iSCSIAttemptInstance` property of each object to find the boot sources you are
prefer to change.

3. Create a new JSON object with the `iSCSISources` property.
  *  Use an empty object in the position of instance 1 to indicate that it should not be modified.
Use an object in the position of instance 2 containing the properties that should be
modified—all omitted properties remain unmodified.
  * To add a new boot source, find any position of instance 0 and replace it with an object
containing all the new settings, and most importantly, a new unique value of
`iSCSIAttemptInstance.`

4. Change the iSCSI software initiator settings.
  * `PATCH {ilo-address}/redfish/v1/Systems/1/BIOS/iSCSI/Settings` 

# Scalable Persistent Memory Configuration


### HPE Scalable Persistent Memory has two resources within the RESTful API tree:
- **Current settings resource (read-only) : redfish/v1/systems/{item}/bios/hpescalablepmem**
    - Contains current Persistent Memory and Drive configuration data present in the system
- **Pending settings resource (read/write) : redfish/v1/systems/{item}/bios/hpescalablepmem/settings**

* Modifiable properties:
  * `"FeatureEnabled"` - Enable/disable the Scalable Persistent Memory feature
  * `"StorageInitialize"` - Reinitialize drives on the next boot
  * `"ConfigurationRestoration"` - Restore the Logical NVDIMM-N configuration contained on the storage devices
  * `"Processor1LogicalNvdimm1SizeGiB"` - Memory size in Gibibytes allocated for processor 1 logical NVDIMM 1
  * `"Processor1LogicalNvdimm2SizeGiB"` - Memory size in Gibibytes allocated for processor 1 logical NVDIMM 2
  * `"Processor2LogicalNvdimm1SizeGiB"` - Memory size in Gibibytes allocated for processor 2 logical NVDIMM 1
  * `"Processor2LogicalNvdimm2SizeGiB"` - Memory size in Gibibytes allocated for processor 2 logical NVDIMM 2
  * `"Processor3LogicalNvdimm1SizeGiB"` - Memory size in Gibibytes allocated for processor 3 logical NVDIMM 1
  * `"Processor3LogicalNvdimm2SizeGiB"` - Memory size in Gibibytes allocated for processor 3 logical NVDIMM 2
  * `"Processor4LogicalNvdimm1SizeGiB"` - Memory size in Gibibytes allocated for processor 4 logical NVDIMM 1
  * `"Processor4LogicalNvdimm2SizeGiB"` - Memory size in Gibibytes allocated for processor 5 logical NVDIMM 2   

### View Scalable Persistent Memory settings

You may view the Scalable Persistent Memory settings with a GET

> GET /redfish/v1/Systems/{item}/bios/hpescalablepmem/

```json
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
```

### Enabling Scalable Persistent Memory
The Scalable Persistent Memory feature must be enabled before any configuration is allowed. 
    
>PATCH /redfish/v1/Systems/{item}/bios/hpescalablepmem/settings/

```json
{
    "FeatureEnabled": true
}
```

### Configuring NVMe Drives for Persistent Memory
The NVMe drive configuration properties are found in the /bios/ REST resource. 
NVMe drive properties are displayed with its Box Bay configuration as shown below. 
Valid drive configurations : "Nvme" or "ScalablePMEM".

> PATCH /redfish/v1/Systems/1/bios/settings/

```json
{
    "NVMeDriveBox2Bay1": "ScalablePMEM",
    "NVMeDriveBox2Bay3": "ScalablePMEM",
    "NVMeDriveBox2Bay5": "Nvme",
    "NVMeDriveBox2Bay8": "Nvme"
}
```

### Sanitize NVMe Drives
> PATCH /redfish/v1/Systems/1/bios/hpescalablepmem/settings/

```json
{
    "StorageInitialize": true
}
```
    
### Restore NVMe Drives
> PATCH /redfish/v1/Systems/1/bios/hpescalablepmem/settings/

```json
{
    "ConfigurationRestoration": true
}    
```
  
### Creating Logical NVDIMM regions

> Example: Create a 100 GiB logical NVDIMM on processor 1   
> PATCH /redfish/v1/Systems/1/bios/hpescalablepmem/settings/

```json
{
    "Processor1LogicalNvdimm1SizeGiB": 100
}    
```

# HTTPS Boot TLS Configuration

 TLS Certificates Resource has three resources within the RESTful API tree:
- **Current Settings Resource (read-only) : redfish/v1/systems/1/bios/tlsconfig/**
    - Contains current TLS certificates resource configuration data present in the system
- **Pending Settings Resource (read/write) : redfish/v1/systems/1/bios/tlsconfig/settings/**
    - Writable resource used to configure TLS certificates settings
    - Modifable properties: 
        - `"Ciphers"` - Set the desired supported ciphers
        - `"HostnameCheck"` - Enable/Disable host name checking
        - `"ProtocolVersion"` - Set the desired protocol version
        - `"VerifyMode"` - Set the verification method (PEER/NONE)
        - `"NewCertificates"` - An array of the certificates to be installed
        - `"DeleteCertificates"` - An array of the fingerprints of the certificates to be deleted 
    - Read Only properties that gets modified internally:
        - `"Certificates"` - An array of all the installed certificates
        - `"TlsCaCertificateCount"` - The number of the installed certificates

- **TLS Default Settings Resource (read-only) : redfish/v1/systems/1/bios/tlsconfig/baseconfigs/**
   Holds the default values of the resource

### Installing Certificates
  
  The certificates are X509 keys. In PEM format, the certificates are encoded in a series of strings with new line characters between 
  them:

  This an example of a certificate in a PEM format:
    
    -----BEGIN CERTIFICATE-----
    MIIEHTCCAwWgAwIBAgIQe8LmWgF5edKw01/avJg69DANBgkqhkiG9w0BAQsFADCB
    kTELMAkGA1UEBhMCVVMxKzApBgNVBAoTIkhld2xldHQgUGFja2FyZCBFbnRlcnBy
    aXNlIENvbXBhbnkxIDAeBgNVBAsTF0luZnJhc3RydWN0dXJlIFNlcnZpY2VzMTMw
    
  It should be modified to add the new line characters:
    
    "-----BEGIN CERTIFICATE-----\r\nMIIGxDCCBaygAwIBAgIQUkL9757013wOQ2heZMCLizANBgkqhkiG9w0BAQsFADCB\r\nkTELMAkGA1UEBhMCVVMxKzApBgNVBAo
    TIkhld2xldHQgUGFja2FyZCBFbnRlcnBy\r\naXNlIENvbXBhbnkxIDAeBgNVBAsTF0luZnJhc3RydWN0dXJlIFNlcnZpY2VzMTMw\r\n
    
  Note the "\r\n" added at the end of each line in the certificate body.
  Finally, the certificate needs to be PUT (only a PUT would work) through the API (Postman,..), as many as needed to be installed:

> PUT /redfish/v1/Systems/{item}/bios/tlsconfig/settings/

```json
{
  "NewCertificates": [
    {
      "X509Certificate0":"-----BEGIN CERTIFICATE-----\r\nMIIGxDCCBaygAwIBAgIQUkL9757013wOQ2heZMCLizANBg......"
    }
  ]
}
```    
  
> Once installed, it will look like this after rebooting:

```json
{
  "@odata.context": "/redfish/v1/$metadata#HpeTlsConfig.HpeTlsConfig",
  "@odata.etag": "W/\"DAE5B73CD430CFCFCF7E180C05FE6C9E\"",
  "@odata.id": "/redfish/v1/systems/1/bios/tlsconfig/settings/",
  "@odata.type": "#HpeTlsConfig.v1_0_0.HpeTlsConfig",
  "Certificates": [
    {
        "FingerPrint": "54:8C:8B:45:55:30:47:8D:43:8D:44:BF:33:E0:C5:A5:44:1E:E9:5E:B2:0A:AC:A6:CA:59:B6:D9:7B:FC:83:A9",
        "Issuer": "C=US, O=Whatever, OU=Infrastructure Services, CN=Whatever Private Root CA",
        "SerialNumber": "5242FDEF9EF4D77CE43685E64C08B8B",
        "Subject": "O=Whatever, CN=John Smith, OU=XXX-WEB-H, OU=Computer Name - Smith.John, OU=Employment Status - Employees, OU=SmartCard, emailAddress=John.Smith@whatever.com",
        "ValidNotAfter": "07/11/2017  23:59",
        "ValidNotBefore": "07/11/2016  00:00"
    }
  ],
  "Ciphers": "AES128-SHA:AES256-SHA:AES128-SHA256:AES256-SHA256:AES128-GCM-SHA256:AES256-GCM-SHA384",
  "DeleteCertificates": [],
  "HostnameCheck": "Enabled",
  "Id": "settings",
  "Name": "TLS Pending Settings",
  "NewCertificates": [],
  "ProtocolVersion": "AUTO",
  "TlsCaCertificateCount": 1,
  "VerifyMode": "NONE"
}
```

### Deleting Certificates
When a certificate is installed, a new field is created with the Fingerprint of that certificate (SHA256).  To remove a certificate, PUT the fingerprint to remove

> PUT /redfish/v1/Systems/1/bios/tlsconfig/settings/

```json
{
  "DeleteCertificates": [
    {
      "FingerPrint": "54:8C:8B:45:55:30:47:8D:43:8D:44:BF:33:E0:C5:A5:44:1E:E9:5E:B2:0A:AC:A6:CA:59:B6:D9:7B:FC:83:A9"
    }
  ]
}
```

You can delete more than one certificate at a time.

### Resetting the resource to its default settings

> PUT /redfish/v1/Systems/1/bios/tlsconfig/settings/

```json
{
  "BaseConfig": "Default"
}
```

> The default resource would look like:

```json
{
  "@odata.context": "/redfish/v1/$metadata#HpeTlsConfig.HpeTlsConfig",
  "@odata.etag": "W/\"F5B8B30487AB151515845B0C2CC520E0\"",
  "@odata.id": "/redfish/v1/systems/1/bios/tlsconfig/settings/",
  "@odata.type": "#HpeTlsConfig.v1_0_0.HpeTlsConfig",
  "Certificates": [],
  "Ciphers": "AES128-SHA:AES256-SHA:AES128-SHA256:AES256-SHA256:AES128-GCM-SHA256:AES256-GCM-SHA384",
  "DeleteCertificates": [],
  "HostnameCheck": "Disabled",
  "Id": "settings",
  "Name": "TLS Current Settings",
  "NewCertificates": [],
  "ProtocolVersion": "AUTO",
  "TlsCaCertificateCount": 0,
  "VerifyMode": "PEER"
}
```

### Examples of other changes

- **Modifying Ciphers** 

> PATCH /redfish/v1/Systems/1/bios/tlsconfig/settings/

```json
{
  "Ciphers": "AES128-SHA:AES256-SHA"
}
```

- **Modifying VerifyMode**
PEER or NONE.

> PATCH /redfish/v1/Systems/1/bios/tlsconfig/settings/

```json
{
  "VerifyMode": "PEER"
}    
```

- **Modifying HostnameCheck**
Can not be changed if VerifyMode is set to NONE.

> PATCH /redfish/v1/Systems/1/bios/tlsconfig/settings/

```json
{
  "HostnameCheck": "Enabled"
}    
```

- **Modifying ProtocolVersion**
"AUTO", "1.0", "1.1" or "1.2".

> PATCH /redfish/v1/Systems/1/bios/tlsconfig/settings/

```json
{
  "ProtocolVersion": "1.1"
}    
```
