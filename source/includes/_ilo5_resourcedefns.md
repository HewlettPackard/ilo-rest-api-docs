## AccountService
```@odata.type: "#AccountService.v1_0_2.AccountService"```

This is the schema definition for the Account service. It represents the properties for this service and has links to the list of accounts.

> **Resource Instances of this Type**:  

> * `https://{iLO}/redfish/v1/accountservice/`

### Managing User Accounts with the Accounts Collection

**JSONPath**: `/Accounts/@odata.id`

The destination of this link is a collection of user accounts (see ManagerAccount).

* You may create a new user account by POSTing a new account description the the Accounts collection.  See ManagerAccount for details.
> e.g. `POST https://{iLO}/redfish/v1/accountservice/accounts/ with new account description`
* You may modify an existing user by PATCHing properties to the user account resource.  See ManagerAccount for details.
> e.g. `PATCH https://{iLO}/redfish/v1/accountservice/accounts/{item} with different properties`
* You may remove a user account by DELETEing the resources representing the user
> e.g. `DELETE https://{iLO}/redfish/v1/accountservice/accounts/{item}`

### Oem.Hpe.AuthFailureDelayTimeSeconds

The time in seconds to delay for each failure after AuthFailuresBeforeDelay authentication attempts have failed.  Values of 2, 5, 10, and 30 seconds are valid.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Oem": {"Hpe": {"AuthFailureDelayTimeSeconds": &lt;integer-value&gt;}}}

### Oem.Hpe.AuthFailureLoggingThreshold

This property enables you to view and configure logging criteria for failed authentications. A failed login log entry is recorded after the configured number of attempts. 0 = feature disabled; 1-3 and 5 are allowable values.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Oem": {"Hpe": {"AuthFailureLoggingThreshold": &lt;integer-value&gt;}}}

### Oem.Hpe.AuthFailuresBeforeDelay

The number of failed authentication attempts allowed before authentication is delayed by AuthFailureDelayTimeSeconds. Values of  0, 1, 3, and 5 are valid, with 0 indicating delay after every authentication failure.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Oem": {"Hpe": {"AuthFailuresBeforeDelay": &lt;integer-value&gt;}}}

### Oem.Hpe.MinPasswordLength

This property specifies the minimum number of characters allowed when a user password is set or changed. It must be a value from 0 to 39.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Oem": {"Hpe": {"MinPasswordLength": &lt;integer-value&gt;}}}

## Bios
```@odata.type: "#Bios.v1_0_0.Bios"```

Bios contains properties surrounding a BIOS Attribute Registry (where the system-specific BIOS attributes are described) and the Actions needed to perform changes to BIOS settings, which typically require a system reset to apply.

> **Resource Instances of this Type**:  

> * `https://{iLO}/redfish/v1/systems/{item}/bios/settings/`

> * `https://{iLO}/redfish/v1/systems/{item}/bios/`

**BIOS Attributes**

### AcpiHpet

Use this option to disable the High Precision Event Timer (HPET) table and device object in ACPI. When disabled, the HPET is not available to an operating system that supports the HPET through the industry standard ACPI name space.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`AcpiHpet` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### AcpiRootBridgePxm

When enabled, the System BIOS reports the proximity relationship between I/O devices and system memory to the operating system. Most operating systems can use this information to efficiently assign memory resources for devices, such as network controllers and storage devices. Additionally, certain I/O devices might not be able to take advantage of I/O handling benefits if their OS drivers are not properly optimized to support this feature. See your operating system and I/O device documentation for more details.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`AcpiRootBridgePxm` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### AcpiSlit

The ACPI SLIT (System Locality Information Table) defines the relative access times between processors, memory subsystems, and I/O subsystems. Operating systems that support the SLIT can use this information to improve performance by allocating resources and workloads more efficiently.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`AcpiSlit` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### AdjSecPrefetch

Use this option to disable the processor Adjacent Sector Prefetch feature. In some cases, setting this option to disabled can improve performance. Typically, setting this option to enabled provides better performance. Only disable this option after performing application benchmarking to verify improved performance in the environment.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`AdjSecPrefetch` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### AdminEmail

Enter the server administrator's e-mail address.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
### AdminName

Enter the server administrator's name text.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
### AdminOtherInfo

Enter the server administrator's information text.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
### AdminPassword

Use this option to enter the administrator password to protect the server configuration. When this option is enabled, you are prompted for this password before being allowed to modify the configuration.


| | |
|---|---|
|JSON type|password|
|HTTP PATCH|Yes (if resource allows PATCH)
### AdminPhone

Enter the server administrator's phone number text.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
### AdvancedMemProtection

Use this option to configure additional memory protection with ECC (Error Checking and Correcting). Options and support vary per system.
Advanced ECC keeps all installed memory available for use while still protecting the system against all single-bit failures and certain multi-bit failures.
Online Spare Memory enables a system to automatically map out a group of memory that is detected to be at an increased risk of receiving uncorrected memory errors based on an advanced analysis of corrected memory errors. The mapped out memory is automatically replaced by a spare group of memory without interrupting the system.
Mirrored Memory provides the maximum protection against uncorrected memory errors that might otherwise result in a system failure.
Fault Tolerant Advanced Double Device Data Correction (ADDDC) enables the system to correct memory errors and continue to operate in cases of multiple DRAM device failures on a DIMM. This provides protection against uncorrectable memory errors beyond what is available with Advanced ECC.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`AdvancedMemProtection` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`FastFaultTolerantADDDC`|Fast Fault Tolerant Memory (ADDDC)
|`AdvancedEcc`|Advanced ECC Support
|`OnlineSpareAdvancedEcc`|Online Spare with Advanced ECC Support
|`MirroredAdvancedEcc`|Mirrored Memory with Advanced ECC Support
### AsrStatus

Use this option to configure the Automatic Server Recovery option, which enables the system to automatically reboot if the server locks up.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`AsrStatus` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### AsrTimeoutMinutes

When Automatic Server Recovery is enabled, you can use this option to set the time to wait before rebooting the server in the event of an operating system crash or server lockup.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`AsrTimeoutMinutes` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Timeout10`|10 Minutes
|`Timeout15`|15 Minutes
|`Timeout20`|20 Minutes
|`Timeout30`|30 Minutes
|`Timeout5`|5 Minutes
### AssetTagProtection

Use this option to lock Asset Tag information. When set to lock, the Asset Tag is not erased if the default system settings are restored.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`AssetTagProtection` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Locked`|Locked
|`Unlocked`|Unlocked
### AutoPowerOn

Use this option to configure the server power state when AC power is applied to the system. By default, the system returns to its previous power state when AC power is restored after an AC power loss. Always Power On and Always Power Off cause the system to always return to the "on" and "off" state, respectively, whenever power is applied, even if the system is in the "off" state when power is lost.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`AutoPowerOn` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`AlwaysPowerOn`|Always Power On
|`AlwaysPowerOff`|Always Power Off
|`RestoreLastState`|Restore Last Power State
### BootMode

Use this option to select the boot mode of the system. Selecting UEFI Mode configures the system to boot Unified Extensible Firmware Interface (UEFI) compatible operating systems. Selecting Legacy BIOS Mode configures the system to boot traditional operating systems in Legacy BIOS compatibility mode. The operating system can only boot in the mode in which it is installed. The following options require booting in UEFI Mode: Secure Boot, IPv6 PXE Boot, boot > 2.2 TB Disks in AHCI SATA Mode, and Smart Array SW RAID.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`BootMode` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Uefi`|UEFI Mode
|`LegacyBios`|Legacy BIOS Mode
### BootOrderPolicy

Use this option to configure how the system attempts to boot devices per the Boot Order list when no bootable device is found. If configured to 'Retry Boot Order Indefinitely,' the system continuously attempts to process the Boot Order list until a bootable device is found. If configured to 'Attempt Boot Order Once,' the system attempts to process all items in the Boot Order list once, and if unsuccessful, waits for user input to proceed. If configured for 'Reset After Failed Boot Attempt,' the system attempts to process all items in the Boot Order list once, and then reboots the system.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`BootOrderPolicy` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`RetryIndefinitely`|Retry Boot Order Indefinitely
|`AttemptOnce`|Attempt Boot Order Once
|`ResetAfterFailed`|Reset After Failed Boot Attempt
### ChannelInterleaving

You can only configure this option if the Workload Profile is set to Custom. Use this option to modify the level of interleaving for which the memory system is configured. Typically, higher levels of memory interleaving result in maximum performance. However, reducing the level of interleaving can result in power savings.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`ChannelInterleaving` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### Chipset_TpmFeatureEnableOrDisable

Information: Use this option to enable chipset based TPM 2.0 feature


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`Chipset_TpmFeatureEnableOrDisable` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Disabled`|Disabled
|`Enabled`|Enabled
### Chipset_TpmFeatureType

Information: Use this option to enable chipset based TPM 2.0 feature


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Chipset_TpmFeatureType` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Chipset-TpmFeature:NONE`|Chipset-TPM feature: NONE
|`Chipset-TpmFeature:PTT`|Chipset-TPM feature: PTT
|`Chipset-TpmFeature:OTHER`|Chipset-TPM feature: OTHER
### CollabPowerControl

For operating systems that support the Processor Clocking Control (PCC) Interface, enabling this option enables the Operating System to request processor frequency changes even if the Power Regulator option on the server are configured for Dynamic Power Savings Mode. For Operating Systems that do not support the PCC Interface, or when the Power Regulator Mode is not configured for Dynamic Power Savings Mode, this option has no effect on system operation.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`CollabPowerControl` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### ConsistentDevNaming

Use this option to select the level of Consistent Device Naming. On supported operating systems, NIC ports are named based on their location in the system. CDN Support for LOMs Only names Embedded NICs and FlexibleLOMs. Existing NIC connections retain their names until reinstalled under the OS environment.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`ConsistentDevNaming` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`LomsAndSlots`|CDN Support for LOMs and Slots
|`LomsOnly`|CDN Support for LOMs Only
|`Disabled`|Disabled
### CustomPostMessage

Enter a message to be displayed on POST screen during system startup. This feature limits POST screen messaging to 62 characters, special characters are also accepted.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
### DaylightSavingsTime

This option controls the Daylight Savings Time (DST) adjustment to the displayed local time.  If this option is disabled, the displayed local time will not be adjusted for DST.  If this option is enabled, the displayed local time will be advanced by one hour.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`DaylightSavingsTime` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Disabled`|Disabled
|`Enabled`|Enabled
### DcuIpPrefetcher

Use this option to disable the processor DCU IP Prefetcher feature. In some cases, setting this option to disabled can improve performance. In most cases, the default value of enabled provides optimal performance. Only disable this option after performing application benchmarking to verify improved performance in the environment. 


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`DcuIpPrefetcher` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### DcuStreamPrefetcher

Use this option to disable the processor DCU Stream Prefetcher feature. In some cases, setting this option to disabled can improve performance. Typically, setting this option to enabled provides better performance. Only disable this option after performing application benchmarking to verify improved performance in your environment.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`DcuStreamPrefetcher` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### Dhcpv4

When enabled, this option enables obtaining the pre-boot network IPv4 configuration from a DHCP server. Individual settings are not available. When disabled, you must configure static IP address settings individually.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`Dhcpv4` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### DynamicPowerCapping

Use this option to configure when the System BIOS executes power calibration during the boot process. In Auto mode, calibration is run the first time the server is booted, and is then only run again when the server's hardware configuration or configuration settings change. When disabled, the calibration does not run, and Dynamic Power Capping is not supported. When enabled, the calibration is run on every boot.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`DynamicPowerCapping` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Auto`|Auto
|`Enabled`|Enabled
|`Disabled`|Disabled
### EmbNicAspm

Use this option to configure the PCIe Link Power Management (ASPM) support for the selected device. When configured for L0s Enabled, the selected device's link enters a standby energy savings state. When configured for L1 Enabled, the selected device's link enters a lower power standby state at the expense of a longer exit latency. When configured for L1 and L0s Enabled, the selected device's link enters either power savings mode, depending on link utilization, and provides the highest energy savings.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`EmbNicAspm` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Auto`|Auto
|`Disabled`|Disabled
|`AspmL1Enabled`|L1 Enabled
### EmbNicEnable

Select this option to enable or disable PCI devices.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`EmbNicEnable` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Auto`|Auto
|`Disabled`|Disabled
### EmbNicLinkSpeed

Use this option to configure the PCIe Link Speed for the selected device. When configured for Auto, the selected device trains at the maximum supported speed of the PCIe link. When configured for PCIe Generation 2 Link Speed, the selected device trains at a maximum of PCIe Generation 2 speed. When configured for PCIe Generation  Link 1 speed, the selected device trains at a maximum of PCIe Generation 1 speed.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`EmbNicLinkSpeed` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Auto`|Auto
|`PcieGen1`|PCIe Generation 1.0
### EmbNicPCIeOptionROM

Use this option to enable or disable Device Option ROM 


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`EmbNicPCIeOptionROM` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### EmbSas1Aspm

Use this option to configure the PCIe Link Power Management (ASPM) support for the selected device. When configured for L0s Enabled, the selected device's link enters a standby energy savings state. When configured for L1 Enabled, the selected device's link enters a lower power standby state at the expense of a longer exit latency. When configured for L1 and L0s Enabled, the selected device's link enters either power savings mode, depending on link utilization, and provides the highest energy savings.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`EmbSas1Aspm` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Auto`|Auto
|`Disabled`|Disabled
|`AspmL1Enabled`|L1 Enabled
### EmbSas1Boot

When Boot All Targets is selected, all valid boot targets attached to the storage controller are made available in the UEFI Boot Order list. If Boot No Targets is selected, no boot targets from this storage controller are made available in the UEFI Boot Order list.If Boot Limit to 24 Targets is selected, 24 boot targets attached to the storage controller are made available in the UEFI Boot Order list.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`EmbSas1Boot` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`AllTargets`|Boot All Targets
|`TwentyFourTargets`|Boot Limit to 24 Targets
|`NoTargets`|Boot No Targets
### EmbSas1Enable

Select this option to enable or disable PCI devices.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`EmbSas1Enable` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Auto`|Auto
|`Disabled`|Disabled
### EmbSas1LinkSpeed

Use this option to configure the PCIe Link Speed for the selected device. When configured for Auto, the selected device trains at the maximum supported speed of the PCIe link. When configured for PCIe Generation 2 Link Speed, the selected device trains at a maximum of PCIe Generation 2 speed. When configured for PCIe Generation  Link 1 speed, the selected device trains at a maximum of PCIe Generation 1 speed.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`EmbSas1LinkSpeed` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Auto`|Auto
|`PcieGen1`|PCIe Generation 1.0
|`PcieGen2`|PCIe Generation 2.0
### EmbSas1PcieOptionROM

Use this option to enable or disable Device Option ROM 


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`EmbSas1PcieOptionROM` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### EmbSata1Aspm

Use this option to enable or disable Aggressive Link Power Management(SALP).


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`EmbSata1Aspm` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Disabled`|Disabled
|`Enabled`|Enabled
### EmbSata1Enable

Select this option to enable or disable SATA devices.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`EmbSata1Enable` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Auto`|Auto
|`Disabled`|Disabled
### EmbSata1PCIeOptionROM

Use this option to enable or disable Device Option ROM 


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`EmbSata1PCIeOptionROM` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### EmbSata2Aspm

Use this option to enable or disable Aggressive Link Power Management(SALP).


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`EmbSata2Aspm` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Disabled`|Disabled
|`Enabled`|Enabled
### EmbSata2Enable

Select this option to enable or disable PCI devices.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`EmbSata2Enable` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Auto`|Auto
|`Disabled`|Disabled
### EmbSata2PCIeOptionROM

Use this option to enable or disable Device Option ROM 


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`EmbSata2PCIeOptionROM` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### EmbVideoConnection

When configured for Auto mode, the external video connection to the embedded video controller is automatically disabled to save power when a monitor is not attached. It is automatically enabled when a monitor is attached, including when the server is operating. When configured for Always Disabled, the external video connection to the embedded video controller is disabled, and a monitor connected to this port does not display except during system boot. This can be used for security reasons. When configured for Always Enabled, the external video connection to the embedded video controller is always enabled. This option is only required if a monitor is attached with a monitor detection that does not function properly (making AUTO mode not work properly). Note: This option does not affect Integrated Remote Console video. Also, if you press F9 or F11 during system boot, the configured video connector behavior is overridden, and the video console remains enabled. This lets you reconfigure the Embedded Video Connection option even if the video is disabled.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`EmbVideoConnection` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Auto`|Auto
|`AlwaysDisabled`|Always Disabled
|`AlwaysEnabled`|Always Enabled
### EmbeddedDiagnostics

Use this option to enable or disable Embedded Diagnostics functionality. If disabled, you cannot launch Embedded Diagnostics. Enable this option to use the Embedded Diagnostics functionality.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`EmbeddedDiagnostics` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### EmbeddedDiagsMode

Use this option to configure Embedded Diagnostics in Auto or Text Console mode.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`EmbeddedDiagsMode` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Auto`|Auto
|`TextConsole`|Text Console
### EmbeddedSata

Important: Smart Array SW RAID is not supported when Boot Mode is set to Legacy BIOS Mode. 

Use this option to configure the embedded chipset SATA controller. When selecting the Advanced Host Controller Interface (AHCI) or RAID (if supported), make sure the proper operating system drivers are used for proper operation.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`EmbeddedSata` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Ahci`|SATA AHCI Support
|`Raid`|Smart Array SW RAID Support
### EmbeddedSerialPort

Select this option to assign the logical COM port address and associated default resources to the selected physical serial port. The operating system can overwrite this setting.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`EmbeddedSerialPort` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Com1Irq4`|COM 1; IRQ4; I/O: 3F8h-3FFh
|`Com2Irq3`|COM 2; IRQ3; I/O: 2F8h-2FFh
|`Disabled`|Disabled
### EmbeddedUefiShell

Use this option to enable or disable the Embedded UEFI Shell. When enabled, you can launch the Embedded UEFI Shell from the pre-boot environment. When enabled and the Boot Mode is configured for UEFI Mode, you can add the Embedded UEFI Shell to the UEFI Boot Order list  by selecting the option entitled 'Add Embedded UEFI Shell to Boot Order'. When disabled, the Embedded UEFI Shell is not available in the pre-boot environment, and you cannot add it to the UEFI Boot Order list. The Embedded UEFI Shell is a pre-boot command line environment that you can use for scripting and running UEFI applications. It provides CLI-based commands to configure the server, update the System BIOS and other firmware, and obtain system information and error logs.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`EmbeddedUefiShell` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### EmsConsole

Use this option to configure the ACPI serial port settings, which include the ability to redirect the Windows Server Emergency Management console (EMS) through either the physical or virtual serial port.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`EmsConsole` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Disabled`|Disabled
|`Physical`|Physical Serial Port
|`Virtual`|Virtual Serial Port
### EnabledCoresPerProc

This option enables limiting the number of enabled processor cores per physical processor. You can set the number of enabled cores to a value supported by the physical processor. Setting the value to 0 or a value larger than the number of supported cores of the installed processor will result in all processor cores in the socket being enabled.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|Yes (if resource allows PATCH)
### EnergyEfficientTurbo

This option controls whether the processor uses an energy efficiency based policy when engaging turbo range frequencies. This option is only applicable when Turbo Mode is enabled.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`EnergyEfficientTurbo` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### EnergyPerfBias

You can only configure this option if the Workload Profile is set to Custom. Use this option to configure several processor subsystems to optimize the performance and power usage of the processor. Balanced Performance provides optimum power efficiency, and is recommended for most environments. Maximum Performance Mode is recommended for environments that require the highest performance and lowest latency but are not sensitive to power consumption. Only use Power Savings Mode in environments that are power sensitive and can accept reduced performance.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`EnergyPerfBias` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`MaxPerf`|Maximum Performance
|`BalancedPerf`|Balanced Performance
|`BalancedPower`|Balanced Power
|`PowerSavingsMode`|Power Savings Mode
### EraseUserDefaults

Select this option to erase the user defaults backup.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`EraseUserDefaults` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`No`|No, Cancel
|`Yes`|Yes, erase the current settings.
### ExtendedAmbientTemp

Use this option to enable the server to operate at higher ambient temperatures than normally supported. These options are only supported with specific hardware configurations. See your server documentation before configuring the server to enable extended ambient temperature support. Improper system operation or damage to hardware components can result from enabling these options in unsupported configurations. Selecting Enabled for 40c Ambient (ASHRAE 3) enables the server to operate in environments with ambient temperatures up to 40 degrees Celsius. Selecting Enabled for 45c Ambient (ASHRAE 4) enables the server to operate in environments with ambient temperatures up to 45 degrees Celsius. Not all servers support both 40c Ambient (ASHRAE 3) and 45c Ambient (ASHRAE 4).


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`ExtendedAmbientTemp` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Disabled`|Disabled
|`ASHRAE3`|Enabled for 40c Ambient (ASHRAE 3)
|`ASHRAE4`|Enabled for 45c Ambient (ASHRAE 4)
### ExtendedMemTest

When enabled, the system validates memory during the memory initialization process. If uncorrectable memory errors are detected, the memory is mapped out, and the failed DIMMs are logged to the Integrated Management Log (IML). Enabling this option can result in a significant increase in the server boot time.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`ExtendedMemTest` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### F11BootMenu

Use this option to disable the POST One-Time Boot F11 Prompt.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`F11BootMenu` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### FCScanPolicy

Use this option to change the default Fibre Channel or FCoE policy for scanning for boot targets. When configured for Scan All Targets, each installed FC/FCoE adapter scans all available targets. When configured for Scan Configured Targets Only, the FC/FCoE adapters only scan targets that are preconfigured in the devices settings. This option overrides any individual device settings configured in the device-specific setup.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`FCScanPolicy` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`AllTargets`|Scan All Targets
|`CardConfig`|Scan Configured Targets Only
### FanFailPolicy

Use this option to configure how the server reacts when fans fail, resulting in the server not having required fans in operation. When configured for "Shutdown/Halt on Critical Fan Failures," the server cannot boot or operate when it does not have required fans operating due to one or more fan failures.  When configured for "Allow Operation with Critical Fan Failures," the server can boot and operate if it does not have required fans operating due to one or more fan failures. It is recommended that you configure the Fan Failure Policy to the default state of "Shutdown/Halt on Critical Fan Failures." Operating without the required fans operating can result in damage to hardware components.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`FanFailPolicy` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Shutdown`|Shutdown/Halt on Critical Fan Failures
|`Allow`|Allow Operation with Critical Fan Failures
### FanInstallReq

Use this option to configure how the server reacts when all required fans are not installed. When configured for Enable Messaging, the server displays messages and log events to the Integrated Management Log (IML) when required fans are not installed. The server can still boot and operate. When configured for Disable Messaging, the server does not display messages and log events when required fans are not installed. All indications that the server is operating without required fans are removed. It is recommended that you leave Fan Installation Requirements in the default state of Enable Messaging. Operating without the required fans can result in damage to hardware components.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`FanInstallReq` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`EnableMessaging`|Enable Messaging
|`DisableMessaging`|Disable Messaging
### FlexLom1Aspm

Use this option to configure the PCIe Link Power Management (ASPM) support for the selected device. When configured for L0s Enabled, the selected device's link enters a standby energy savings state. When configured for L1 Enabled, the selected device's link enters a lower power standby state at the expense of a longer exit latency. When configured for L1 and L0s Enabled, the selected device's link enters either power savings mode, depending on link utilization, and provides the highest energy savings.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`FlexLom1Aspm` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Auto`|Auto
|`Disabled`|Disabled
|`AspmL1Enabled`|L1 Enabled
### FlexLom1Enable

Select this option to enable or disable PCI devices.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`FlexLom1Enable` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Auto`|Auto
|`Disabled`|Disabled
### FlexLom1LinkSpeed

Use this option to configure the PCIe Link Speed for the selected device. When configured for Auto, the selected device trains at the maximum supported speed of the PCIe link. When configured for PCIe Generation 2 Link Speed, the selected device trains at a maximum of PCIe Generation 2 speed. When configured for PCIe Generation  Link 1 speed, the selected device trains at a maximum of PCIe Generation 1 speed.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`FlexLom1LinkSpeed` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Auto`|Auto
|`PcieGen1`|PCIe Generation 1.0
|`PcieGen2`|PCIe Generation 2.0
### FlexLom1PCIeOptionROM

Use this option to enable or disable Device Option ROM 


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`FlexLom1PCIeOptionROM` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### HpeScalablePmemConfigurationEnabled

When enabled, the persistent memory regions may be re-configured. A reconfiguration will not be allowed if the current Backup state is 'Pending'.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`HpeScalablePmemConfigurationEnabled` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### HpeScalablePmemConfigurationRestoration

When enabled, the persistent memory configuration contained on the storage devices will be restored.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`HpeScalablePmemConfigurationRestoration` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### HpeScalablePmemFunctionalityEnabled

When enabled, data in the persistent memory regions will be saved to non-volantile storage upon power loss and power events. Note that enabling this option will disable the following options:  Advanced Memory Protection, Node Interleaving, Memory Fast Training, Extended Memory Test,  Memory Clear on Warm Reset, Memory Mirroring, Online Spare Memory, and ADDDC. For more information: http://www.hpe.com/support/NVDIMM 


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`HpeScalablePmemFunctionalityEnabled` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### HpeScalablePmemStorageInitialize

When enabled, the persistent memory Storage devices will be reinitialized on the next boot.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`HpeScalablePmemStorageInitialize` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### HttpSupport

Use this option to control the UEFI HTTP(s) boot support when in UEFI Mode, and the 'Discover Shell Auto-Start Script using DHCP' option under 'Embedded UEFI Shell' settings.
When 'Auto' is selected, the system automatically adds HTTP(S) boot options to the UEFI Boot Order list for every network port that is enabled for Network Boot. Selecting this option enables the system to boot to the HTTP or HTTPS URLs provided by the DHCP server. Any other URLs provided by the DHCP server are ignored. 
When 'HTTP only' is selected, the system automatically adds HTTP boot options to the UEFI Boot Order list for every network port that is enabled for Network Boot. Selecting this option enables the system to boot to the HTTP URLs provided by the DHCP server, and to ignore any HTTPS or other URLs that are provided. 
When 'HTTPS only' is selected, the system automatically adds HTTPS boot options to the UEFI Boot Order list for every network port that is enabled for Network Boot. Selecting this option enables the system to boot to the HTTPS URLs provided by the DHCP server, and to ignore any HTTP or other URLs that are provided. 
To enable HTTPS boot either by selecting 'Auto' or 'HTTPS only', you must enroll the respective TLS certificate of the HTTPS server under Server Security > TLS(HTTPS) Options. 
Note: This setting only affects the HTTP boot options added for the network ports, and the Discover Shell Auto-Start Script provided by the DHCP server. Other settings, such as Boot from URL, are not affected by this setting.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`HttpSupport` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Auto`|Auto
|`HttpsOnly`|HTTPS only
|`HttpOnly`|HTTP only
|`Disabled`|Disabled
### HwPrefetcher

Use this option to disable the processor HW prefetch feature. In some cases, setting this option to disabled can improve performance. Typically, setting this option to enabled provides better performance. Only disable this option after performing application benchmarking to verify improved performance in the environment.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`HwPrefetcher` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### IntelDmiLinkFreq

Use this option to force the link speed between the processor and the southbridge to run at slower speeds to save power.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`IntelDmiLinkFreq` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Auto`|Auto
|`DmiGen1`|Gen 1 Speed
|`DmiGen2`|Gen 2 Speed
### IntelNicDmaChannels

Use this option to select the Intel NIC DMA Channels support. This is a NIC acceleration option that only runs on Intel-based NICs.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`IntelNicDmaChannels` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### IntelPerfMonitoring

This option does not impact performance. When enabled, this option exposes certain chipset devices that can be used with the Intel Performance Monitoring Toolkit.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`IntelPerfMonitoring` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Disabled`|Disabled
|`Enabled`|Enabled
### IntelProcVtd

If enabled, a hypervisor or operating system supporting this option can use hardware capabilities provided by Intel VT for Directed I/O. You can leave this set to enabled even if you are not using a hypervisor or an operating system that uses this option.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`IntelProcVtd` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### IntelTxt

Use this option to modify Intel TXT support.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`IntelTxt` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### IntelUpiFreq

Use this option to set the UPI Link frequency to a lower speed. Running at a lower frequency can reduce power consumption, but can also affect system performance. You can only configure this option if two or more CPUs are present and the Workload Profile is set to custom.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`IntelUpiFreq` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Auto`|Auto
|`MinUpiSpeed`|Min UPI Speed
### IntelUpiLinkEn

Use this option to configure the UPI topology to use fewer links between processors, when available. Changing from the default can reduce UPI bandwidth performance in exchange for less power consumption.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`IntelUpiLinkEn` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Auto`|Auto
|`SingleLink`|Single Link Operation
### IntelUpiPowerManagement

Use this option to place the Quick Path Interconnect (UPI) links into a low power state when the links are not being used. This lowers power usage with minimal effect on performance. You can only configure this option if two or more CPUs are present and the Workload Profile is set to custom.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`IntelUpiPowerManagement` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### IntelligentProvisioning

Use this option to enable or disable the Intelligent Provisioning functionality. When disabled, you are prevented from entering the Intelligent Provisioning environment by pressing F10 during server boot. You must set this option to enabled to use Intelligent Provisioning functionality.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`IntelligentProvisioning` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### InternalSDCardSlot

Use this option to enable or disable the Internal SD Card Slot. When set to disabled, the SD card slot is disabled, regardless of whether an SD Card is installed or not. The SD Card will not be visible in the pre-boot environment or under the operating system.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`InternalSDCardSlot` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### Ipv4Address

Use this option to specify the pre-boot network IPv4 address. Enter a static IP address using dotted-decimal notation (for example, 127.0.0.1). If DHCP is used (the DHCPv4 option is enabled), this setting is unavailable because the value is supplied automatically.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
### Ipv4Gateway

Use this option to specify the pre-boot network gateway IPv4 address. Enter a static IP address using dotted-decimal notation (for example, 127.0.0.1). If DHCP is used (the DHCPv4 option is enabled), this setting is unavailable because the value is supplied automatically.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
### Ipv4PrimaryDNS

Use this option to specify the pre-boot network Primary DNS Server IPv4 address. Enter a static IP address using dotted-decimal notation (for example, 127.0.0.1). If DHCP is used (the DHCPv4 option is enabled), this setting is unavailable because the value is supplied automatically.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
### Ipv4SecondaryDNS

Use this option to specify the pre-boot network Secondary DNS Server IPv4 address. Enter a static IP address using dotted-decimal notation (for example, 127.0.0.1). If DHCP is used (the DHCPv4 option is enabled), this setting is unavailable because the value is supplied automatically.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
### Ipv4SubnetMask

Use this option to specify the pre-boot network subnet mask. Enter a static IP address using dotted-decimal notation (for example, 255.255.255.0). If DHCP is used (the DHCPv4 option is enabled), this setting is unavailable because the value is supplied automatically.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
### Ipv6Address

Use this option to specify the pre-boot network IPv6 address. Enter a static IP address in the standard colon seperated format (for example, 1234::1000). If IPv6 Config Policy is set to Automatic, this setting is unavailable because the value is supplied automatically.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
### Ipv6ConfigPolicy

When set to Automatic, this option enables obtaining the pre-boot network IPv6 configuration automatically. Individual settings are not available. When set to Manual, you must configure static IP address settings individually.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`Ipv6ConfigPolicy` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Automatic`|Automatic
|`Manual`|Manual
### Ipv6Duid

Use this option to control the IPv6 DHCP Unique Identifier (DUID). If configured for Auto, the DUID is set using the Universal Unique Identifier (UUID) of the server, or using the DUID-LLT method if the server UUID is not available. If configured for DUID-LLT, the DUID is set based on the Link-layer Address Plus Time [DUID-LLT] method. 


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`Ipv6Duid` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Auto`|Auto
|`DuidLlt`|DUID-LLT
### Ipv6Gateway

Use this option to specify the pre-boot network gateway IPv6 address. Enter a static IP address in the standard colon seperated format (for example, 1234::1000). If IPv6 Config Policy is set to Automatic, this setting is unavailable because the value is supplied automatically.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
### Ipv6PrimaryDNS

Use this option to specify the pre-boot network Primary DNS Server IPv6 address. Enter a static IP address in the standard colon seperated format (for example, 1234::1000). If IPv6 Config Policy is set to Automatic, this setting is unavailable because the value is supplied automatically.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
### Ipv6SecondaryDNS

Use this option to specify the pre-boot network Secondary DNS Server IPv6 address. Enter a static IP address in the standard colon seperated format (for example, 1234::1000). If IPv6 Config Policy is set to Automatic, this setting is unavailable because the value is supplied automatically.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
### LlcPrefetch

Use this option to configure the processor Last Level Cache (LLC) prefetch feature. In some cases, setting this option to disabled can improve performance. Typically, setting this option to enabled provides better performance. Only disable this option after performing application benchmarking to verify improved performance in the environment.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`LlcPrefetch` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### LocalRemoteThreshold

Local/Remote Threshold setting.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`LocalRemoteThreshold` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Auto`|Auto
|`Low`|Low
|`Medium`|Medium
|`High`|High
|`Disabled`|Disabled
### MaxMemBusFreqMHz

You can only configure this option if the Workload Profile is set to Custom. Use this option to configure the memory system to run memory at a lower maximum speed than that supported by the installed processor and DIMM configuration. Setting this option to Auto configures the system to run memory at the maximum speed supported.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`MaxMemBusFreqMHz` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Auto`|Auto
|`MaxMemBusFreq2667`|2667 MHz
|`MaxMemBusFreq2400`|2400 MHz
|`MaxMemBusFreq2133`|2133 MHz
|`MaxMemBusFreq1867`|1867 MHz
### MaxPcieSpeed

You can only configure this option if the Workload Profile is set to Custom. If a PCI Express device does not run properly at its optimal speed, lowering the speed at which the device is running can address this issue. This option enables you to lower the maximum PCI Express speed at which the server allows PCI Express devices to operate. You can also use it to address issues with problematic PCI Express devices. Setting this value to Maximum Supported configures the platform to run at the maximum speed supported by the platform or the PCIe device, whichever is lower.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`MaxPcieSpeed` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`PerPortCtrl`|Per Port Control
|`PcieGen1`|PCIe Generation 1.0
### MemClearWarmReset

Use this option to configure when memory is cleared on warm resets. When disabled, the contents of memory are only cleared on a warm reset if requested by the operating system. When enabled, memory is cleared on all reboots. Disabling this option can save boot time by skipping the clearing of memory on warm resets.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`MemClearWarmReset` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### MemFastTraining

This option enables a boot time reduction by controlling when the BIOS bypasses the full memory training. When enabled, the server bypasses the full memory training during boot, and uses memory parameters determined on a previous boot to decrease boot time. Note that even when enabled, the BIOS performs a full memory training if the DIMM configuration or processor configuration changes, or if there is a change in any BIOS setting related to memory or processor configuration. When disabled, the server performs a full memory training on every server boot.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`MemFastTraining` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### MemMirrorMode

Use this option to select from the available Memory Mirroring modes. Full Mirror - reserves 50% of the total available memory for mirroring. Partial Mirror (20% above 4GB) - reserves 20% of the total available Memory above 4GB for Mirroring. Partial Mirror (10% above 4GB) - reserves 10% of the total available Memory above 4GB for Mirroring. Partial Mirror (Memory below 4GB) - depending on the memory configuration, sets up 2GB or 3GB of lower memory below 4GB for Mirroring. Partial Mirror (OS Configured) - sets up the system to configure Partial Mirroring at OS level. 


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`MemMirrorMode` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Full`|Full Mirror
|`PartialOsConfig`|Partial Mirror (OS Configured)
|`PartialFirst4GB`|Partial Mirror (Memory below 4GB)
|`Partial10PercentAbove4GB`|Partial Mirror (10% above 4GB)
|`Partial20PercentAbove4GB`|Partial Mirror (20% above 4GB)
### MemPatrolScrubbing

This option corrects memory soft errors so that, over the length of the system runtime, the risk of producing multi-bit and uncorrectable errors is reduced.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`MemPatrolScrubbing` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### MemRefreshRate

This option controls the refresh rate of the memory controller and might affect the performance and resiliency of the server memory. It is recommended that you leave this setting in the default state unless indicated in other documentation for this server.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`MemRefreshRate` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Refreshx1`|1x Refresh
|`Refreshx2`|2x Refresh
### MemoryRemap

Use this option to remap memory that may have been previously disabled from the system due to a failure event, such as an uncorrectable memory error. The Remap All Memory Option causes the system to make all memory in the system available again on the next boot. The No Action option leaves any affected memory unavailable to the system.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`MemoryRemap` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`NoAction`|No Action
|`AllMemory`|All Memory
### MinProcIdlePkgState

You can configure this option only if the Workload Profile is set to Custom. Use this option to select the lowest idle package power state (C-state) of the processor. The processor automatically transitions into package C-states based on the Core C-states in which cores on the processor have transitioned. The higher the package C-state, the lower the power usage of that idle package state. (Package C6 (retention) is the lowest power idle package state supported by the processor).


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`MinProcIdlePkgState` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`C6Retention`|Package C6 (retention) State
|`C6NonRetention`|Package C6 (non-retention) State
|`NoState`|No Package State
### MinProcIdlePower

You can only configure this option if Workload Profile is set to Custom. Use this option to select the lowest idle power state (C-state) of the processor that the operating system uses. The higher the C-state, the lower the power usage of that idle state. (C6 is the lowest power idle state supported by the processor).


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`MinProcIdlePower` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`C6`|C6 State
|`C1E`|C1E State
|`NoCStates`|No C-states
### MixedPowerSupplyReporting

When enabled, the server logs a message that a mixed power supply configuration is present. When disabled, the server no longer logs messages that a mixed power supply configuration is present.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`MixedPowerSupplyReporting` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### NetworkBootRetry

Use this option to configure the Network Boot Retry Support. When enabled, the system BIOS attempts to boot the network device up to the number of times configured in the Network Boot Retry Count option before attempting to boot the next network device. This setting only takes effect when attempting to boot a network device from the F12 function key and one-time boot options.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`NetworkBootRetry` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### NetworkBootRetryCount

Use this option to control the number of times the system BIOS attempts to boot a network device.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|Yes (if resource allows PATCH)
### NicBoot1

Use this option to enable or disable network boot (PXE, iSCSI, FCoE or UEFI HTTP) for the selected NIC. You might need to configure the NIC firmware for the boot option to be active.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`NicBoot1` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`NetworkBoot`|Network Boot
|`Disabled`|Disabled
### NicBoot10

Use this option to enable or disable network boot (PXE, iSCSI, FCoE or UEFI HTTP) for the selected NIC. You might need to configure the NIC firmware for the boot option to be active.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`NicBoot10` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`NetworkBoot`|Network Boot
|`Disabled`|Disabled
### NicBoot11

Use this option to enable or disable network boot (PXE, iSCSI, FCoE or UEFI HTTP) for the selected NIC. You might need to configure the NIC firmware for the boot option to be active.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`NicBoot11` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`NetworkBoot`|Network Boot
|`Disabled`|Disabled
### NicBoot12

Use this option to enable or disable network boot (PXE, iSCSI, FCoE or UEFI HTTP) for the selected NIC. You might need to configure the NIC firmware for the boot option to be active.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`NicBoot12` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`NetworkBoot`|Network Boot
|`Disabled`|Disabled
### NicBoot2

Use this option to enable or disable network boot (PXE, iSCSI, FCoE or UEFI HTTP) for the selected NIC. You might need to configure the NIC firmware for the boot option to be active.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`NicBoot2` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`NetworkBoot`|Network Boot
|`Disabled`|Disabled
### NicBoot3

Use this option to enable or disable network boot (PXE, iSCSI, FCoE or UEFI HTTP) for the selected NIC. You might need to configure the NIC firmware for the boot option to be active.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`NicBoot3` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`NetworkBoot`|Network Boot
|`Disabled`|Disabled
### NicBoot4

Use this option to enable or disable network boot (PXE, iSCSI, FCoE or UEFI HTTP) for the selected NIC. You might need to configure the NIC firmware for the boot option to be active.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`NicBoot4` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`NetworkBoot`|Network Boot
|`Disabled`|Disabled
### NicBoot5

Use this option to enable or disable network boot (PXE, iSCSI, FCoE or UEFI HTTP) for the selected NIC. You might need to configure the NIC firmware for the boot option to be active.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`NicBoot5` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`NetworkBoot`|Network Boot
|`Disabled`|Disabled
### NicBoot6

Use this option to enable or disable network boot (PXE, iSCSI, FCoE or UEFI HTTP) for the selected NIC. You might need to configure the NIC firmware for the boot option to be active.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`NicBoot6` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`NetworkBoot`|Network Boot
|`Disabled`|Disabled
### NicBoot7

Use this option to enable or disable network boot (PXE, iSCSI, FCoE or UEFI HTTP) for the selected NIC. You might need to configure the NIC firmware for the boot option to be active.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`NicBoot7` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`NetworkBoot`|Network Boot
|`Disabled`|Disabled
### NicBoot8

Use this option to enable or disable network boot (PXE, iSCSI, FCoE or UEFI HTTP) for the selected NIC. You might need to configure the NIC firmware for the boot option to be active.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`NicBoot8` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`NetworkBoot`|Network Boot
|`Disabled`|Disabled
### NicBoot9

Use this option to enable or disable network boot (PXE, iSCSI, FCoE or UEFI HTTP) for the selected NIC. You might need to configure the NIC firmware for the boot option to be active.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`NicBoot9` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`NetworkBoot`|Network Boot
|`Disabled`|Disabled
### NodeInterleaving

Use this option to disable the NUMA architecture properties for the system. All operating system platforms support NUMA architectures. In most cases, optimum performance is obtained by disabling the Node Interleaving option. When this option is enabled, memory addresses are interleaved across the memory installed for each processor. Some workloads might experience improved performance when this option is enabled. Node Interleaving cannot be enabled when NVDIMMs are present in the system.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`NodeInterleaving` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### NumaGroupSizeOpt

Use this option to configure how the System BIOS reports the size of a NUMA node (number of logical processors), which assists the Operating System in grouping processors for application use (referred to as Kgroups). The default setting of Clustered provides better performance due to optimizing the resulting groups along NUMA boundaries. However, some applications might not be optimized to take advantage of processors spanning multiple groups. In such cases, selecting the Flat option might be necessary in order for those applications to utilize more logical processors.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`NumaGroupSizeOpt` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Flat`|Flat
|`Clustered`|Clustered
### NvDimmNMemFunctionality

This option controls whether NVDIMM-N support (including backing up the contents of the memory to flash on power down or reset) is enabled. If this option is configured for Disabled, then the NVDIMMs of type NVDIMM-N in the system are NOT used by the operating system as persistent storage, and are NOT used by the operating system as system memory.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`NvDimmNMemFunctionality` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### NvDimmNMemInterleaving

This option controls whether the NVDIMMs of type NVDIMM-N installed on a particular processor will be interleaved with each other in the memory map. This option does NOT impact the interleaving of standard DIMMs, and interleaving is never enabled across NVDIMMs of type NVDIMM-N and standard DIMMs. NVDIMMs of type NVDIMM-N installed on different processors are never interleaved together. If this setting is changed, then all installed NVDIMMs of type NVDIMM-N must be sanitized.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`NvDimmNMemInterleaving` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### NvDimmNSanitizePolicy

This option is used to Sanitize/Erase all user data and error status data saved in the selected NVDIMMs of type NVDIMM-N. Selected NVDIMMs of type NVDIMM-N are sanitized/erased on the next reboot of the system. This process is required BEFORE the NVDIMM-N Memory Interleaving option can be modified. An NVDIMM-N must be sanitized/erased when it is initially installed in the system or installed in a different DIMM slot on the system. In addition, an NVDIMM-N can be recovered to normal operation if it has received an Uncorrectable Memory Error, a Backup Error, a Restore Error, or an Arming Error (if the NVDIMM hardware is functional). Note that the largest group of NVDIMMs of type NVDIMM-N selected are sanitized/erased. For instance, if 'Sanitize/Erase all NVDIMM-N on Processor 1' is enabled and 'Sanitize/Erase Processor 1 DIMM 8' is disabled, all NVDIMMs of type NVDIMM-N on Processor 1 are sanitized/erased including Processor 1 DIMM 8. There are four policies that control the action of the system after NVDIMMs of type NVDIMM-N are sanitized/erased. The options are to power off the system after sanitizing/erasing NVDIMMs, to enable the system to boot to the operating system after sanitizing/erasing NVDIMMs, to boot to the System Utilities after sanitizing/erasing NVDIMMs, or to sanitize/erase the NVDIMMs back to the factory default settings and power off the system. 'Sanitize/Erase to Factory Defaults and Power System Off' is recommended when retiring the NVDIMMs with no intention of reuse.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`NvDimmNSanitizePolicy` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Disabled`|Disabled
|`SanitizeAndRebootSystem`|Sanitize/Erase and Boot to Operating System
|`SanitizeAndShutdownSystem`|Sanitize/Erase and Power System Off
|`SanitizeAndBootToFirmwareUI`|Sanitize/Erase and Boot to System Utilities
|`SanitizeToFactoryDefaults`|Sanitize/Erase to Factory Defaults and Power System Off
### NvmeDrive1

Use this option to configure different NVM Express Drives Usage. When NVMe is selected, NVM Express Drive is used as storeage device. When Scalable PMEM is selected, NVM Express Drive is used as Logical NVDIMM Backup/Restore device.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`NvmeDrive1` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Nvme`|NVMe
|`ScalablePMEM`|Scalable PMEM
### NvmeDrive10

Use this option to configure different NVM Express Drives Usage. When NVMe is selected, NVM Express Drive is used as storeage device. When Scalable PMEM is selected, NVM Express Drive is used as Logical NVDIMM Backup/Restore device.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`NvmeDrive10` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Nvme`|NVMe
|`ScalablePMEM`|Scalable PMEM
### NvmeDrive11

Use this option to configure different NVM Express Drives Usage. When NVMe is selected, NVM Express Drive is used as storeage device. When Scalable PMEM is selected, NVM Express Drive is used as Logical NVDIMM Backup/Restore device.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`NvmeDrive11` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Nvme`|NVMe
|`ScalablePMEM`|Scalable PMEM
### NvmeDrive12

Use this option to configure different NVM Express Drives Usage. When NVMe is selected, NVM Express Drive is used as storeage device. When Scalable PMEM is selected, NVM Express Drive is used as Logical NVDIMM Backup/Restore device.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`NvmeDrive12` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Nvme`|NVMe
|`ScalablePMEM`|Scalable PMEM
### NvmeDrive13

Use this option to configure different NVM Express Drives Usage. When NVMe is selected, NVM Express Drive is used as storeage device. When Scalable PMEM is selected, NVM Express Drive is used as Logical NVDIMM Backup/Restore device.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`NvmeDrive13` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Nvme`|NVMe
|`ScalablePMEM`|Scalable PMEM
### NvmeDrive14

Use this option to configure different NVM Express Drives Usage. When NVMe is selected, NVM Express Drive is used as storeage device. When Scalable PMEM is selected, NVM Express Drive is used as Logical NVDIMM Backup/Restore device.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`NvmeDrive14` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Nvme`|NVMe
|`ScalablePMEM`|Scalable PMEM
### NvmeDrive15

Use this option to configure different NVM Express Drives Usage. When NVMe is selected, NVM Express Drive is used as storeage device. When Scalable PMEM is selected, NVM Express Drive is used as Logical NVDIMM Backup/Restore device.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`NvmeDrive15` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Nvme`|NVMe
|`ScalablePMEM`|Scalable PMEM
### NvmeDrive16

Use this option to configure different NVM Express Drives Usage. When NVMe is selected, NVM Express Drive is used as storeage device. When Scalable PMEM is selected, NVM Express Drive is used as Logical NVDIMM Backup/Restore device.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`NvmeDrive16` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Nvme`|NVMe
|`ScalablePMEM`|Scalable PMEM
### NvmeDrive17

Use this option to configure different NVM Express Drives Usage. When NVMe is selected, NVM Express Drive is used as storeage device. When Scalable PMEM is selected, NVM Express Drive is used as Logical NVDIMM Backup/Restore device.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`NvmeDrive17` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Nvme`|NVMe
|`ScalablePMEM`|Scalable PMEM
### NvmeDrive18

Use this option to configure different NVM Express Drives Usage. When NVMe is selected, NVM Express Drive is used as storeage device. When Scalable PMEM is selected, NVM Express Drive is used as Logical NVDIMM Backup/Restore device.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`NvmeDrive18` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Nvme`|NVMe
|`ScalablePMEM`|Scalable PMEM
### NvmeDrive19

Use this option to configure different NVM Express Drives Usage. When NVMe is selected, NVM Express Drive is used as storeage device. When Scalable PMEM is selected, NVM Express Drive is used as Logical NVDIMM Backup/Restore device.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`NvmeDrive19` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Nvme`|NVMe
|`ScalablePMEM`|Scalable PMEM
### NvmeDrive2

Use this option to configure different NVM Express Drives Usage. When NVMe is selected, NVM Express Drive is used as storeage device. When Scalable PMEM is selected, NVM Express Drive is used as Logical NVDIMM Backup/Restore device.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`NvmeDrive2` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Nvme`|NVMe
|`ScalablePMEM`|Scalable PMEM
### NvmeDrive20

Use this option to configure different NVM Express Drives Usage. When NVMe is selected, NVM Express Drive is used as storeage device. When Scalable PMEM is selected, NVM Express Drive is used as Logical NVDIMM Backup/Restore device.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`NvmeDrive20` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Nvme`|NVMe
|`ScalablePMEM`|Scalable PMEM
### NvmeDrive21

Use this option to configure different NVM Express Drives Usage. When NVMe is selected, NVM Express Drive is used as storeage device. When Scalable PMEM is selected, NVM Express Drive is used as Logical NVDIMM Backup/Restore device.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`NvmeDrive21` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Nvme`|NVMe
|`ScalablePMEM`|Scalable PMEM
### NvmeDrive22

Use this option to configure different NVM Express Drives Usage. When NVMe is selected, NVM Express Drive is used as storeage device. When Scalable PMEM is selected, NVM Express Drive is used as Logical NVDIMM Backup/Restore device.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`NvmeDrive22` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Nvme`|NVMe
|`ScalablePMEM`|Scalable PMEM
### NvmeDrive23

Use this option to configure different NVM Express Drives Usage. When NVMe is selected, NVM Express Drive is used as storeage device. When Scalable PMEM is selected, NVM Express Drive is used as Logical NVDIMM Backup/Restore device.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`NvmeDrive23` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Nvme`|NVMe
|`ScalablePMEM`|Scalable PMEM
### NvmeDrive24

Use this option to configure different NVM Express Drives Usage. When NVMe is selected, NVM Express Drive is used as storeage device. When Scalable PMEM is selected, NVM Express Drive is used as Logical NVDIMM Backup/Restore device.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`NvmeDrive24` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Nvme`|NVMe
|`ScalablePMEM`|Scalable PMEM
### NvmeDrive25

Use this option to configure different NVM Express Drives Usage. When NVMe is selected, NVM Express Drive is used as storeage device. When Scalable PMEM is selected, NVM Express Drive is used as Logical NVDIMM Backup/Restore device.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`NvmeDrive25` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Nvme`|NVMe
|`ScalablePMEM`|Scalable PMEM
### NvmeDrive26

Use this option to configure different NVM Express Drives Usage. When NVMe is selected, NVM Express Drive is used as storeage device. When Scalable PMEM is selected, NVM Express Drive is used as Logical NVDIMM Backup/Restore device.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`NvmeDrive26` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Nvme`|NVMe
|`ScalablePMEM`|Scalable PMEM
### NvmeDrive27

Use this option to configure different NVM Express Drives Usage. When NVMe is selected, NVM Express Drive is used as storeage device. When Scalable PMEM is selected, NVM Express Drive is used as Logical NVDIMM Backup/Restore device.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`NvmeDrive27` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Nvme`|NVMe
|`ScalablePMEM`|Scalable PMEM
### NvmeDrive28

Use this option to configure different NVM Express Drives Usage. When NVMe is selected, NVM Express Drive is used as storeage device. When Scalable PMEM is selected, NVM Express Drive is used as Logical NVDIMM Backup/Restore device.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`NvmeDrive28` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Nvme`|NVMe
|`ScalablePMEM`|Scalable PMEM
### NvmeDrive29

Use this option to configure different NVM Express Drives Usage. When NVMe is selected, NVM Express Drive is used as storeage device. When Scalable PMEM is selected, NVM Express Drive is used as Logical NVDIMM Backup/Restore device.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`NvmeDrive29` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Nvme`|NVMe
|`ScalablePMEM`|Scalable PMEM
### NvmeDrive3

Use this option to configure different NVM Express Drives Usage. When NVMe is selected, NVM Express Drive is used as storeage device. When Scalable PMEM is selected, NVM Express Drive is used as Logical NVDIMM Backup/Restore device.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`NvmeDrive3` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Nvme`|NVMe
|`ScalablePMEM`|Scalable PMEM
### NvmeDrive30

Use this option to configure different NVM Express Drives Usage. When NVMe is selected, NVM Express Drive is used as storeage device. When Scalable PMEM is selected, NVM Express Drive is used as Logical NVDIMM Backup/Restore device.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`NvmeDrive30` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Nvme`|NVMe
|`ScalablePMEM`|Scalable PMEM
### NvmeDrive31

Use this option to configure different NVM Express Drives Usage. When NVMe is selected, NVM Express Drive is used as storeage device. When Scalable PMEM is selected, NVM Express Drive is used as Logical NVDIMM Backup/Restore device.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`NvmeDrive31` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Nvme`|NVMe
|`ScalablePMEM`|Scalable PMEM
### NvmeDrive32

Use this option to configure different NVM Express Drives Usage. When NVMe is selected, NVM Express Drive is used as storeage device. When Scalable PMEM is selected, NVM Express Drive is used as Logical NVDIMM Backup/Restore device.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`NvmeDrive32` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Nvme`|NVMe
|`ScalablePMEM`|Scalable PMEM
### NvmeDrive33

Use this option to configure different NVM Express Drives Usage. When NVMe is selected, NVM Express Drive is used as storeage device. When Scalable PMEM is selected, NVM Express Drive is used as Logical NVDIMM Backup/Restore device.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`NvmeDrive33` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Nvme`|NVMe
|`ScalablePMEM`|Scalable PMEM
### NvmeDrive34

Use this option to configure different NVM Express Drives Usage. When NVMe is selected, NVM Express Drive is used as storeage device. When Scalable PMEM is selected, NVM Express Drive is used as Logical NVDIMM Backup/Restore device.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`NvmeDrive34` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Nvme`|NVMe
|`ScalablePMEM`|Scalable PMEM
### NvmeDrive35

Use this option to configure different NVM Express Drives Usage. When NVMe is selected, NVM Express Drive is used as storeage device. When Scalable PMEM is selected, NVM Express Drive is used as Logical NVDIMM Backup/Restore device.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`NvmeDrive35` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Nvme`|NVMe
|`ScalablePMEM`|Scalable PMEM
### NvmeDrive36

Use this option to configure different NVM Express Drives Usage. When NVMe is selected, NVM Express Drive is used as storeage device. When Scalable PMEM is selected, NVM Express Drive is used as Logical NVDIMM Backup/Restore device.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`NvmeDrive36` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Nvme`|NVMe
|`ScalablePMEM`|Scalable PMEM
### NvmeDrive37

Use this option to configure different NVM Express Drives Usage. When NVMe is selected, NVM Express Drive is used as storeage device. When Scalable PMEM is selected, NVM Express Drive is used as Logical NVDIMM Backup/Restore device.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`NvmeDrive37` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Nvme`|NVMe
|`ScalablePMEM`|Scalable PMEM
### NvmeDrive38

Use this option to configure different NVM Express Drives Usage. When NVMe is selected, NVM Express Drive is used as storeage device. When Scalable PMEM is selected, NVM Express Drive is used as Logical NVDIMM Backup/Restore device.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`NvmeDrive38` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Nvme`|NVMe
|`ScalablePMEM`|Scalable PMEM
### NvmeDrive39

Use this option to configure different NVM Express Drives Usage. When NVMe is selected, NVM Express Drive is used as storeage device. When Scalable PMEM is selected, NVM Express Drive is used as Logical NVDIMM Backup/Restore device.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`NvmeDrive39` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Nvme`|NVMe
|`ScalablePMEM`|Scalable PMEM
### NvmeDrive4

Use this option to configure different NVM Express Drives Usage. When NVMe is selected, NVM Express Drive is used as storeage device. When Scalable PMEM is selected, NVM Express Drive is used as Logical NVDIMM Backup/Restore device.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`NvmeDrive4` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Nvme`|NVMe
|`ScalablePMEM`|Scalable PMEM
### NvmeDrive40

Use this option to configure different NVM Express Drives Usage. When NVMe is selected, NVM Express Drive is used as storeage device. When Scalable PMEM is selected, NVM Express Drive is used as Logical NVDIMM Backup/Restore device.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`NvmeDrive40` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Nvme`|NVMe
|`ScalablePMEM`|Scalable PMEM
### NvmeDrive41

Use this option to configure different NVM Express Drives Usage. When NVMe is selected, NVM Express Drive is used as storeage device. When Scalable PMEM is selected, NVM Express Drive is used as Logical NVDIMM Backup/Restore device.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`NvmeDrive41` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Nvme`|NVMe
|`ScalablePMEM`|Scalable PMEM
### NvmeDrive42

Use this option to configure different NVM Express Drives Usage. When NVMe is selected, NVM Express Drive is used as storeage device. When Scalable PMEM is selected, NVM Express Drive is used as Logical NVDIMM Backup/Restore device.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`NvmeDrive42` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Nvme`|NVMe
|`ScalablePMEM`|Scalable PMEM
### NvmeDrive43

Use this option to configure different NVM Express Drives Usage. When NVMe is selected, NVM Express Drive is used as storeage device. When Scalable PMEM is selected, NVM Express Drive is used as Logical NVDIMM Backup/Restore device.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`NvmeDrive43` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Nvme`|NVMe
|`ScalablePMEM`|Scalable PMEM
### NvmeDrive44

Use this option to configure different NVM Express Drives Usage. When NVMe is selected, NVM Express Drive is used as storeage device. When Scalable PMEM is selected, NVM Express Drive is used as Logical NVDIMM Backup/Restore device.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`NvmeDrive44` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Nvme`|NVMe
|`ScalablePMEM`|Scalable PMEM
### NvmeDrive45

Use this option to configure different NVM Express Drives Usage. When NVMe is selected, NVM Express Drive is used as storeage device. When Scalable PMEM is selected, NVM Express Drive is used as Logical NVDIMM Backup/Restore device.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`NvmeDrive45` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Nvme`|NVMe
|`ScalablePMEM`|Scalable PMEM
### NvmeDrive46

Use this option to configure different NVM Express Drives Usage. When NVMe is selected, NVM Express Drive is used as storeage device. When Scalable PMEM is selected, NVM Express Drive is used as Logical NVDIMM Backup/Restore device.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`NvmeDrive46` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Nvme`|NVMe
|`ScalablePMEM`|Scalable PMEM
### NvmeDrive47

Use this option to configure different NVM Express Drives Usage. When NVMe is selected, NVM Express Drive is used as storeage device. When Scalable PMEM is selected, NVM Express Drive is used as Logical NVDIMM Backup/Restore device.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`NvmeDrive47` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Nvme`|NVMe
|`ScalablePMEM`|Scalable PMEM
### NvmeDrive48

Use this option to configure different NVM Express Drives Usage. When NVMe is selected, NVM Express Drive is used as storeage device. When Scalable PMEM is selected, NVM Express Drive is used as Logical NVDIMM Backup/Restore device.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`NvmeDrive48` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Nvme`|NVMe
|`ScalablePMEM`|Scalable PMEM
### NvmeDrive49

Use this option to configure different NVM Express Drives Usage. When NVMe is selected, NVM Express Drive is used as storeage device. When Scalable PMEM is selected, NVM Express Drive is used as Logical NVDIMM Backup/Restore device.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`NvmeDrive49` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Nvme`|NVMe
|`ScalablePMEM`|Scalable PMEM
### NvmeDrive5

Use this option to configure different NVM Express Drives Usage. When NVMe is selected, NVM Express Drive is used as storeage device. When Scalable PMEM is selected, NVM Express Drive is used as Logical NVDIMM Backup/Restore device.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`NvmeDrive5` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Nvme`|NVMe
|`ScalablePMEM`|Scalable PMEM
### NvmeDrive50

Use this option to configure different NVM Express Drives Usage. When NVMe is selected, NVM Express Drive is used as storeage device. When Scalable PMEM is selected, NVM Express Drive is used as Logical NVDIMM Backup/Restore device.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`NvmeDrive50` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Nvme`|NVMe
|`ScalablePMEM`|Scalable PMEM
### NvmeDrive6

Use this option to configure different NVM Express Drives Usage. When NVMe is selected, NVM Express Drive is used as storeage device. When Scalable PMEM is selected, NVM Express Drive is used as Logical NVDIMM Backup/Restore device.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`NvmeDrive6` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Nvme`|NVMe
|`ScalablePMEM`|Scalable PMEM
### NvmeDrive7

Use this option to configure different NVM Express Drives Usage. When NVMe is selected, NVM Express Drive is used as storeage device. When Scalable PMEM is selected, NVM Express Drive is used as Logical NVDIMM Backup/Restore device.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`NvmeDrive7` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Nvme`|NVMe
|`ScalablePMEM`|Scalable PMEM
### NvmeDrive8

Use this option to configure different NVM Express Drives Usage. When NVMe is selected, NVM Express Drive is used as storeage device. When Scalable PMEM is selected, NVM Express Drive is used as Logical NVDIMM Backup/Restore device.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`NvmeDrive8` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Nvme`|NVMe
|`ScalablePMEM`|Scalable PMEM
### NvmeDrive9

Use this option to configure different NVM Express Drives Usage. When NVMe is selected, NVM Express Drive is used as storeage device. When Scalable PMEM is selected, NVM Express Drive is used as Logical NVDIMM Backup/Restore device.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`NvmeDrive9` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Nvme`|NVMe
|`ScalablePMEM`|Scalable PMEM
### NvmeOptionRom

Use this option to enable or disable embedded NVM Express Option ROM. When enabled, the system loads the NVM Express Option ROM provided by the system BIOS. When disabled, the system loads the NVM Express Option ROM provided by the adapter.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`NvmeOptionRom` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### OldAdminPassword

In order to set a new Admin Password, the previous Admin Password must be specified.


| | |
|---|---|
|JSON type|password|
|HTTP PATCH|Yes (if resource allows PATCH)
### OldPowerOnPassword

In order to set a new Power On Password, the previous Power On Password must be specified.


| | |
|---|---|
|JSON type|password|
|HTTP PATCH|Yes (if resource allows PATCH)
### PciResourcePadding

Use this option to configure PCIe resources to support PCIe hot-add for NVMe drives. When Normal is selected, PCIe resources are only allocated to devices installed at boot time, and PCIe hot-add is not supported. When Medium is selected, additional PCIe resources are allocated for each PCIe Root Port, which might enable a PCIe hot-add event to work without requiring a system reboot to enumerate the device. When High is selected, a maximum amount of PCIe resources are set aside to allow for the best chance of supporting a PCIe hot-add event.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`PciResourcePadding` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Normal`|Normal
|`Medium`|Medium
|`High`|High
### PciSlot1Aspm

Use this option to configure the PCIe Link Power Management (ASPM) support for the selected device. When configured for L0s Enabled, the selected device's link enters a standby energy savings state. When configured for L1 Enabled, the selected device's link enters a lower power standby state at the expense of a longer exit latency. When configured for L1 and L0s Enabled, the selected device's link enters either power savings mode, depending on link utilization, and provides the highest energy savings.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`PciSlot1Aspm` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Auto`|Auto
|`Disabled`|Disabled
|`AspmL1Enabled`|L1 Enabled
### PciSlot1Enable

Select this option to enable or disable PCI devices.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`PciSlot1Enable` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Auto`|Auto
|`Disabled`|Disabled
### PciSlot1LinkSpeed

Use this option to configure the PCIe Link Speed for the selected device. When configured for Auto, the selected device trains at the maximum supported speed of the PCIe link. When configured for PCIe Generation 2 Link Speed, the selected device trains at a maximum of PCIe Generation 2 speed. When configured for PCIe Generation  Link 1 speed, the selected device trains at a maximum of PCIe Generation 1 speed.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`PciSlot1LinkSpeed` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Auto`|Auto
|`PcieGen1`|PCIe Generation 1.0
|`PcieGen2`|PCIe Generation 2.0
### PciSlot1OptionROM

Use this option to enable or disable Device Option ROM 


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`PciSlot1OptionROM` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### PciSlot2Aspm

Use this option to configure the PCIe Link Power Management (ASPM) support for the selected device. When configured for L0s Enabled, the selected device's link enters a standby energy savings state. When configured for L1 Enabled, the selected device's link enters a lower power standby state at the expense of a longer exit latency. When configured for L1 and L0s Enabled, the selected device's link enters either power savings mode, depending on link utilization, and provides the highest energy savings.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`PciSlot2Aspm` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Auto`|Auto
|`Disabled`|Disabled
|`AspmL1Enabled`|L1 Enabled
### PciSlot2Enable

Select this option to enable or disable PCI devices.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`PciSlot2Enable` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Auto`|Auto
|`Disabled`|Disabled
### PciSlot2LinkSpeed

Use this option to configure the PCIe Link Speed for the selected device. When configured for Auto, the selected device trains at the maximum supported speed of the PCIe link. When configured for PCIe Generation 2 Link Speed, the selected device trains at a maximum of PCIe Generation 2 speed. When configured for PCIe Generation  Link 1 speed, the selected device trains at a maximum of PCIe Generation 1 speed.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`PciSlot2LinkSpeed` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Auto`|Auto
|`PcieGen1`|PCIe Generation 1.0
|`PcieGen2`|PCIe Generation 2.0
### PciSlot2OptionROM

Use this option to enable or disable Device Option ROM 


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`PciSlot2OptionROM` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### PciSlot3Aspm

Use this option to configure the PCIe Link Power Management (ASPM) support for the selected device. When configured for L0s Enabled, the selected device's link enters a standby energy savings state. When configured for L1 Enabled, the selected device's link enters a lower power standby state at the expense of a longer exit latency. When configured for L1 and L0s Enabled, the selected device's link enters either power savings mode, depending on link utilization, and provides the highest energy savings.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`PciSlot3Aspm` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Auto`|Auto
|`Disabled`|Disabled
|`AspmL1Enabled`|L1 Enabled
### PciSlot3Enable

Select this option to enable or disable PCI devices.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`PciSlot3Enable` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Auto`|Auto
|`Disabled`|Disabled
### PciSlot3LinkSpeed

Use this option to configure the PCIe Link Speed for the selected device. When configured for Auto, the selected device trains at the maximum supported speed of the PCIe link. When configured for PCIe Generation 2 Link Speed, the selected device trains at a maximum of PCIe Generation 2 speed. When configured for PCIe Generation  Link 1 speed, the selected device trains at a maximum of PCIe Generation 1 speed.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`PciSlot3LinkSpeed` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Auto`|Auto
|`PcieGen1`|PCIe Generation 1.0
|`PcieGen2`|PCIe Generation 2.0
### PciSlot3OptionROM

Use this option to enable or disable Device Option ROM 


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`PciSlot3OptionROM` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### PciSlot4Aspm

Use this option to configure the PCIe Link Power Management (ASPM) support for the selected device. When configured for L0s Enabled, the selected device's link enters a standby energy savings state. When configured for L1 Enabled, the selected device's link enters a lower power standby state at the expense of a longer exit latency. When configured for L1 and L0s Enabled, the selected device's link enters either power savings mode, depending on link utilization, and provides the highest energy savings.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`PciSlot4Aspm` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Auto`|Auto
|`Disabled`|Disabled
|`AspmL1Enabled`|L1 Enabled
### PciSlot4Enable

Select this option to enable or disable PCI devices.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`PciSlot4Enable` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Auto`|Auto
|`Disabled`|Disabled
### PciSlot4LinkSpeed

Use this option to configure the PCIe Link Speed for the selected device. When configured for Auto, the selected device trains at the maximum supported speed of the PCIe link. When configured for PCIe Generation 2 Link Speed, the selected device trains at a maximum of PCIe Generation 2 speed. When configured for PCIe Generation  Link 1 speed, the selected device trains at a maximum of PCIe Generation 1 speed.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`PciSlot4LinkSpeed` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Auto`|Auto
|`PcieGen1`|PCIe Generation 1.0
|`PcieGen2`|PCIe Generation 2.0
### PciSlot4OptionROM

Use this option to enable or disable Device Option ROM 


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`PciSlot4OptionROM` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### PciSlot5Aspm

Use this option to configure the PCIe Link Power Management (ASPM) support for the selected device. When configured for L0s Enabled, the selected device's link enters a standby energy savings state. When configured for L1 Enabled, the selected device's link enters a lower power standby state at the expense of a longer exit latency. When configured for L1 and L0s Enabled, the selected device's link enters either power savings mode, depending on link utilization, and provides the highest energy savings.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`PciSlot5Aspm` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Auto`|Auto
|`Disabled`|Disabled
|`AspmL1Enabled`|L1 Enabled
### PciSlot5Enable

Select this option to enable or disable PCI devices.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`PciSlot5Enable` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Auto`|Auto
|`Disabled`|Disabled
### PciSlot5LinkSpeed

Use this option to configure the PCIe Link Speed for the selected device. When configured for Auto, the selected device trains at the maximum supported speed of the PCIe link. When configured for PCIe Generation 2 Link Speed, the selected device trains at a maximum of PCIe Generation 2 speed. When configured for PCIe Generation  Link 1 speed, the selected device trains at a maximum of PCIe Generation 1 speed.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`PciSlot5LinkSpeed` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Auto`|Auto
|`PcieGen1`|PCIe Generation 1.0
|`PcieGen2`|PCIe Generation 2.0
### PciSlot5OptionROM

Use this option to enable or disable Device Option ROM 


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`PciSlot5OptionROM` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### PciSlot6Aspm

Use this option to configure the PCIe Link Power Management (ASPM) support for the selected device. When configured for L0s Enabled, the selected device's link enters a standby energy savings state. When configured for L1 Enabled, the selected device's link enters a lower power standby state at the expense of a longer exit latency. When configured for L1 and L0s Enabled, the selected device's link enters either power savings mode, depending on link utilization, and provides the highest energy savings.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`PciSlot6Aspm` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Auto`|Auto
|`Disabled`|Disabled
|`AspmL1Enabled`|L1 Enabled
### PciSlot6Enable

Select this option to enable or disable PCI devices.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`PciSlot6Enable` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Auto`|Auto
|`Disabled`|Disabled
### PciSlot6LinkSpeed

Use this option to configure the PCIe Link Speed for the selected device. When configured for Auto, the selected device trains at the maximum supported speed of the PCIe link. When configured for PCIe Generation 2 Link Speed, the selected device trains at a maximum of PCIe Generation 2 speed. When configured for PCIe Generation  Link 1 speed, the selected device trains at a maximum of PCIe Generation 1 speed.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`PciSlot6LinkSpeed` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Auto`|Auto
|`PcieGen1`|PCIe Generation 1.0
|`PcieGen2`|PCIe Generation 2.0
### PciSlot6OptionROM

Use this option to enable or disable Device Option ROM 


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`PciSlot6OptionROM` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### PciSlot7Aspm

Use this option to configure the PCIe Link Power Management (ASPM) support for the selected device. When configured for L0s Enabled, the selected device's link enters a standby energy savings state. When configured for L1 Enabled, the selected device's link enters a lower power standby state at the expense of a longer exit latency. When configured for L1 and L0s Enabled, the selected device's link enters either power savings mode, depending on link utilization, and provides the highest energy savings.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`PciSlot7Aspm` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Auto`|Auto
|`Disabled`|Disabled
|`AspmL1Enabled`|L1 Enabled
### PciSlot7Enable

Select this option to enable or disable PCI devices.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`PciSlot7Enable` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Auto`|Auto
|`Disabled`|Disabled
### PciSlot7LinkSpeed

Use this option to configure the PCIe Link Speed for the selected device. When configured for Auto, the selected device trains at the maximum supported speed of the PCIe link. When configured for PCIe Generation 2 Link Speed, the selected device trains at a maximum of PCIe Generation 2 speed. When configured for PCIe Generation  Link 1 speed, the selected device trains at a maximum of PCIe Generation 1 speed.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`PciSlot7LinkSpeed` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Auto`|Auto
|`PcieGen1`|PCIe Generation 1.0
|`PcieGen2`|PCIe Generation 2.0
### PciSlot7OptionROM

Use this option to enable or disable Device Option ROM 


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`PciSlot7OptionROM` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### PciSlot8Aspm

Use this option to configure the PCIe Link Power Management (ASPM) support for the selected device. When configured for L0s Enabled, the selected device's link enters a standby energy savings state. When configured for L1 Enabled, the selected device's link enters a lower power standby state at the expense of a longer exit latency. When configured for L1 and L0s Enabled, the selected device's link enters either power savings mode, depending on link utilization, and provides the highest energy savings.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`PciSlot8Aspm` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Auto`|Auto
|`Disabled`|Disabled
|`AspmL1Enabled`|L1 Enabled
### PciSlot8Enable

Select this option to enable or disable PCI devices.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`PciSlot8Enable` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Auto`|Auto
|`Disabled`|Disabled
### PciSlot8LinkSpeed

Use this option to configure the PCIe Link Speed for the selected device. When configured for Auto, the selected device trains at the maximum supported speed of the PCIe link. When configured for PCIe Generation 2 Link Speed, the selected device trains at a maximum of PCIe Generation 2 speed. When configured for PCIe Generation  Link 1 speed, the selected device trains at a maximum of PCIe Generation 1 speed.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`PciSlot8LinkSpeed` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Auto`|Auto
|`PcieGen1`|PCIe Generation 1.0
|`PcieGen2`|PCIe Generation 2.0
### PciSlot8OptionROM

Use this option to enable or disable Device Option ROM 


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`PciSlot8OptionROM` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### PersistentMemAddressRangeScrub

Use this option to configure the NVDIMM memory Address Range Scrub support. When enabled, this option allows a supported OS to attempt recovery from an uncorrectable memory error detected in the NVDIMM memory. When disabled, the NVDIMM memory will be disabled on the following boot after detecting an uncorrectable memory error in the NVDIMM. If the NVDIMM memory Memory Interleaving option is enabled, a disabled NVDIMM will include all the modules or regions within the set.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`PersistentMemAddressRangeScrub` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### PersistentMemBackupPowerPolicy

This option controls whether the system waits during system boot for batteries to charge if sufficient battery backup power for the installed persistent memory is not available. If this option is configured for 'Continue Boot without Backup Power', the server boots even if sufficient battery backup power is not installed. In this case, if sufficient battery backup power is not enabled, the configured memory will NOT be used by the operating system as persistent storage or as system memory.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`PersistentMemBackupPowerPolicy` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`WaitForBackupPower`|Wait for Backup Power on Boot
|`BootWithoutBackupPower`|Continue Boot without Backup Power
### PersistentMemScanMem

When this option is enabled, persistent memory will be checked during system boot to determine data integrity. Depending on the Persistent Memory Address Range Scrub setting, discovered errors during the data integrity check will either be presented to the operating system for recovery or cause the persistent memory to be mapped out and unavailable to the operating system. If this option is disabled, any persistent memory which has issues with the ability to read data or which has bad data may result in uncorrectable errors that result in a system crash. 
 


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`PersistentMemScanMem` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### PostBootProgress

Use this option to enable verbose boot progress messaging. Because this option displays additional debug information to the screen and serial console, it might be helpful for determining why a server became unresponsive during the boot process.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`PostBootProgress` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Disabled`|Disabled
|`Serial`|Serial Only
|`All`|All
### PostDiscoveryMode

Use this option to configure the UEFI POST Discovery Mode. When Auto is selected, the system selectively starts devices which are required for booting the devices in the UEFI Boot Order list. Note: For some situations with auto mode like system configuration change, the system will change to start all devices for discovering all boot devices. When Force Full Discovery is selected, the system starts all devices in the system providing full boot target availability. Note: When Force Full Discovery is selected, boot time might significantly increase. When Force Fast Discovery is selected, the system starts devices as less as possible for getting the shortest boot time. Note: When Force Fast Discovery is selected, some unsupported device might not work properly. You might need to replace the unsupported device with the supported one.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`PostDiscoveryMode` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Auto`|Auto
|`ForceFullDiscovery`|Force Full Discovery
|`ForceFastDiscovery`|Force Fast Discovery
### PostF1Prompt

Use this option to configure the system to display the F1 key on the server POST screen. If an error is encountered, you can press the F1 key to continue with the server power-up sequence. Select one of the following options: 
Delayed 20 Seconds - If an error occurs, the system pauses for 20 seconds at the F1 prompt and continues to boot the OS. 
Delayed 2 Seconds - If an error occurs, the system pauses for 2 seconds at the F1 prompt and continues to boot the OS. 
Disabled - If an error occurs, the system bypasses the F1 prompt and continues to boot the OS. 
Note: For critical errors, the system pauses for 20 seconds at the F1 prompt, regardless of how this option is configured.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`PostF1Prompt` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Delayed20Sec`|Delayed 20 seconds
|`Delayed2Sec`|Delayed 2 seconds
|`Disabled`|Disabled
### PowerButton

Disabling this option disables the momentary power button functionality. This option does not affect the four-second power button override or the remote power control functionality.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`PowerButton` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### PowerOnDelay

Use this option to delay the server from turning on for a specified time. Pressing the power button (using the Virtual Power Button), or Wake-ON LAN events, and RTC Wake-up events override the delay and power on the server without any additional delay. This enablesstaggering when servers power-up after a power loss to prevent power usage spikes.Note that the actual delay before the server is powered on will be longer than the specifiedtime because the server must always wait for iLO FW to initialize before the server attempts to power on.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`PowerOnDelay` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`NoDelay`|No Delay
|`Random`|Random Delay
|`Delay15Sec`|15 Second Delay
|`Delay30Sec`|30 Second Delay
|`Delay45Sec`|45 Second Delay
|`Delay60Sec`|60 Second Delay
### PowerOnLogo

Use this option to disable the display of the logo during system boot. This option does not affect the server boot time.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`PowerOnLogo` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### PowerOnPassword

When the server powers on, a prompt is displayed to enter a password before continuing the boot process. In the event of an ASR reboot, the Power-On Password is bypassed, and the server boots normally.


| | |
|---|---|
|JSON type|password|
|HTTP PATCH|Yes (if resource allows PATCH)
### PowerRegulator

You can only configure this option if the Workload Profile is set to Custom. Use this option to configure the following Power Regulator support: 
- Dynamic Power Savings Mode: Automatically varies processor speed and power usage based on processor utilization. Enables the reduction of overall power consumption with little or no impact on performance. Does not require OS support. 
- Static Low Power Mode: Reduces processor speed and power usage. Guarantees a lower maximum power usage for the system. Performance impacts are greater for environments with higher processor utilization. 
- Static High Performance Mode: Processors run in their maximum power/performance state at all times, regardless of the OS power management policy. 
- OS Control Mode: Processors run in their maximum power/performance state at all times unless the OS enables a power management policy.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`PowerRegulator` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`DynamicPowerSavings`|Dynamic Power Savings Mode
|`StaticLowPower`|Static Low Power Mode
|`StaticHighPerf`|Static High Performance Mode
|`OsControl`|OS Control Mode
### PreBootNetwork

Use this option to select the network interface used for pre-boot network connections. When the selection is Auto, the system uses the first available port with a network connection.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`PreBootNetwork` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Auto`|Auto
|`EmbNicPort1`|Embedded NIC Port 1
|`EmbNicPort2`|Embedded NIC Port 2
|`EmbNicPort3`|Embedded NIC Port 3
|`EmbNicPort4`|Embedded NIC Port 4
|`EmbNicPort5`|Embedded NIC Port 5
|`EmbNicPort6`|Embedded NIC Port 6
|`EmbNicPort7`|Embedded NIC Port 7
|`EmbNicPort8`|Embedded NIC Port 8
|`FlexLom1Port1`|Embedded FlexibleLOM 1 Port 1
|`FlexLom1Port2`|Embedded FlexibleLOM 1 Port 2
|`FlexLom1Port3`|Embedded FlexibleLOM 1 Port 3
|`FlexLom1Port4`|Embedded FlexibleLOM 1 Port 4
|`FlexLom1Port5`|Embedded FlexibleLOM 1 Port 5
|`FlexLom1Port6`|Embedded FlexibleLOM 1 Port 6
|`FlexLom1Port7`|Embedded FlexibleLOM 1 Port 7
|`FlexLom1Port8`|Embedded FlexibleLOM 1 Port 8
|`Slot1NicPort1`|Slot 1 NIC Port 1
|`Slot1NicPort2`|Slot 1 NIC Port 2
|`Slot1NicPort3`|Slot 1 NIC Port 3
|`Slot1NicPort4`|Slot 1 NIC Port 4
|`Slot1NicPort5`|Slot 1 NIC Port 5
|`Slot1NicPort6`|Slot 1 NIC Port 6
|`Slot1NicPort7`|Slot 1 NIC Port 7
|`Slot1NicPort8`|Slot 1 NIC Port 8
|`Slot2NicPort1`|Slot 2 NIC Port 1
|`Slot2NicPort2`|Slot 2 NIC Port 2
|`Slot2NicPort3`|Slot 2 NIC Port 3
|`Slot2NicPort4`|Slot 2 NIC Port 4
|`Slot2NicPort5`|Slot 2 NIC Port 5
|`Slot2NicPort6`|Slot 2 NIC Port 6
|`Slot2NicPort7`|Slot 2 NIC Port 7
|`Slot2NicPort8`|Slot 2 NIC Port 8
|`Slot3NicPort1`|Slot 3 NIC Port 1
|`Slot3NicPort2`|Slot 3 NIC Port 2
|`Slot3NicPort3`|Slot 3 NIC Port 3
|`Slot3NicPort4`|Slot 3 NIC Port 4
|`Slot3NicPort5`|Slot 3 NIC Port 5
|`Slot3NicPort6`|Slot 3 NIC Port 6
|`Slot3NicPort7`|Slot 3 NIC Port 7
|`Slot3NicPort8`|Slot 3 NIC Port 8
|`Slot4NicPort1`|Slot 4 NIC Port 1
|`Slot4NicPort2`|Slot 4 NIC Port 2
|`Slot4NicPort3`|Slot 4 NIC Port 3
|`Slot4NicPort4`|Slot 4 NIC Port 4
|`Slot4NicPort5`|Slot 4 NIC Port 5
|`Slot4NicPort6`|Slot 4 NIC Port 6
|`Slot4NicPort7`|Slot 4 NIC Port 7
|`Slot4NicPort8`|Slot 4 NIC Port 8
|`Slot5NicPort1`|Slot 5 NIC Port 1
|`Slot5NicPort2`|Slot 5 NIC Port 2
|`Slot5NicPort3`|Slot 5 NIC Port 3
|`Slot5NicPort4`|Slot 5 NIC Port 4
|`Slot5NicPort5`|Slot 5 NIC Port 5
|`Slot5NicPort6`|Slot 5 NIC Port 6
|`Slot5NicPort7`|Slot 5 NIC Port 7
|`Slot5NicPort8`|Slot 5 NIC Port 8
|`Slot6NicPort1`|Slot 6 NIC Port 1
|`Slot6NicPort2`|Slot 6 NIC Port 2
|`Slot6NicPort3`|Slot 6 NIC Port 3
|`Slot6NicPort4`|Slot 6 NIC Port 4
|`Slot6NicPort5`|Slot 6 NIC Port 5
|`Slot6NicPort6`|Slot 6 NIC Port 6
|`Slot6NicPort7`|Slot 6 NIC Port 7
|`Slot6NicPort8`|Slot 6 NIC Port 8
|`Slot7NicPort1`|Slot 7 NIC Port 1
|`Slot7NicPort2`|Slot 7 NIC Port 2
|`Slot7NicPort3`|Slot 7 NIC Port 3
|`Slot7NicPort4`|Slot 7 NIC Port 4
|`Slot7NicPort5`|Slot 7 NIC Port 5
|`Slot7NicPort6`|Slot 7 NIC Port 6
|`Slot7NicPort7`|Slot 7 NIC Port 7
|`Slot7NicPort8`|Slot 7 NIC Port 8
|`Slot8NicPort1`|Slot 8 NIC Port 1
|`Slot8NicPort2`|Slot 8 NIC Port 2
|`Slot8NicPort3`|Slot 8 NIC Port 3
|`Slot8NicPort4`|Slot 8 NIC Port 4
|`Slot8NicPort5`|Slot 8 NIC Port 5
|`Slot8NicPort6`|Slot 8 NIC Port 6
|`Slot8NicPort7`|Slot 8 NIC Port 7
|`Slot8NicPort8`|Slot 8 NIC Port 8
### PrebootNetworkEnvPolicy

Use this option to set the preference for Pre-Boot Network.
If configured for Auto, all the network operations initiated in the pre boot environment occur over IPv4 or IPv6. The order of the existing network boot targets is not modified in the UEFI Boot Order list. New network boot targets are added to the end of the list using the default policy of the System BIOS.
If configured for IPv4, all the network operations initiated in the pre boot environment only occur over IPv4. All existing IPv6 network boot targets are removed in the UEFI Boot Order. No new IPv6 network boot targets are added to the list.
If configured for IPv6, all the network operations initiated in the pre boot environment only occur over IPv6. All existing IPv4 network boot targets in the UEFI Boot Order are removed. No new IPv4 network boot targets are added to the list.



| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`PrebootNetworkEnvPolicy` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Auto`|Auto
|`IPv4`|IPv4
|`IPv6`|IPv6
### PrebootNetworkProxy

Use this option to configure a pre-boot network proxy. When set, network operations for 'Pre-Boot Network Interface' are attempted through the configured proxy. The proxy must be in a HTTP URL format, and can be specified as http://IPv4_address:port, http://IPv6 address:port or http://FQDN:port.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
### ProcAes

Use this option to enable or disable the Advanced Encryption Standard Instruction Set (AES-NI) in the processor.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`ProcAes` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### ProcHyperthreading

Use this option to enable or disable Intel Hyper-Threading. When enabled, each physical processor core operates as two logical processor cores. When disabled, each physical processor core operates as one logical processor core. Enabling this option can improve overall performance for applications that benefit from a higher processor core count.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`ProcHyperthreading` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### ProcTurbo

Turbo Boost Technology enables the processor to transition to a higher frequency than the processor's rated speed if the processor has available power and is within temperature specifications. Disabling this option reduces power usage, and also reduces the system's maximum achievable performance under some workloads.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`ProcTurbo` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Disabled`|Disabled
|`Enabled`|Enabled
### ProcVirtualization

When enabled, a hypervisor or operating system supporting this option can use hardware capabilities provided by Intel VT. Some hypervisors require that you enable Intel VT. You can leave this set to enabled even if you are not using a hypervisor or an 


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`ProcVirtualization` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### ProcX2Apic

x2APIC support enables operating systems to run more efficiently on high core count configurations. It also optimizes interrupt distribution in virtualized environments. In most cases, set this option to enabled. This configures the operating system to optionally enable x2APIC support when it loads. Some older hypervisors and operating systems might have issues with optional x2APIC support, in which case disabling x2APIC might be necessary to address those issues. Additionally, some hypervisors and operating systems will not use X2APIC unless this option is set to Force Enabled prior to booting.  The Force Enabled option also causes the Intel(R) VT-d setting to be set to enabled.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`ProcX2Apic` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`ForceEnabled`|Force Enabled
|`Disabled`|Disabled
### Processor1LogicalNvdimm1SizeGiB

Use this option to specify the amount of regular memory, in gigabytes (1,073,741,824 bytes), to allocate for use as a logical NVDIMM for each specified region. Entries for processor pairs represent logical NVDIMMs which may span multiple processors. An attempt will be made to balance these regions across sockets. The processor-specific entries represent Logical NVDIMMs assigned to a designated socket. These regions are allocated from the top of the memory range for each domain.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|Yes (if resource allows PATCH)
### Processor1LogicalNvdimm2SizeGiB

Use this option to specify the amount of regular memory, in gigabytes (1,073,741,824 bytes), to allocate for use as a logical NVDIMM for each specified region. Entries for processor pairs represent logical NVDIMMs which may span multiple processors. An attempt will be made to balance these regions across sockets. The processor-specific entries represent Logical NVDIMMs assigned to a designated socket. These regions are allocated from the top of the memory range for each domain.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|Yes (if resource allows PATCH)
### Processor1ScalablePmemAvailableGiB

Displays the maximum amount of persistent memory available in the system. The 'Total Available' value represents the amount of total system memory available for use as persistent memory.  The processor-specific values represent the amount of domain (socket) specific system memory that is available for use as logical NVDIMMs. The 'Storage' value represents the total size available on the backup device(s) for storing persistent memory.  All values are in gigabytes (1,073,741,824 bytes).


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Processor2LogicalNvdimm1SizeGiB

Use this option to specify the amount of regular memory, in gigabytes (1,073,741,824 bytes), to allocate for use as a logical NVDIMM for each specified region. Entries for processor pairs represent logical NVDIMMs which may span multiple processors. An attempt will be made to balance these regions across sockets. The processor-specific entries represent Logical NVDIMMs assigned to a designated socket. These regions are allocated from the top of the memory range for each domain.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|Yes (if resource allows PATCH)
### Processor2LogicalNvdimm2SizeGiB

Use this option to specify the amount of regular memory, in gigabytes (1,073,741,824 bytes), to allocate for use as a logical NVDIMM for each specified region. Entries for processor pairs represent logical NVDIMMs which may span multiple processors. An attempt will be made to balance these regions across sockets. The processor-specific entries represent Logical NVDIMMs assigned to a designated socket. These regions are allocated from the top of the memory range for each domain.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|Yes (if resource allows PATCH)
### Processor2ScalablePmemAvailableGiB

Displays the maximum amount of persistent memory available in the system. The 'Total Available' value represents the amount of total system memory available for use as persistent memory.  The processor-specific values represent the amount of domain (socket) specific system memory that is available for use as logical NVDIMMs. The 'Storage' value represents the total size available on the backup device(s) for storing persistent memory.  All values are in gigabytes (1,073,741,824 bytes).


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### ProcessorJitterControl

Processor Jitter Control allows the customer to manage processor frequency variance to do technologies such as Turbo which vary the frequency based on power, thermals, and active cores. When configured for Auto-tuned, the platform will monitor frequency variance and automatically make adjustments to minimize variance over time. When configured for Manual-tuned, the customer can choose to attempt to operate the processor at a fixed frequency and can select lower or higher frequencies statically. 


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`ProcessorJitterControl` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Disabled`|Disabled
|`Auto-tuned`|Auto-tuned
|`Manual-tuned`|Manual-tuned
### ProcessorJitterControlFrequency

Processor Jitter Control Frequency allows the customer to stipulate the starting frequency in the Auto-tuned mode, or the desired frequency in the Manual-tuned mode. The input frequency is in units of Megahertz. System firmware will adjust the frequency to the nearest higher intermediate frequency supported by the processor if the input frequency is not supported.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|Yes (if resource allows PATCH)
### ProductId

Use this option to set the system product ID. This value must always match the product ID sticker located on the chassis.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
### RedundantPowerSupply

Use this option to configure how the system handles redundant power supply configurations. Balanced Mode shares the power delivery equally between all installed power supplies. All High Efficiency Mode options provide the most power efficient operation with redundant power supplies by keeping half of the power supplies in standby mode at lower power usage levels. The High Efficiency Mode options enable the system to select which power supply to place in standby. Auto enables the system to select between the odd or even power supply based on a semi-random distribution within a group of systems.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`RedundantPowerSupply` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`BalancedMode`|Balanced Mode
|`HighEfficiencyAuto`|High Efficiency Mode (Auto)
|`HighEfficiencyOddStandby`|High Efficiency Mode (Odd Supply Standby)
|`HighEfficiencyEvenStandby`|High Efficiency Mode (Even Supply Standby)
### RemovableFlashBootSeq

Use this option to select which USB or SD Card devices you want to search for first when enumerating boot devices. You can select whether the system boots to external USB drive keys, internal USB drive keys, or the internal SD card slot. This option does not override the device boot order in the Standard Boot Order (IPL) option. You can only configure this option when Boot Mode is set to Legacy BIOS.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`RemovableFlashBootSeq` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`InternalSdCardFirst`|Internal SD Card First
|`InternalKeysFirst`|Internal DriveKeys First
|`ExternalKeysFirst`|External DriveKeys First
### RestoreDefaults

Use this option to reset all configuration settings to their default values. Changes that have been made might be lost. You must reboot the system for changes to take effect.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`RestoreDefaults` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`No`|No, cancel the restore procedure.
|`Yes`|Yes, restore the default settings.
### RestoreManufacturingDefaults

Use this option to reset all configuration settings to their default manufacturing values. Changes that have been made might be lost. If Secure Boot is enabled, related security settings might be lost. You must reboot the system for changes to take effect.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`RestoreManufacturingDefaults` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`No`|No, cancel restore procedure.
|`Yes`|Yes, restore the default settings.
### RomSelection

Use this option to revert the server to a previous BIOS ROM image. The backup image is the BIOS ROM image that was used prior to the last flash event.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`RomSelection` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`CurrentRom`|Use Current ROM
|`BackupRom`|Switch to Backup ROM
### SanitizeAllNvDimmN

When Enabled, all user data in ALL NVDIMMs of type NVDIMM-N in the system are erased on the next reboot.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`SanitizeAllNvDimmN` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### SanitizeProc1Dimm1

When Enabled, all user data in the selected NVDIMM-N are erased on the next reboot.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`SanitizeProc1Dimm1` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### SanitizeProc1Dimm10

When Enabled, all user data in the selected NVDIMM-N are erased on the next reboot.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`SanitizeProc1Dimm10` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### SanitizeProc1Dimm11

When Enabled, all user data in the selected NVDIMM-N are erased on the next reboot.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`SanitizeProc1Dimm11` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### SanitizeProc1Dimm12

When Enabled, all user data in the selected NVDIMM-N are erased on the next reboot.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`SanitizeProc1Dimm12` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### SanitizeProc1Dimm2

When Enabled, all user data in the selected NVDIMM-N are erased on the next reboot.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`SanitizeProc1Dimm2` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### SanitizeProc1Dimm3

When Enabled, all user data in the selected NVDIMM-N are erased on the next reboot.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`SanitizeProc1Dimm3` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### SanitizeProc1Dimm4

When Enabled, all user data in the selected NVDIMM-N are erased on the next reboot.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`SanitizeProc1Dimm4` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### SanitizeProc1Dimm5

When Enabled, all user data in the selected NVDIMM-N are erased on the next reboot.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`SanitizeProc1Dimm5` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### SanitizeProc1Dimm6

When Enabled, all user data in the selected NVDIMM-N are erased on the next reboot.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`SanitizeProc1Dimm6` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### SanitizeProc1Dimm7

When Enabled, all user data in the selected NVDIMM-N are erased on the next reboot.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`SanitizeProc1Dimm7` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### SanitizeProc1Dimm8

When Enabled, all user data in the selected NVDIMM-N are erased on the next reboot.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`SanitizeProc1Dimm8` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### SanitizeProc1Dimm9

When Enabled, all user data in the selected NVDIMM-N are erased on the next reboot.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`SanitizeProc1Dimm9` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### SanitizeProc1NvDimmN

When Enabled, all user data in ALL NVDIMMs of type NVDIMM-N installed on the selected processor are erased on the next reboot.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`SanitizeProc1NvDimmN` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### SanitizeProc2Dimm1

When Enabled, all user data in the selected NVDIMM-N are erased on the next reboot.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`SanitizeProc2Dimm1` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### SanitizeProc2Dimm10

When Enabled, all user data in the selected NVDIMM-N are erased on the next reboot.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`SanitizeProc2Dimm10` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### SanitizeProc2Dimm11

When Enabled, all user data in the selected NVDIMM-N are erased on the next reboot.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`SanitizeProc2Dimm11` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### SanitizeProc2Dimm12

When Enabled, all user data in the selected NVDIMM-N are erased on the next reboot.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`SanitizeProc2Dimm12` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### SanitizeProc2Dimm2

When Enabled, all user data in the selected NVDIMM-N are erased on the next reboot.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`SanitizeProc2Dimm2` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### SanitizeProc2Dimm3

When Enabled, all user data in the selected NVDIMM-N are erased on the next reboot.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`SanitizeProc2Dimm3` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### SanitizeProc2Dimm4

When Enabled, all user data in the selected NVDIMM-N are erased on the next reboot.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`SanitizeProc2Dimm4` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### SanitizeProc2Dimm5

When Enabled, all user data in the selected NVDIMM-N are erased on the next reboot.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`SanitizeProc2Dimm5` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### SanitizeProc2Dimm6

When Enabled, all user data in the selected NVDIMM-N are erased on the next reboot.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`SanitizeProc2Dimm6` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### SanitizeProc2Dimm7

When Enabled, all user data in the selected NVDIMM-N are erased on the next reboot.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`SanitizeProc2Dimm7` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### SanitizeProc2Dimm8

When Enabled, all user data in the selected NVDIMM-N are erased on the next reboot.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`SanitizeProc2Dimm8` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### SanitizeProc2Dimm9

When Enabled, all user data in the selected NVDIMM-N are erased on the next reboot.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`SanitizeProc2Dimm9` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### SanitizeProc2NvDimmN

When Enabled, all user data in ALL NVDIMMs of type NVDIMM-N installed on the selected processor are erased on the next reboot.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`SanitizeProc2NvDimmN` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### SataSecureErase

Use this option to control whether Secure Erase functionality is supported. When enabled, the Security Freeze Lock command is not sent to supported SATA hard drives, enabling Secure erase to function (the Secure Erase command is supported). This option is only supported when the SATA controller is in AHCI mode. Secure Erase only operates with hard drives that support the Secure Erase command.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`SataSecureErase` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### SaveUserDefaults

Select this option to save the current settings as the system defaults.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`SaveUserDefaults` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`No`|No, Cancel
|`Yes`|Yes, Save
### ScalablePmemCapacity

Total Scalable Persistent Memory Capacity in GB.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### SecStartBackupImage

Use this option to enable cryptographic authentication of the backup ROM image on startup. When this option is disabled, only the primary image is authenticated on each startup. Enable this option to also perform cryptographic authentication of the backup ROM image.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`SecStartBackupImage` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### SecureBootStatus

The current state of Secure Boot configuration.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`SecureBootStatus` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### SerialConsoleBaudRate

This is the transfer rate at which data is transmitted through the serial port.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`SerialConsoleBaudRate` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`BaudRate9600`|9600
|`BaudRate19200`|19200
|`BaudRate38400`|38400
|`BaudRate57600`|57600
|`BaudRate115200`|115200
### SerialConsoleEmulation

Use this option to select the emulation mode type. The option you select depends on the emulation you want to use in your serial terminal program (such as HyperTerminal or PuTTy). The BIOS emulation mode must match the mode you select in your terminal program.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`SerialConsoleEmulation` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Vt100`|VT100
|`Ansi`|ANSI
|`Vt100Plus`|VT100+
|`VtUtf8`|VT-UTF8
### SerialConsolePort

Use this option to re-direct video and keystrokes through the serial port to OS boot. This option can interfere with non-terminal devices attached to the serial port. In such cases, set this option to disabled. This option is only supported in English language mode when running in the UEFI pre-boot System Utilities.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`SerialConsolePort` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Auto`|Auto
|`Disabled`|Disabled
|`Physical`|Physical Serial Port
|`Virtual`|Virtual Serial Port
### SerialNumber

Use this option to set the system serial number. This value must always match the serial number sticker located on the chassis.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
### ServerAssetTag

Select this option to modify the Server Asset Tag text line.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
### ServerName

Select this option to modify the server name text line.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
### ServerOtherInfo

Use this option to modify the Other Server text line.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
### ServerPrimaryOs

Use this option to modify the Server Primary OS text line.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
### ServiceEmail

Enter the server service contact e-mail address.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
### ServiceName

Enter the server service contact name text.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
### ServiceOtherInfo

Enter the other server service contact information text.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
### ServicePhone

Enter the server service contact phone number text.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
### SetupBrowserSelection

Select which setup browser to use: GUI or Text. Auto mode uses text when the user enters RBSU via serial console, and uses GUI via IRC or physical terminal.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`SetupBrowserSelection` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`GUI`|GUI
|`Text`|Text
|`Auto`|Auto
### Slot1NicBoot1

Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`Slot1NicBoot1` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`NetworkBoot`|Network Boot
|`Disabled`|Disabled
### Slot1NicBoot2

Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`Slot1NicBoot2` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`NetworkBoot`|Network Boot
|`Disabled`|Disabled
### Slot1NicBoot3

Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`Slot1NicBoot3` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`NetworkBoot`|Network Boot
|`Disabled`|Disabled
### Slot1NicBoot4

Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`Slot1NicBoot4` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`NetworkBoot`|Network Boot
|`Disabled`|Disabled
### Slot1NicBoot5

Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`Slot1NicBoot5` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`NetworkBoot`|Network Boot
|`Disabled`|Disabled
### Slot1NicBoot6

Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`Slot1NicBoot6` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`NetworkBoot`|Network Boot
|`Disabled`|Disabled
### Slot1NicBoot7

Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`Slot1NicBoot7` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`NetworkBoot`|Network Boot
|`Disabled`|Disabled
### Slot1NicBoot8

Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`Slot1NicBoot8` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`NetworkBoot`|Network Boot
|`Disabled`|Disabled
### Slot1StorageBoot

When Boot All Targets is selected, all valid boot targets attached to the storage controller are made available in the UEFI Boot Order list. If Boot No Targets is selected, no boot targets from this storage controller are made available in the UEFI Boot Order.If Boot Limit to 24 Targets is selected, 24 boot targets attached to the storage controller are made available in the UEFI Boot Order.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`Slot1StorageBoot` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`AllTargets`|Boot All Targets
|`TwentyFourTargets`|Boot Limit to 24 Targets
|`NoTargets`|Boot No Targets
### Slot2NicBoot1

Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`Slot2NicBoot1` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`NetworkBoot`|Network Boot
|`Disabled`|Disabled
### Slot2NicBoot2

Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`Slot2NicBoot2` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`NetworkBoot`|Network Boot
|`Disabled`|Disabled
### Slot2NicBoot3

Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`Slot2NicBoot3` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`NetworkBoot`|Network Boot
|`Disabled`|Disabled
### Slot2NicBoot4

Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`Slot2NicBoot4` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`NetworkBoot`|Network Boot
|`Disabled`|Disabled
### Slot2NicBoot5

Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`Slot2NicBoot5` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`NetworkBoot`|Network Boot
|`Disabled`|Disabled
### Slot2NicBoot6

Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`Slot2NicBoot6` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`NetworkBoot`|Network Boot
|`Disabled`|Disabled
### Slot2NicBoot7

Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`Slot2NicBoot7` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`NetworkBoot`|Network Boot
|`Disabled`|Disabled
### Slot2NicBoot8

Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`Slot2NicBoot8` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`NetworkBoot`|Network Boot
|`Disabled`|Disabled
### Slot2StorageBoot

When Boot All Targets is selected, all valid boot targets attached to the storage controller are made available in the UEFI Boot Order list. If Boot No Targets is selected, no boot targets from this storage controller are made available in the UEFI Boot Order.If Boot Limit to 24 Targets is selected, 24 boot targets attached to the storage controller are made available in the UEFI Boot Order.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`Slot2StorageBoot` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`AllTargets`|Boot All Targets
|`TwentyFourTargets`|Boot Limit to 24 Targets
|`NoTargets`|Boot No Targets
### Slot3NicBoot1

Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`Slot3NicBoot1` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`NetworkBoot`|Network Boot
|`Disabled`|Disabled
### Slot3NicBoot2

Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`Slot3NicBoot2` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`NetworkBoot`|Network Boot
|`Disabled`|Disabled
### Slot3NicBoot3

Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`Slot3NicBoot3` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`NetworkBoot`|Network Boot
|`Disabled`|Disabled
### Slot3NicBoot4

Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`Slot3NicBoot4` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`NetworkBoot`|Network Boot
|`Disabled`|Disabled
### Slot3NicBoot5

Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`Slot3NicBoot5` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`NetworkBoot`|Network Boot
|`Disabled`|Disabled
### Slot3NicBoot6

Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`Slot3NicBoot6` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`NetworkBoot`|Network Boot
|`Disabled`|Disabled
### Slot3NicBoot7

Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`Slot3NicBoot7` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`NetworkBoot`|Network Boot
|`Disabled`|Disabled
### Slot3NicBoot8

Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`Slot3NicBoot8` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`NetworkBoot`|Network Boot
|`Disabled`|Disabled
### Slot3StorageBoot

When Boot All Targets is selected, all valid boot targets attached to the storage controller are made available in the UEFI Boot Order list. If Boot No Targets is selected, no boot targets from this storage controller are made available in the UEFI Boot Order.If Boot Limit to 24 Targets is selected, 24 boot targets attached to the storage controller are made available in the UEFI Boot Order.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`Slot3StorageBoot` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`AllTargets`|Boot All Targets
|`TwentyFourTargets`|Boot Limit to 24 Targets
|`NoTargets`|Boot No Targets
### Slot4NicBoot1

Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`Slot4NicBoot1` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`NetworkBoot`|Network Boot
|`Disabled`|Disabled
### Slot4NicBoot2

Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`Slot4NicBoot2` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`NetworkBoot`|Network Boot
|`Disabled`|Disabled
### Slot4NicBoot3

Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`Slot4NicBoot3` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`NetworkBoot`|Network Boot
|`Disabled`|Disabled
### Slot4NicBoot4

Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`Slot4NicBoot4` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`NetworkBoot`|Network Boot
|`Disabled`|Disabled
### Slot4NicBoot5

Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`Slot4NicBoot5` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`NetworkBoot`|Network Boot
|`Disabled`|Disabled
### Slot4NicBoot6

Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`Slot4NicBoot6` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`NetworkBoot`|Network Boot
|`Disabled`|Disabled
### Slot4NicBoot7

Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`Slot4NicBoot7` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`NetworkBoot`|Network Boot
|`Disabled`|Disabled
### Slot4NicBoot8

Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`Slot4NicBoot8` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`NetworkBoot`|Network Boot
|`Disabled`|Disabled
### Slot4StorageBoot

When Boot All Targets is selected, all valid boot targets attached to the storage controller are made available in the UEFI Boot Order list. If Boot No Targets is selected, no boot targets from this storage controller are made available in the UEFI Boot Order.If Boot Limit to 24 Targets is selected, 24 boot targets attached to the storage controller are made available in the UEFI Boot Order.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`Slot4StorageBoot` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`AllTargets`|Boot All Targets
|`TwentyFourTargets`|Boot Limit to 24 Targets
|`NoTargets`|Boot No Targets
### Slot5NicBoot1

Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`Slot5NicBoot1` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`NetworkBoot`|Network Boot
|`Disabled`|Disabled
### Slot5NicBoot2

Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`Slot5NicBoot2` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`NetworkBoot`|Network Boot
|`Disabled`|Disabled
### Slot5NicBoot3

Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`Slot5NicBoot3` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`NetworkBoot`|Network Boot
|`Disabled`|Disabled
### Slot5NicBoot4

Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`Slot5NicBoot4` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`NetworkBoot`|Network Boot
|`Disabled`|Disabled
### Slot5NicBoot5

Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`Slot5NicBoot5` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`NetworkBoot`|Network Boot
|`Disabled`|Disabled
### Slot5NicBoot6

Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`Slot5NicBoot6` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`NetworkBoot`|Network Boot
|`Disabled`|Disabled
### Slot5NicBoot7

Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`Slot5NicBoot7` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`NetworkBoot`|Network Boot
|`Disabled`|Disabled
### Slot5NicBoot8

Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`Slot5NicBoot8` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`NetworkBoot`|Network Boot
|`Disabled`|Disabled
### Slot5StorageBoot

When Boot All Targets is selected, all valid boot targets attached to the storage controller are made available in the UEFI Boot Order list. If Boot No Targets is selected, no boot targets from this storage controller are made available in the UEFI Boot Order.If Boot Limit to 24 Targets is selected, 24 boot targets attached to the storage controller are made available in the UEFI Boot Order.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`Slot5StorageBoot` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`AllTargets`|Boot All Targets
|`TwentyFourTargets`|Boot Limit to 24 Targets
|`NoTargets`|Boot No Targets
### Slot6NicBoot1

Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`Slot6NicBoot1` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`NetworkBoot`|Network Boot
|`Disabled`|Disabled
### Slot6NicBoot2

Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`Slot6NicBoot2` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`NetworkBoot`|Network Boot
|`Disabled`|Disabled
### Slot6NicBoot3

Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`Slot6NicBoot3` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`NetworkBoot`|Network Boot
|`Disabled`|Disabled
### Slot6NicBoot4

Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`Slot6NicBoot4` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`NetworkBoot`|Network Boot
|`Disabled`|Disabled
### Slot6NicBoot5

Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`Slot6NicBoot5` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`NetworkBoot`|Network Boot
|`Disabled`|Disabled
### Slot6NicBoot6

Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`Slot6NicBoot6` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`NetworkBoot`|Network Boot
|`Disabled`|Disabled
### Slot6NicBoot7

Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`Slot6NicBoot7` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`NetworkBoot`|Network Boot
|`Disabled`|Disabled
### Slot6NicBoot8

Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`Slot6NicBoot8` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`NetworkBoot`|Network Boot
|`Disabled`|Disabled
### Slot6StorageBoot

When Boot All Targets is selected, all valid boot targets attached to the storage controller are made available in the UEFI Boot Order list. If Boot No Targets is selected, no boot targets from this storage controller are made available in the UEFI Boot Order.If Boot Limit to 24 Targets is selected, 24 boot targets attached to the storage controller are made available in the UEFI Boot Order.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`Slot6StorageBoot` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`AllTargets`|Boot All Targets
|`TwentyFourTargets`|Boot Limit to 24 Targets
|`NoTargets`|Boot No Targets
### Slot7NicBoot1

Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`Slot7NicBoot1` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`NetworkBoot`|Network Boot
|`Disabled`|Disabled
### Slot7NicBoot2

Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`Slot7NicBoot2` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`NetworkBoot`|Network Boot
|`Disabled`|Disabled
### Slot7NicBoot3

Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`Slot7NicBoot3` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`NetworkBoot`|Network Boot
|`Disabled`|Disabled
### Slot7NicBoot4

Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`Slot7NicBoot4` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`NetworkBoot`|Network Boot
|`Disabled`|Disabled
### Slot7StorageBoot

When Boot All Targets is selected, all valid boot targets attached to the storage controller are made available in the UEFI Boot Order list. If Boot No Targets is selected, no boot targets from this storage controller are made available in the UEFI Boot Order.If Boot Limit to 24 Targets is selected, 24 boot targets attached to the storage controller are made available in the UEFI Boot Order.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`Slot7StorageBoot` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`AllTargets`|Boot All Targets
|`TwentyFourTargets`|Boot Limit to 24 Targets
|`NoTargets`|Boot No Targets
### Slot8NicBoot1

Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`Slot8NicBoot1` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`NetworkBoot`|Network Boot
|`Disabled`|Disabled
### Slot8NicBoot2

Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`Slot8NicBoot2` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`NetworkBoot`|Network Boot
|`Disabled`|Disabled
### Slot8NicBoot3

Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`Slot8NicBoot3` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`NetworkBoot`|Network Boot
|`Disabled`|Disabled
### Slot8NicBoot4

Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`Slot8NicBoot4` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`NetworkBoot`|Network Boot
|`Disabled`|Disabled
### Slot8StorageBoot

When Boot All Targets is selected, all valid boot targets attached to the storage controller are made available in the UEFI Boot Order list. If Boot No Targets is selected, no boot targets from this storage controller are made available in the UEFI Boot Order.If Boot Limit to 24 Targets is selected, 24 boot targets attached to the storage controller are made available in the UEFI Boot Order.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`Slot8StorageBoot` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`AllTargets`|Boot All Targets
|`TwentyFourTargets`|Boot Limit to 24 Targets
|`NoTargets`|Boot No Targets
### SpannedLogicalNvdimm1AvailableMemoryGiB

Displays the maximum amount of persistent memory available in the system. The 'Total Available' value represents the amount of total system memory available for use as persistent memory.  The processor-specific values represent the amount of domain (socket) specific system memory that is available for use as logical NVDIMMs. The 'Storage' value represents the total size available on the backup device(s) for storing persistent memory.  All values are in gigabytes (1,073,741,824 bytes).


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### SpannedLogicalNvdimm1SizeGiB

Use this option to specify the amount of regular memory, in gigabytes (1,073,741,824 bytes), to allocate for use as a logical NVDIMM for each specified region. Entries for processor pairs represent logical NVDIMMs which may span multiple processors. An attempt will be made to balance these regions across sockets. The processor-specific entries represent Logical NVDIMMs assigned to a designated socket. These regions are allocated from the top of the memory range for each domain.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|Yes (if resource allows PATCH)
### SpannedLogicalNvdimm1StartingDomainId

Use this option to specify the amount of regular memory, in gigabytes (1,073,741,824 bytes), to allocate for use as a logical NVDIMM for each specified region. Entries for processor pairs represent logical NVDIMMs which may span multiple processors. An attempt will be made to balance these regions across sockets. The processor-specific entries represent Logical NVDIMMs assigned to a designated socket. These regions are allocated from the top of the memory range for each domain.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|Yes (if resource allows PATCH)
### SpannedLogicalNvdimm1StartingDomainSize

Use this option to specify the amount of regular memory, in gigabytes (1,073,741,824 bytes), to allocate for use as a logical NVDIMM for each specified region. Entries for processor pairs represent logical NVDIMMs which may span multiple processors. An attempt will be made to balance these regions across sockets. The processor-specific entries represent Logical NVDIMMs assigned to a designated socket. These regions are allocated from the top of the memory range for each domain.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|Yes (if resource allows PATCH)
### Sriov

If enabled, SR-IOV support enables a hypervisor to create virtual instances of a PCI-express device, potentially increasing performance. If enabled, the BIOS allocates additional resources to PCI-express devices. You can leave this option set to enabled even if you are not using a hypervisor.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`Sriov` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### SubNumaClustering

When enabled, Sub-NUMA Clustering divides the processor's cores, cache, and memory into multiple NUMA domains. Enabling this feature can increase performance for workloads that are NUMA aware and optimized. 
Note: When this option is enabled, up to 1GB of system memory may become unavailable.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`SubNumaClustering` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### ThermalConfig

Use this option to select the fan cooling solution for the system. Optimal Cooling provides the most efficient solution by configuring fan speeds to the minimum required speed to provide adequate cooling. Increased Cooling runs fans at higher speeds to provide additional cooling. Select Increased Cooling when third-party storage controllers are cabled to the embedded hard drive cage, or if the system is experiencing thermal issues that cannot be resolved. Maximum cooling provides the maximum cooling available on this platform.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`ThermalConfig` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`OptimalCooling`|Optimal Cooling
|`IncreasedCooling`|Increased Cooling
|`MaxCooling`|Maximum Cooling
### ThermalShutdown

Use this option to control the reaction of the system to caution level thermal events. When disabled, the System Management Firmware ignores thermal events, and the system immediately powers off in data-destructive situations.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`ThermalShutdown` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### TimeFormat

This option controls how the system time is stored in the hardware Real Time Clock (RTC). When configured to 'Coordinated Universal Time (UTC)' (default) the local time is calculated from the associated time zone value. When configured to 'Local Time' the time is stored directly as local time and the time zone option does not have meaning. Setting this option to 'Local Time' works around an issue when using Microsoft Windows operating systems in Legacy Boot Mode where the time is set incorrectly.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`TimeFormat` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Utc`|Coordinated Universal Time (UTC)
|`Local`|Local Time
### TimeZone

This option displays the current time zone setting for the system.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`TimeZone` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`UtcM12`|UTC-12:00, International Date Line West
|`UtcM11`|UTC-11:00, Midway Island, Samoa
|`UtcM10`|UTC-10:00, Hawaii
|`UtcM9`|UTC-09:00, Alaska
|`UtcM8`|UTC-08:00, Pacific Time(US & Canada)
|`UtcM7`|UTC-07:00, Mountain Time (US & Canada)
|`UtcM6`|UTC-06:00, Central America, Central Time(US & Canada)
|`UtcM5`|UTC-05:00, Eastern Time(US & Canada)
|`UtcM430`|UTC-04:30, Caracas
|`UtcM4`|UTC-04:00, Atlantic Time(Canada), Caracas, Santiago
|`UtcM330`|UTC-03:30, Newfoundland
|`UtcM3`|UTC-03:00, Brasilia, Buenos Aires, Georgetown, Greenland
|`UtcM2`|UTC-02:00, Mid-Atlantic
|`UtcM1`|UTC-01:00, Azores, Cape Verde Is.
|`Utc0`|UTC-00:00, Greenwich Mean Time, Dublin, London
|`UtcP1`|UTC+01:00, Amsterdam, Berlin, Rome, Paris, West Central Africa
|`UtcP2`|UTC+02:00, Athens, Istanbul, Cairo, Jerusalem
|`UtcP3`|UTC+03:00, Baghdad, Kuwait, Riyadh, Moscow, Nairobi
|`UtcP330`|UTC+03:30, Tehran
|`UtcP4`|UTC+04:00, Abu Dhabi, Muscat, Baku, Tbilisi, Yerevan
|`UtcP430`|UTC+04:30, Kabul
|`UtcP5`|UTC+05:00, Ekaterinburg, Islamabad, Karachi, Tashkent
|`UtcP530`|UTC+05:30, Chennai, Kolkata, Mumbai, New Delhi
|`UtcP545`|UTC+05:45, Kathmandu
|`UtcP6`|UTC+06:00, Almaty, Novosibirsk, Astana, Dhaka
|`UtcP630`|UTC+06:30, Rangoon
|`UtcP7`|UTC+07:00, Bangkok, Hanoi, Jakarta, Krasnoyarsk
|`UtcP8`|UTC+08:00, Taipei, Beijing, Chongqing, Hong Kong, Urumqi
|`UtcP9`|UTC+09:00, Osaka, Sapporo, Tokyo, Seoul, Yakutsk
|`UtcP930`|UTC+09:30, Adelaide, Darwin
|`UtcP10`|UTC+10:00, Canberra, Melbourne, Sydney, Guam, Hobart, Vladivostok
|`UtcP11`|UTC+11:00, Magadan, Solomon Is., New Caledonia
|`UtcP12`|UTC+12:00, Auckland, Wellington, Fiji, Kamchatka, Marshall Is.
|`UtcP13`|UTC+13:00, Nuku'alofa
|`UtcP14`|UTC+14:00, Line Islands
|`Unspecified`|Unspecified Time Zone
### Tpm20SoftwareInterfaceOperation

TPM 2.0 Software Interface Operation: FIFO or CRB.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`Tpm20SoftwareInterfaceOperation` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`NoAction`|No Action
|`Fifo`|FIFO interface
|`Crb`|CRB interface
### Tpm20SoftwareInterfaceStatus

Current TPM 2.0 Software Interface Status: FIFO or CRB.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Tpm20SoftwareInterfaceStatus` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`NoAction`|No Action
|`Fifo`|FIFO interface
|`Crb`|CRB interface
### Tpm2Operation

Use this option to perform a clear operation on the TPM. Clearing the TPM can prevent the server from booting to a TPM-aware operating system if the operating system uses TPM's measurements. TPM 2.0 is only supported in UEFI Mode.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`Tpm2Operation` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`NoAction`|No Action
|`Clear`|Clear
### TpmActivePcrs

Current TPM 2.0 Active PCRs: SHA1, SHA256 or SHA1_SHA256


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`TpmActivePcrs` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`NotSpecified`|Not specified
|`Sha1`|SHA1 only
|`Sha256`|SHA256 only
|`Sha1Sha256`|SHA1 and SHA256
### TpmChipId

Current TPM Chip: STMicro, Intel PTT fTPM or Nationz TPM20


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`TpmChipId` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`None`|None
|`StMicroGen10`|ST Micro Gen10
|`IntelPttFTpm`|Intel PTT fTPM
|`NationzTpm20`|Nationz TPM20
### TpmFips

Current TPM FIPS (Federal Information Processing Standard) status: Not specified; non-FIPS certified; FIPS certified.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`TpmFips` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`NotSpecified`|Not specified
|`NonFipsMode`|Non-FIPS Mode
|`FipsMode`|FIPS mode
### TpmFipsModeSwitch

Use this option to switch the TPM chip to FIPS mode, regular mode.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`TpmFipsModeSwitch` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`NoAction`|No Action
|`RegularMode`|Regular mode
|`FipsMode`|FIPS mode
### TpmModeSwitchOperation

Use this option to switch the TPM chip to TPM 1.2/2.0, FIPS mode or non-FIPS mode.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`TpmModeSwitchOperation` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`NoAction`|No Action
|`Tpm12`|TPM 1.2
|`Tpm20`|TPM 2.0
### TpmOperation

Use this option to enable the Trusted Platform Module and BIOS secure startup. When enabled, the TPM is fully functional. When disabled, the TPM is visible; however, functionality is limited. This option also enables you to reset the TPM to factory settings, which clears any assigned passwords, keys, or ownership data. Clearing the TPM can prevent the server from booting to a TPM-aware operating system if the operating system uses TPM's measurements.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`TpmOperation` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`NoAction`|No Action
|`Enable`|Enable
|`Disable`|Disable
|`Clear`|Clear
### TpmState

Current TPM device state: Not Present; Present and Disabled; Present and Enabled.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`TpmState` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`NotPresent`|Not Present
|`PresentDisabled`|Present and Disabled
|`PresentEnabled`|Present and Enabled
### TpmType

Current TPM device type.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`TpmType` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`NoTpm`|No TPM
|`Tpm12`|TPM 1.2
|`Tpm20`|TPM 2.0
### TpmUefiOpromMeasuring

Use this option to enable measuring the UEFI PCI option ROMs. Disabling this option skips measuring the UEFI PCI option ROMs.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`TpmUefiOpromMeasuring` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### TpmVisibility

Use this option to hide the TPM from the operating system. When the TPM is hidden, BIOS secure startup is disabled, and the TPM does not respond to any commands. Intended use is for removing the TPM option from the system without removing the actual hardware.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`TpmVisibility` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Hidden`|Hidden
|`Visible`|Visible
### UefiOptimizedBoot

When enabled, the system BIOS boots using native UEFI graphics drivers. When disabled, the system BIOS boots using INT10 legacy video support. You cannot disable this option if Secure Boot is enabled. You can only configure this option if Boot Mode is configured to UEFI Mode. 
Set this option to disabled for compatibility with Microsoft Windows 2008 and Windows 2008 R2 operating systems on a system configured for UEFI Mode. 
Set this option to enabled for compatibility with VMWare ESXi operating systems on a system configured for UEFI Mode.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`UefiOptimizedBoot` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### UefiSerialDebugLevel

Use this option to enable the UEFI Serial Debug output and verbosity level. Selecting Verbose can impact server boot time significantly. This option is only applicable in UEFI Mode.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`UefiSerialDebugLevel` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Disabled`|Disabled
|`ErrorsOnly`|Errors Only
|`Medium`|Medium
|`Network`|Network
|`Verbose`|Verbose
|`Custom`|Custom
### UefiShellBootOrder

When enabled, this option adds the Embedded UEFI Shell as an entry in the UEFI Boot Order list. This option is only available when the Boot Mode is configured to UEFI Mode and the Embedded UEFI Shell is enabled.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`UefiShellBootOrder` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### UefiShellScriptVerification

Enable this option to allow verification of UEFI shell script files when Secure Boot is enabled. For successful execution of script, make sure that UEFI shell scripts are enrolled in the Secure Boot database (db).


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`UefiShellScriptVerification` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### UefiShellStartup

Use this option to enable or disable automatic execution of the Embedded UEFI Shell startup script. You can store the script file on local media or access it from a network location. You must name the script file "startup.nsh" and place it on local media or a network location accessible to the server.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`UefiShellStartup` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### UefiShellStartupLocation

Use this option to select the location of the Embedded UEFI Shell startup script. For the 'File Systems on Attached Media' option, you must name the script file "startup.nsh" and place it on a UEFI accessible local file system, such as a FAT32 partition on a USB disk or HDD. For the 'Network Location' option, the file must end with a .nsh extension, and must be placed at an HTTP/HTTPS or FTP location accessible to the system. When you select the 'Auto' option, the system attempts to retrieve the startup script from the network location first, followed by locally attached media.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`UefiShellStartupLocation` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Auto`|Auto
|`AttachedMedia`|File Systems on Attached Media
|`NetworkLocation`|Network Location
### UefiShellStartupUrl

Use this option to configure a network URL to a UEFI Shell startup script. This option is available and used only when the Auto-Start Script Location is set to 'Network Location', or 'Auto', and the Shell Auto-Start Script discovery using DHCP is set to 'Disabled'. URLs in HTTP/HTTPS are accepted using either an IPv4 or IPv6 server address, or using a host name. FTP formats are accepted using either an IPv4 server address or a host name. For example, the URLs can be in any of the following formats: http://192.168.0.1/file/file.nsh, http://example.com/file/file.nsh, https://example.com/file/file.nsh, http://[1234::1000]/file.nsh. The file must end with an .nsh extension. When configured, the Embedded UEFI Shell attempts to load and execute the startup script from the network location pointed to by this URL. When a HTTPS URL is configured, you must enroll the respective HTTPS server's TLS certificate under Server Security > TLS(HTTPS) Options.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
### UefiShellStartupUrlFromDhcp

Use this option to let the Shell discover its startup script URL using DHCP. This option is available only if the 'HTTP Support' policy is not set to 'Disabled' and Auto-Start Script Location is set to 'Network Location', or 'Auto'. When set to 'Enabled', the Shell sends DHCP requests with the DHCP User Class option set to the string 'UEFIShell'. The DHCP server must be configured to provide HTTP/HTTPS or FTP URLs when this DHCP User Class string is present in the DHCP request. The User Class option is Option 77 when using DHCP over IPv4, and Option 15 when using DHCP over IPv6. URLs in HTTP/HTTPS must use either an IPv4 or IPv6 server address, or a host name. FTP formats are accepted using either an IPv4 server address or a host name. The URL provided by the DHCP server should match the 'HTTP Support' policy. When 'HTTP Support' policy is set to 'Auto', any HTTP/HTTPS or FTP URL provided by the DHCP server is used. When policy is set to 'HTTPS only', only HTTPS URLs are used, and other URLs are ignored. When policy is set to 'HTTP only', only HTTP or FTP URLs are used, and other URLs are ignored. When policy is set to 'Disabled', the Shell does not send any DHCP request.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`UefiShellStartupUrlFromDhcp` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### UncoreFreqScaling

This option controls the frequency scaling of the processor's internal busses (the uncore.) Setting this option to Auto enables the processor to dynamically change frequencies based on workload. Forcing to the maximum or minimum frequency enables tuning for latency or power consumption.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`UncoreFreqScaling` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Auto`|Auto
|`Maximum`|Maximum
|`Minimum`|Minimum
### UpiPrefetcher

Use this option to disable the processor UPI Prefetch feature. In some cases, setting this option to disabled can improve performance. Typically, setting this option to enabled provides better performance. Only disable this option after performing application benchmarking to verify improved performance in the environment. This option must be enabled when Sub-Numa Clustering (SNC) is enabled.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`UpiPrefetcher` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### UrlBootFile

Use this option to configure a network URL to a bootable ISO or EFI file. URLs in HTTP/HTTPS are accepted using either an IPv4 or IPv6 server address, or using a host name. For example, the URLs can be in any of the following formats: http://192.168.0.1/file/image.iso, http://example.com/file/image.efi, https://example.com/file/image.efi, http://[1234::1000]/image.iso. 
When configured, this URL is listed as a boot option in the UEFI boot menu. Selecting this boot option downloads the file to the system memory, and configures the system to attempt to boot from it. There is no specific ordering on this option. It can be independently ordered in the boot menu. 
This setting requires configuring the 'Pre-Boot Network Interface' option if you want to access the URL location through a specific network interface. When a HTTPS URL is configured, this setting requires enrolling the respective TLS certificate of the HTTPS server under Server Security > TLS(HTTPS) Options. 
This is only applicable in UEFI Mode. 
Note: Booting from an ISO file can involve only booting a preliminary OS environment image, such as WinPE or a mini Linux, or a complete OS install image if the OS supports the HTTP Boot feature (Old OS versions may not support this). Please check your OS documentation for the HTTP Boot feature support.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
### UrlBootFile2

Use this option to configure a network URL to a bootable ISO or EFI file. URLs in HTTP/HTTPS are accepted using either an IPv4 or IPv6 server address, or using a host name. For example, the URLs can be in any of the following formats: http://192.168.0.1/file/image.iso, http://example.com/file/image.efi, https://example.com/file/image.efi, http://[1234::1000]/image.iso. 
When configured, this URL is listed as a boot option in the UEFI boot menu. Selecting this boot option downloads the file to the system memory, and configures the system to attempt to boot from it. There is no specific ordering on this option. It can be independently ordered in the boot menu. 
This setting requires configuring the 'Pre-Boot Network Interface' option if you want to access the URL location through a specific network interface. When a HTTPS URL is configured, this setting requires enrolling the respective TLS certificate of the HTTPS server under Server Security > TLS(HTTPS) Options. 
This is only applicable in UEFI Mode. 
Note: Booting from an ISO file can involve only booting a preliminary OS environment image, such as WinPE or a mini Linux, or a complete OS install image if the OS supports the HTTP Boot feature (Old OS versions may not support this). Please check your OS documentation for the HTTP Boot feature support.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
### UrlBootFile3

Use this option to configure a network URL to a bootable ISO or EFI file. URLs in HTTP/HTTPS are accepted using either an IPv4 or IPv6 server address, or using a host name. For example, the URLs can be in any of the following formats: http://192.168.0.1/file/image.iso, http://example.com/file/image.efi, https://example.com/file/image.efi, http://[1234::1000]/image.iso. 
When configured, this URL is listed as a boot option in the UEFI boot menu. Selecting this boot option downloads the file to the system memory, and configures the system to attempt to boot from it. There is no specific ordering on this option. It can be independently ordered in the boot menu. 
This setting requires configuring the 'Pre-Boot Network Interface' option if you want to access the URL location through a specific network interface. When a HTTPS URL is configured, this setting requires enrolling the respective TLS certificate of the HTTPS server under Server Security > TLS(HTTPS) Options. 
This is only applicable in UEFI Mode. 
Note: Booting from an ISO file can involve only booting a preliminary OS environment image, such as WinPE or a mini Linux, or a complete OS install image if the OS supports the HTTP Boot feature (Old OS versions may not support this). Please check your OS documentation for the HTTP Boot feature support.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
### UrlBootFile4

Use this option to configure a network URL to a bootable ISO or EFI file. URLs in HTTP/HTTPS are accepted using either an IPv4 or IPv6 server address, or using a host name. For example, the URLs can be in any of the following formats: http://192.168.0.1/file/image.iso, http://example.com/file/image.efi, https://example.com/file/image.efi, http://[1234::1000]/image.iso. 
When configured, this URL is listed as a boot option in the UEFI boot menu. Selecting this boot option downloads the file to the system memory, and configures the system to attempt to boot from it. There is no specific ordering on this option. It can be independently ordered in the boot menu. 
This setting requires configuring the 'Pre-Boot Network Interface' option if you want to access the URL location through a specific network interface. When a HTTPS URL is configured, this setting requires enrolling the respective TLS certificate of the HTTPS server under Server Security > TLS(HTTPS) Options. 
This is only applicable in UEFI Mode. 
Note: Booting from an ISO file can involve only booting a preliminary OS environment image, such as WinPE or a mini Linux, or a complete OS install image if the OS supports the HTTP Boot feature (Old OS versions may not support this). Please check your OS documentation for the HTTP Boot feature support.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
### UsbBoot

Set this option to disabled to prevent the system from booting to any USB devices connected to the server. This includes preventing boot to virtual media devices, and the embedded SD or uSD card slot (if supported).


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`UsbBoot` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### UsbControl

All USB Ports Enabled: Enables all USB ports and embedded devices.All USB Ports Disabled: Disables all USB ports and embedded devices.External USB Ports Disabled: Disables only external USB ports.Internal USB Ports Disabled: Disables only internal USB ports.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`UsbControl` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`UsbEnabled`|All USB Ports Enabled
|`UsbDisabled`|All USB Ports Disabled
|`ExternalUsbDisabled`|External USB Ports Disabled
|`InternalUsbDisabled`|Internal USB Ports Disabled
### UserDefaultsState

Displays whether user default settings are enabled or disabled.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`UserDefaultsState` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### UtilityLang

Select this option to adjust the current language for the system.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`UtilityLang` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`English`|English
|`Japanese`|日本語
|`Chinese`|中文（简体）
### VideoOptions

Use this option to configure video settings in the system. When set to Add-in Video Enabled, Embedded Video Disabled, the system only displays video to the first discovered add-in video controller. When set to Both Add-in and Embedded Video Enabled, the system displays video to both the embedded and the first discovered add-in video controllers. In both modes, early system startup video is displayed to the embedded video controller.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`VideoOptions` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`OptionalVideoOnly`|Add-in Video Enabled, Embedded Video Disabled
|`BothVideoEnabled`|Both Add-in and Embedded Video Enabled
### VirtualInstallDisk

Use this option to control the Virtual Install Disk. The Virtual Install Disk contains drivers specific to this server that an OS can use during installation. If enabled, the Virtual Install Disk appears as a drive in the operating system.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`VirtualInstallDisk` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### VirtualSerialPort

Use this option to assign the logical COM port address and associated default resources used by the Virtual Serial Port (VSP). VSP enables the Management Processor to present an emulated serial port to support the BIOS Serial Console and operating system serial console.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`VirtualSerialPort` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Com1Irq4`|COM 1; IRQ4; I/O: 3F8h-3FFh
|`Com2Irq3`|COM 2; IRQ3; I/O: 2F8h-2FFh
|`Disabled`|Disabled
### VlanControl

Use this option to enable or disable VLAN tagging on all enabled network interfaces.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`VlanControl` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### VlanId

Use this option to set the global VLAN ID for all enabled network interfaces. Valid values are 0 to 4094.A value of 0 sets the device to send untagged frames.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|Yes (if resource allows PATCH)
### VlanPriority

Use this option to set the priority for the VLAN tagged frames. Valid values are 0 to 7.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|Yes (if resource allows PATCH)
### WakeOnLan

You can configure the server to be powered on remotely when it receives a special packet. This option requires a NIC, NIC driver, and operating system that are WOL-capable.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`WakeOnLan` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### WorkloadProfile

Select this option to choose a workload profile for power and performance.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`WorkloadProfile` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`GeneralPowerEfficientCompute`|General Power Efficient Compute
|`GeneralPeakFrequencyCompute`|General Peak Frequency Compute
|`GeneralThroughputCompute`|General Throughput Compute
|`Virtualization-PowerEfficient`|Virtualization - Power Efficient
|`Virtualization-MaxPerformance`|Virtualization - Max Performance
|`LowLatency`|Low Latency
|`MissionCritical`|Mission Critical
|`TransactionalApplicationProcessing`|Transactional Application Processing
|`HighPerformanceCompute(HPC)`|High Performance Compute (HPC)
|`DecisionSupport`|Decision Support
|`GraphicProcessing`|Graphic Processing
|`I/OThroughput`|I/O Throughput
|`Custom`|Custom
### XptPrefetcher

Use this option to disable the processor XPT Prefetch feature. In some cases, setting this option to disabled can improve performance. Typically, setting this option to enabled provides better performance. Only disable this option after performing application benchmarking to verify improved performance in the environment. This option must be enabled when Sub-Numa Clustering (SNC) is enabled.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`XptPrefetcher` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|Enabled
|`Disabled`|Disabled
### iSCSIPolicy

Use this option to set the iSCSI Policy. If configured to Software Initiator, the iSCSI software initiator will be used to access iSCSI targets on any configured NIC ports. If configured to Adapter Initiator, the adapter specific iSCSI initiator will be used instead. The adapter firmware must be configured to access iSCSI targets from the adapter initiator.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`iSCSIPolicy` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`SoftwareInitiator`|Software Initiator
|`AdapterInitiator`|Adapter Initiator
## Chassis
```@odata.type: "#Chassis.v1_2_0.Chassis"```

The schema definition for the Chassis resource represents the properties for physical components for any system. This object represents racks, rack mount servers, blades, standalone, modular systems, enclosures, and all other containers. The non-CPU/device-centric parts of the schema are accessed either directly or indirectly through this resource.

> **Resource Instances of this Type**:  

> * `https://{iLO}/redfish/v1/chassis/{item}/`

### AssetTag

The chassis user-assigned asset tag.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"AssetTag": "&lt;string-value&gt;"}

### ChassisType

This property indicates the physical form factor type of this resource.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`ChassisType` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Rack`|
|`Blade`|
|`Enclosure`|
|`StandAlone`|
|`RackMount`|
|`Card`|
|`Cartridge`|
|`Row`|
|`Pod`|
|`Expansion`|
|`Sidecar`|
|`Zone`|
|`Sled`|
|`Shelf`|
|`Other`|
### IndicatorLED

The chassis indicator LED that is used to identify the chassis. The user can manipulate this LED.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"IndicatorLED": "Lit"}

`IndicatorLED` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`Unknown`|
|`Lit`|
|`Blinking`|
|`Off`|
### Manufacturer

The chassis manufacturer.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Model

The chassis model number.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.BayNumber

The position of the chassis inside an enclosure.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Oem.Hpe.BaysConsumedHeight

The number of enclosure bays this chassis consumes in height.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Oem.Hpe.BaysConsumedWidth

The number of enclosure bays this chassis consumes in width.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Oem.Hpe.Firmware.PlatformDefinitionTable.Current.VersionString

The version of the Intelligent Platform Abstraction Data.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.Firmware.PowerManagementController.Current.VersionString

The firmware version of the Power Monitor.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.Firmware.PowerManagementControllerBootloader.Current.Family

The family type of the Power Monitor hardware.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.Firmware.PowerManagementControllerBootloader.Current.VersionString

The firmware version of the Power Monitor boot loader.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.Firmware.SASProgrammableLogicDevice.Current.VersionString

The firmware version of the SAS controller.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.Firmware.SPSFirmwareVersionData.Current.VersionString

The SPS FW Version number, aka ME FW Version, AAAA.BBBB.CCCC.DDDD.E


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.Firmware.SystemProgrammableLogicDevice.Current.VersionString

The firmware version of the CPLD.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.Images.Front.extref

The URI of an external resource.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.Images.Model.extref

The URI of an external resource.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.Location.GeographicLocation.RackName

The name of the chassis enclosure.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.Location.LocationInRack.RackLdsPartNumber

The chassis rack part number.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.Location.LocationInRack.RackLdsProductDescription

 The chassis rack product description.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.Location.LocationInRack.RackUHeight

The chassis rack U height.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Oem.Hpe.Location.LocationInRack.RackUUID

The chassis rack UUID.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.Location.LocationInRack.TagVersion

The chassis rack tag version.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Oem.Hpe.Location.LocationInRack.ULocation

The chassis rack U location.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.Location.LocationInRack.UPosition

The chassis U position in the rack.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Oem.Hpe.Location.LocationOfChassis.UUID

The chassis UUID provided by SMBIOS.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.PowerAlertMode.Activated

The power alert mode activation state.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### Oem.Hpe.PowerAlertMode.AlertPowerWatts

The power consumption of the system when operating in alert mode.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Oem.Hpe.SmartStorageBattery[array-item].BatteryWearLevelPercent

The battery wear level percentage. When this value reaches 100%, the battery is completely worn out and needs to be replaced. The value is null if battery wear level cannot be determined or is not supported.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Oem.Hpe.SmartStorageBattery[array-item].ChargeLevelPercent

State of charge of the battery.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Oem.Hpe.SmartStorageBattery[array-item].ErrorCode

Error code of the battery.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Oem/Hpe/SmartStorageBattery[]/ErrorCode` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`GeneralFailure`|
|`HighInternalBatteryResistance`|
|`LowOpenCircuitVoltage`|
|`BatteryCellFailure`|
|`BatteryChargeTimeout`|
|`OverTemperature`|
|`DischargeBelowMinimumVoltage`|
|`DischargeCurrentHigh`|
|`LoadCountExceeded`|
|`BackupSucceeded`|
|`OverCurrent`|
|`PermanentFailure`|
|`BackupTimeExceeded`|
### Oem.Hpe.SmartStorageBattery[array-item].FailurePredicted

Is this battery currently predicting a failure in the near future.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### Oem.Hpe.SmartStorageBattery[array-item].FirmwareVersion

Firmware version of the battery.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.SmartStorageBattery[array-item].Index

Index of the battery.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Oem.Hpe.SmartStorageBattery[array-item].MaximumCapWatts

Maximum capacity of the battery in watts.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Oem.Hpe.SmartStorageBattery[array-item].Model

Model of the battery.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.SmartStorageBattery[array-item].ProductName

Product name of the battery.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.SmartStorageBattery[array-item].RemainingChargeTimeSeconds

Remaining charging time of the battery in seconds.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Oem.Hpe.SmartStorageBattery[array-item].SerialNumber

Serial number of the battery.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.SmartStorageBattery[array-item].SparePartNumber

Spare part number of the battery.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.SmartStorageBattery[array-item].Status.Health

This represents the health state of this resource in the absence of its dependent resources.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Oem/Hpe/SmartStorageBattery[]/Status/Health` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`OK`|
|`Warning`|
|`Critical`|
### Oem.Hpe.SmartStorageBattery[array-item].Status.HealthRollup

This represents the overall health state from the view of this resource.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Oem/Hpe/SmartStorageBattery[]/Status/HealthRollup` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`OK`|
|`Warning`|
|`Critical`|
### Oem.Hpe.SmartStorageBattery[array-item].Status.State

This indicates the known state of the resource, such as if it is enabled.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Oem/Hpe/SmartStorageBattery[]/Status/State` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`Enabled`|
|`Disabled`|
|`Offline`|
|`InTest`|
|`Starting`|
|`Absent`|
### Oem.Hpe.SystemMaintenanceSwitches.Sw1

Override iLO security.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Oem/Hpe/SystemMaintenanceSwitches/Sw1` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`On`|
|`Off`|
### Oem.Hpe.SystemMaintenanceSwitches.Sw10

Reserved.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Oem/Hpe/SystemMaintenanceSwitches/Sw10` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`On`|
|`Off`|
### Oem.Hpe.SystemMaintenanceSwitches.Sw11

Reserved.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Oem/Hpe/SystemMaintenanceSwitches/Sw11` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`On`|
|`Off`|
### Oem.Hpe.SystemMaintenanceSwitches.Sw12

Reserved.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Oem/Hpe/SystemMaintenanceSwitches/Sw12` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`On`|
|`Off`|
### Oem.Hpe.SystemMaintenanceSwitches.Sw2

Reserved.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Oem/Hpe/SystemMaintenanceSwitches/Sw2` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`On`|
|`Off`|
### Oem.Hpe.SystemMaintenanceSwitches.Sw3

Reserved.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Oem/Hpe/SystemMaintenanceSwitches/Sw3` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`On`|
|`Off`|
### Oem.Hpe.SystemMaintenanceSwitches.Sw4

Reserved.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Oem/Hpe/SystemMaintenanceSwitches/Sw4` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`On`|
|`Off`|
### Oem.Hpe.SystemMaintenanceSwitches.Sw5

BIOS/UEFI Password Disable.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Oem/Hpe/SystemMaintenanceSwitches/Sw5` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`On`|
|`Off`|
### Oem.Hpe.SystemMaintenanceSwitches.Sw6

Reset Configuration.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Oem/Hpe/SystemMaintenanceSwitches/Sw6` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`On`|
|`Off`|
### Oem.Hpe.SystemMaintenanceSwitches.Sw7

Reserved.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Oem/Hpe/SystemMaintenanceSwitches/Sw7` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`On`|
|`Off`|
### Oem.Hpe.SystemMaintenanceSwitches.Sw8

Reserved.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Oem/Hpe/SystemMaintenanceSwitches/Sw8` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`On`|
|`Off`|
### Oem.Hpe.SystemMaintenanceSwitches.Sw9

Reserved.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Oem/Hpe/SystemMaintenanceSwitches/Sw9` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`On`|
|`Off`|
### PartNumber

The chassis part number.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### PhysicalSecurity.IntrusionSensor

This indicates the known state of the physical security sensor, such as if it is hardware intrusion detected.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`PhysicalSecurity/IntrusionSensor` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Normal`|
|`HardwareIntrusion`|
|`TamperingDetected`|
### PhysicalSecurity.IntrusionSensorReArm

This indicates how the Normal state to be restored.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`PhysicalSecurity/IntrusionSensorReArm` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Manual`|
|`Automatic`|
### SKU

The chassis SKU.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### SerialNumber

The chassis serial number.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Status.Health

This represents the health state of this resource in the absence of its dependent resources.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Status/Health` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`OK`|
|`Warning`|
|`Critical`|
### Status.HealthRollup

This represents the overall health state from the view of this resource.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Status/HealthRollup` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`OK`|
|`Warning`|
|`Critical`|
### Status.State

This indicates the known state of the resource, such as if it is enabled.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Status/State` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`Enabled`|
|`Disabled`|
|`Offline`|
|`InTest`|
|`Starting`|
|`Absent`|
## ComputerSystem
```@odata.type: "#ComputerSystem.v1_2_0.ComputerSystem"```

The schema definition of a computer system and its properties. A computer system represents a physical or virtual machine and the local resources, such as memory, CPU, and other devices that can be accessed from that machine.

> **Resource Instances of this Type**:  

> * `https://{iLO}/redfish/v1/systems/{item}/`

### AssetTag

A user-definable tag that is used to track this system for inventory or other client purposes.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"AssetTag": "&lt;string-value&gt;"}

### BiosVersion

The version of the system BIOS or primary system firmware.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
### Boot.BootSourceOverrideEnabled

BootSourceOverrideTarget must be specified before BootSourceOverrideEnabled can be used.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Boot": {"BootSourceOverrideEnabled": "Once"}}

`Boot/BootSourceOverrideEnabled` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`Disabled`|
|`Once`|
|`Continuous`|
### Boot.BootSourceOverrideMode


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Boot": {"BootSourceOverrideMode": "UEFI"}}

`Boot/BootSourceOverrideMode` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Legacy`|
|`UEFI`|
### Boot.BootSourceOverrideTarget

The current boot source to be used at next boot instead of the normal boot device, if BootSourceOverrideEnabled is true.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Boot": {"BootSourceOverrideTarget": "&lt;string-value&gt;"}}

### Boot.UefiTargetBootSourceOverride

This property is the UEFI Device Path of the device to boot from when BootSourceOverrideSupported is UefiTarget.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Boot": {"UefiTargetBootSourceOverride": "&lt;string-value&gt;"}}

### HostName

The DNS Host Name, without any domain information


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
### IndicatorLED

The state of the indicator LED.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"IndicatorLED": "Lit"}

`IndicatorLED` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`Unknown`|
|`Lit`|
|`Blinking`|
|`Off`|
### Manufacturer

The manufacturer or OEM of this system.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### MemorySummary.Status.Health

This represents the health state of this resource in the absence of its dependent resources.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`MemorySummary/Status/Health` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`OK`|
|`Warning`|
|`Critical`|
### MemorySummary.Status.HealthRollup

This represents the overall health state from the view of this resource.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`MemorySummary/Status/HealthRollup` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`OK`|
|`Warning`|
|`Critical`|
### MemorySummary.Status.State

This indicates the known state of the resource, such as if it is enabled.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`MemorySummary/Status/State` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`Enabled`|
|`Disabled`|
|`Offline`|
|`InTest`|
|`Starting`|
|`Absent`|
### MemorySummary.TotalSystemMemoryGiB

This is the total amount of memory in the system measured in GiB.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Model

The model information that the manufacturer uses to refer to this system.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.AggregateHealthStatus.AgentlessManagementService

This indicates if the Agentless Management Service is available or not. 


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Oem/Hpe/AggregateHealthStatus/AgentlessManagementService` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Unavailable`|
|`Ready`|
### Oem.Hpe.AggregateHealthStatus.BiosOrHardwareHealth.Status.Health

This represents the health state of this resource in the absence of its dependent resources.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Oem/Hpe/AggregateHealthStatus/BiosOrHardwareHealth/Status/Health` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`OK`|
|`Warning`|
|`Critical`|
### Oem.Hpe.AggregateHealthStatus.BiosOrHardwareHealth.Status.HealthRollup

This represents the overall health state from the view of this resource.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Oem/Hpe/AggregateHealthStatus/BiosOrHardwareHealth/Status/HealthRollup` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`OK`|
|`Warning`|
|`Critical`|
### Oem.Hpe.AggregateHealthStatus.BiosOrHardwareHealth.Status.State

This indicates the known state of the resource, such as if it is enabled.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Oem/Hpe/AggregateHealthStatus/BiosOrHardwareHealth/Status/State` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`Enabled`|
|`Disabled`|
|`Offline`|
|`InTest`|
|`Starting`|
|`Absent`|
### Oem.Hpe.AggregateHealthStatus.FanRedundancy

This indicates if the Fan is redundant or not. 


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Oem/Hpe/AggregateHealthStatus/FanRedundancy` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Redundant`|
|`NonRedundant`|
|`FailedRedundant`|
|`Unknown`|
### Oem.Hpe.AggregateHealthStatus.Fans.Status.Health

This represents the health state of this resource in the absence of its dependent resources.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Oem/Hpe/AggregateHealthStatus/Fans/Status/Health` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`OK`|
|`Warning`|
|`Critical`|
### Oem.Hpe.AggregateHealthStatus.Fans.Status.HealthRollup

This represents the overall health state from the view of this resource.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Oem/Hpe/AggregateHealthStatus/Fans/Status/HealthRollup` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`OK`|
|`Warning`|
|`Critical`|
### Oem.Hpe.AggregateHealthStatus.Fans.Status.State

This indicates the known state of the resource, such as if it is enabled.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Oem/Hpe/AggregateHealthStatus/Fans/Status/State` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`Enabled`|
|`Disabled`|
|`Offline`|
|`InTest`|
|`Starting`|
|`Absent`|
### Oem.Hpe.AggregateHealthStatus.Memory.Status.Health

This represents the health state of this resource in the absence of its dependent resources.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Oem/Hpe/AggregateHealthStatus/Memory/Status/Health` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`OK`|
|`Warning`|
|`Critical`|
### Oem.Hpe.AggregateHealthStatus.Memory.Status.HealthRollup

This represents the overall health state from the view of this resource.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Oem/Hpe/AggregateHealthStatus/Memory/Status/HealthRollup` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`OK`|
|`Warning`|
|`Critical`|
### Oem.Hpe.AggregateHealthStatus.Memory.Status.State

This indicates the known state of the resource, such as if it is enabled.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Oem/Hpe/AggregateHealthStatus/Memory/Status/State` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`Enabled`|
|`Disabled`|
|`Offline`|
|`InTest`|
|`Starting`|
|`Absent`|
### Oem.Hpe.AggregateHealthStatus.Network.Status.Health

This represents the health state of this resource in the absence of its dependent resources.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Oem/Hpe/AggregateHealthStatus/Network/Status/Health` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`OK`|
|`Warning`|
|`Critical`|
### Oem.Hpe.AggregateHealthStatus.Network.Status.HealthRollup

This represents the overall health state from the view of this resource.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Oem/Hpe/AggregateHealthStatus/Network/Status/HealthRollup` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`OK`|
|`Warning`|
|`Critical`|
### Oem.Hpe.AggregateHealthStatus.Network.Status.State

This indicates the known state of the resource, such as if it is enabled.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Oem/Hpe/AggregateHealthStatus/Network/Status/State` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`Enabled`|
|`Disabled`|
|`Offline`|
|`InTest`|
|`Starting`|
|`Absent`|
### Oem.Hpe.AggregateHealthStatus.PowerSupplies.PowerSuppliesMismatch

This indicates if the there is a mismatch in the power supplies.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### Oem.Hpe.AggregateHealthStatus.PowerSupplies.Status.Health

This represents the health state of this resource in the absence of its dependent resources.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Oem/Hpe/AggregateHealthStatus/PowerSupplies/Status/Health` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`OK`|
|`Warning`|
|`Critical`|
### Oem.Hpe.AggregateHealthStatus.PowerSupplies.Status.HealthRollup

This represents the overall health state from the view of this resource.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Oem/Hpe/AggregateHealthStatus/PowerSupplies/Status/HealthRollup` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`OK`|
|`Warning`|
|`Critical`|
### Oem.Hpe.AggregateHealthStatus.PowerSupplies.Status.State

This indicates the known state of the resource, such as if it is enabled.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Oem/Hpe/AggregateHealthStatus/PowerSupplies/Status/State` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`Enabled`|
|`Disabled`|
|`Offline`|
|`InTest`|
|`Starting`|
|`Absent`|
### Oem.Hpe.AggregateHealthStatus.PowerSupplyRedundancy

This indicates if the Power Supply is redundant or not. 


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Oem/Hpe/AggregateHealthStatus/PowerSupplyRedundancy` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Redundant`|
|`NonRedundant`|
|`FailedRedundant`|
|`Unknown`|
### Oem.Hpe.AggregateHealthStatus.Processors.Status.Health

This represents the health state of this resource in the absence of its dependent resources.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Oem/Hpe/AggregateHealthStatus/Processors/Status/Health` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`OK`|
|`Warning`|
|`Critical`|
### Oem.Hpe.AggregateHealthStatus.Processors.Status.HealthRollup

This represents the overall health state from the view of this resource.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Oem/Hpe/AggregateHealthStatus/Processors/Status/HealthRollup` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`OK`|
|`Warning`|
|`Critical`|
### Oem.Hpe.AggregateHealthStatus.Processors.Status.State

This indicates the known state of the resource, such as if it is enabled.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Oem/Hpe/AggregateHealthStatus/Processors/Status/State` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`Enabled`|
|`Disabled`|
|`Offline`|
|`InTest`|
|`Starting`|
|`Absent`|
### Oem.Hpe.AggregateHealthStatus.SmartStorageBattery.Status.Health

This represents the health state of this resource in the absence of its dependent resources.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Oem/Hpe/AggregateHealthStatus/SmartStorageBattery/Status/Health` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`OK`|
|`Warning`|
|`Critical`|
### Oem.Hpe.AggregateHealthStatus.SmartStorageBattery.Status.HealthRollup

This represents the overall health state from the view of this resource.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Oem/Hpe/AggregateHealthStatus/SmartStorageBattery/Status/HealthRollup` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`OK`|
|`Warning`|
|`Critical`|
### Oem.Hpe.AggregateHealthStatus.SmartStorageBattery.Status.State

This indicates the known state of the resource, such as if it is enabled.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Oem/Hpe/AggregateHealthStatus/SmartStorageBattery/Status/State` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`Enabled`|
|`Disabled`|
|`Offline`|
|`InTest`|
|`Starting`|
|`Absent`|
### Oem.Hpe.AggregateHealthStatus.Storage.Status.Health

This represents the health state of this resource in the absence of its dependent resources.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Oem/Hpe/AggregateHealthStatus/Storage/Status/Health` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`OK`|
|`Warning`|
|`Critical`|
### Oem.Hpe.AggregateHealthStatus.Storage.Status.HealthRollup

This represents the overall health state from the view of this resource.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Oem/Hpe/AggregateHealthStatus/Storage/Status/HealthRollup` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`OK`|
|`Warning`|
|`Critical`|
### Oem.Hpe.AggregateHealthStatus.Storage.Status.State

This indicates the known state of the resource, such as if it is enabled.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Oem/Hpe/AggregateHealthStatus/Storage/Status/State` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`Enabled`|
|`Disabled`|
|`Offline`|
|`InTest`|
|`Starting`|
|`Absent`|
### Oem.Hpe.AggregateHealthStatus.Temperatures.Status.Health

This represents the health state of this resource in the absence of its dependent resources.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Oem/Hpe/AggregateHealthStatus/Temperatures/Status/Health` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`OK`|
|`Warning`|
|`Critical`|
### Oem.Hpe.AggregateHealthStatus.Temperatures.Status.HealthRollup

This represents the overall health state from the view of this resource.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Oem/Hpe/AggregateHealthStatus/Temperatures/Status/HealthRollup` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`OK`|
|`Warning`|
|`Critical`|
### Oem.Hpe.AggregateHealthStatus.Temperatures.Status.State

This indicates the known state of the resource, such as if it is enabled.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Oem/Hpe/AggregateHealthStatus/Temperatures/Status/State` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`Enabled`|
|`Disabled`|
|`Offline`|
|`InTest`|
|`Starting`|
|`Absent`|
### Oem.Hpe.Bios.Backup.BuildNumber

The build number of the firmware.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Oem.Hpe.Bios.Backup.BuildNumberString

The string version of the build number of the firmware.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.Bios.Backup.Date

The build date of the firmware.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.Bios.Backup.DebugBuild

True if the firmware is a debug build; False if it is not.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### Oem.Hpe.Bios.Backup.Family

The family of the firmware.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.Bios.Backup.MajorVersion

The major version of the firmware.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Oem.Hpe.Bios.Backup.MinorVersion

The minor version of the firmware.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Oem.Hpe.Bios.Backup.Time

The build time of the firmware.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.Bios.Backup.VersionString

The version string of the firmware. This value might be null if VersionString is unavailable.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.Bios.Bootblock.BuildNumber

The build number of the firmware.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Oem.Hpe.Bios.Bootblock.BuildNumberString

The string version of the build number of the firmware.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.Bios.Bootblock.Date

The build date of the firmware.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.Bios.Bootblock.DebugBuild

True if the firmware is a debug build; False if it is not.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### Oem.Hpe.Bios.Bootblock.Family

The family of the firmware.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.Bios.Bootblock.MajorVersion

The major version of the firmware.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Oem.Hpe.Bios.Bootblock.MinorVersion

The minor version of the firmware.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Oem.Hpe.Bios.Bootblock.Time

The build time of the firmware.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.Bios.Bootblock.VersionString

The version string of the firmware. This value might be null if VersionString is unavailable.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.Bios.Current.BuildNumber

The build number of the firmware.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Oem.Hpe.Bios.Current.BuildNumberString

The string version of the build number of the firmware.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.Bios.Current.Date

The build date of the firmware.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.Bios.Current.DebugBuild

True if the firmware is a debug build; False if it is not.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### Oem.Hpe.Bios.Current.Family

The family of the firmware.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.Bios.Current.MajorVersion

The major version of the firmware.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Oem.Hpe.Bios.Current.MinorVersion

The minor version of the firmware.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Oem.Hpe.Bios.Current.Time

The build time of the firmware.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.Bios.Current.VersionString

The version string of the firmware. This value might be null if VersionString is unavailable.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.Bios.UefiClass

The UEFI BIOS Class value defined in the UEFI specification.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Oem.Hpe.DeviceDiscoveryComplete.AMSDeviceDiscovery

This property indicates the current AMS Device Discovery Status.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Oem/Hpe/DeviceDiscoveryComplete/AMSDeviceDiscovery` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`Busy`|
|`Complete`|
|`NoAMS`|
|`Initial`|
### Oem.Hpe.DeviceDiscoveryComplete.DeviceDiscovery

This property indicates the current device discovery status of devices that are not Smart Array or AMS related.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Oem/Hpe/DeviceDiscoveryComplete/DeviceDiscovery` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`Busy`|
|`vAuxDeviceDiscoveryComplete`|
|`vMainDeviceDiscoveryComplete`|
|`DataIncomplete`|
|`Initial`|
### Oem.Hpe.DeviceDiscoveryComplete.SmartArrayDiscovery

This property indicates the current Smart Array Storage Device Discovery Status.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Oem/Hpe/DeviceDiscoveryComplete/SmartArrayDiscovery` can take one of the following values (note that some implementations might support a subset of the values):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`Busy`|
|`PendingSoftwareRAID`|
|`Complete`|
|`Initial`|
|`Cached`|
### Oem.Hpe.EndOfPostDelaySeconds

Supported on UEFI based systems only. The number of seconds to delay before finalizing POST with the Mode action (For example, the delay before shutdown.).


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Oem": {"Hpe": {"EndOfPostDelaySeconds": &lt;integer-value&gt;}}}

### Oem.Hpe.HostOS.OsName

From cpqHoName if AMS is running.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.HostOS.OsSysDescription

from cpqHosysDesc if AMS is running


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.HostOS.OsType

from cpqHoOsType if AMS is running.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Oem.Hpe.HostOS.OsVersion

from cpqHoVersion if AMS is running


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.IntelligentProvisioningAlwaysOn

Always on Intelligent Provisioning is available.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### Oem.Hpe.IntelligentProvisioningIndex

 Index in the Firmware Version Table for Intelligent Provisioning.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Oem.Hpe.IntelligentProvisioningLocation

 Location string of Intelligent Provisioning in Firmware Version Table.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.IntelligentProvisioningVersion

 Intelligent Provisioning Version.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.PCAPartNumber

The PCA part number.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.PCASerialNumber

The PCA serial number.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.PostDiscoveryCompleteTimeStamp

Displays the last known POST Discovery Complete time


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.PostDiscoveryMode

The manner in which the system will operate during the discovery section of POST.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Oem": {"Hpe": {"PostDiscoveryMode": "ForceFullDiscovery"}}}

`Oem/Hpe/PostDiscoveryMode` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`Auto`|
|`ForceFullDiscovery`|
|`ForceFastBoot`|
### Oem.Hpe.PostMode

The manner in which the system will operate during and at completion of POST.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Oem": {"Hpe": {"PostMode": "PostToShutdown"}}}

`Oem/Hpe/PostMode` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`Normal`|
|`PostToShutdown`|
|`PostToReboot`|
### Oem.Hpe.PostState

The current state of system POST.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Oem/Hpe/PostState` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`Unknown`|
|`Reset`|
|`PowerOff`|
|`InPost`|
|`InPostDiscoveryComplete`|
|`FinishedPost`|
### Oem.Hpe.PowerAllocationLimit

The total amount of power allocated to the system.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Oem.Hpe.PowerAutoOn

Auto Power-On mode defines what occurs when the AC power is applied to the system.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Oem": {"Hpe": {"PowerAutoOn": "PowerOn"}}}

`Oem/Hpe/PowerAutoOn` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`RemainOff`|
|`PowerOn`|
|`Restore`|
### Oem.Hpe.PowerOnDelay

The PowerAutoOn policy delay that can also be found in the HpBios::PowerOnDelay object.  Will be null if PowerAutoOn is set to RemainOff.  Blades only support Minimum and RandomUpTo120Sec.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Oem": {"Hpe": {"PowerOnDelay": "30Sec"}}}

`Oem/Hpe/PowerOnDelay` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`Minimum`|
|`15Sec`|
|`30Sec`|
|`45Sec`|
|`60Sec`|
|`RandomUpTo120Sec`|
### Oem.Hpe.PowerRegulatorMode

HPE Power Regulator mode.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Oem": {"Hpe": {"PowerRegulatorMode": "Max"}}}

`Oem/Hpe/PowerRegulatorMode` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`OSControl`|
|`Dynamic`|
|`Max`|
|`Min`|
|`Unknown`|
### Oem.Hpe.SMBIOS.extref

The URI of an external resource.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.ServerSignature

 The CRC32 of:  All Device Signatures combined together, Blade Slot Location in Enclosure, Enclosure UUID, and OneView Domain IP Address


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Oem.Hpe.ServerSignatureStatus

The current state of Server Signature.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Oem/Hpe/ServerSignatureStatus` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`Initial`|
|`Busy`|
|`Invalid`|
|`Complete`|
### Oem.Hpe.VirtualProfile

The current state of the systems virtual profile.  This profile is the one that, when the server is rebooted, will set the  Virtual properties.  Intent is to use this state to determine whether the server needs to be rebooted so these values are set.  Additional informaiton about the profile will be considered later.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Oem/Hpe/VirtualProfile` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Active`|
|`Busy`|
|`Inactive`|
|`Unknown`|
### Oem.Hpe.VirtualUUID

Used in conjunction with the UUID (Logical) value.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.actions.actions.HpeComputerSystemExt.PowerButton.Action

The Action to be performed.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`Oem/Hpe/actions/actions/HpeComputerSystemExt.PowerButton/Action` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`HpeComputerSystemExt.PowerButton`|
### Oem.Hpe.actions.actions.HpeComputerSystemExt.PowerButton.PushType

PushType identifies the type of Action to be performed.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Oem/Hpe/actions/actions/HpeComputerSystemExt.PowerButton/PushType` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Press`|
|`PressAndHold`|
### Oem.Hpe.actions.actions.HpeComputerSystemExt.ServerSigRecompute.Action

The Action to be performed.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`Oem/Hpe/actions/actions/HpeComputerSystemExt.ServerSigRecompute/Action` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`HpeComputerSystemExt.ServerSigRecompute`|
### Oem.Hpe.actions.actions.HpeComputerSystemExt.SystemReset.Action

The Action to be performed.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`Oem/Hpe/actions/actions/HpeComputerSystemExt.SystemReset/Action` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`HpeComputerSystemExt.SystemReset`|
### Oem.Hpe.actions.actions.HpeComputerSystemExt.SystemReset.ResetType

ResetType identifies the type of Action to be performed.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`Oem/Hpe/actions/actions/HpeComputerSystemExt.SystemReset/ResetType` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`ColdBoot`|
### PartNumber

The manufacturer's system part number.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### PowerState

This is the current power state of the system


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`PowerState` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`On`|
|`Off`|
|`Unknown`|
|`Reset`|
### ProcessorSummary.Count

The number of processors in the system.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### ProcessorSummary.Model

The processor model for the primary or majority of processors in this system.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### ProcessorSummary.Status.Health

This represents the health state of this resource in the absence of its dependent resources.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`ProcessorSummary/Status/Health` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`OK`|
|`Warning`|
|`Critical`|
### ProcessorSummary.Status.HealthRollup

This represents the overall health state from the view of this resource.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`ProcessorSummary/Status/HealthRollup` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`OK`|
|`Warning`|
|`Critical`|
### ProcessorSummary.Status.State

This indicates the known state of the resource, such as if it is enabled.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`ProcessorSummary/Status/State` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`Enabled`|
|`Disabled`|
|`Offline`|
|`InTest`|
|`Starting`|
|`Absent`|
### SKU

SKU for this system.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### SerialNumber

The system serial number.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Status.Health

This represents the health state of this resource in the absence of its dependent resources.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Status/Health` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`OK`|
|`Warning`|
|`Critical`|
### Status.HealthRollup

This represents the overall health state from the view of this resource.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Status/HealthRollup` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`OK`|
|`Warning`|
|`Critical`|
### Status.State

This indicates the known state of the resource, such as if it is enabled.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Status/State` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`Enabled`|
|`Disabled`|
|`Offline`|
|`InTest`|
|`Starting`|
|`Absent`|
### SystemType

The type of computer system that this resource represents.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`SystemType` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Physical`|
|`Virtual`|
|`OS`|
|`PhysicallyPartitioned`|
|`VirtuallyPartitioned`|
### TrustedModules[array-item].FirmwareVersion

The firmware version of this Trusted Module


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### TrustedModules[array-item].InterfaceType

This property indicates the interface type of the Trusted Module.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`TrustedModules[]/InterfaceType` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`TM1_0`|
|`TPM1_2`|
|`TPM2_0`|
### TrustedModules[array-item].Status.Health

This represents the health state of this resource in the absence of its dependent resources.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`TrustedModules[]/Status/Health` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`OK`|
|`Warning`|
|`Critical`|
### TrustedModules[array-item].Status.HealthRollup

This represents the overall health state from the view of this resource.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`TrustedModules[]/Status/HealthRollup` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`OK`|
|`Warning`|
|`Critical`|
### TrustedModules[array-item].Status.State

This indicates the known state of the resource, such as if it is enabled.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`TrustedModules[]/Status/State` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`Enabled`|
|`Disabled`|
|`Offline`|
|`InTest`|
|`Starting`|
|`Absent`|
### UUID

The universal unique identifier for this system.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### POST Action "ComputerSystem.Reset"

Parameters:

"**ResetType**" (string) with one of the following value(s):

* On
* ForceOff
* ForceRestart
* Nmi
* PushPowerButton

> example "ComputerSystem.Reset" action:

```
POST <target-uri>
Content-Type: application/json
OData-Version: 4.0

{
    "ResetType": "On"
}
```

## Drive
```@odata.type: "#Drive.v1_0_0.Drive"```

> **Resource Instances of this Type**:  

> * `https://{iLO}/redfish/v1/chassis/{item}/drives/{item}/`

### BlockSizeBytes

The size of the smallest addressible unit (Block) of this drive in bytes


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|Yes (if resource allows PATCH)
### CapableSpeedGbs

The speed which this drive can communicate to a storage controller in ideal conditions in Gigabits per second


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|Yes (if resource allows PATCH)
### CapacityBytes

The size in bytes of this Drive


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|Yes (if resource allows PATCH)
### FailurePredicted

Is this drive currently predicting a failure in the near future


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
### Location[array-item].Info

This indicates the location of the resource.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
### Location[array-item].InfoFormat

This represents the format of the Info property.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`Location[]/InfoFormat` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Box:Bay`|
|`BayNumber`|
### Manufacturer

This is the manufacturer of this drive.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
### MediaType

The type of media contained in this drive.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`MediaType` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`HDD`|
|`SSD`|
### Model

This is the model number for the drive.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
### NegotiatedSpeedGbs

The speed which this drive is currently communicating to the storage controller in Gigabits per second


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|Yes (if resource allows PATCH)
### Oem.Hpe.HealthUpdated

Describes how the health related data (FailurePredicted, PredictedMediaLifeLeftPercent, Status) is updated.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Oem/Hpe/HealthUpdated` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Boot`|
|`Dynamic`|
### Oem.Hpe.NVMeId

NVMe Identifier:  ModelName, SerialNumber, PCI-Vendor-ID.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### PartNumber

The part number for this drive.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
### PredictedMediaLifeLeftPercent

The percentage of reads and writes that are predicted to still be available for the media


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|Yes (if resource allows PATCH)
### Protocol

The protocol this drive is using to communicate to the storage controller


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`Protocol` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`NVMe`|
|`SATA`|
|`USB`|
### Revision

The revision of this Drive


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
### RotationSpeedRPM

The rotation speed of this Drive in Revolutions per Minute (RPM)


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|Yes (if resource allows PATCH)
### SerialNumber

Serial Number of the drive.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
### Status.Health

This represents the health state of this resource in the absence of its dependent resources.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Status/Health` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`OK`|
|`Warning`|
|`Critical`|
### Status.HealthRollup

This represents the overall health state from the view of this resource.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Status/HealthRollup` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`OK`|
|`Warning`|
|`Critical`|
### Status.State

This indicates the known state of the resource, such as if it is enabled.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Status/State` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`Enabled`|
|`Disabled`|
|`Offline`|
|`InTest`|
|`Starting`|
|`Absent`|
## EthernetInterface
```@odata.type: "#EthernetInterface.v1_0_3.EthernetInterface"```

The schema definition of a simple Ethernet NIC resource.

> **Resource Instances of this Type**:  

> * `https://{iLO}/redfish/v1/managers/{item}/ethernetinterfaces/{item}/`

### AutoNeg

This indicates if the speed and duplex is automatically configured by the NIC.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"AutoNeg": true}

### FQDN

The complete, fully qualified domain name obtained by DNS for this NIC.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### FrameSize

The MAC frame size (bytes).


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"FrameSize": &lt;integer-value&gt;}

### FullDuplex

The connection duplex status. If AutoNeg is enabled, this property cannot be modified. AutoNeg is only applicable and modifiable for a dedicated network port and cannot be modified for blade servers.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"FullDuplex": true}

### HostName

The DNS Host Name, without any domain information.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### IPv4Addresses[array-item].Address

The IPv4 Address.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"IPv4Addresses": [{"Address": "&lt;string-value&gt;"}|null, ...]}

### IPv4Addresses[array-item].AddressOrigin

How the address was determined.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`IPv4Addresses[]/AddressOrigin` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`DHCP`|
|`Static`|
### IPv4Addresses[array-item].Gateway

The IPv4 gateway for this address.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"IPv4Addresses": [{"Gateway": "&lt;string-value&gt;"}|null, ...]}

### IPv4Addresses[array-item].SubnetMask

The IPv4 Subnet mask.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"IPv4Addresses": [{"SubnetMask": "&lt;string-value&gt;"}|null, ...]}

### IPv6AddressPolicyTable[array-item].Label

The label value for this table entry, as defined in RFC3484 section 2.1.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"IPv6AddressPolicyTable": [{"Label": &lt;integer-value&gt;}|null, ...]}

### IPv6AddressPolicyTable[array-item].Precedence

The precedence value for this table entry as defined in RFC3484 section 2.1.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"IPv6AddressPolicyTable": [{"Precedence": &lt;integer-value&gt;}|null, ...]}

### IPv6AddressPolicyTable[array-item].Prefix

The IPv6 Address Prefix for this table entry as defined in RFC3484 section 2.1.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"IPv6AddressPolicyTable": [{"Prefix": "&lt;string-value&gt;"}|null, ...]}

### IPv6Addresses[array-item].Address

The IPv6 Address.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### IPv6Addresses[array-item].AddressOrigin

How the address was determined.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`IPv6Addresses[]/AddressOrigin` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`DHCP`|
|`Static`|
|`SLAAC`|
### IPv6Addresses[array-item].AddressState

The current state of this address as defined in RFC 4862.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`IPv6Addresses[]/AddressState` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`Preferred`|
|`Deprecated`|
|`Tentative`|
|`Failed`|
### IPv6Addresses[array-item].PrefixLength

The IPv6 Address Prefix Length.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### IPv6DefaultGateway

The IPv6 default gateway address that is currently in use on this interface.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### IPv6StaticAddresses[array-item].Address

A valid IPv6 address.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"IPv6StaticAddresses": [{"Address": "&lt;string-value&gt;"}|null, ...]}

### IPv6StaticAddresses[array-item].PrefixLength

The Prefix Length of this IPv6 address.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"IPv6StaticAddresses": [{"PrefixLength": &lt;integer-value&gt;}|null, ...]}

### MACAddress

The effective current MAC address. If the assignable MAC address is not supported, this is a read-only alias of FactoryMacAddress.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"MACAddress": "&lt;string-value&gt;"}

### MaxIPv6StaticAddresses

The maximum number of IPv6 static addresses that can be configured on this interface.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Oem.Hpe.ConfigurationSettings

The state of the currently displayed configuration settings.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Oem/Hpe/ConfigurationSettings` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Current`|
|`SomePendingReset`|
### Oem.Hpe.DHCPv4.Enabled

Determines whether DHCPv4 is enabled.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Oem": {"Hpe": {"DHCPv4": {"Enabled": true}}}}

### Oem.Hpe.DHCPv4.UseDNSServers

Determines whether to use DHCPv4-supplied DNS servers. Can only be enabled when DHCPv4 is also enabled; otherwise, this property will be set to false and will be read-only.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Oem": {"Hpe": {"DHCPv4": {"UseDNSServers": true}}}}

### Oem.Hpe.DHCPv4.UseDomainName

Determines whether to use a DHCPv4-supplied domain name. Can only be enabled when DHCPv4 is also enabled; otherwis,e this property will be set to false and will be read-only.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Oem": {"Hpe": {"DHCPv4": {"UseDomainName": true}}}}

### Oem.Hpe.DHCPv4.UseGateway

Determines whether to use a DHCPv4-supplied gateway. Can only be enabled when DHCPv4 is also enabled; otherwise, this property will be set to false and will be read-only.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Oem": {"Hpe": {"DHCPv4": {"UseGateway": true}}}}

### Oem.Hpe.DHCPv4.UseNTPServers

Determines whether to use DHCPv4-supplied NTP servers. Can only be enabled when DHCPv4 is also enabled; otherwise, this property will be set to false and will be read-only.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Oem": {"Hpe": {"DHCPv4": {"UseNTPServers": true}}}}

### Oem.Hpe.DHCPv4.UseStaticRoutes

Determines whether to use DHCPv4-supplied static routes. Can only be enabled when DHCPv4 is also enabled; otherwise, this property will be set to false and will be read-only.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Oem": {"Hpe": {"DHCPv4": {"UseStaticRoutes": true}}}}

### Oem.Hpe.DHCPv4.UseWINSServers

Determines whether to use DHCPv4-supplied WINS servers. Can only be enabled when DHCPv4 is also enabled; otherwise, this property will be set to false and will be read-only.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Oem": {"Hpe": {"DHCPv4": {"UseWINSServers": true}}}}

### Oem.Hpe.DHCPv6.StatefulModeEnabled

Determines whether DHCPv6 Stateful mode is enabled.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Oem": {"Hpe": {"DHCPv6": {"StatefulModeEnabled": true}}}}

### Oem.Hpe.DHCPv6.StatelessModeEnabled

Determines whether DHCPv6 Stateless mode is enabled.  Always enabled by default whenever DHCPv6 Stateful mode is also enabled.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Oem": {"Hpe": {"DHCPv6": {"StatelessModeEnabled": true}}}}

### Oem.Hpe.DHCPv6.UseDNSServers

Determines whether to use DHCPv6-supplied DNS servers. Can only be enabled when DHCPv6 Stateless mode is also enabled; otherwise, this property will be set to false and will be read-only.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Oem": {"Hpe": {"DHCPv6": {"UseDNSServers": true}}}}

### Oem.Hpe.DHCPv6.UseDomainName

Determines whether to use a DHCPv6-supplied domain name. Can only be enabled when DHCPv6 Stateless mode is also enabled; otherwise, this property will be set to false and will be read-only.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Oem": {"Hpe": {"DHCPv6": {"UseDomainName": true}}}}

### Oem.Hpe.DHCPv6.UseNTPServers

Determines whether to use DHCPv6-supplied NTP servers. Can only be enabled when DHCPv6 Stateless mode is also enabled; otherwise, this property will be set to false and will be read-only.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Oem": {"Hpe": {"DHCPv6": {"UseNTPServers": true}}}}

### Oem.Hpe.DHCPv6.UseRapidCommit

Determines whether to use DHCPv6 rapid commit mode. Can only be enabled when DHCPv6 Stateful mode is also enabled; otherwise, this property will be set to false and will be read-only. Do not enable in networks where more than one DHCPv6 server is configured to provide address assignments.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Oem": {"Hpe": {"DHCPv6": {"UseRapidCommit": true}}}}

### Oem.Hpe.DomainName

Domain name of the network to which this management processor belongs. This property can only be modified when the management processor is not configured to use a DHCP supplied domain name; otherwise this property is read-only indicating the value is provided by DHCP.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Oem": {"Hpe": {"DomainName": "&lt;string-value&gt;"}}}

### Oem.Hpe.HostName

The management processor host name.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Oem": {"Hpe": {"HostName": "&lt;string-value&gt;"}}}

### Oem.Hpe.IPv4.DDNSRegistration

Determines whether DDNS registration is enabled.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Oem": {"Hpe": {"IPv4": {"DDNSRegistration": true}}}}

### Oem.Hpe.IPv4.StaticRoutes[array-item].Destination

An IPv4 static route destination. Only writeable when use of DHCPv4-supplied static routes is disabled; otherwise this property is read-only indicating the value is provided by DHCPv4.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Oem": {"Hpe": {"IPv4": {"StaticRoutes": [{"Destination": "&lt;string-value&gt;"}|null, ...]}}}}

### Oem.Hpe.IPv4.StaticRoutes[array-item].Gateway

An IPv4 static route gateway. Only writeable when use of DHCPv4-supplied static routes is disabled; otherwise this property is read-only indicating the value is provided by DHCPv4.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Oem": {"Hpe": {"IPv4": {"StaticRoutes": [{"Gateway": "&lt;string-value&gt;"}|null, ...]}}}}

### Oem.Hpe.IPv4.StaticRoutes[array-item].SubnetMask

An IPv4 static route subnet mask. Only writeable when use of DHCPv4-supplied static routes is disabled; otherwise this property is read-only indicating the value is provided by DHCPv4.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Oem": {"Hpe": {"IPv4": {"StaticRoutes": [{"SubnetMask": "&lt;string-value&gt;"}|null, ...]}}}}

### Oem.Hpe.IPv4.WINSRegistration

Determines whether WINS registration is enabled.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Oem": {"Hpe": {"IPv4": {"WINSRegistration": true}}}}

### Oem.Hpe.IPv6.DDNSRegistration

Determines whether IPv6 DDNS registration is enabled.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Oem": {"Hpe": {"IPv6": {"DDNSRegistration": true}}}}

### Oem.Hpe.IPv6.SLAACEnabled

Determines whether StateLess Address Auto-Configuration is enabled.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Oem": {"Hpe": {"IPv6": {"SLAACEnabled": true}}}}

### Oem.Hpe.IPv6.StaticDefaultGateway

The IPv6 static default gateway entry.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Oem": {"Hpe": {"IPv6": {"StaticDefaultGateway": "&lt;string-value&gt;"}}}}

### Oem.Hpe.IPv6.StaticRoutes[array-item].Destination

The IPv6 static route destination address.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Oem": {"Hpe": {"IPv6": {"StaticRoutes": [{"Destination": "&lt;string-value&gt;"}|null, ...]}}}}

### Oem.Hpe.IPv6.StaticRoutes[array-item].Gateway

The IPv6 static route gateway.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Oem": {"Hpe": {"IPv6": {"StaticRoutes": [{"Gateway": "&lt;string-value&gt;"}|null, ...]}}}}

### Oem.Hpe.IPv6.StaticRoutes[array-item].PrefixLength

The prefix length of the IPv6 static route destination address.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Oem": {"Hpe": {"IPv6": {"StaticRoutes": [{"PrefixLength": &lt;integer-value&gt;}|null, ...]}}}}

### Oem.Hpe.IPv6.StaticRoutes[array-item].Status

Status of this static route entry.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Oem/Hpe/IPv6/StaticRoutes[]/Status` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Unknown`|
|`Pending`|
|`Active`|
|`Failed`|
### Oem.Hpe.InterfaceType

Describes the network interface type.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Oem/Hpe/InterfaceType` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Dedicated`|
|`Shared`|
### Oem.Hpe.NICEnabled

Determines whether this NIC is enabled or disabled. Enabling one NIC will disable the others. If no NIC is enabled, this management processor is not accessible over the network.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Oem": {"Hpe": {"NICEnabled": true}}}

### Oem.Hpe.NICSupportsIPv6

Indicates whether or not this NIC can support the IPv6 protocol.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### Oem.Hpe.PingGatewayOnStartup

Determines whether to ping the IPv4 gateway on startup.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Oem": {"Hpe": {"PingGatewayOnStartup": true}}}

### Oem.Hpe.SharedNetworkPortOptions.NIC

Selects the system NIC that is to be shared with this management processor.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Oem": {"Hpe": {"SharedNetworkPortOptions": {"NIC": "FlexibleLOM"}}}}

`Oem/Hpe/SharedNetworkPortOptions/NIC` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`LOM`|
|`FlexibleLOM`|
### Oem.Hpe.SharedNetworkPortOptions.Port

The network adapter port number that is used for sharing. This feature is only applicable on systems and network adapters that support it.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Oem": {"Hpe": {"SharedNetworkPortOptions": {"Port": &lt;integer-value&gt;}}}}

### Oem.Hpe.SupportsFlexibleLOM

Indicates whether this system supports FlexibleLOM. Only applies to Shared Network Port.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### Oem.Hpe.SupportsLOM

Indicates whether this system supports LOM. Only applies to Shared Network Port.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### PermanentMACAddress

This is the MAC address assigned to this NIC at the factory.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### SettingsResult.ETag

The ETag of the resource to which the settings were applied, after the application.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### SettingsResult.Operation

Last operation detail.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`SettingsResult/Operation` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`SettingsApply`|
### SettingsResult.Time

Indicates the time the settings were applied.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### SpeedMbps

The link speed of the Ethernet interface in megabits per second. If AutoNeg is enabled, this property cannot be modified. This property can only be modified on a dedicated network port. It cannot be modified for blade servers.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"SpeedMbps": &lt;integer-value&gt;}

### Status.Health

This represents the health state of this resource in the absence of its dependent resources.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Status/Health` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`OK`|
|`Warning`|
|`Critical`|
### Status.HealthRollup

This represents the overall health state from the view of this resource.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Status/HealthRollup` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`OK`|
|`Warning`|
|`Critical`|
### Status.State

This indicates the known state of the resource, such as if it is enabled.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Status/State` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`Enabled`|
|`Disabled`|
|`Offline`|
|`InTest`|
|`Starting`|
|`Absent`|
### UefiDevicePath

The UEFI device path for this NIC.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### VLAN.VLANEnable

This indicates if this VLAN is enabled.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"VLAN": {"VLANEnable": true}}

### VLAN.VLANId

This indicates the VLAN identifier for this VLAN.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"VLAN": {"VLANId": &lt;integer-value&gt;}}

### VLANs

This is a reference to a collection of VLANs and is only used if the interface supports more than one VLANs.


| | |
|---|---|
|JSON type|null|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"VLANs": "&lt;string-value&gt;"}

## EventService
```@odata.type: "#EventService.v1_0_1.EventService"```

This is the schema definition for the Event Service.  It represents the properties for the service itself and has links to the actual list of subscriptions.

> **Resource Instances of this Type**:  

> * `https://{iLO}/redfish/v1/eventservice/`

### DeliveryRetryAttempts

This is the number of attempts an event posting is retried before the subscription is terminated.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### DeliveryRetryIntervalSeconds

This represents the number of seconds between retry attempts for sending any given Event


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Oem.Hpe.RequestedMaxEventsToQueueDefault

This represents the default number of events the service should queue.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Oem.Hpe.RetireOldEventInMinutesDefault

This represents the default number of minutes until an event is expired.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Oem.Hpe.TTLCountDefault

The default number of TTLUnits until this listener destination subscription expires.  It may be renewed prior to expire to reset the Time to Live counter.  The value 999999 is reserved to mean a perpetual subscription.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Oem.Hpe.TTLUnitsDefault

The default time unit used to measure the subscription time of this listener destination.  This is the units for TTLCount and is used to express the subscription lifetime of the listener destination.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Oem/Hpe/TTLUnitsDefault` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`seconds`|
|`minutes`|
|`days`|
### Status.Health

This represents the health state of this resource in the absence of its dependent resources.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Status/Health` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`OK`|
|`Warning`|
|`Critical`|
### Status.HealthRollup

This represents the overall health state from the view of this resource.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Status/HealthRollup` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`OK`|
|`Warning`|
|`Critical`|
### Status.State

This indicates the known state of the resource, such as if it is enabled.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Status/State` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`Enabled`|
|`Disabled`|
|`Offline`|
|`InTest`|
|`Starting`|
|`Absent`|
### POST Action "EventService.SubmitTestEvent"

Parameters:

"**EventID**" (string) with the value **"<string>"**

"**EventTimestamp**" (string) with the value **"<date-time>"**

"**EventType**" (string) with one of the following value(s):

* StatusChange
* ResourceUpdated
* ResourceAdded
* ResourceRemoved
* Alert

"**Message**" (string) with the value **"<string>"**

"**MessageArgs**" (string)

"**MessageID**" (string) with the value **"<string>"**

"**OriginOfCondition**" (string) with the value **"<string>"**

"**Severity**" (string) with one of the following value(s):

* OK
* Warning
* Critical

> example "EventService.SubmitTestEvent" action:

```
POST <target-uri>
Content-Type: application/json
OData-Version: 4.0

{
    "EventID": "<string>", 
    "EventTimestamp": "<date-time>", 
    "EventType": "StatusChange", 
    "Message": "<string>", 
    "MessageArgs": "<string>", 
    "MessageID": "<string>", 
    "OriginOfCondition": "<string>", 
    "Severity": "OK"
}
```

## HpeBaseConfigs
```@odata.type: "#HpeBaseConfigs.v2_0_0.HpeBaseConfigs"```

> **Resource Instances of this Type**:  

> * `https://{iLO}/redfish/v1/systems/{item}/bios/tlsconfig/baseconfigs/`

> * `https://{iLO}/redfish/v1/systems/{item}/bios/iscsi/baseconfigs/`

> * `https://{iLO}/redfish/v1/systems/{item}/bios/baseconfigs/`

> * `https://{iLO}/redfish/v1/systems/{item}/bios/boot/baseconfigs/`

### Capabilities.BaseConfig


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### Capabilities.BaseConfigs


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
## HpeBaseNetworkAdapter
```@odata.type: "#HpeBaseNetworkAdapter.v2_0_0.HpeBaseNetworkAdapter"```

> **Resource Instances of this Type**:  

> * `https://{iLO}/redfish/v1/systems/{item}/networkadapters/{item}/`

### FcPorts[array-item].PortNumber

Port Number.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### FcPorts[array-item].WWNN

World Wide Node Name.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### FcPorts[array-item].WWPN

World Wide Port Name.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Firmware.Current.VersionString

This string represents the version of the firmware image.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### PartNumber

The device part number.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### PhysicalPorts[array-item].FullDuplex

Full-duplex data transmission means that data can be transmitted in both directions on a signal carrier at the same time.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### PhysicalPorts[array-item].IPv4Addresses[array-item].Address

This is the IPv4 Address.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### PhysicalPorts[array-item].IPv6Addresses[array-item].Address

This is the IPv6 Address.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### PhysicalPorts[array-item].MacAddress

The port MAC address.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### PhysicalPorts[array-item].Oem.Hpe.BadReceives

A count of frames that were received by the adapter but which had an error.  This counter is the sum of mib items cpqNicIfPhysAdapterAlignmentErrors, cpqNicIfPhysAdapterFCSErrors, cpqNicIfPhysAdapterFrameTooLongs, and cpqNicIfPhysAdapterInternalMacReceiveErrors. If this counter increments frequently, check the more detailed error statistics and take appropriate action.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### PhysicalPorts[array-item].Oem.Hpe.BadTransmits

A count of frames that were not transmitted by the adapter because of an error.  This counter is the sum of MIB items cpqNicIfPhysAdapterDeferredTransmissions, cpqNicIfPhysAdapterLateCollisions, cpqNicIfPhysAdapterExcessiveCollisions, cpqNicIfPhysAdapterCarrierSenseErrors, and cpqNicIfPhysAdapterInternalMacTransmitErrors. If this counter increments frequently, check the more detailed error statistics and take appropriate action.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### PhysicalPorts[array-item].Oem.Hpe.GoodReceives

A count of frames successfully received by the physical adapter.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### PhysicalPorts[array-item].Oem.Hpe.GoodTransmits

A count of frames successfully transmitted by the physical adapter.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### PhysicalPorts[array-item].Oem.Hpe.StructuredName

PCI device structured name in UTF-8 format (e.g. 'NIC.LOM.1.1' - see PCIDevices in /rest/v1/Systems/x/PCIDevices - this comes from SMBIOS


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### PhysicalPorts[array-item].Oem.Hpe.Team

If a port is configured for NIC teaming, the name of the configured link between the physical ports that form a logical network adapter. This value is displayed for system NICs only (embedded and stand-up).


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### PhysicalPorts[array-item].SpeedMbps

An estimate of the interface's current bandwidth in Megabits per second.  For interfaces which do not vary in bandwidth or for those where no accurate estimation can be made, this object should contain the nominal bandwidth.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### PhysicalPorts[array-item].Status.Health

This represents the health state of this resource in the absence of its dependent resources.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`PhysicalPorts[]/Status/Health` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`OK`|
|`Warning`|
|`Critical`|
### PhysicalPorts[array-item].Status.HealthRollup

This represents the overall health state from the view of this resource.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`PhysicalPorts[]/Status/HealthRollup` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`OK`|
|`Warning`|
|`Critical`|
### PhysicalPorts[array-item].Status.State

This indicates the known state of the resource, such as if it is enabled.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`PhysicalPorts[]/Status/State` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`Enabled`|
|`Disabled`|
|`Offline`|
|`InTest`|
|`Starting`|
|`Absent`|
### PhysicalPorts[array-item].UEFIDevicePath

UEFIDevice Path for correlation purposes


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### SerialNumber

The device serial number.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Status.Health

This represents the health state of this resource in the absence of its dependent resources.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Status/Health` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`OK`|
|`Warning`|
|`Critical`|
### Status.HealthRollup

This represents the overall health state from the view of this resource.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Status/HealthRollup` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`OK`|
|`Warning`|
|`Critical`|
### Status.State

This indicates the known state of the resource, such as if it is enabled.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Status/State` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`Enabled`|
|`Disabled`|
|`Offline`|
|`InTest`|
|`Starting`|
|`Absent`|
### StructuredName

PCI device structured name in UTF-8 format (e.g. 'NIC.LOM.1.1' - see PCIDevices in /rest/v1/Systems/x/PCIDevices - this comes from SMBIOS


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### UEFIDevicePath

UEFIDevice Path for correlation purposes


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
## HpeBiosMapping
```@odata.type: "#HpeBiosMapping.v2_0_0.HpeBiosMapping"```

This is the schema definition for the BIOS Attributes Mappings resource.

> **Resource Instances of this Type**:  

> * `https://{iLO}/redfish/v1/systems/{item}/bios/mappings/`

### AttributeRegistry

The Resource ID of the Attribute Registry for the BIOS Attributes resource.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
### BiosPciSettingsMappings[array-item].CorrelatableID

Contains any CorrelatableIDs that represent this PCI device. The CorrelatableID values can be JSON Pointers or UEFI identifiers.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### BiosPciSettingsMappings[array-item].Instance

The instance number of the parent PCI device for this association set.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### BiosPciSettingsMappings[array-item].Subinstances[array-item].CorrelatableID

Contains any CorrelatableIDs that represent this PCI device. The CorrelatableID values can be JSON Pointers or UEFI identifiers.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### BiosPciSettingsMappings[array-item].Subinstances[array-item].Subinstance

The sub-instance number of the child PCI device for this association set.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
## HpeCertAuth
```@odata.type: "#HpeCertAuth.v1_0_0.HpeCertAuth"```

This is the schema definition for certificate based authentication configuration.

> **Resource Instances of this Type**:  

> * `https://{iLO}/redfish/v1/managers/{item}/securityservice/certificateauthentication/`

### CRLIssuer

Issuer of the installed CRL, if present.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### CRLSerial

Serial Number of the installed CRL, if present.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### CertificateLoginEnabled

Specifies whether Certificate login is enabled.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"CertificateLoginEnabled": true}

### LDAPCertificateNameMapping

The method used to map a certificate to its associated LDAP user account.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"LDAPCertificateNameMapping": "SANRFC822"}

`LDAPCertificateNameMapping` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`SubjectCN`|
|`SubjectDN`|
|`SANRFC822`|
|`SANUPN`|
### StrictCACModeEnabled

Whether or not Strict CAC Mode is enabled.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"StrictCACModeEnabled": true}

### POST Action "HpeCertAuth.DeleteCRL"

Parameters:

> example "HpeCertAuth.DeleteCRL" action:

```
POST <target-uri>
Content-Type: application/json
OData-Version: 4.0

{}
```

### POST Action "HpeCertAuth.ImportCACertificate"

Parameters:

"**Certificate**" (string) with the value **"<text>"**

> example "HpeCertAuth.ImportCACertificate" action:

```
POST <target-uri>
Content-Type: application/json
OData-Version: 4.0

{
    "Certificate": "<text>"
}
```

### POST Action "HpeCertAuth.ImportCRL"

Parameters:

"**ImportUri**" (string) with the value **"<text>"**

> example "HpeCertAuth.ImportCRL" action:

```
POST <target-uri>
Content-Type: application/json
OData-Version: 4.0

{
    "ImportUri": "<text>"
}
```

## HpeComponent
```@odata.type: "#HpeComponent.v1_0_0.HpeComponent"```

> **Resource Instances of this Type**:  

> * `https://{iLO}/redfish/v1/updateservice/componentrepository/{item}/`

### Activates

Indicates when a component becomes active after being updated.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Activates` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Immediately`|
|`AfterReboot`|
|`AfterDeviceReset`|
|`AfterHardPowerCycle`|
### ComponentType

HTTP-style content-type of binary


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### ComponentUri

URI of the component binary.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Configuration

string defining customized parameters for some components provided by client at upload time and given to the component at execution time (Type D only).


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Configuration": "&lt;string-value&gt;"}

### Created

ISO 8601 time string indicating when this component was added to the NAND.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Criticality.0

### Criticality.1


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`Criticality/1` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Optional`|
|`Recommended`|
|`Critical`|
### DeviceClass

Device type GUID from iLO secure flash header


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### ExecutionParameters

Client supplied execution parameters.  These are supplied at upload time and given to the component at execution time (Type D only).


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"ExecutionParameters": "&lt;string-value&gt;"}

### Filename

The unique filename of the component.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Filepath

Path of file on the USB LUN if you mount the repo as USB.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Locked

If true, this component cannot be removed with DELETE because it is referenced by an Install Set


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### SizeBytes

Size of the component file in bytes.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Version

Version of the component from secure flash header or sidecar file.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
## HpeComponentInstallSet
```@odata.type: "#HpeComponentInstallSet.v1_0_0.HpeComponentInstallSet"```

> **Resource Instances of this Type**:  

> * `https://{iLO}/redfish/v1/updateservice/installsets/{item}/`

### Created

ISO-time of install set creation.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### IsRecovery

If true, this install set is reserved to hold only critical firmware recovery updatable by iLO.  Additionally the 'Administrate Recovery Set' iLO privilege is required to modify or remove this install set.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"IsRecovery": true}

### Sequence[array-item].Command

Command to execute.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Sequence": [{"Command": "ResetBmc"}|null, ...]}

`Sequence[]/Command` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`ApplyUpdate`|
|`ResetServer`|
|`ResetBmc`|
|`Wait`|
### Sequence[array-item].Component


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Sequence[array-item].Filename

The unique filename of the component.  This correlates to 'Filename' in the HpeComponent.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Sequence": [{"Filename": "&lt;string-value&gt;"}|null, ...]}

### Sequence[array-item].WaitTimeSeconds

The number of seconds to pause if the command is 'Wait'.  Ignored otherwise.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Sequence": [{"WaitTimeSeconds": &lt;integer-value&gt;}|null, ...]}

### POST Action "HpeComponentInstallSet.Invoke"

Parameters:

"**ClearTaskQueue**" (string) with one of the following value(s):

* true
* false

"**Expire**" (string)

"**StartAfter**" (string)

"**TPMOverride**" (string) with one of the following value(s):

* true
* false

> example "HpeComponentInstallSet.Invoke" action:

```
POST <target-uri>
Content-Type: application/json
OData-Version: 4.0

{
    "ClearTaskQueue": "true", 
    "Expire": "<string>", 
    "StartAfter": "<string>", 
    "TPMOverride": "true"
}
```

## HpeComponentUpdateTask
```@odata.type: "#HpeComponentUpdateTask.v1_0_0.HpeComponentUpdateTask"```

> **Resource Instances of this Type**:  

> * `https://{iLO}/redfish/v1/updateservice/updatetaskqueue/{item}/`

### Command

Command to execute.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Command": "ResetBmc"}

`Command` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`ApplyUpdate`|
|`ResetServer`|
|`ResetBmc`|
|`Wait`|
### Component


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Created

ISO-time of task creation (by whomever created this thing)


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Expire

ISO 8601 Redfish-style time string after which we will automatically change state to Expired - null for no expire time


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Expire": "&lt;string-value&gt;"}

### Filename

The unique filename of the component.  This correlates to 'Filename' in the HpeComponent.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Filename": "&lt;string-value&gt;"}

### Result.MessageId

The key for this message that can be used to look up the message in a message registry.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Result": {"MessageId": "&lt;string-value&gt;"}}

### ResultLog

base64 encoded entry to capture component log.  Estimated to be generally 1-2KB. written by updater


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"ResultLog": "&lt;string-value&gt;"}

### StartAfter

ISO 8601 Redfish-style time string of earliest execution - null for no start time specified


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"StartAfter": "&lt;string-value&gt;"}

### State

The current state of the update task.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"State": "Expired"}

`State` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Pending`|
|`InProgress`|
|`Complete`|
|`Expired`|
|`Exception`|
|`Canceled`|
### TPMOverride

If true then the TPMOverrideFlag is passed in on the associated flash operations.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"TPMOverride": true}

### WaitTimeSeconds

The number of seconds to pause if the command is 'Wait'.  Ignored otherwise.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"WaitTimeSeconds": &lt;integer-value&gt;}

## HpeESKM
```@odata.type: "#HpeESKM.v2_0_0.HpeESKM"```

ESKM (Enterprise Security Key Manager) object enables user to connect to an operational key manager, change redundancy settings, view the key manager connection settings, test the connection, and view key management events.

> **Resource Instances of this Type**:  

> * `https://{iLO}/redfish/v1/managers/{item}/securityservice/eskm/`

### ESKMEvents[array-item].Event

ESKM event description.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### ESKMEvents[array-item].Timestamp

Time of ESKM event.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### KeyManagerConfig.AccountGroup

Account group on ESKM.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"KeyManagerConfig": {"AccountGroup": "&lt;string-value&gt;"}}

### KeyManagerConfig.AccountName

Account name on ESKM.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### KeyManagerConfig.ESKMLocalCACertificateName

This is the name of Local CA (Certificate Authority) in ESKM that is used to sign the ESKM server certificate. iLO will retrieve this certificate from the ESKM server.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"KeyManagerConfig": {"ESKMLocalCACertificateName": "&lt;string-value&gt;"}}

### KeyManagerConfig.ImportedCertificateIssuer

Imported certificate issuer.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### KeyManagerConfig.ImportedCertificateSubject

Imported certificate subject.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### KeyManagerConfig.LoginName

ESKM administrator account login name. This property always returns null on GET.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"KeyManagerConfig": {"LoginName": "&lt;string-value&gt;"}}

### KeyManagerConfig.Password

ESKM administrator account password. This property always returns null on GET.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"KeyManagerConfig": {"Password": "&lt;string-value&gt;"}}

### KeyServerRedundancyReq

If true encryption keys will be maintained on both the configured key servers. When this option is disabled, iLO will not verify that encryption keys are copied to both of the configured key servers.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"KeyServerRedundancyReq": true}

### PrimaryKeyServerAddress

Primary key server IP address or FQDN. Set to null to clear the value.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"PrimaryKeyServerAddress": "&lt;string-value&gt;"}

### PrimaryKeyServerPort

Primary key server port number. Set to null to clear the value.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"PrimaryKeyServerPort": &lt;integer-value&gt;}

### SecondaryKeyServerAddress

Secondary key server IP address or FQDN. Set to null to clear the value.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"SecondaryKeyServerAddress": "&lt;string-value&gt;"}

### SecondaryKeyServerPort

Secondary key server port number. Set to null to clear the value.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"SecondaryKeyServerPort": &lt;integer-value&gt;}

### POST Action "HpeESKM.ClearESKMLog"

Parameters:

> example "HpeESKM.ClearESKMLog" action:

```
POST <target-uri>
Content-Type: application/json
OData-Version: 4.0

{}
```

### POST Action "HpeESKM.TestESKMConnections"

Parameters:

> example "HpeESKM.TestESKMConnections" action:

```
POST <target-uri>
Content-Type: application/json
OData-Version: 4.0

{}
```

## HpeHttpsCert
```@odata.type: "#HpeHttpsCert.v2_0_0.HpeHttpsCert"```

This is the schema definition for the X509 Certificate.

> **Resource Instances of this Type**:  

> * `https://{iLO}/redfish/v1/managers/{item}/securityservice/httpscert/`

### CertificateSigningRequest

GenerateCSR action, wait few minutes (upto 10), perform GET operation, fills CSR. Contains a public and private key pair.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### X509CertificateInformation.Issuer

The Certificate Authority that issued the certificate.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### X509CertificateInformation.SerialNumber

The serial number that the Certificate Authority assigned to the certificate.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### X509CertificateInformation.Subject

The entity to which the certificate was issued.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### X509CertificateInformation.ValidNotAfter

The date on which the certificate validity period ends.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### X509CertificateInformation.ValidNotBefore

The date on which the certificate validity period begins.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### POST Action "HpeHttpsCert.GenerateCSR"

Parameters:

"**City**" (string) with the value **"<string>"**

"**CommonName**" (string) with the value **"<string>"**

"**Country**" (string) with the value **"<string>"**

"**OrgName**" (string) with the value **"<string>"**

"**OrgUnit**" (string) with the value **"<string>"**

"**State**" (string) with the value **"<string>"**

"**IncludeIP**" (string) with one of the following value(s):

* true
* false

> example "HpeHttpsCert.GenerateCSR" action:

```
POST <target-uri>
Content-Type: application/json
OData-Version: 4.0

{
    "City": "<string>", 
    "CommonName": "<string>", 
    "Country": "<string>", 
    "OrgName": "<string>", 
    "OrgUnit": "<string>", 
    "State": "<string>", 
    "IncludeIP": "true"
}
```

### POST Action "HpeHttpsCert.ImportCertificate"

Parameters:

"**Certificate**" (string) with the value **"<text>"**

> example "HpeHttpsCert.ImportCertificate" action:

```
POST <target-uri>
Content-Type: application/json
OData-Version: 4.0

{
    "Certificate": "<text>"
}
```

## HpePowerMeter
```@odata.type: "#HpePowerMeter.v2_0_0.HpePowerMeter"```

> **Resource Instances of this Type**:  

> * `https://{iLO}/redfish/v1/chassis/{item}/power/fastpowermeter/`

> * `https://{iLO}/redfish/v1/chassis/{item}/power/powermeter/`

### Average

Average power across all samples, over the last 24 hours.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Maximum

Maximum power across all samples, taken from the 24 hour history.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Minimum

Minimum power across all samples, taken from the 24 hour history.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### PowerDetail[array-item].AmbTemp

Ambient temperature, in degrees Celsius.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### PowerDetail[array-item].Average

Average power over the sample time.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### PowerDetail[array-item].Cap

Overall power cap for the power meter.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### PowerDetail[array-item].CpuAvgFreq

CPU average frequency of the power supply.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### PowerDetail[array-item].CpuCapLim

CPU cap limit for the power meter.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### PowerDetail[array-item].CpuMax

CPU maximum power consumed by the power meter.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### PowerDetail[array-item].CpuPwrSavLim

CPU power-saving limit for the power meter.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### PowerDetail[array-item].CpuUtil

CPU power utilization.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### PowerDetail[array-item].Minimum

Minimum power over the sample time.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### PowerDetail[array-item].Peak

Peak power over the sample time.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### PowerDetail[array-item].PrMode

Power regulator mode, which can be OS Control, Static High, Static Low or Dynamic.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`PowerDetail[]/PrMode` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`dyn`|
|`min`|
|`max`|
|`osc`|
### PowerDetail[array-item].PunCap

Punitive cap for the power meter.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### PowerDetail[array-item].Time

Time at which the power detail was captured.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### PowerDetail[array-item].UnachCap

Unachievable cap for the power meter.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### Samples

Number of samples in the array.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
## HpeSecurityService
```@odata.type: "#HpeSecurityService.v2_0_0.HpeSecurityService"```

> **Resource Instances of this Type**:  

> * `https://{iLO}/redfish/v1/managers/{item}/securityservice/`

### SecurityState

The operational security level of this Manager.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"SecurityState": "HighSecurity"}

`SecurityState` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Wipe`|
|`Production`|
|`HighSecurity`|
|`FIPS`|
|`SuiteB`|
## HpeServerBootSettings
```@odata.type: "#HpeServerBootSettings.v2_0_0.HpeServerBootSettings"```

The schema definition of the server UEFI Boot Order resource.

> **Resource Instances of this Type**:  

> * `https://{iLO}/redfish/v1/systems/{item}/bios/boot/settings/`

> * `https://{iLO}/redfish/v1/systems/{item}/bios/boot/`

### BootSources[array-item].BootString

User-readable string that describes the UEFI boot option.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
### BootSources[array-item].CorrelatableID

Contains any CorrelatableIDs that represent this boot option. The correlatableID values can be JSON Pointers or UEFI identifiers.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
### BootSources[array-item].StructuredBootString

Uniquely identifies this boot option within the server.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
### BootSources[array-item].UEFIDevicePath

Standardized text representation of the UEFI device path for this boot option, in UTF-8 format.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
### DesiredBootDevices[array-item].CorrelatableID

Standardized text representation of the UEFI device path of the desired boot device, in UTF-8 format. For example 'PciRoot(0x0)/Pci(0x2,0x2)/Pci(0x0,0x0)'


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"DesiredBootDevices": [{"CorrelatableID": "&lt;string-value&gt;"}|null, ...]}

### DesiredBootDevices[array-item].Lun

The Logical Unit Number (LUN) of the desired boot device. This value must be a hexadecimal string with an even number of 2 to 16 characters, excluding the first two characters, 0x (for example, '0x01').


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"DesiredBootDevices": [{"Lun": "&lt;string-value&gt;"}|null, ...]}

### DesiredBootDevices[array-item].Wwn

The Fibre Channel World Wide Name (WWN) of the desired boot device. This value must be a hexadecimal string with an even number of 2 to 16 characters, excluding the first two characters, 0x (for example, '0x0001020304050607').


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"DesiredBootDevices": [{"Wwn": "&lt;string-value&gt;"}|null, ...]}

### DesiredBootDevices[array-item].iScsiTargetName

The iSCSI node target name of the desired boot device. The value must be a string based on IETF RFC 3270, and can be up to 223 characters in length (for example, 'iqn.1991-05.com.microsoft:iscsitarget-iscsidisk-target').


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"DesiredBootDevices": [{"iScsiTargetName": "&lt;string-value&gt;"}|null, ...]}

## HpeServerPCISlot
```@odata.type: "#HpeServerPCISlot.v2_0_0.HpeServerPCISlot"```

> **Resource Instances of this Type**:  

> * `https://{iLO}/redfish/v1/systems/{item}/pcislots/{item}/`

### Length

PCI slot length


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Length` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Short`|
|`Long`|
|`Other`|
### LinkLanes

Bandwidth capacity of the slot, measured by the number of PCI Express Lanes present. Also known as the slot width.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`LinkLanes` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`8 bit`|
|`16 bit`|
|`32 bit`|
|`64 bit`|
|`128 bit`|
|`x1`|
|`x2`|
|`x4`|
|`x8`|
|`x16`|
|`x32`|
|`Other`|
### Status.EnabledState

Specifies whether the slot is enabled or disabled.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Status.OperationalStatus[array-item].Status

Current usage status of the slot: InUse or Empty


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### SupportsHotPlug

Specifies whether the slot supports hot-plug devices.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### Technology

PCI technology


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Technology` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`PCIExpressGen3`|
|`PCIExpressGen2`|
|`PCIExpress`|
### UEFIDevicePath

Standardized text representation of the UEFI device path, in UTF-8 format


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
## HpeServerPciDevice
```@odata.type: "#HpeServerPciDevice.v2_0_0.HpeServerPciDevice"```

> **Resource Instances of this Type**:  

> * `https://{iLO}/redfish/v1/systems/{item}/pcidevices/{item}/`

### BayNumber

Bay number value.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### BusNumber

PCI device bus number value.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### ClassCode

PCI class code of the endpoint.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### DeviceID

PCI device ID of the device.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### DeviceInstance

PCI device instance value.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### DeviceLocation

PCI device location.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### DeviceNumber

PCI device number value.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### DeviceSubInstance

PCI device sub-instance value.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### DeviceType

Device type value.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`DeviceType` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Flexible LOM`|
|`Embedded LOM`|
|`NIC`|
|`HDD Not attached to a SA Controller`|
|`HDD Attached to a SA Controller`|
|`Other PCI Device`|
|`Unknown`|
|`Other`|
|`Video`|
|`SCSI Controller`|
|`Ethernet`|
|`Token Ring`|
|`Sound`|
|`PATA Controller`|
|`SATA Controller`|
|`SAS Controller`|
|`Storage Controller`|
|`Storage Array Controller`|
|`USB Hard Disk Drive`|
|`Firmware Volume`|
|`UEFI Shell`|
|`Generic UEFI USB Boot Entry`|
|`Dynamic Storage Array Controller`|
|`File`|
|`NVMe Hard Drive`|
|`NVDIMM`|
### EnclosureNumber

Enclosure number value.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### FunctionNumber

PCI device function number value.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### LocationString

Text representation of the UEFI device location, in UTF-8 format


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### SegmentNumber

PCI segment group number value.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### StructuredName

PCI device structured name in UTF-8 format.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### SubclassCode

PCI sub class code of the endpoint.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### SubsystemDeviceID

PCI subsystem device ID of the device.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### SubsystemVendorID

PCI subsystem vendor ID of the device.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### UEFIDevicePath

Standardized text representation of the UEFI device path, in UTF-8 format.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### VendorID

PCI vendor ID of the device.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
## HpeSmartStorage
```@odata.type: "#HpeSmartStorage.v2_0_0.HpeSmartStorage"```

HpSmartStorage

> **Resource Instances of this Type**:  

> * `https://{iLO}/redfish/v1/systems/{item}/smartstorage/`

### Status.Health

This represents the health state of this resource in the absence of its dependent resources.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Status/Health` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`OK`|
|`Warning`|
|`Critical`|
### Status.HealthRollup

This represents the overall health state from the view of this resource.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Status/HealthRollup` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`OK`|
|`Warning`|
|`Critical`|
### Status.State

This indicates the known state of the resource, such as if it is enabled.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Status/State` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`Enabled`|
|`Disabled`|
|`Offline`|
|`InTest`|
|`Starting`|
|`Absent`|
## HpeSmartStorageArrayController
```@odata.type: "#HpeSmartStorageArrayController.v2_0_0.HpeSmartStorageArrayController"```

HpSmartStorageArrayController

> **Resource Instances of this Type**:  

> * `https://{iLO}/redfish/v1/systems/{item}/smartstorage/arraycontrollers/{item}/`

### AdapterType

Type of Smart controller


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`AdapterType` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`SmartArray`|
|`SmartHBA`|
|`DynamicSmartArray`|
### ArrayCount

The number of arrays configured on this controller.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### BackupPowerSourceStatus

The current status of the backup power source (battery, capacitor, megacell etc.)


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`BackupPowerSourceStatus` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Present`|
|`NotPresent`|
|`PresentAndCharged`|
|`PresentAndCharging`|
### BootVolumePrimary

The primary boot volume of this controller


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### BootVolumeSecondary

The secondary boot volume of this controller


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### CacheArrayCount

The number of cache arrays configured on this controller


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### CacheLogicalDriveCount

The number of cache logical drives configured on this controller


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### CacheMemorySizeMiB

The total cache memory size for the controller in MiB


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### CachePhysicalDriveCount

The number of physical drives assigned as cache drives attached to this controller


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### ControllerPartNumber

Smart Array Controller Part Number


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### CurrentOperatingMode

The current operating mode of the controller.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`CurrentOperatingMode` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`RAID`|
|`HBA`|
|`Mixed`|
### CurrentParallelSurfaceScanCount

Number of disks the controller is scanning in parallel


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### DataLogicalDriveCount

The number of data logical drives configured on this controller


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### DataPhysicalDriveCount

The number of physical drives assigned as data drives attached to this controller


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### DegradedPerformanceOptimization

Enables the controller to attempt to improve performance on RAID 5/50/6(ADG)/60 logical drives when one or more physical drives in the logical drive are failed


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`DegradedPerformanceOptimization` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|
|`Disabled`|
### DriveWriteCache

Enables or disables the write cache of the physical drives attached to the controller


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`DriveWriteCache` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|
|`Disabled`|
### ElevatorSort

Enables the controller to sort requests to a physical drive


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`ElevatorSort` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|
|`Disabled`|
### EncryptionBootPasswordSet

True if there is a boot password set, false otherwise


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### EncryptionCryptoOfficerPasswordSet

True if a password has been set for the Encryption Crypto Officer, false otherwise


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### EncryptionEnabled

True if encryption is currently enabled for this controller, false otherwise


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### EncryptionFwLocked

True if the controller firmware has been locked, preventing firmware updates, false otherwise


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### EncryptionHasLockedVolumes

True if the controller has one or more volumes that are locked, false otherwise


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### EncryptionHasLockedVolumesMissingBootPassword

True if there are locked drives due to a missing boot password, false otherwise


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### EncryptionHasSuspendedVolumes

True if the controller password has been temporarily suspended, false otherwise


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### EncryptionKekSet

True if the Master Key has been set, false otherwise


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### EncryptionLocalKeyCacheEnabled

True if the controller caches encryption keys locally when a remote key manager is being used, false otherwise


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### EncryptionMixedVolumesEnabled

True if the controller will allow plaintext and encrypted volumes to exist simultaneously, false otherwise


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### EncryptionPhysicalDriveCount

The number of encrypted physical drives attached to the controller


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### EncryptionRecoveryParamsSet

True if the encryption password recovery question and answer have been set, false otherwise


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### EncryptionStandaloneModeEnabled

True if the controller manages encryption keys locally, false if a remote key manager is being used


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### EncryptionUserPasswordSet

True if a password has been set for the Encryption User, false otherwise.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### ExpandPriority

The level of priority that transformations have over handling current operating system requests


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`ExpandPriority` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`High`|
|`Medium`|
|`Low`|
### ExternalPortCount

The number of external ports


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### FirmwareVersion.Current.VersionString

This string represents the version of the firmware image.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### FlexibleLatencySchedulerSetting

This allows the controller to process certain high-latency requests after a delay that may time out when elevator sorting


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`FlexibleLatencySchedulerSetting` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Default`|
|`Low250`|
|`Middle100`|
|`Middle50`|
|`Aggressive30`|
|`Aggressive10`|
### HardwareRevision

The hardware revision of the controller


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### InconsistencyRepairPolicy

Enables the controller to update data on RAID 6(ADG) and 60 volumes based on parity information when an inconsistency is discovered during surface scan


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`InconsistencyRepairPolicy` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|
|`Disabled`|
### InternalPortCount

The number of internal ports


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### IsBootController

True if this controller is the OS boot controller, false otherwise


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### Location

Location identifier


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### LocationFormat

Format for Location Identifier


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`LocationFormat` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`PCISlot`|
### LogicalDriveCount

The number of logical drives configured on this controller


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Manufacturer

The manufacturer of the controller


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### MaxParallelSurfaceScanCount

Maximum number of disks that the controller supports scanning in parallel


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Model

The model number for the controller


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### OperatingModeAfterReboot

The operating mode the controller will be functioning in (RAID versus HBA) after a reboot


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`OperatingModeAfterReboot` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`RAID`|
|`HBA`|
|`Mixed`|
### ParallelSurfaceScanSupported

True if the controller supports scanning multiple disk surfaces


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### PhysicalDriveCount

The number of physical drives attached to this controller


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### PowerModeAfterReboot

The power mode of the controller after a reboot


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`PowerModeAfterReboot` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Invalid`|
|`Low`|
|`LowAutomated`|
|`Performant`|
### PowerModeConfigured

The current power mode of the controller


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`PowerModeConfigured` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Invalid`|
|`Low`|
|`LowAutomated`|
|`Performant`|
### PowerModeWarningChangedDrive

True if the controller's drive configuration has changed while using configuration based power settings, false otherwise


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### PowerModeWarningChangedMode

True if the controller has a new power mode configured, false otherwise


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### PowerModeWarningReboot

True if a reboot is required to change the active power mode on the controller, false otherwise


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`PowerModeWarningReboot` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`NotRequired`|
|`RequiredNoReason`|
|`RequiredPowerSavings`|
|`RequiredPerformance`|
### PowerModeWarningTemperature

True if the controller has crossed a critical temperature threshold and performance has been reduced to prevent damage to the controller, false otherwise


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### PredictiveSpareRebuild

Enables or disables predictive spare rebuild mode


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`PredictiveSpareRebuild` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|
|`Disabled`|
### QueueDepth

This sets the maximum number of requests the controller will submit to a drive at any given time


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`QueueDepth` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`2`|
|`4`|
|`8`|
|`16`|
|`32`|
|`Automatic`|
### RebuildPriority

The level of priority that rebuilds have over handling current operating system requests


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`RebuildPriority` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`High`|
|`Medium`|
|`Low`|
|`RapidHigh`|
|`RapidMediumHigh`|
|`RapidMedium`|
|`RapidLow`|
### SerialNumber

The serial number for this controller


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### SoftwareRaidHbaFirmwareRev

The firmware version of the underlying HBA that is being used by the software RAID stack


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### SoftwareRaidHbaModeOptionRomRev

The option ROM firmware version used to bootstrap the software RAID stack


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### SparePhysicalDriveCount

he number of physical drives assigned as spare drives attached to this controller


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Status.Health

This represents the health state of this resource in the absence of its dependent resources.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Status/Health` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`OK`|
|`Warning`|
|`Critical`|
### Status.HealthRollup

This represents the overall health state from the view of this resource.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Status/HealthRollup` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`OK`|
|`Warning`|
|`Critical`|
### Status.State

This indicates the known state of the resource, such as if it is enabled.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Status/State` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`Enabled`|
|`Disabled`|
|`Offline`|
|`InTest`|
|`Starting`|
|`Absent`|
### SurfaceScanAnalysisPriority

Priority that the controller takes to find and correct disk surface errors


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`SurfaceScanAnalysisPriority` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Disabled`|
|`High`|
|`Medium`|
|`Low`|
|`Idle`|
### UnassignedPhysicalDriveCount

The number of unassigned physical drives attached to this controller


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
## HpeSmartStorageDiskDrive
```@odata.type: "#HpeSmartStorageDiskDrive.v2_0_0.HpeSmartStorageDiskDrive"```

HpSmartStorageDiskDrive

> **Resource Instances of this Type**:  

> * `https://{iLO}/redfish/v1/systems/{item}/smartstorage/arraycontrollers/{item}/diskdrives/{item}/`

### BlockSizeBytes

Block size of the drive in bytes. This is the block size presented by the drive to clients such as the array controller or operating system.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### CapacityGB

Total capacity of the drive in GB. This denotes the marketing capacity (base 10)


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### CapacityLogicalBlocks

Total number of logical blocks in the drive


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### CapacityMiB

Total capacity of the drive in MiB


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### CarrierApplicationVersion

Carrier PIC firmware version currently running


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### CarrierAuthenticationStatus

Authentication status of the drive carrier


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`CarrierAuthenticationStatus` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`OK`|
|`Fail`|
|`NoCommunication`|
|`NotApplicable`|
### CurrentTemperatureCelsius

The current temperature of the drive


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### DiskDriveUse

The current use of the physical drive.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`DiskDriveUse` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Data`|
|`Spare`|
|`Raw`|
|`Unconfigured`|
|`Unknown`|
### EncryptedDrive

True if encryption is currently enabled on this disk drive, false otherwise


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### EraseCompletionPercentage

The percent complete for an erase operation currently occurring on the disk drive or null if not currently erasing a drive.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### ErasePattern

The pattern used for erasing the disk drive


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### FirmwareVersion.Current.VersionString

This string represents the version of the firmware image.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### IndicatorLED

The state of the indicator LED.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`IndicatorLED` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`Unknown`|
|`Lit`|
|`Blinking`|
|`Off`|
### InterfaceSpeedMbps

Native interface speed for the device


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### InterfaceType

The connection interface of the drive. The value NVME has been deprecated.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`InterfaceType` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`SAS`|
|`SATA`|
|`NVME`|
|`PCIe`|
|`Unknown`|
### LegacyBootPriority

This indicates that the array controller should provide legacy boot support.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`LegacyBootPriority` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Primary`|
|`Secondary`|
|`None`|
### Location

The location of the drive


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### LocationFormat

Format for the location property


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`LocationFormat` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`ControllerPort:Box:Bay`|
|`SwitchPort:Box:Bay`|
|`SwitchPort:SwitchBay:Bay`|
### Manufacturer

Manufacturer of the disk drive


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### MaximumTemperatureCelsius

The maximum recommended temperature for the drive


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### MediaType

Type of disk


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`MediaType` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`HDD`|
|`SSD`|
|`SMR`|
### MinimumGoodFirmwareVersion

The minimum recommended firmware revision for the drive


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Model

Drive model number


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### NativeBlockSizeBytes

Native block size of the drive in bytes. This is the underlying sector size used by the physical drive to store data. For example, an advanced format drive that uses 4K sector sizes to store data will return 4K as the NativeBlockSizeBytes but may return 512 for the BlockSizeBytes when running in 512e (emulation) mode for backward compatibility


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### PhyCount

The number of phys the drive has


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### PortCount

The number of ports on the drive. Typically 1 (single-domain) or 2 (dual-domain)


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### PowerOnHours

The number of lifetime hours that the drive has been powered on. The value is null if the disk power on hours cannot be determined or is not supported.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### RotationalSpeedRpm

The rotational speed of the drive, only applicable on HDDs


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### SSDEnduranceUtilizationPercentage

This is the percentage of the drive that has been worn out and can no longer be used. When this values reaches 100%, the drive has 0% usage remaining and is completely worn out. The value is null if percent endurance used cannot be determined or is not supported.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### SerialNumber

The serial number of the drive


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### SpareRebuildMode

Method to used activate this drive when another drive fails, this is only applicable if the drive is configured as a spare drive


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`SpareRebuildMode` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Dedicated`|
|`Roaming`|
### Status.Health

This represents the health state of this resource in the absence of its dependent resources.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Status/Health` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`OK`|
|`Warning`|
|`Critical`|
### Status.HealthRollup

This represents the overall health state from the view of this resource.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Status/HealthRollup` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`OK`|
|`Warning`|
|`Critical`|
### Status.State

This indicates the known state of the resource, such as if it is enabled.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Status/State` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`Enabled`|
|`Disabled`|
|`Offline`|
|`InTest`|
|`Starting`|
|`Absent`|
### TransferSpeedMbps

Effective transfer speed to the device taking into account hardware acceleration such as edge-buffering


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### WWID

Unique identifier for the device


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
## HpeSmartStorageHostBusAdapter
```@odata.type: "#HpeSmartStorageHostBusAdapter.v2_0_0.HpeSmartStorageHostBusAdapter"```

HpSmartStorageHostBusAdapter

> **Resource Instances of this Type**:  

> * `https://{iLO}/redfish/v1/systems/{item}/smartstorage/hostbusadapters/{item}/`

### FirmwareVersion.Current.VersionString

This string represents the version of the firmware image.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### HardwareRevision

The hardware revision of the controller


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Location

Location identifier


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### LocationFormat

Format for Location Identifier


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`LocationFormat` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`PCISlot`|
### Manufacturer

The manufacturer of the controller


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Model

The model number for the controller


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### SerialNumber

The serial number for this controller


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Status.Health

This represents the health state of this resource in the absence of its dependent resources.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Status/Health` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`OK`|
|`Warning`|
|`Critical`|
### Status.HealthRollup

This represents the overall health state from the view of this resource.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Status/HealthRollup` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`OK`|
|`Warning`|
|`Critical`|
### Status.State

This indicates the known state of the resource, such as if it is enabled.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Status/State` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`Enabled`|
|`Disabled`|
|`Offline`|
|`InTest`|
|`Starting`|
|`Absent`|
## HpeSmartStorageLogicalDrive
```@odata.type: "#HpeSmartStorageLogicalDrive.v2_0_0.HpeSmartStorageLogicalDrive"```

HpSmartStorageLogicalDrive

> **Resource Instances of this Type**:  

> * `https://{iLO}/redfish/v1/systems/{item}/smartstorage/arraycontrollers/{item}/logicaldrives/{item}/`

### BlockSizeBytes

The block size of the disk drive in bytes


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### CapacityMiB

Total usable capacity available on this logical drive in MiB units


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### DriveAccessName

The access ID of the logical drive given by the OS


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### DriveGeometryCylinders

The number of cylinders on the drive


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### DriveGeometryHeads

The number of heads on the drive


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### DriveGeometrySectors

The number of sectors on the drive


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### InterfaceType

The connection interface of the logical drive.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`InterfaceType` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`SAS`|
|`SATA`|
|`Mixed`|
|`Unknown`|
### LegacyBootPriority


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`LegacyBootPriority` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Primary`|
|`Secondary`|
|`None`|
### LogicalDriveEncryption

True if encryption is currently enabled on this logical drive, false otherwise


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### LogicalDriveEncryptionDataKeysVolatile

True if volatile keys are enabled for encryption, false otherwise


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### LogicalDriveEncryptionDataKeysVolatileBackup

True if volatile keys are backed up to a remote key manager, false if volatile keys are not backed up


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### LogicalDriveEncryptionDataKeysVolatileStatus

The status of the encryption volatile keys


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`LogicalDriveEncryptionDataKeysVolatileStatus` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`NoOp`|
|`BackupInProgress`|
|`BackupAndSetInProgress`|
|`RestoreInProgress`|
|`DeleteInProgress`|
### LogicalDriveName

Label given to the logical drive


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### LogicalDriveNumber

logical drive number


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### LogicalDriveType

How the logical drive is being used


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`LogicalDriveType` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Data`|
|`Cache`|
|`SplitMirrorSetPrimary`|
|`SplitMirrorSetBackup`|
|`SplitMirrorSetBackupOrphan`|
### MediaType

Type of the disk this logical drive is associated with.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`MediaType` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`HDD`|
|`SSD`|
|`SMR`|
|`Mixed`|
|`Unknown`|
### ParityInitializationCompletionPercentage

Parity initialization complete percentage for a parity based logical drive (e.g. RAID 5)


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### ParityInitializationType

When creating a logical drive with a RAID level that requires parity, parity blocks can be initialized with two different methods


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`ParityInitializationType` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Default`|
|`Rapid`|
### PartitionInformation

OS partition information for the drive


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Raid

The current RAID level configured on the logical drive


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Raid` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`0`|
|`1`|
|`1ADM`|
|`10`|
|`10ADM`|
|`5`|
|`50`|
|`6`|
|`60`|
### RebuildCompletionPercentage

The percent complete for a rebuild operation currently occurring on the logical drive


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### SmartCacheState

The state of the SmartCache cache. This is valid if this drive either is a cache drive, or has a cache drive attached to it


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`SmartCacheState` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Good`|
|`Limited`|
|`DDRUnsafe`|
|`CacheLUNOffline`|
|`PrimaryLUNOffline`|
|`Destroyed`|
|`Flushing`|
|`Configuring`|
|`PairFailAtPowerup`|
|`Unknown`|
### Status.Health

This represents the health state of this resource in the absence of its dependent resources.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Status/Health` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`OK`|
|`Warning`|
|`Critical`|
### Status.HealthRollup

This represents the overall health state from the view of this resource.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Status/HealthRollup` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`OK`|
|`Warning`|
|`Critical`|
### Status.State

This indicates the known state of the resource, such as if it is enabled.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Status/State` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`Enabled`|
|`Disabled`|
|`Offline`|
|`InTest`|
|`Starting`|
|`Absent`|
### StripSizeBytes

The strip size of the logical drive in bytes


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### StripeSizeBytes

The stripe size of the logical drive in bytes


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### TransformationCompletionPercentage

The percent complete for any transformations the logical drive may be undergoing such as RAID migration, stripesize migration, capacity expansion etc.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### VolumeUniqueIdentifier

An identifier (typically SCSI Inquiry based such as Inquiry VPD Page 0x83 NAA 64 identifier) used to uniquely identify this volume.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
## HpeSmartStorageStorageEnclosure
```@odata.type: "#HpeSmartStorageStorageEnclosure.v2_0_0.HpeSmartStorageStorageEnclosure"```

HpSmartStorageStorageEnclosure

> **Resource Instances of this Type**:  

> * `https://{iLO}/redfish/v1/systems/{item}/smartstorage/arraycontrollers/{item}/storageenclosures/{item}/`

### DoorLockLED

The state of the Door Lock LED. When Lit, this indicates that the Enclosure should not be removed since the drives are currently in use.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`DoorLockLED` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`Unknown`|
|`Lit`|
|`Off`|
### DriveBayCount

Number of drive bays supported within the storage enclosure


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### EnclosureLogicalID

Unique ID for the storage enclosure


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### FaultLED

The state of the Fault LED.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`FaultLED` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`Unknown`|
|`Lit`|
|`Off`|
### FirmwareVersion.Current.VersionString

This string represents the version of the firmware image.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### IndicatorLED

The state of the indicator LED.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`IndicatorLED` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`Unknown`|
|`Lit`|
|`Blinking`|
|`Off`|
### Location

Location identifier


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### LocationFormat

Format for Location Identifier


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`LocationFormat` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Controller:Box`|
|`SwitchPort:Box`|
|`SwitchPort:SwitchBay`|
### Manufacturer

The manufacturer of the storage enclosure


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Model

The model string for the storage enclosure


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### PartNumber

Part number of this storage enclosure


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### SKU

SKU for the storage enclosure


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### SerialNumber

The serial number for this storage enclosure


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Status.Health

This represents the health state of this resource in the absence of its dependent resources.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Status/Health` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`OK`|
|`Warning`|
|`Critical`|
### Status.HealthRollup

This represents the overall health state from the view of this resource.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Status/HealthRollup` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`OK`|
|`Warning`|
|`Critical`|
### Status.State

This indicates the known state of the resource, such as if it is enabled.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Status/State` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`Enabled`|
|`Disabled`|
|`Offline`|
|`InTest`|
|`Starting`|
|`Absent`|
### SubEnclosureLocation

Location within the chassis if this storage enclosure is part of a larger chassis hosting multiple storage enclosures


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
## HpeTlsConfig
```@odata.type: "#HpeTlsConfig.v1_0_0.HpeTlsConfig"```

The schema definition for TLS configuration.

> **Resource Instances of this Type**:  

> * `https://{iLO}/redfish/v1/systems/{item}/bios/tlsconfig/settings/`

> * `https://{iLO}/redfish/v1/systems/{item}/bios/tlsconfig/`

### Certificates[array-item].FingerPrint

The fingerprint of the certificate. It is the sha256 (SHA2) of the Der format of the certificate


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Certificates[array-item].Issuer

The Issuer of the certificate


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Certificates[array-item].SerialNumber

The Serial Number of the certificate.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Certificates[array-item].Subject

The Subject of the certificate.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Certificates[array-item].ValidNotAfter

The expiration date of the certificate.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Certificates[array-item].ValidNotBefore

The date when the certificate becomes valid.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Ciphers

The encryption used. It can have more than one type of encryption, example: "AES128-SHA:AES256-SHA:AES128-SHA256:AES256-SHA256"


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Ciphers": "&lt;string-value&gt;"}

### DeleteCertificates[array-item].FingerPrint

To delete a certificate, the user should place its fingerprint here. The fingerprint would be found as a property under the single certificate object in the "Certificates" array 


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"DeleteCertificates": [{"FingerPrint": "&lt;string-value&gt;"}|null, ...]}

### HostnameCheck

Use this option to enable or disable verification of the connected server's hostname with the hostname in the certificate supplied by the server


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"HostnameCheck": "Enabled"}

`HostnameCheck` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Disabled`|
|`Enabled`|
### NewCertificates[array-item].X509Certificate

the body (PEM format) of the Certificate to be added


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"NewCertificates": [{"X509Certificate": "&lt;string-value&gt;"}|null, ...]}

### ProtocolVersion




| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`ProtocolVersion` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`AUTO`|
|`1.0`|
|`1.1`|
|`1.2`|
### TlsCaCertificateCount

The certificates count.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"TlsCaCertificateCount": &lt;integer-value&gt;}

### VerifyMode

It determines if/how the certificates are validated.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"VerifyMode": "PEER"}

`VerifyMode` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`NONE`|
|`PEER`|
## HpeUSBPort
```@odata.type: "#HpeUSBPort.v2_0_0.HpeUSBPort"```

> **Resource Instances of this Type**:  

> * `https://{iLO}/redfish/v1/systems/{item}/usbports/{item}/`

### InstanceNumber

Instance number of the USB Port


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Location

Location of the USB Device on the server


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Location` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Back`|
|`Front`|
|`Internal`|
|`InternalManagement`|
|`InternalSDCard`|
|`iLOManagement`|
### PCIBusNumber

PCI Bus number of the USB controller that controls this USB port 


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### PCIDeviceNumber

PCI Device Number of the USB Controller that controls this USB Port.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### PCIFunctionNumber

PCI Function Number of the USB Controller that controls this USB Port.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### ParentHubInstance

Parent Hub Instance that provides an instance number of the internal hub this USB Port is connected to.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### SharedCapability

Shared Capability of the USB Port


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`SharedCapability` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`UnsharedManagement`|
|`SharedManagementPhysicalSwitch`|
|`SharedManagementPortAutomaticControl`|
### SpeedCapability

USB speed capability of the USB port as configured by the BIOS during POST.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`SpeedCapability` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`USB1FullSpeed`|
|`USB2HighSpeed`|
|`USB3SuperSpeed`|
### UEFIDevicePath

UEFI Device Path of USB Endpoint. Standardized text representation of the UEFI device path, in UTF-8 format


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
## HpeiLOActiveHealthSystem
```@odata.type: "#HpeiLOActiveHealthSystem.v2_0_0.HpeiLOActiveHealthSystem"```

> **Resource Instances of this Type**:  

> * `https://{iLO}/redfish/v1/managers/{item}/activehealthsystem/`

### AHSEnabled

Determines whether HPE Active Health System logging is enabled or disabled.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"AHSEnabled": true}

### AHSFileEnd

The end of the AHS log.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### AHSFileStart

The start of the AHS log.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### LocationParameters.case_no

This query parameter may be added to the AHS location URI to insert the case number into the AHS log header. For example, http://iloname.example.net/ahsdata/HPE_xxxxxxxxxx_20140821.ahs?downloadAll=1&&case_no=abc123.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### LocationParameters.co_name

This query parameter may be added to the AHS location URI to insert the company name into the AHS log header. For example, http://iloname.example.net/ahsdata/HPE_xxxxxxxxxx_20140821.ahs?downloadAll=1&&co_name=myCompany.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### LocationParameters.contact_name

This query parameter may be added to the AHS location URI to insert the contact name into the AHS log header. For example, http://iloname.example.net/ahsdata/HPE_xxxxxxxxxx_20140821.ahs?downloadAll=1&&contact_name=JohnDoe.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### LocationParameters.downloadAll

This query parameter should be used to download entire AHS log. For example, http://iloname.example.net/ahsdata/HPE_xxxxxxxxxx_20140821.ahs?downloadAll=1.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### LocationParameters.email

This query parameter may be added to the AHS location URI to insert the contacts email address into the AHS log header. For example, http://iloname.example.net/ahsdata/HPE_xxxxxxxxxx_20140821.ahs?downloadAll=1&&email=abc@xyz.com.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### LocationParameters.from

This query parameter may be added with the 'to' query parameter to the AHS location URI to limit the range of data returned. The default range is the last seven days of the log and the format is (yyyy-mm-dd). 'downloadAll' parameter should not be used with this query parameter. For example, http://iloname.example.net/ahsdata/HPE_xxxxxxxxxx_20140821.ahs?from=2014-03-01&&to=2014-03-30.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### LocationParameters.phone

This query parameter may be added to the AHS location URI to insert the contacts phone number into the AHS log header. For example, http://iloname.example.net/ahsdata/HPE_xxxxxxxxxx_20140821.ahs?downloadAll=1&&contact_name=JohnDoe&&phone=555-555-5555.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### LocationParameters.to

This query parameter may be added with the 'from' query parameter to the AHS location URI to limit the range of data returned. The default range is the last seven days of the log and the format is (yyyy-mm-dd). 'downloadAll' parameter should not be used with this query parameter. For example, http://iloname.example.net/ahsdata/HPE_xxxxxxxxxx_20140821.ahs?from=2014-03-01&&to=2014-03-30.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### POST Action "HpeiLOActiveHealthSystem.ClearLog"

Parameters:

> example "HpeiLOActiveHealthSystem.ClearLog" action:

```
POST <target-uri>
Content-Type: application/json
OData-Version: 4.0

{}
```

## HpeiLODateTime
```@odata.type: "#HpeiLODateTime.v2_0_0.HpeiLODateTime"```

The management processor date and time.

> **Resource Instances of this Type**:  

> * `https://{iLO}/redfish/v1/managers/{item}/datetime/`

### ConfigurationSettings

The state of the currently displayed configuration settings.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`ConfigurationSettings` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Current`|
|`SomePendingReset`|
### DateTime

The date and time used by management processor.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### PropagateTimeToHost

Determines whether the server time is synchronized with the management processor time during the first POST after AC power is applied.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"PropagateTimeToHost": true}

### TimeZone.Index

The index of the current time zone. To set a new time zone, specify a different time zone index. This property can be set only when DHCPv4 or DHCPv6 supplied time settings are disabled. Since the time zone list might vary from one firmware version to another (which often leads to differences in time zone indices), setting the time zone by name is recommended over setting by index, for better compatibility.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"TimeZone": {"Index": &lt;integer-value&gt;}}

### TimeZone.UtcOffset

The UTC offset of the current time zone, in the format {+/-}hh:mm


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### TimeZone.Value

The environment variable value.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### TimeZoneList[array-item].Index

The time zone index.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### TimeZoneList[array-item].UtcOffset

The UTC offset of the time zone, in the format {+/-}hh:mm


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### TimeZoneList[array-item].Value

The environment variable value.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
## HpeiLOEmbeddedMedia
```@odata.type: "#HpeiLOEmbeddedMedia.v2_0_0.HpeiLOEmbeddedMedia"```

> **Resource Instances of this Type**:  

> * `https://{iLO}/redfish/v1/managers/{item}/embeddedmedia/`

### Controller.Firmware.Current.VersionString

The current version of the embedded media controller.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Controller.Status.Health

This represents the health state of this resource in the absence of its dependent resources.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Controller/Status/Health` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`OK`|
|`Warning`|
|`Critical`|
### Controller.Status.HealthRollup

This represents the overall health state from the view of this resource.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Controller/Status/HealthRollup` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`OK`|
|`Warning`|
|`Critical`|
### Controller.Status.State

This indicates the known state of the resource, such as if it is enabled.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Controller/Status/State` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`Enabled`|
|`Disabled`|
|`Offline`|
|`InTest`|
|`Starting`|
|`Absent`|
### SDCard.SizeMB

The size of the SD card present in the server, in MB.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### SDCard.Status.Health

This represents the health state of this resource in the absence of its dependent resources.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`SDCard/Status/Health` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`OK`|
|`Warning`|
|`Critical`|
### SDCard.Status.HealthRollup

This represents the overall health state from the view of this resource.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`SDCard/Status/HealthRollup` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`OK`|
|`Warning`|
|`Critical`|
### SDCard.Status.State

This indicates the known state of the resource, such as if it is enabled.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`SDCard/Status/State` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`Enabled`|
|`Disabled`|
|`Offline`|
|`InTest`|
|`Starting`|
|`Absent`|
## HpeiLOFederatedGroupCapping
```@odata.type: "#HpeiLOFederatedGroupCapping.v2_0_0.HpeiLOFederatedGroupCapping"```

> **Resource Instances of this Type**:  

> * `https://{iLO}/redfish/v1/chassis/{item}/power/federatedgroupcapping/`

### CapWatts

The configured power cap for all servers in a group. This value is 0 if the power cap is not configured.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### CapacityWatts

The total power supply capacity for all servers in a group.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Throttle

High, Med, or Low based on the percentage of power usage.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
## HpeiLOFederationGroup
```@odata.type: "#HpeiLOFederationGroup.v2_0_0.HpeiLOFederationGroup"```

> **Resource Instances of this Type**:  

> * `https://{iLO}/redfish/v1/managers/{item}/federationgroups/{item}/`

### Key

The password used by the Federation Group.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Key": "&lt;string-value&gt;"}

### Privileges.HostBIOSConfigPriv

Host BIOS configuration privileges.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Privileges": {"HostBIOSConfigPriv": true}}

### Privileges.HostNICConfigPriv

Host NIC configuration privileges.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Privileges": {"HostNICConfigPriv": true}}

### Privileges.HostStorageConfigPriv

Host Storage configuration privileges.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Privileges": {"HostStorageConfigPriv": true}}

### Privileges.LoginPriv

Login privileges.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Privileges": {"LoginPriv": true}}

### Privileges.RemoteConsolePriv

Remote console privileges.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Privileges": {"RemoteConsolePriv": true}}

### Privileges.SystemRecoveryConfigPriv

System Recovery configuration privileges.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Privileges": {"SystemRecoveryConfigPriv": true}}

### Privileges.UserConfigPriv

User configuration privileges.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Privileges": {"UserConfigPriv": true}}

### Privileges.VirtualMediaPriv

Virtual media privileges.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Privileges": {"VirtualMediaPriv": true}}

### Privileges.VirtualPowerAndResetPriv

Virtual power and reset privileges.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Privileges": {"VirtualPowerAndResetPriv": true}}

### Privileges.iLOConfigPriv

The management processor configuration privileges.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Privileges": {"iLOConfigPriv": true}}

## HpeiLOFederationPeers
```@odata.type: "#HpeiLOFederationPeers.v2_0_0.HpeiLOFederationPeers"```

> **Resource Instances of this Type**:  

> * `https://{iLO}/redfish/v1/managers/{item}/federationpeers/{item}/`

### Peers[array-item].HttpErrorCode

Error code for success or failure.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Peers[array-item].ManagerIPAddress

Manager IP address of the federation peer.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Peers[array-item].Time

Time when the federation peer was added.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Peers[array-item].URL

URL of the federation peer.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Peers[array-item].UUID

UUID peers that are part of the federation group.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
## HpeiLOLicense
```@odata.type: "#HpeiLOLicense.v2_0_0.HpeiLOLicense"```

> **Resource Instances of this Type**:  

> * `https://{iLO}/redfish/v1/managers/{item}/licenseservice/{item}/`

### Confirmation.Code

Confirmation service response code.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Confirmation.Message

User-friendly confirmation information for the current managment processor license.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Confirmation.Service

Confirmation service URI.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Confirmation.Status

Confirmation status.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### ConfirmationRequest.EON.License

The current license of this management processor.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### ConfirmationRequest.EON.LicenseKey

The license key installed on this management processor.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### ConfirmationRequest.EON.Quantity

The number of entitlements licensed.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### ConfirmationRequest.EON.State

The current licensing state and behavior of the management processor.  This is affected by license installation, activation and confirmation.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`ConfirmationRequest/EON/State` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`unlicensed`|
|`evaluation`|
|`nfr`|
|`expired`|
|`unconfirmed`|
|`timeout`|
|`confirmed`|
|`static`|
|`err`|
### ConfirmationRequest.Signer

Source of confirmation request.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### ConfirmationRequest.System.ChipId

Management processor unique chip identifier.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### ConfirmationRequest.System.Product

System housing management processor.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### ConfirmationRequest.System.SerialNumber

System serial number.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### License

The current license of this management processor.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### LicenseErr

Error information from the most recent attempt to alter the installed management processor license.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### LicenseExpire

Expiration information of the installed management processor license.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### LicenseFeatures.DirectoryAuth

Directory integrated authentication.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### LicenseFeatures.EmailAlert

Email based alerting.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### LicenseFeatures.FWScan

Runtime FW Integrity check.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### LicenseFeatures.Federation

Distributed peer to peer management.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### LicenseFeatures.Jitter

Jitter Control.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### LicenseFeatures.KD

Kernel Debugging (VSP raw mode).


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### LicenseFeatures.KeyMgr

Store and retrieve keys from an external key manager.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### LicenseFeatures.MURC

Shared Multi-User Remote Console.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### LicenseFeatures.PowerReg

Power Regulator.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### LicenseFeatures.RC

Graphical Remote Console.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### LicenseFeatures.RemoteSyslog

Remote Syslog.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### LicenseFeatures.Scrncap

Video Capture.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### LicenseFeatures.SecureErase

Secure Erase of embedded media.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### LicenseFeatures.SmartCard

2-Factor Authentication (Smart Card).


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### LicenseFeatures.SuiteB

SuiteB/CNSA mode support.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### LicenseFeatures.TextCons

Text Console.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### LicenseFeatures.VM

Remote Console based Virtual Media.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### LicenseFeatures.VMScript

Scripted Virtual Media.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### LicenseFeatures.VSPLogging

Virtual Serial Port Logging and Playback.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### LicenseKey

User-visible license key installed on this management processor. License keys are 25 or 29 characters and contain letters, numbers and hypens. Use POST method to collection of membertype HpeiLOLicense to install / update the license.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### LicenseTier

The licensed feature-set of the management processor.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`LicenseTier` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`STD`|
|`BLSTD`|
|`ADV`|
|`BLADV`|
|`ESS`|
|`SCALEOUT`|
|`APSE`|
### LicenseType

The type of current license activation on this management processor.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`LicenseType` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Unlicensed`|
|`Evaluation`|
|`Perpetual`|
|`Subscription`|
|`Internal`|
|`Duration`|
|`Expired`|
## HpeiLOResourceDirectory
```@odata.type: "#HpeiLOResourceDirectory.v2_0_0.HpeiLOResourceDirectory"```

> **Resource Instances of this Type**:  

> * `https://{iLO}/redfish/v1/resourcedirectory/`

### Instances[array-item].ETag

This is the last known etag of the resource. The property is omitted if not known.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Instances[array-item].MemberType

This property has the type of members for collection resources.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
## HpeiLOSSO
```@odata.type: "#HpeiLOSSO.v2_0_0.HpeiLOSSO"```

This is the schema definition for the HPE SSO Trusted Server.

> **Resource Instances of this Type**:  

> * `https://{iLO}/redfish/v1/managers/{item}/securityservice/sso/`

### ManagerTrustedCertificates[array-item].Certificate

Contains PEM formatted X509 certificate (Base64 encoded).


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### ManagerTrustedCertificates[array-item].CertificateDetails

Contains X509 certificate information.


| | |
|---|---|
|JSON type|object|
|HTTP PATCH|No (read only)
### ManagerTrustedCertificates[array-item].CertificateDetails.Issuer

The Certificate Authority that issued the certificate.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### ManagerTrustedCertificates[array-item].CertificateDetails.Subject

The entity to which the certificate was issued.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### ManagerTrustedCertificates[array-item].CertificateDetails.ValidNotAfter

The date on which the certificate validity period ends.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### ManagerTrustedCertificates[array-item].CertificateDetails.ValidNotBefore

The date on which the certificate validity period begins.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### ManagerTrustedCertificates[array-item].SerialNumber

Contains the Serial number for the SSO records.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### ManagerTrustedCertificates[array-item].ServerName

The Server name (or certificate subject).


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### ManagerTrustedCertificates[array-item].Status


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`ManagerTrustedCertificates[]/Status` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`OK`|
|`Degraded`|
|`Failed`|
### SSOsettings.AdminPrivilege.HostBIOSConfigPriv

Host BIOS Configuration Privileges.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"SSOsettings": {"AdminPrivilege": {"HostBIOSConfigPriv": true}}}

### SSOsettings.AdminPrivilege.HostNICConfigPriv

Host NIC Configuration Privileges.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"SSOsettings": {"AdminPrivilege": {"HostNICConfigPriv": true}}}

### SSOsettings.AdminPrivilege.HostStorageConfigPriv

Host Storage Configuration Privileges.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"SSOsettings": {"AdminPrivilege": {"HostStorageConfigPriv": true}}}

### SSOsettings.AdminPrivilege.LoginPriv

Login Privileges.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"SSOsettings": {"AdminPrivilege": {"LoginPriv": true}}}

### SSOsettings.AdminPrivilege.RemoteConsolePriv

Remote Console Privileges.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"SSOsettings": {"AdminPrivilege": {"RemoteConsolePriv": true}}}

### SSOsettings.AdminPrivilege.SystemRecoveryConfigPriv

System Recovery Configuration Privileges.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"SSOsettings": {"AdminPrivilege": {"SystemRecoveryConfigPriv": true}}}

### SSOsettings.AdminPrivilege.UserConfigPriv

User Configuration Privileges.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"SSOsettings": {"AdminPrivilege": {"UserConfigPriv": true}}}

### SSOsettings.AdminPrivilege.VirtualMediaPriv

Virtual Media Privileges.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"SSOsettings": {"AdminPrivilege": {"VirtualMediaPriv": true}}}

### SSOsettings.AdminPrivilege.VirtualPowerAndResetPriv

Power and Reset Privileges.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"SSOsettings": {"AdminPrivilege": {"VirtualPowerAndResetPriv": true}}}

### SSOsettings.AdminPrivilege.iLOConfigPriv

iLO Configuration Privileges.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"SSOsettings": {"AdminPrivilege": {"iLOConfigPriv": true}}}

### SSOsettings.OperatorPrivilege.HostBIOSConfigPriv

Host BIOS Configuration Privileges.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"SSOsettings": {"OperatorPrivilege": {"HostBIOSConfigPriv": true}}}

### SSOsettings.OperatorPrivilege.HostNICConfigPriv

Host NIC Configuration Privileges.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"SSOsettings": {"OperatorPrivilege": {"HostNICConfigPriv": true}}}

### SSOsettings.OperatorPrivilege.HostStorageConfigPriv

Host Storage Configuration Privileges.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"SSOsettings": {"OperatorPrivilege": {"HostStorageConfigPriv": true}}}

### SSOsettings.OperatorPrivilege.LoginPriv

Login Privileges.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"SSOsettings": {"OperatorPrivilege": {"LoginPriv": true}}}

### SSOsettings.OperatorPrivilege.RemoteConsolePriv

Remote Console Privileges.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"SSOsettings": {"OperatorPrivilege": {"RemoteConsolePriv": true}}}

### SSOsettings.OperatorPrivilege.SystemRecoveryConfigPriv

System Recovery Configuration Privileges.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"SSOsettings": {"OperatorPrivilege": {"SystemRecoveryConfigPriv": true}}}

### SSOsettings.OperatorPrivilege.UserConfigPriv

User Configuration Privileges.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"SSOsettings": {"OperatorPrivilege": {"UserConfigPriv": true}}}

### SSOsettings.OperatorPrivilege.VirtualMediaPriv

Virtual Media Privileges.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"SSOsettings": {"OperatorPrivilege": {"VirtualMediaPriv": true}}}

### SSOsettings.OperatorPrivilege.VirtualPowerAndResetPriv

Power and Reset Privileges.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"SSOsettings": {"OperatorPrivilege": {"VirtualPowerAndResetPriv": true}}}

### SSOsettings.OperatorPrivilege.iLOConfigPriv

iLO Configuration Privileges.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"SSOsettings": {"OperatorPrivilege": {"iLOConfigPriv": true}}}

### SSOsettings.SSOTrustMode

Represents the SSO Trust Mode.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"SSOsettings": {"SSOTrustMode": "TrustbyName"}}

`SSOsettings/SSOTrustMode` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`TrustNone`|
|`TrustAll`|
|`TrustbyName`|
|`TrustbyCert`|
### SSOsettings.UserPrivilege.HostBIOSConfigPriv

Host BIOS Configuration Privileges.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"SSOsettings": {"UserPrivilege": {"HostBIOSConfigPriv": true}}}

### SSOsettings.UserPrivilege.HostNICConfigPriv

Host NIC Configuration Privileges.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"SSOsettings": {"UserPrivilege": {"HostNICConfigPriv": true}}}

### SSOsettings.UserPrivilege.HostStorageConfigPriv

Host Storage Configuration Privileges.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"SSOsettings": {"UserPrivilege": {"HostStorageConfigPriv": true}}}

### SSOsettings.UserPrivilege.LoginPriv

Login Privileges.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"SSOsettings": {"UserPrivilege": {"LoginPriv": true}}}

### SSOsettings.UserPrivilege.RemoteConsolePriv

Remote Console Privileges.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"SSOsettings": {"UserPrivilege": {"RemoteConsolePriv": true}}}

### SSOsettings.UserPrivilege.SystemRecoveryConfigPriv

System Recovery Configuration Privileges.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"SSOsettings": {"UserPrivilege": {"SystemRecoveryConfigPriv": true}}}

### SSOsettings.UserPrivilege.UserConfigPriv

User Configuration Privileges.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"SSOsettings": {"UserPrivilege": {"UserConfigPriv": true}}}

### SSOsettings.UserPrivilege.VirtualMediaPriv

Virtual Media Privileges.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"SSOsettings": {"UserPrivilege": {"VirtualMediaPriv": true}}}

### SSOsettings.UserPrivilege.VirtualPowerAndResetPriv

Power and Reset Privileges.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"SSOsettings": {"UserPrivilege": {"VirtualPowerAndResetPriv": true}}}

### SSOsettings.UserPrivilege.iLOConfigPriv

iLO Configuration Privileges.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"SSOsettings": {"UserPrivilege": {"iLOConfigPriv": true}}}

### POST Action "HpeiLOSSO.DeleteAllSSORecords"

Parameters:

> example "HpeiLOSSO.DeleteAllSSORecords" action:

```
POST <target-uri>
Content-Type: application/json
OData-Version: 4.0

{}
```

### POST Action "HpeiLOSSO.DeleteSSORecordbyNumber"

Parameters:

"**RecordNumber**" (string) with the value **"<integer>"**

> example "HpeiLOSSO.DeleteSSORecordbyNumber" action:

```
POST <target-uri>
Content-Type: application/json
OData-Version: 4.0

{
    "RecordNumber": "<integer>"
}
```

### POST Action "HpeiLOSSO.ImportCertificate"

Parameters:

"**CertInput**" (string) with the value **"<text>"**

"**CertType**" (string) with one of the following value(s):

* DirectImportCert
* ImportCertUri

> example "HpeiLOSSO.ImportCertificate" action:

```
POST <target-uri>
Content-Type: application/json
OData-Version: 4.0

{
    "CertInput": "<text>", 
    "CertType": "DirectImportCert"
}
```

### POST Action "HpeiLOSSO.ImportDNSName"

Parameters:

"**DNSName**" (string) with the value **"<string>"**

> example "HpeiLOSSO.ImportDNSName" action:

```
POST <target-uri>
Content-Type: application/json
OData-Version: 4.0

{
    "DNSName": "<string>"
}
```

## HpeiLOSnmpService
```@odata.type: "#HpeiLOSnmpService.v2_0_0.HpeiLOSnmpService"```

> **Resource Instances of this Type**:  

> * `https://{iLO}/redfish/v1/managers/{item}/snmpservice/`

### AlertsEnabled

The alert conditions that the management processor detects independently of the host operating system can be sent to specified SNMP alert destinations, such as SIM.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"AlertsEnabled": true}

### Contact

The string of up to 49 characters that specifies the system administrator or server owner. The string can include a name, email address, or phone number.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Contact": "&lt;string-value&gt;"}

### Location

The string of up to 49 characters that specifies the physical location of the server.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Location": "&lt;string-value&gt;"}

### Oem.Hpe.SNMPColdStartTrapBroadcast

If set to true, the Cold Start Trap will be enabled. The Cold Start Trap is broadcast to a subnet broadcast address if there are no trap destinations configured in the SNMP Alert Destination(s) boxes.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Oem": {"Hpe": {"SNMPColdStartTrapBroadcast": true}}}

### Role

The string of up to 64 characters that describes the server role or function.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Role": "&lt;string-value&gt;"}

### RoleDetail

The string of up to 512 characters that describes specific tasks that the server might perform.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"RoleDetail": "&lt;string-value&gt;"}

### SNMPv1Traps

When enabled, SNMPv1 traps are sent to the remote management systems configured in the SNMP Alert Destination(s) boxes.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"SNMPv1Traps": true}

### SNMPv3EngineID

The SNMPv3 Engine ID is the unique identifier of an SNMP engine that belongs to an SNMP agent entity. This value must be a hexadecimal string with an even number of 6 to 32 characters, excluding the first two characters, 0x (for example, 0x01020304abcdef).


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"SNMPv3EngineID": "&lt;string-value&gt;"}

### Status.Health

This represents the health state of this resource in the absence of its dependent resources.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Status/Health` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`OK`|
|`Warning`|
|`Critical`|
### Status.HealthRollup

This represents the overall health state from the view of this resource.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Status/HealthRollup` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`OK`|
|`Warning`|
|`Critical`|
### Status.State

This indicates the known state of the resource, such as if it is enabled.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Status/State` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`Enabled`|
|`Disabled`|
|`Offline`|
|`InTest`|
|`Starting`|
|`Absent`|
### TrapSourceHostname

Determines the host name that is used in the SNMP-defined sysName variable when the management processor generates SNMP traps.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"TrapSourceHostname": "System"}

`TrapSourceHostname` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Manager`|
|`System`|
### Users[array-item].AuthPassphrase

Sets the passphrase to use for sign operations. Enter a value of 8 to 49 characters.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Users": [{"AuthPassphrase": "&lt;string-value&gt;"}|null, ...]}

### Users[array-item].AuthProtocol

Sets the message digest algorithm to use for encoding the authorization passphrase. The message digest is calculated over an appropriate portion of an SNMP message, and is included as part of the message sent to the recipient. Select MD5 (Message Digest) or SHA (Secure Hash Algorithm).


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Users": [{"AuthProtocol": "SHA"}|null, ...]}

`Users[]/AuthProtocol` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`MD5`|
|`SHA`|
### Users[array-item].PrivacyPassphrase

Sets the passphrase to use for encrypt operations. Enter a value of 8 to 49 characters.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Users": [{"PrivacyPassphrase": "&lt;string-value&gt;"}|null, ...]}

### Users[array-item].PrivacyProtocol

Sets the encryption algorithm to use for encoding the privacy passphrase. A portion of an SNMP message is encrypted before transmission. Select AES (Advanced Encryption Standard) or DES (Data Encryption Standard).


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Users": [{"PrivacyProtocol": "AES"}|null, ...]}

`Users[]/PrivacyProtocol` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`DES`|
|`AES`|
### Users[array-item].SecurityName

The user profile name. Enter an alphanumeric string of 1 to 32 characters.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Users": [{"SecurityName": "&lt;string-value&gt;"}|null, ...]}

### POST Action "HpeiLOSnmpService.SendSNMPTestAlert"

Parameters:

> example "HpeiLOSnmpService.SendSNMPTestAlert" action:

```
POST <target-uri>
Content-Type: application/json
OData-Version: 4.0

{}
```

## HpeiSCSISoftwareInitiator
```@odata.type: "#HpeiSCSISoftwareInitiator.v2_0_0.HpeiSCSISoftwareInitiator"```

> **Resource Instances of this Type**:  

> * `https://{iLO}/redfish/v1/systems/{item}/bios/iscsi/`

> * `https://{iLO}/redfish/v1/systems/{item}/bios/iscsi/settings/`

### iSCSIInitiatorName

The worldwide unique iSCSI Qualified Name (IQN) of this iSCSI Initiator. Only IQN format is accepted. EUI format is not supported (for example, 'iqn.1986-03.com.hp:init.sn-123456').


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
### iSCSISources[array-item].StructuredBootString

Identifies this iSCSI option within the server.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### iSCSISources[array-item].UEFIDevicePath

Standardized text representation of the UEFI device path for this option, in UTF-8 format.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### iSCSISources[array-item].iSCSIAttemptInstance

Uniquely identifies this iSCSI attempt within iSCSISources array. If set to zero, all other properties in the boot option object are ignored (which will delete an existing boot attempt).


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|Yes (if resource allows PATCH)
### iSCSISources[array-item].iSCSIAttemptName

Human readable descriptive name for this iSCSI attempt configuration


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
### iSCSISources[array-item].iSCSIAuthenticationMethod

The iSCSI connection authentication method.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`iSCSISources[]/iSCSIAuthenticationMethod` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`None`|
|`CHAP`|
### iSCSISources[array-item].iSCSIChapSecret

The password needed for CHAP authentication. This is applicable only when the Authentication Method is set to CHAP, and the CHAP Type is set to Mutual.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
### iSCSISources[array-item].iSCSIChapType

The CHAP authentication type. This is applicable only when the Authentication Method is set to CHAP.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`iSCSISources[]/iSCSIChapType` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`OneWay`|
|`Mutual`|
### iSCSISources[array-item].iSCSIChapUsername

The password needed for CHAP authentication. This is applicable only when the Authentication Method is set to CHAP.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
### iSCSISources[array-item].iSCSIConnectRetry

The number of times to retry the iSCSI connection. Zero means no retries.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|Yes (if resource allows PATCH)
### iSCSISources[array-item].iSCSIConnectTimeoutMS

The iSCSI connection timeout value in milliseconds.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|Yes (if resource allows PATCH)
### iSCSISources[array-item].iSCSIConnection

Enables or Disables iSCSI mode for a selected iSCSI attempt.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`iSCSISources[]/iSCSIConnection` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Disabled`|
|`Enabled`|
|`EnabledMpio`|
### iSCSISources[array-item].iSCSIInitiatorGateway

The gateway address of the iSCSI Initiator, if not configured via DHCP. The address must be an IPv4 or IPv6 address, depending on the IP Address Type.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
### iSCSISources[array-item].iSCSIInitiatorInfoViaDHCP

If enabled, the iSCSI Initiator information is configured from DHCP. Otherwise, the iSCSI initiator information must be statically configured.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
### iSCSISources[array-item].iSCSIInitiatorIpAddress

The IP Address of the iSCSI Initiator, if not configured via DHCP. The Initiator IP Address is always auto-assigned if IP address type is IPv6. The address must be an IPv4 or IPv6 address, depending on the IP Address Type.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
### iSCSISources[array-item].iSCSIInitiatorNetmask

The subnet mask of the iSCSI Initiator, if not configured via DHCP. The address must be an IPv4.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
### iSCSISources[array-item].iSCSIIpAddressType

The iSCSI IP Address type. If set to Auto, IPv4 will be attempted first, followed by IPv6.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`iSCSISources[]/iSCSIIpAddressType` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`IPv4`|
|`IPv6`|
|`Auto`|
### iSCSISources[array-item].iSCSILUN

The iSCSI target Logical Unit Number (LUN), if not obtained from DHCP. This value must follow the SAM-2 spec. E.g. 0001-1234-5678-9ABC. If the digit number is less then 5 characters, a dash character is not required. E.g. 0001. If the lun number is 12345, input 1234-5


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
### iSCSISources[array-item].iSCSINicSource

A BIOS Attribute that describes this selected NIC instance. This must match one of the possible values listed in the iSCSINicSources array.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
### iSCSISources[array-item].iSCSIReverseChapSecret

The password needed for reverse CHAP authentication (from the target to the initiator). This is applicable only when the Authentication Method is set to CHAP, and the CHAP Type is set to Mutual.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
### iSCSISources[array-item].iSCSIReverseChapUsername

User Name for reverse CHAP authentication (from the target to the initiator). This is applicable only when the Authentication Method is set to CHAP, and the CHAP Type is set to Mutual.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
### iSCSISources[array-item].iSCSITargetInfoViaDHCP

If enabled, the iSCSI target information are configured from DHCP. Otherwise, the iSCSI target information must be statically configured.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
### iSCSISources[array-item].iSCSITargetIpAddress

The IP Address of the iSCSI Target, if not obtained from DHCP. The address must be an IPv4 or IPv6 address, depending on the IP Address Type.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
### iSCSISources[array-item].iSCSITargetName

The worldwide unique iSCSI Qualified Name (IQN) of this iSCSI target. Only the IQN format is accepted. EUI format is not supported (for example, 'iqn.1991-05.com.microsoft:iscsitarget-iscsidisk-target').


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
### iSCSISources[array-item].iSCSITargetTcpPort

The iSCSI Target TCP Port number, if not obtained from DHCP.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|Yes (if resource allows PATCH)
## JsonSchemaFile
```@odata.type: "#JsonSchemaFile.v1_0_2.JsonSchemaFile"```

> **Resource Instances of this Type**:  

> * `https://{iLO}/redfish/v1/registries/{item}/`

> * `https://{iLO}/redfish/v1/schemas/{item}/`

### Location[array-item].Language

The RFC 5646 language code for this schema or registry item.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Location[array-item].Uri

Link to locally available URI for schema.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Schema

The typename this schema describes.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
## LogEntry
```@odata.type: "#LogEntry.v1_0_0.LogEntry"```

> **Resource Instances of this Type**:  

> * `https://{iLO}/redfish/v1/managers/{item}/logservices/iel/entries/{item}/`

> * `https://{iLO}/redfish/v1/systems/{item}/logservices/iml/entries/{item}/`

### Created

The date and time when the log entry was created, for example, 2014-04-15T00:38:00Z.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### EntryType

The log entry type.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`EntryType` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Oem`|
### Message

The log entry details.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.Class

The IML event class.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Oem.Hpe.Code

The IML event code.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Oem.Hpe.Count

The occurrence count of the log entry.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Oem.Hpe.EventNumber

The event log identification number. Events are numbered in the order in which they are generated.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Oem.Hpe.LearnMoreLink

The HPSC link for troubleshooting information.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.RecommendedAction

The recommended action for the event.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.Repaired

The repaired status of the IML event.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Oem": {"Hpe": {"Repaired": true}}}

### Oem.Hpe.Updated

The date and time of the latest log entry update, for example, 2014-04-15T00:38:00Z.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### OemRecordFormat

The format of an OEM record.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`OemRecordFormat` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Hpe-IML`|
|`Hpe-iLOEventLog`|
### Severity

The log entry severity.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Severity` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`OK`|
|`Warning`|
|`Critical`|
## LogService
```@odata.type: "#LogService.v1_0_0.LogService"```

> **Resource Instances of this Type**:  

> * `https://{iLO}/redfish/v1/systems/{item}/logservices/iml/`

> * `https://{iLO}/redfish/v1/managers/{item}/logservices/iel/`

### MaxNumberOfRecords

The maximum number of log entries.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### OverWritePolicy

When the log is full, the overwrite policy is enforced.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`OverWritePolicy` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Unknown`|
|`WrapsWhenFull`|
|`NeverOverwrites`|
### POST Action "LogService.ClearLog"

Parameters:

> example "LogService.ClearLog" action:

```
POST <target-uri>
Content-Type: application/json
OData-Version: 4.0

{}
```

## Manager
```@odata.type: "#Manager.v1_1_0.Manager"```

This is the schema definition for a manager.  Examples of managers are BMCs, Enclosure Managers, Management Controllers and other subsystems assigned manageability functions.

> **Resource Instances of this Type**:  

> * `https://{iLO}/redfish/v1/managers/{item}/`

### CommandShell.MaxConcurrentSessions

This is the maximum number of Command Shell sessions, regardless of protocol, that this manager supports.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### CommandShell.ServiceEnabled

Indicates if the Command Shell service is enabled for this manager.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"CommandShell": {"ServiceEnabled": true}}

### FirmwareVersion

The firmware version of this Manager


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### GraphicalConsole.MaxConcurrentSessions

Indicates the maximum number of Graphical Console sessions, regardless of protocol, this manager supports.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### GraphicalConsole.ServiceEnabled

Indicates if the Command Shell service is enabled for this manager.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"GraphicalConsole": {"ServiceEnabled": true}}

### ManagerType

This property is the manager type for this resource.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`ManagerType` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`ManagementController`|
|`EnclosureManager`|
|`BMC`|
### Model

Model name of the manager.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.ClearRestApiStatus

Status of external provider data in NVRAM.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Oem/Hpe/ClearRestApiStatus` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`DataPresent`|
|`DataCleared`|
### Oem.Hpe.ConfigurationSettings

State of the currently displayed configuration settings.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Oem/Hpe/ConfigurationSettings` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Current`|
|`SomePendingReset`|
### Oem.Hpe.FederationConfig.IPv6MulticastScope

The IPv6 network scope of multicast announcements.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Oem": {"Hpe": {"FederationConfig": {"IPv6MulticastScope": "Site"}}}}

`Oem/Hpe/FederationConfig/IPv6MulticastScope` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Link`|
|`Site`|
|`Organization`|
### Oem.Hpe.FederationConfig.MulticastAnnouncementInterval

The frequency in Seconds at which the iLO system announces itself on the network. A value of 0 disables multicast announcments.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Oem": {"Hpe": {"FederationConfig": {"MulticastAnnouncementInterval": &lt;integer-value&gt;}}}}

### Oem.Hpe.FederationConfig.MulticastDiscovery

Enables or Disables Multicast Discovery for the local iLO system.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Oem": {"Hpe": {"FederationConfig": {"MulticastDiscovery": "Disabled"}}}}

`Oem/Hpe/FederationConfig/MulticastDiscovery` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|
|`Disabled`|
### Oem.Hpe.FederationConfig.MulticastTimeToLive

The maximum number of switches a multicast announcement will traverse before being discarded.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Oem": {"Hpe": {"FederationConfig": {"MulticastTimeToLive": &lt;integer-value&gt;}}}}

### Oem.Hpe.FederationConfig.iLOFederationManagement

Enables or Disables iLO Federation features for the local iLO system.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Oem": {"Hpe": {"FederationConfig": {"iLOFederationManagement": "Disabled"}}}}

`Oem/Hpe/FederationConfig/iLOFederationManagement` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|
|`Disabled`|
### Oem.Hpe.Firmware.Backup.BuildNumber

The build number of the firmware.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Oem.Hpe.Firmware.Backup.BuildNumberString

The string version of the build number of the firmware.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.Firmware.Backup.Date

The build date of the firmware.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.Firmware.Backup.DebugBuild

True if the firmware is a debug build; False if it is not.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### Oem.Hpe.Firmware.Backup.Family

The family of the firmware.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.Firmware.Backup.MajorVersion

The major version of the firmware.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Oem.Hpe.Firmware.Backup.MinorVersion

The minor version of the firmware.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Oem.Hpe.Firmware.Backup.Time

The build time of the firmware.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.Firmware.Backup.VersionString

The version string of the firmware. This value might be null if VersionString is unavailable.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.Firmware.Bootblock.BuildNumber

The build number of the firmware.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Oem.Hpe.Firmware.Bootblock.BuildNumberString

The string version of the build number of the firmware.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.Firmware.Bootblock.Date

The build date of the firmware.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.Firmware.Bootblock.DebugBuild

True if the firmware is a debug build; False if it is not.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### Oem.Hpe.Firmware.Bootblock.Family

The family of the firmware.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.Firmware.Bootblock.MajorVersion

The major version of the firmware.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Oem.Hpe.Firmware.Bootblock.MinorVersion

The minor version of the firmware.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Oem.Hpe.Firmware.Bootblock.Time

The build time of the firmware.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.Firmware.Bootblock.VersionString

The version string of the firmware. This value might be null if VersionString is unavailable.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.Firmware.Current.BuildNumber

The build number of the firmware.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Oem.Hpe.Firmware.Current.BuildNumberString

The string version of the build number of the firmware.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.Firmware.Current.Date

The build date of the firmware.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.Firmware.Current.DebugBuild

True if the firmware is a debug build; False if it is not.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### Oem.Hpe.Firmware.Current.Family

The family of the firmware.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.Firmware.Current.MajorVersion

The major version of the firmware.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Oem.Hpe.Firmware.Current.MinorVersion

The minor version of the firmware.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Oem.Hpe.Firmware.Current.Time

The build time of the firmware.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.Firmware.Current.VersionString

The version string of the firmware. This value might be null if VersionString is unavailable.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.Firmware.Pending.BuildNumber

The build number of the firmware.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Oem.Hpe.Firmware.Pending.BuildNumberString

The string version of the build number of the firmware.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.Firmware.Pending.Date

The build date of the firmware.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.Firmware.Pending.DebugBuild

True if the firmware is a debug build; False if it is not.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### Oem.Hpe.Firmware.Pending.Family

The family of the firmware.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.Firmware.Pending.MajorVersion

The major version of the firmware.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Oem.Hpe.Firmware.Pending.MinorVersion

The minor version of the firmware.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Oem.Hpe.Firmware.Pending.Time

The build time of the firmware.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.Firmware.Pending.VersionString

The version string of the firmware. This value might be null if VersionString is unavailable.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.FrontPanelUSB.State

The state of the front USB port device.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Oem/Hpe/FrontPanelUSB/State` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`Ready`|
|`Busy`|
|`Complete`|
|`Error`|
|`Disabled`|
### Oem.Hpe.License.LicenseKey

The installed license key.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.License.LicenseString

Describes the type of license installed on management processor.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.License.LicenseType

Indicates whether the license is Perpetual or Evaluation.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.RIBCLEnabled

This property enables or disables RIBCL for the management processor. The management processor will require reset when this field is modified.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Oem": {"Hpe": {"RIBCLEnabled": true}}}

### Oem.Hpe.RequiredLoginForiLORBSU

Determines whether a user-credential prompt is displayed when a user accesses the iLO RBSU or the iLO Configuration Utility. The following settings are valid: Enabled-A login dialog box opens when a user accesses the iLO RBSU or the iLO Configuration Utility. Disabled (default)-No login is required when a user accesses the iLO RBSU or the iLO Configuration Utility.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Oem": {"Hpe": {"RequiredLoginForiLORBSU": true}}}

### Oem.Hpe.SerialCLISpeed

Serial command line interface speed in bits/second.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Oem": {"Hpe": {"SerialCLISpeed": &lt;integer-value&gt;}}}

### Oem.Hpe.SerialCLIStatus

Status of serial command line interface.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Oem": {"Hpe": {"SerialCLIStatus": "EnabledNoAuth"}}}

`Oem/Hpe/SerialCLIStatus` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`Disabled`|
|`EnabledNoAuth`|
|`EnabledAuthReq`|
### Oem.Hpe.VSPDlLoggingEnabled

This property enables or disables logging to the downloadable Virtual Serial Port (VSP) log.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Oem": {"Hpe": {"VSPDlLoggingEnabled": true}}}

### Oem.Hpe.VSPLogDownloadEnabled

This property enables or disables download of the downloadable Virtual Serial Port (VSP) log.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Oem": {"Hpe": {"VSPLogDownloadEnabled": true}}}

### Oem.Hpe.WebGuiEnabled

This property enables or disables WEB GUI access for the management processor. The management processor will require reset when this field is modified.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Oem": {"Hpe": {"WebGuiEnabled": true}}}

### Oem.Hpe.actions.actions.HpeiLO.ClearRestApiState.Action


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`Oem/Hpe/actions/actions/HpeiLO.ClearRestApiState/Action` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`HpeiLO.ClearRestApiState`|
### Oem.Hpe.actions.actions.HpeiLO.DisableiLOFunctionality.Action


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`Oem/Hpe/actions/actions/HpeiLO.DisableiLOFunctionality/Action` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`HpeiLO.DisableiLOFunctionality`|
### Oem.Hpe.actions.actions.HpeiLO.ResetToFactoryDefaults.Action


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`Oem/Hpe/actions/actions/HpeiLO.ResetToFactoryDefaults/Action` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`HpeiLO.ResetToFactoryDefaults`|
### Oem.Hpe.actions.actions.HpeiLO.ResetToFactoryDefaults.ResetType


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`Oem/Hpe/actions/actions/HpeiLO.ResetToFactoryDefaults/ResetType` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Default`|
### Oem.Hpe.definitions.HpeFirmwareVersionBlock.Backup.BuildNumber

The build number of the firmware.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Oem.Hpe.definitions.HpeFirmwareVersionBlock.Backup.BuildNumberString

The string version of the build number of the firmware.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.definitions.HpeFirmwareVersionBlock.Backup.Date

The build date of the firmware.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.definitions.HpeFirmwareVersionBlock.Backup.DebugBuild

True if the firmware is a debug build; False if it is not.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### Oem.Hpe.definitions.HpeFirmwareVersionBlock.Backup.Family

The family of the firmware.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.definitions.HpeFirmwareVersionBlock.Backup.MajorVersion

The major version of the firmware.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Oem.Hpe.definitions.HpeFirmwareVersionBlock.Backup.MinorVersion

The minor version of the firmware.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Oem.Hpe.definitions.HpeFirmwareVersionBlock.Backup.Time

The build time of the firmware.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.definitions.HpeFirmwareVersionBlock.Backup.VersionString

The version string of the firmware. This value might be null if VersionString is unavailable.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.definitions.HpeFirmwareVersionBlock.Bootblock.BuildNumber

The build number of the firmware.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Oem.Hpe.definitions.HpeFirmwareVersionBlock.Bootblock.BuildNumberString

The string version of the build number of the firmware.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.definitions.HpeFirmwareVersionBlock.Bootblock.Date

The build date of the firmware.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.definitions.HpeFirmwareVersionBlock.Bootblock.DebugBuild

True if the firmware is a debug build; False if it is not.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### Oem.Hpe.definitions.HpeFirmwareVersionBlock.Bootblock.Family

The family of the firmware.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.definitions.HpeFirmwareVersionBlock.Bootblock.MajorVersion

The major version of the firmware.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Oem.Hpe.definitions.HpeFirmwareVersionBlock.Bootblock.MinorVersion

The minor version of the firmware.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Oem.Hpe.definitions.HpeFirmwareVersionBlock.Bootblock.Time

The build time of the firmware.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.definitions.HpeFirmwareVersionBlock.Bootblock.VersionString

The version string of the firmware. This value might be null if VersionString is unavailable.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.definitions.HpeFirmwareVersionBlock.Current.BuildNumber

The build number of the firmware.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Oem.Hpe.definitions.HpeFirmwareVersionBlock.Current.BuildNumberString

The string version of the build number of the firmware.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.definitions.HpeFirmwareVersionBlock.Current.Date

The build date of the firmware.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.definitions.HpeFirmwareVersionBlock.Current.DebugBuild

True if the firmware is a debug build; False if it is not.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### Oem.Hpe.definitions.HpeFirmwareVersionBlock.Current.Family

The family of the firmware.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.definitions.HpeFirmwareVersionBlock.Current.MajorVersion

The major version of the firmware.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Oem.Hpe.definitions.HpeFirmwareVersionBlock.Current.MinorVersion

The minor version of the firmware.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Oem.Hpe.definitions.HpeFirmwareVersionBlock.Current.Time

The build time of the firmware.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.definitions.HpeFirmwareVersionBlock.Current.VersionString

The version string of the firmware. This value might be null if VersionString is unavailable.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.definitions.HpeFirmwareVersionBlock.Pending.BuildNumber

The build number of the firmware.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Oem.Hpe.definitions.HpeFirmwareVersionBlock.Pending.BuildNumberString

The string version of the build number of the firmware.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.definitions.HpeFirmwareVersionBlock.Pending.Date

The build date of the firmware.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.definitions.HpeFirmwareVersionBlock.Pending.DebugBuild

True if the firmware is a debug build; False if it is not.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### Oem.Hpe.definitions.HpeFirmwareVersionBlock.Pending.Family

The family of the firmware.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.definitions.HpeFirmwareVersionBlock.Pending.MajorVersion

The major version of the firmware.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Oem.Hpe.definitions.HpeFirmwareVersionBlock.Pending.MinorVersion

The minor version of the firmware.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Oem.Hpe.definitions.HpeFirmwareVersionBlock.Pending.Time

The build time of the firmware.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.definitions.HpeFirmwareVersionBlock.Pending.VersionString

The version string of the firmware. This value might be null if VersionString is unavailable.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.definitions.HpeFirmwareVersionInfo.BuildNumber

The build number of the firmware.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Oem.Hpe.definitions.HpeFirmwareVersionInfo.BuildNumberString

The string version of the build number of the firmware.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.definitions.HpeFirmwareVersionInfo.Date

The build date of the firmware.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.definitions.HpeFirmwareVersionInfo.DebugBuild

True if the firmware is a debug build; False if it is not.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### Oem.Hpe.definitions.HpeFirmwareVersionInfo.Family

The family of the firmware.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.definitions.HpeFirmwareVersionInfo.MajorVersion

The major version of the firmware.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Oem.Hpe.definitions.HpeFirmwareVersionInfo.MinorVersion

The minor version of the firmware.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Oem.Hpe.definitions.HpeFirmwareVersionInfo.Time

The build time of the firmware.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.definitions.HpeFirmwareVersionInfo.VersionString

The version string of the firmware. This value might be null if VersionString is unavailable.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.iLOFunctionalityRequired

iLO is required and can't be disabled on this platform (usually blades).


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### Oem.Hpe.iLORBSUEnabled

Enables or disables the iLO Configuration Utility. The following settings are valid: Enabled (default)-On servers that support the iLO Configuration Utility,  the iLO Configuration Utility is available when you access the UEFI System Utilities by pressing F9 during POST. Disabled-On servers that support the iLO Configuration Utility, the iLO Configuration Utility is not available when you access the UEFI System Utilities by pressing F9 during POST.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Oem": {"Hpe": {"iLORBSUEnabled": true}}}

### Oem.Hpe.iLOSelfTestResults[array-item].Notes

Additional Information (if any) about the Self Test.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.iLOSelfTestResults[array-item].SelfTestName

iLO Self Test Name.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Oem/Hpe/iLOSelfTestResults[]/SelfTestName` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`UnknownSelfTest`|
|`CryptographicHardware`|
|`Memory`|
|`WebServerCryptography`|
|`MiscCryptography`|
|`UART`|
|`HoodSense`|
|`NVRAMInterface`|
|`NVRAMData`|
|`NVRAMSpace`|
|`NIC`|
|`EmbeddedFlash/SDCard`|
|`StaticRAM`|
|`EEPROM`|
|`I2C`|
|`BootBlock`|
|`ThreadInit`|
|`Infrastructure`|
|`HostRom`|
|`SupportedHost`|
|`EEPROMContent`|
|`PowerManagementController`|
|`CPLDPAL0`|
|`CPLDPAL1`|
|`CPLDPAL2`|
|`CPLDPAL3`|
|`CPLDPAL4`|
|`CPLDPAL5`|
### Oem.Hpe.iLOSelfTestResults[array-item].Status

Status of the Self Test.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Oem/Hpe/iLOSelfTestResults[]/Status` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`NA`|
|`OK`|
|`Informational`|
|`Degraded`|
### Oem.Hpe.iLOServicePort.MassStorageAuthenticationRequired

Indicates whether mass storage authentication is required or not.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Oem": {"Hpe": {"iLOServicePort": {"MassStorageAuthenticationRequired": true}}}}

### Oem.Hpe.iLOServicePort.USBEthernetAdaptersEnabled

Indicates whether the USB Ethernet Adapters are enabled or not.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Oem": {"Hpe": {"iLOServicePort": {"USBEthernetAdaptersEnabled": true}}}}

### Oem.Hpe.iLOServicePort.USBFlashDriveEnabled

Indicates whether the USB Flash Drive is enabled or not.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Oem": {"Hpe": {"iLOServicePort": {"USBFlashDriveEnabled": true}}}}

### Oem.Hpe.iLOServicePort.iLOServicePortEnabled

Indicates whether the iLO Service Port is enabled or not.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Oem": {"Hpe": {"iLOServicePort": {"iLOServicePortEnabled": true}}}}

### Redundancy.MaxNumSupported

This is the maximum number of members allowable for this particular managers redundancy, including this manager.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Redundancy.MemberId

This is the identifier for the member within the collection.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
### Redundancy.MinNumNeeded

This is the minumum number of managers needed for this manager to be redundant.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Redundancy.Mode

This is the redundancy mode of the group.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Redundancy/Mode` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`Failover`|
|`N+1`|
|`LoadBalanced`|
|`Sparing`|
|`LimitedSparing`|
### Redundancy.Status.Health

This represents the health state of this resource in the absence of its dependent resources.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Redundancy/Status/Health` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`OK`|
|`Warning`|
|`Critical`|
### Redundancy.Status.HealthRollup

This represents the overall health state from the view of this resource.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Redundancy/Status/HealthRollup` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`OK`|
|`Warning`|
|`Critical`|
### Redundancy.Status.State

This indicates the known state of the resource, such as if it is enabled.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Redundancy/Status/State` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`Enabled`|
|`Disabled`|
|`Offline`|
|`InTest`|
|`Starting`|
|`Absent`|
### SerialConsole.MaxConcurrentSessions

This is the maximum number of Serial Console sessions, regardless of protocol, that this manager supports.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### SerialConsole.ServiceEnabled

Indicates if the Command Shell service is enabled for this manager.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"SerialConsole": {"ServiceEnabled": true}}

### Status.Health

This represents the health state of this resource in the absence of its dependent resources.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Status/Health` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`OK`|
|`Warning`|
|`Critical`|
### Status.HealthRollup

This represents the overall health state from the view of this resource.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Status/HealthRollup` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`OK`|
|`Warning`|
|`Critical`|
### Status.State

This indicates the known state of the resource, such as if it is enabled.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Status/State` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`Enabled`|
|`Disabled`|
|`Offline`|
|`InTest`|
|`Starting`|
|`Absent`|
### UUID

This is a universally unique identifier that software (for example, SIM) uses to uniquely identify this manager. The UUID is assigned when the system is manufactured.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### POST Action "Manager.Reset"

Parameters:

> example "Manager.Reset" action:

```
POST <target-uri>
Content-Type: application/json
OData-Version: 4.0

{}
```

## ManagerAccount
```@odata.type: "#ManagerAccount.v1_0_0.ManagerAccount"```

> **Resource Instances of this Type**:  

> * `https://{iLO}/redfish/v1/accountservice/accounts/{item}/`

### Oem.Hpe.LoginName

Descriptive login name that helps to easily identify the owner of each user name. The login name does not have to be the same as the user name and must use printable characters. The maximum length for a user name is 39 characters.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Oem": {"Hpe": {"LoginName": "&lt;string-value&gt;"}}}

### Oem.Hpe.Privileges.HostBIOSConfigPriv

This privilege enables a user to configure Host Bios Settings.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Oem": {"Hpe": {"Privileges": {"HostBIOSConfigPriv": true}}}}

### Oem.Hpe.Privileges.HostNICConfigPriv

This privilege enables a user to configure Host NIC Settings.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Oem": {"Hpe": {"Privileges": {"HostNICConfigPriv": true}}}}

### Oem.Hpe.Privileges.HostStorageConfigPriv

This privilege enables a user to configure Host Storage Settings.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Oem": {"Hpe": {"Privileges": {"HostStorageConfigPriv": true}}}}

### Oem.Hpe.Privileges.LoginPriv

This privilege enables a user to log in to management processor. All local accounts have the login privilege. This privilege is added automatically if it is not specified.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Oem": {"Hpe": {"Privileges": {"LoginPriv": true}}}}

### Oem.Hpe.Privileges.RemoteConsolePriv

This privilege enables a user to remotely access the host system Remote Console, including video, keyboard, and mouse control.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Oem": {"Hpe": {"Privileges": {"RemoteConsolePriv": true}}}}

### Oem.Hpe.Privileges.SystemRecoveryConfigPriv

This privilege enables a user to manage the critical recovery firmware images on iLO Drive.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Oem": {"Hpe": {"Privileges": {"SystemRecoveryConfigPriv": true}}}}

### Oem.Hpe.Privileges.UserConfigPriv

This privilege enables a user to add, edit, and delete local management processor user accounts. A user with this privilege can change privileges for all users.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Oem": {"Hpe": {"Privileges": {"UserConfigPriv": true}}}}

### Oem.Hpe.Privileges.VirtualMediaPriv

This privilege enables a user to use the Virtual Media feature on the host system.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Oem": {"Hpe": {"Privileges": {"VirtualMediaPriv": true}}}}

### Oem.Hpe.Privileges.VirtualPowerAndResetPriv

This privilege enables a user to power-cycle or reset the host system. These activities interrupt system availability. A user with this privilege can diagnose the system by using the Generate NMI to System button.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Oem": {"Hpe": {"Privileges": {"VirtualPowerAndResetPriv": true}}}}

### Oem.Hpe.Privileges.iLOConfigPriv

This privilege enables a user to configure most management processor settings, including security settings, and to remotely update the management processor firmware. This privilege does not enable local user account administration.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Oem": {"Hpe": {"Privileges": {"iLOConfigPriv": true}}}}

### Password

The password used to log in to the management processor. The maximum length for a password is 39 characters. The minimum length for a password is specified in the MinPasswordLength property of the AccountService schema.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Password": "&lt;string-value&gt;"}

### UserName

The name used to log in to the management processor. The user name does not have to be the same as the login name. The maximum length for the user name is 39 characters. The user name must use printable characters.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"UserName": "&lt;string-value&gt;"}

## ManagerNetworkProtocol
```@odata.type: "#ManagerNetworkProtocol.v1_0_0.ManagerNetworkProtocol"```

This resource is used to obtain or modify the network services managed by this manager.

> **Resource Instances of this Type**:  

> * `https://{iLO}/redfish/v1/managers/{item}/networkservice/`

### FQDN

The fully-qualified domain name of the manager that is obtained by DNS and includes the host name and top-level domain name.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### HTTP.Port

The HTTP port number.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"HTTP": {"Port": &lt;integer-value&gt;}}

### HTTP.ProtocolEnabled

Indicates whether HTTP is enabled or disabled.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"HTTP": {"ProtocolEnabled": true}}

### HTTPS.Port

The HTTPS/SSL port number.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"HTTPS": {"Port": &lt;integer-value&gt;}}

### HTTPS.ProtocolEnabled

Indicates whether HTTPS/SSL is enabled or disabled.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"HTTPS": {"ProtocolEnabled": true}}

### HostName

The host name of the manager that is obtained by DNS and does not include any domain information.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"HostName": "&lt;string-value&gt;"}

### IPMI.Port

The IPMI over LAN port number.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"IPMI": {"Port": &lt;integer-value&gt;}}

### IPMI.ProtocolEnabled

Indicates whether IPMI over LAN is enabled for the manager.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"IPMI": {"ProtocolEnabled": true}}

### KVMIP.Port

The KVM-IP port number.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"KVMIP": {"Port": &lt;integer-value&gt;}}

### KVMIP.ProtocolEnabled

Indicates whether KVM-IP is enabled for the manager.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"KVMIP": {"ProtocolEnabled": true}}

### Oem.Hpe.AlertMailEmail

The destination email address for email alerts.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Oem": {"Hpe": {"AlertMailEmail": "&lt;string-value&gt;"}}}

### Oem.Hpe.AlertMailEnabled

Indicates whether AlertMail is enabled. This can be enabled only when the properties AlertMailEmail, AlertMailSenderDomain and AlertMailSMTPServer are set or not empty.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Oem": {"Hpe": {"AlertMailEnabled": true}}}

### Oem.Hpe.AlertMailSMTPPort

The SMTP server port number.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Oem": {"Hpe": {"AlertMailSMTPPort": &lt;integer-value&gt;}}}

### Oem.Hpe.AlertMailSMTPServer

The IP address or DNS name of the SMTP server or the Mail Submission Agent (MSA).


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Oem": {"Hpe": {"AlertMailSMTPServer": "&lt;string-value&gt;"}}}

### Oem.Hpe.AlertMailSenderDomain

The domain name for the sender email address.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Oem": {"Hpe": {"AlertMailSenderDomain": "&lt;string-value&gt;"}}}

### Oem.Hpe.ConfigurationSettings

State of the currently displayed configuration settings.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Oem/Hpe/ConfigurationSettings` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Current`|
|`SomePendingReset`|
### Oem.Hpe.FederationEnabled

Indicates whether management processor federation management is enabled or disabled.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Oem": {"Hpe": {"FederationEnabled": true}}}

### Oem.Hpe.FederationSupported

Indicates whether management processor federation is supported.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### Oem.Hpe.RemoteSyslogEnabled

Indicates whether Remote Syslog is enabled. When enabled, management processor sends notification messages to the specified Syslog server. This can be enabled only when the property RemoteSyslogServer is set or not empty.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Oem": {"Hpe": {"RemoteSyslogEnabled": true}}}

### Oem.Hpe.RemoteSyslogPort

The port number through which the Syslog servers are listening.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Oem": {"Hpe": {"RemoteSyslogPort": &lt;integer-value&gt;}}}

### Oem.Hpe.RemoteSyslogServer

The IP address, FQDN, IPv6 name, or short name of the servers running the Syslog service.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Oem": {"Hpe": {"RemoteSyslogServer": "&lt;string-value&gt;"}}}

### Oem.Hpe.SNMPTrapPort

The SNMP trap port number.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Oem": {"Hpe": {"SNMPTrapPort": &lt;integer-value&gt;}}}

### Oem.Hpe.SerialOverLanLogging

Indicates whether Serial Over LAN (SOL) or Virtual Serial Port (VSP) logging is enabled.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Oem": {"Hpe": {"SerialOverLanLogging": true}}}

### Oem.Hpe.XMLResponseEnabled

Determines whether management processor responds to anonymous XML discovery requests.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Oem": {"Hpe": {"XMLResponseEnabled": true}}}

### Oem.Hpe.actions.actions.HpeiLOManagerNetworkService.SendTestAlertMail.Action

Sends test alert mail to configured AlertMail email address.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Oem/Hpe/actions/actions/HpeiLOManagerNetworkService.SendTestAlertMail/Action` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`HpeiLOManagerNetworkService.SendTestAlertMail`|
### Oem.Hpe.actions.actions.HpeiLOManagerNetworkService.SendTestSyslog.Action


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`Oem/Hpe/actions/actions/HpeiLOManagerNetworkService.SendTestSyslog/Action` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`HpeiLOManagerNetworkService.SendTestSyslog`|
### SNMP.Port

The SNMP port number.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"SNMP": {"Port": &lt;integer-value&gt;}}

### SNMP.ProtocolEnabled

Indicates whether SNMP is enabled for the manager.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"SNMP": {"ProtocolEnabled": true}}

### SSDP.NotifyIPv6Scope

The scope for IPv6 Notify messages for SSDP.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"SSDP": {"NotifyIPv6Scope": "Site"}}

`SSDP/NotifyIPv6Scope` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`Link`|
|`Site`|
|`Organization`|
### SSDP.NotifyMulticastIntervalSeconds

Indicates how often multicast is performed for SSDP.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"SSDP": {"NotifyMulticastIntervalSeconds": &lt;integer-value&gt;}}

### SSDP.NotifyTTL

The Time to Live (TTL) hop count for SSDP Notify messages.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"SSDP": {"NotifyTTL": &lt;integer-value&gt;}}

### SSDP.Port

The SSDP port number.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### SSDP.ProtocolEnabled

Indicates whether SSDP is enabled for the manager.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"SSDP": {"ProtocolEnabled": true}}

### SSH.Port

The SSH port number.  NOTE: When this field is modified, the Manager will reset automatically.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"SSH": {"Port": &lt;integer-value&gt;}}

### SSH.ProtocolEnabled

Indicates whether SSH is enabled for the manager.  NOTE: When this field is modified, the Manager will reset automatically.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"SSH": {"ProtocolEnabled": true}}

### Status.Health

This represents the health state of this resource in the absence of its dependent resources.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Status/Health` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`OK`|
|`Warning`|
|`Critical`|
### Status.HealthRollup

This represents the overall health state from the view of this resource.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Status/HealthRollup` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`OK`|
|`Warning`|
|`Critical`|
### Status.State

This indicates the known state of the resource, such as if it is enabled.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Status/State` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`Enabled`|
|`Disabled`|
|`Offline`|
|`InTest`|
|`Starting`|
|`Absent`|
### VirtualMedia.Port

The Virtual Media port number.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"VirtualMedia": {"Port": &lt;integer-value&gt;}}

### VirtualMedia.ProtocolEnabled

Indicates whether Virtual Media is enabled for the manager.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"VirtualMedia": {"ProtocolEnabled": true}}

## Memory
```@odata.type: "#Memory.v1_1_0.Memory"```

> **Resource Instances of this Type**:  

> * `https://{iLO}/redfish/v1/systems/{item}/memory/{item}/`

### BaseModuleType


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`BaseModuleType` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`RDIMM`|
|`UDIMM`|
|`SO_DIMM`|
|`LRDIMM`|
|`Mini_RDIMM`|
|`Mini_UDIMM`|
|`SO_RDIMM_72b`|
|`SO_UDIMM_72b`|
|`SO_DIMM_16b`|
|`SO_DIMM_32b`|
### BusWidthBits

Bus Width in bits.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### CapacityMiB

Memory Capacity in MiB.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### DataWidthBits

Data Width in bits.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### DeviceID

Device ID


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### DeviceLocator

Location of the Memory in the platform


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### ErrorCorrection


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`ErrorCorrection` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`NoECC`|
|`SingleBitECC`|
|`MultiBitECC`|
|`AddressParity`|
### FirmwareRevision

The firmware revision of this device


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Manufacturer

The Memory manufacturer


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### MemoryDeviceType


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`MemoryDeviceType` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`DDR`|
|`DDR2`|
|`DDR3`|
|`DDR4`|
|`DDR4_SDRAM`|
|`DDR4E_SDRAM`|
|`LPDDR4_SDRAM`|
|`DDR3_SDRAM`|
|`LPDDR3_SDRAM`|
|`DDR2_SDRAM`|
|`DDR2_SDRAM_FB_DIMM`|
|`DDR2_SDRAM_FB_DIMM_PROBE`|
|`DDR_SGRAM`|
|`DDR_SDRAM`|
|`ROM`|
|`SDRAM`|
|`EDO`|
|`FastPageMode`|
|`PipelinedNibble`|
### MemoryLocation.Channel

Channel number in which Memory is connected


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### MemoryLocation.MemoryController

Memory controller number in which Memory is connected


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### MemoryLocation.Slot

Slot number in which Memory is connected


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### MemoryLocation.Socket

Socket number in which Memory is connected


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### MemoryType


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`MemoryType` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`DRAM`|
|`NVDIMM_N`|
|`NVDIMM_F`|
|`NVDIMM_P`|
### Oem.Hpe.Armed

Specifies the current backup-ready status of the NVDIMM_N if available.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### Oem.Hpe.DIMMStatus

Specifies memory module status and whether the module in use.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Oem/Hpe/DIMMStatus` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`Unknown`|
|`Other`|
|`NotPresent`|
|`PresentUnused`|
|`GoodInUse`|
|`AddedButUnused`|
|`UpgradedButUnused`|
|`ExpectedButMissing`|
|`DoesNotMatch`|
|`NotSupported`|
|`ConfigurationError`|
|`Degraded`|
|`PresentSpare`|
|`GoodPartiallyInUse`|
### Oem.Hpe.MinimumVoltageVoltsX10

The minimum DIMM voltage multiplied by 10, for example, 1.2v = 12.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Oem.Hpe.PredictedMediaLifeLeftPercent

The percentage of media life left.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Oem.Hpe.ProductName

friendly product name from SMBIOS 202 record


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### OperatingSpeedMhz

Operating speed of Memory in MHz


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### PartNumber

The product part number of this device


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### PersistentRegionSizeLimitMiB

Total size of persistent regions in MiB


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### RankCount

Number of ranks available in the Memory


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Status.Health

This represents the health state of this resource in the absence of its dependent resources.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Status/Health` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`OK`|
|`Warning`|
|`Critical`|
### Status.HealthRollup

This represents the overall health state from the view of this resource.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Status/HealthRollup` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`OK`|
|`Warning`|
|`Critical`|
### Status.State

This indicates the known state of the resource, such as if it is enabled.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Status/State` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`Enabled`|
|`Disabled`|
|`Offline`|
|`InTest`|
|`Starting`|
|`Absent`|
### SubsystemDeviceID

Subsystem Device ID


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### SubsystemVendorID

SubSystem Vendor ID


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### VendorID

Vendor ID


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### VolatileRegionSizeLimitMiB

Total size of volatile regions in MiB


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
## Power
```@odata.type: "#Power.v1_2_1.Power"```

This is the schema definition for the Power Metrics.  It represents the properties for Power Consumption and Power Limiting.

> **Resource Instances of this Type**:  

> * `https://{iLO}/redfish/v1/chassis/{item}/power/`

### Oem.Hpe.BatteryBackedUnits[array-item].BBUStatus.Health

This represents the health state of this resource in the absence of its dependent resources.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Oem/Hpe/BatteryBackedUnits[]/BBUStatus/Health` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`OK`|
|`Warning`|
|`Critical`|
### Oem.Hpe.BatteryBackedUnits[array-item].BBUStatus.HealthRollup

This represents the overall health state from the view of this resource.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Oem/Hpe/BatteryBackedUnits[]/BBUStatus/HealthRollup` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`OK`|
|`Warning`|
|`Critical`|
### Oem.Hpe.BatteryBackedUnits[array-item].BBUStatus.State

This indicates the known state of the resource, such as if it is enabled.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Oem/Hpe/BatteryBackedUnits[]/BBUStatus/State` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`Enabled`|
|`Disabled`|
|`Offline`|
|`InTest`|
|`Starting`|
|`Absent`|
### Oem.Hpe.BatteryBackedUnits[array-item].BayNumber

Bay number of the battery backed unit.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Oem.Hpe.BatteryBackedUnits[array-item].CapacityWatts

Total capacity (in Watts) of the battery backed unit.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Oem.Hpe.BatteryBackedUnits[array-item].CutOffSetPointmAh

Cut off threshold (mAh) where battery backed unit stops supplying power to the server.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Oem.Hpe.BatteryBackedUnits[array-item].FirmwareVersion

Firmware version of the battery backed unit.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.BatteryBackedUnits[array-item].PercentCharge

Percentage charge remaining for the battery backed unit.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Oem.Hpe.BatteryBackedUnits[array-item].RemainingCapacitymAh

Remaining capacity (mAh) of the battery backed unit.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Oem.Hpe.BatteryBackedUnits[array-item].SerialNumber

Serial number of the battery backed unit.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.BatteryBackedUnits[array-item].TimeToCutOffSeconds

Run time (in seconds) available with the battery backed unit until cut off. This is detected only when battery is charging or discharging, otherwise set to 0.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Oem.Hpe.BatteryBackedUnits[array-item].TimeToFullChargeMinutes

Time required (in minutes) to fully charge the battery backed unit. This is detected only when battery is charging or discharging, otherwise set to 0.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Oem.Hpe.BatteryBackedUnits[array-item].UsableCapacitymAh

 Usable capacity (mAh) of the battery backed unit.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Oem.Hpe.BbuPowerSupply

Battery Backup Unit Power Supply action determines what will occur when a server is running on battery power.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Oem": {"Hpe": {"BbuPowerSupply": "MomentaryPowerButtonPress"}}}

`Oem/Hpe/BbuPowerSupply` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`DoNothing`|
|`MomentaryPowerButtonPress`|
|`HostShutdown`|
### Oem.Hpe.HasPowerMetering

Indicates if the system has power metering.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### Oem.Hpe.MinimumSafelyAchievableCap

Minimum Safely Achievable Cap is the lowest cap value that is safe for a group power manager to apply to a particular server. It can either be identical to or slightly greater than the 0 percent cap value calculated during ROM power burn.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Oem.Hpe.MinimumSafelyAchievableCapValid

Indicates if the msac is valid.  msac is valid only if this is true.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### Oem.Hpe.SNMPPowerThresholdAlert.DurationInMin

Sets the length of time, in minutes, that power consumption must remain above the warning threshold before an SNMP alert is triggered. The maximum duration is 240 minutes, and the duration must be a multiple of 5.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Oem": {"Hpe": {"SNMPPowerThresholdAlert": {"DurationInMin": &lt;integer-value&gt;}}}}

### Oem.Hpe.SNMPPowerThresholdAlert.ThresholdWatts

Sets the power consumption threshold (watts). If power consumption exceeds this value for the specified time duration, an SNMP alert is triggered.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Oem": {"Hpe": {"SNMPPowerThresholdAlert": {"ThresholdWatts": &lt;integer-value&gt;}}}}

### Oem.Hpe.SNMPPowerThresholdAlert.Trigger

Trigger determines whether alerts are based on peak power consumption, average power consumption, or if they are disabled. Trigger property can only be enabled if the ThresholdWatts and DurationInMin values are specified/configured.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Oem": {"Hpe": {"SNMPPowerThresholdAlert": {"Trigger": "AveragePowerConsumption"}}}}

`Oem/Hpe/SNMPPowerThresholdAlert/Trigger` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Disabled`|
|`AveragePowerConsumption`|
|`PeakPowerConsumption`|
### PowerControl[array-item].MemberId

This is the identifier for the member within the collection.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
### PowerControl[array-item].PowerAllocatedWatts

The total amount of power that has been allocated (or budegeted)to  chassis resources.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### PowerControl[array-item].PowerAvailableWatts

The amount of power not already budgeted and therefore available for additional allocation. (powerCapacity - powerAllocated).  This indicates how much reserve power capacity is left.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### PowerControl[array-item].PowerCapacityWatts

The total amount of power available to the chassis for allocation. This may the power supply capacity, or power budget assigned to the chassis from an up-stream chassis.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### PowerControl[array-item].PowerConsumedWatts

The actual power being consumed by the chassis.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### PowerControl[array-item].PowerLimit.CorrectionInMs

The time required for the limiting process to reduce power consumption to below the limit.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### PowerControl[array-item].PowerLimit.LimitException

The action that is taken if the power cannot be maintained below the LimitInWatts.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"PowerControl": [{"PowerLimit": {"LimitException": "LogEventOnly"}}|null, ...]}

`PowerControl[]/PowerLimit/LimitException` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`NoAction`|
|`HardPowerOff`|
|`LogEventOnly`|
|`Oem`|
### PowerControl[array-item].PowerLimit.LimitInWatts

The Power limit in watts. Set to null to disable power capping.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"PowerControl": [{"PowerLimit": {"LimitInWatts": &lt;integer-value&gt;}}|null, ...]}

### PowerControl[array-item].PowerMetrics.AverageConsumedWatts

The average power level over the measurement window (the last IntervalInMin minutes).


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### PowerControl[array-item].PowerMetrics.IntervalInMin

The time interval (or window) in which the PowerMetrics are measured over.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### PowerControl[array-item].PowerMetrics.MaxConsumedWatts

The highest power consumption level that has occured over the measurement window (the last IntervalInMin minutes).


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### PowerControl[array-item].PowerMetrics.MinConsumedWatts

The lowest power consumption level over the measurement window (the last IntervalInMin minutes).


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### PowerControl[array-item].PowerRequestedWatts

The potential power that the chassis resources are requesting which may be higher than the current level being consumed since requested power includes budget that the chassis resource wants for future use.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### PowerControl[array-item].Status.Health

This represents the health state of this resource in the absence of its dependent resources.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`PowerControl[]/Status/Health` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`OK`|
|`Warning`|
|`Critical`|
### PowerControl[array-item].Status.HealthRollup

This represents the overall health state from the view of this resource.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`PowerControl[]/Status/HealthRollup` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`OK`|
|`Warning`|
|`Critical`|
### PowerControl[array-item].Status.State

This indicates the known state of the resource, such as if it is enabled.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`PowerControl[]/Status/State` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`Enabled`|
|`Disabled`|
|`Offline`|
|`InTest`|
|`Starting`|
|`Absent`|
### PowerSupplies[array-item].FirmwareVersion

The firmware version for this Power Supply


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### PowerSupplies[array-item].LastPowerOutputWatts

The average power output of this Power Supply


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### PowerSupplies[array-item].LineInputVoltage

The line input voltage at which the Power Supply is operating


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### PowerSupplies[array-item].LineInputVoltageType

The line voltage type supported as an input to this Power Supply


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`PowerSupplies[]/LineInputVoltageType` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`Unknown`|
|`ACLowLine`|
|`ACMidLine`|
|`ACHighLine`|
|`DCNeg48V`|
|`HighVoltageDC`|
### PowerSupplies[array-item].MemberId

This is the identifier for the member within the collection.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
### PowerSupplies[array-item].Model

The model number for this Power Supply


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### PowerSupplies[array-item].Oem.Hpe.AveragePowerOutputWatts

The latest observed average power being drawn by the power supply (Watts). This is usually updated every 10 seconds but the period can vary in some circumstances.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### PowerSupplies[array-item].Oem.Hpe.BayNumber

The power supply bay number.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### PowerSupplies[array-item].Oem.Hpe.HotplugCapable

If true, this power supply (and power supply bay) is capable of being hot-plugged.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### PowerSupplies[array-item].Oem.Hpe.MaxPowerOutputWatts

The latest observed maximum output power being drawn by the power supply (Watts). This is usually updated every 10 seconds but the period can vary in some circumstances.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### PowerSupplies[array-item].Oem.Hpe.Mismatched

If true, this power supply is mismatched with others in the system.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### PowerSupplies[array-item].Oem.Hpe.PowerSupplyStatus.State

Indicates the known state of the resource.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`PowerSupplies[]/Oem/Hpe/PowerSupplyStatus/State` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Unknown`|
|`Ok`|
|`Degraded`|
|`Failed`|
|`OverVoltage`|
|`OverCurrent`|
|`OverTemperature`|
|`ACPowerLost`|
|`FanFailure`|
|`WarningHighInputVoltage`|
|`WarningLowInputVoltage`|
|`WarningHighOutputVoltage`|
|`WarningLowOutputVoltage`|
|`WarningInletTemperature`|
|`WarningInternalTemperature`|
|`WarningHighAuxiliaryVoltage`|
|`WarningLowAuxiliaryVoltage`|
|`PowerSupplyMismatch`|
|`GoodInStandby`|
### PowerSupplies[array-item].Oem.Hpe.iPDU.IPAddress

The IP address of the iPDU connected to this power supply.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### PowerSupplies[array-item].Oem.Hpe.iPDU.MacAddress

The Ethernet MAC address of the iPDU connected to this power supply.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### PowerSupplies[array-item].Oem.Hpe.iPDU.Model

The model number of the iPDU connected to this power supply.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### PowerSupplies[array-item].Oem.Hpe.iPDU.SerialNumber

The serial number of the iPDU connected to this power supply.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### PowerSupplies[array-item].Oem.Hpe.iPDU.iPDUStatus.State

Indicates the known state of the resource.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`PowerSupplies[]/Oem/Hpe/iPDU/iPDUStatus/State` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Unknown`|
|`Ok`|
|`Degraded`|
|`Failed`|
|`OverVoltage`|
|`OverCurrent`|
|`OverTemperature`|
|`ACPowerLost`|
|`FanFailure`|
|`WarningHighInputVoltage`|
|`WarningLowInputVoltage`|
|`WarningHighOutputVoltage`|
|`WarningLowOutputVoltage`|
|`WarningInletTemperature`|
|`WarningInternalTemperature`|
|`WarningHighAuxiliaryVoltage`|
|`WarningLowAuxiliaryVoltage`|
|`PowerSupplyMismatch`|
|`GoodInStandby`|
### PowerSupplies[array-item].Oem.Hpe.iPDUCapable

If true, this power supply is capable of being connected to an iPDUs.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### PowerSupplies[array-item].PartNumber

The part number for this Power Supply


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### PowerSupplies[array-item].PowerCapacityWatts

The maximum capacity of this Power Supply


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### PowerSupplies[array-item].PowerSupplyType

The Power Supply type (AC or DC)


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`PowerSupplies[]/PowerSupplyType` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`Unknown`|
|`AC`|
|`DC`|
### PowerSupplies[array-item].Redundancy[array-item].MaxNumSupported

This is the maximum number of members allowable for this particular managers redundancy, including this manager.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### PowerSupplies[array-item].Redundancy[array-item].MemberId

This is the identifier for the member within the collection.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
### PowerSupplies[array-item].Redundancy[array-item].MinNumNeeded

This is the minumum number of managers needed for this manager to be redundant.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### PowerSupplies[array-item].Redundancy[array-item].Mode

This is the redundancy mode of the group.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`PowerSupplies[]/Redundancy[]/Mode` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`Failover`|
|`N+1`|
|`LoadBalanced`|
|`Sparing`|
|`LimitedSparing`|
### PowerSupplies[array-item].Redundancy[array-item].Status.Health

This represents the health state of this resource in the absence of its dependent resources.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`PowerSupplies[]/Redundancy[]/Status/Health` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`OK`|
|`Warning`|
|`Critical`|
### PowerSupplies[array-item].Redundancy[array-item].Status.HealthRollup

This represents the overall health state from the view of this resource.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`PowerSupplies[]/Redundancy[]/Status/HealthRollup` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`OK`|
|`Warning`|
|`Critical`|
### PowerSupplies[array-item].Redundancy[array-item].Status.State

This indicates the known state of the resource, such as if it is enabled.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`PowerSupplies[]/Redundancy[]/Status/State` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`Enabled`|
|`Disabled`|
|`Offline`|
|`InTest`|
|`Starting`|
|`Absent`|
### PowerSupplies[array-item].SerialNumber

The serial number for this Power Supply


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### PowerSupplies[array-item].SparePartNumber

The spare part number for this Power Supply


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### PowerSupplies[array-item].Status.Health

This represents the health state of this resource in the absence of its dependent resources.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`PowerSupplies[]/Status/Health` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`OK`|
|`Warning`|
|`Critical`|
### PowerSupplies[array-item].Status.HealthRollup

This represents the overall health state from the view of this resource.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`PowerSupplies[]/Status/HealthRollup` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`OK`|
|`Warning`|
|`Critical`|
### PowerSupplies[array-item].Status.State

This indicates the known state of the resource, such as if it is enabled.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`PowerSupplies[]/Status/State` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`Enabled`|
|`Disabled`|
|`Offline`|
|`InTest`|
|`Starting`|
|`Absent`|
### Redundancy[array-item].MaxNumSupported

This is the maximum number of members allowable for this particular managers redundancy, including this manager.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Redundancy[array-item].MemberId

This is the identifier for the member within the collection.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
### Redundancy[array-item].MinNumNeeded

This is the minumum number of managers needed for this manager to be redundant.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Redundancy[array-item].Mode

This is the redundancy mode of the group.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Redundancy[]/Mode` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`Failover`|
|`N+1`|
|`LoadBalanced`|
|`Sparing`|
|`LimitedSparing`|
### Redundancy[array-item].Status.Health

This represents the health state of this resource in the absence of its dependent resources.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Redundancy[]/Status/Health` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`OK`|
|`Warning`|
|`Critical`|
### Redundancy[array-item].Status.HealthRollup

This represents the overall health state from the view of this resource.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Redundancy[]/Status/HealthRollup` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`OK`|
|`Warning`|
|`Critical`|
### Redundancy[array-item].Status.State

This indicates the known state of the resource, such as if it is enabled.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Redundancy[]/Status/State` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`Enabled`|
|`Disabled`|
|`Offline`|
|`InTest`|
|`Starting`|
|`Absent`|
### Status.Health

This represents the health state of this resource in the absence of its dependent resources.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Status/Health` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`OK`|
|`Warning`|
|`Critical`|
### Status.HealthRollup

This represents the overall health state from the view of this resource.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Status/HealthRollup` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`OK`|
|`Warning`|
|`Critical`|
### Status.State

This indicates the known state of the resource, such as if it is enabled.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Status/State` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`Enabled`|
|`Disabled`|
|`Offline`|
|`InTest`|
|`Starting`|
|`Absent`|
## Processor
```@odata.type: "#Processor.v1_0_0.Processor"```

This is the schema definition for the Processor resource.  It represents the properties of a processor attached to a System.

> **Resource Instances of this Type**:  

> * `https://{iLO}/redfish/v1/systems/{item}/processors/{item}/`

### InstructionSet

The instruction set of the processor


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`InstructionSet` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`x86`|
|`x86-64`|
|`IA-64`|
|`ARM-A32`|
|`ARM-A64`|
|`MIPS32`|
|`MIPS64`|
|`OEM`|
### Manufacturer

The processor manufacturer


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### MaxSpeedMHz

The maximum clock speed of the processor


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Model

The product model number of this device


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.AssetTag

The processor asset tag.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.Cache[array-item].Associativity

The associativity of the cache.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Oem/Hpe/Cache[]/Associativity` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`DirectMapped`|
|`2waySetAssociative`|
|`4waySetAssociative`|
|`FullyAssociative`|
|`8waySetAssociative`|
|`16waySetAssociative`|
|`12waySetAssociative`|
|`24waySetAssociative`|
|`32waySetAssociative`|
|`48waySetAssociative`|
|`64waySetAssociative`|
|`20waySetAssociative`|
### Oem.Hpe.Cache[array-item].CacheSpeedns

The cache speed (ns).


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Oem.Hpe.Cache[array-item].EccType

The cache memory ECC type.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Oem/Hpe/Cache[]/EccType` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`None`|
|`Parity`|
|`SingleBitECC`|
|`MultiBitECC`|
### Oem.Hpe.Cache[array-item].InstalledSizeKB

The installed cache size (KB).


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Oem.Hpe.Cache[array-item].Location

The cache location (internal or external).


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Oem/Hpe/Cache[]/Location` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Internal`|
|`External`|
### Oem.Hpe.Cache[array-item].MaximumSizeKB

The maximum cache size (KB).


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Oem.Hpe.Cache[array-item].Policy

The caching policy.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Oem/Hpe/Cache[]/Policy` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`WriteThrough`|
|`WriteBack`|
|`Varies`|
### Oem.Hpe.Cache[array-item].Socketed

If true, the cache is a socketed component.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### Oem.Hpe.Cache[array-item].Status.Health

This represents the health state of this resource in the absence of its dependent resources.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Oem/Hpe/Cache[]/Status/Health` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`OK`|
|`Warning`|
|`Critical`|
### Oem.Hpe.Cache[array-item].Status.HealthRollup

This represents the overall health state from the view of this resource.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Oem/Hpe/Cache[]/Status/HealthRollup` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`OK`|
|`Warning`|
|`Critical`|
### Oem.Hpe.Cache[array-item].Status.State

This indicates the known state of the resource, such as if it is enabled.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Oem/Hpe/Cache[]/Status/State` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`Enabled`|
|`Disabled`|
|`Offline`|
|`InTest`|
|`Starting`|
|`Absent`|
### Oem.Hpe.Cache[array-item].SystemCacheType

The cache type (unified, instructions, or data).


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Oem/Hpe/Cache[]/SystemCacheType` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Instruction`|
|`Data`|
|`Unified`|
### Oem.Hpe.ConfigStatus.Populated

True if the processor socket is populated with a CPU.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### Oem.Hpe.ConfigStatus.State

The current state of the processor.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Oem/Hpe/ConfigStatus/State` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|
|`DisabledByUser`|
|`DisabledByBios`|
|`Idle`|
### Oem.Hpe.CoresEnabled

The number of enabled cores in the processor.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Oem.Hpe.ExternalClockMHz

The processor external clock frequency (MHZ), for example, 1000 = 1 GHZ.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Oem.Hpe.MicrocodePatches[array-item].CpuId

The microcode patch CPUID.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.MicrocodePatches[array-item].Date

The microcode patch date.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.MicrocodePatches[array-item].PatchId

The microcode patch ID.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.PartNumber

The processor part number.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.RatedSpeedMHz

The speed of the processor (in MHz) as of the last system boot, for example, 1000 = 1GHz.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Oem.Hpe.SerialNumber

The processor serial number.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.VoltageVoltsX10

The processor voltage multiplied by 10, for example, 3.3v = 33.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### ProcessorArchitecture

The architecture of the processor


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`ProcessorArchitecture` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`x86`|
|`IA-64`|
|`ARM`|
|`MIPS`|
|`OEM`|
### ProcessorId.EffectiveFamily

The effective Family for this processor


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### ProcessorId.EffectiveModel

The effective Model for this processor


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### ProcessorId.MicrocodeInfo

The Microcode Information for this processor


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### ProcessorId.Step

The Step value for this processor


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### ProcessorId.VendorId

The Vendor Identification for this processor


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### ProcessorType

The type of processor


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`ProcessorType` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`CPU`|
|`GPU`|
|`FPGA`|
|`DSP`|
|`Accelerator`|
|`OEM`|
### Socket

The socket or location of the processor


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Status.Health

This represents the health state of this resource in the absence of its dependent resources.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Status/Health` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`OK`|
|`Warning`|
|`Critical`|
### Status.HealthRollup

This represents the overall health state from the view of this resource.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Status/HealthRollup` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`OK`|
|`Warning`|
|`Critical`|
### Status.State

This indicates the known state of the resource, such as if it is enabled.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Status/State` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`Enabled`|
|`Disabled`|
|`Offline`|
|`InTest`|
|`Starting`|
|`Absent`|
### TotalCores

The total number of cores contained in this processor


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### TotalThreads

The total number of execution threads supported by this processor


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
## SecureBoot
```@odata.type: "#SecureBoot.v1_0_0.SecureBoot"```

> **Resource Instances of this Type**:  

> * `https://{iLO}/redfish/v1/systems/{item}/secureboot/`

### SecureBootCurrentBoot

Secure Boot state during the current boot cycle.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`SecureBootCurrentBoot` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Enabled`|
|`Disabled`|
### SecureBootEnable

Enable or disable UEFI Secure Boot (takes effect on next boot).


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"SecureBootEnable": true}

### SecureBootMode

Current Secure Boot Mode.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`SecureBootMode` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`SetupMode`|
|`UserMode`|
|`AuditMode`|
|`DeployedMode`|
### POST Action "SecureBoot.ResetKeys"

Parameters:

"**ResetKeysType**" (string) with one of the following value(s):

* ResetAllKeysToDefault
* DeleteAllKeys
* DeletePK

> example "SecureBoot.ResetKeys" action:

```
POST <target-uri>
Content-Type: application/json
OData-Version: 4.0

{
    "ResetKeysType": "ResetAllKeysToDefault"
}
```

## ServiceRoot
```@odata.type: "#ServiceRoot.v1_1_0.ServiceRoot"```

This object represents the HPE RESTful API root service.

> **Resource Instances of this Type**:  

> * `https://{iLO}/redfish/v1/`

### Oem.Hpe.Manager[array-item].Blade.BayNumber

Specifies the location of the blade in the enclosure.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.Manager[array-item].Blade.EnclosureName

Specifies the name of the enclosure in which the blade is present.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.Manager[array-item].Blade.RackName

Specifies the name of the rack in which the enclosure is present.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.Manager[array-item].DefaultLanguage

Default language used for the Web interface.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.Manager[array-item].FQDN

Fully qualified domain name of the management processor.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.Manager[array-item].HostName

The name of management processor.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.Manager[array-item].IPManager


| | |
|---|---|
|JSON type|object|
|HTTP PATCH|No (read only)
### Oem.Hpe.Manager[array-item].Languages[array-item].Language

Specifies one of the languages supported by the management processor.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.Manager[array-item].Languages[array-item].TranslationName

Specifies one of the languages supported by the management processor.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.Manager[array-item].Languages[array-item].Version

Specifies the version of the management processor in the respective language.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.Manager[array-item].ManagerFirmwareVersion

The major and minor management processor version numbers.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.Manager[array-item].ManagerFirmwareVersionPass

The build or pass number of the management processor version.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.Manager[array-item].ManagerType

The type of the service manager.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.Moniker.ADVLIC

Optional Licensed functionality tier name.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.Moniker.BMC

Generic abbreviation for the management processor.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.Moniker.BSYS

Product category name.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.Moniker.CLASS

Management processor product category.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.Moniker.IPROV

Product name for provisioning and deployment suite.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.Moniker.PRODABR

Abbreviated product name.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.Moniker.PRODFAM

Full product family.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.Moniker.PRODGEN

Abbreviated product name and generation.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.Moniker.PRODNAM

Full product name.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.Moniker.PRODTAG

Branded, abbreviated product name.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.Moniker.STDLIC

Base licensed functionality tier name.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.Moniker.SUMGR

Product name for update deployment suite.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.Moniker.SYSFAM

Host system product family.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.Moniker.VENDABR

Abbreviated vendor name (like stock ticker).


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.Moniker.VENDNAM

Full vendor name.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.Moniker.WWW

Top level public internet vendor URI.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.Moniker.WWWAHSV

Public internet vendor URI for Active Health viewer.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.Moniker.WWWBMC

Public internet vendor URI for the management processor.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.Moniker.WWWDOC

Public internet vendor URI for the management processor documentation / manuals.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.Moniker.WWWERS

Public internet vendor URI for Embedded Remote Support.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.Moniker.WWWGLIS

Public internet vendor URI for management processor licensing infrastructure.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.Moniker.WWWIOL

Public internet vendor URI for Online Insight service.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.Moniker.WWWLIC

Public internet vendor URI for the management processor.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.Moniker.WWWLML

Public internet vendor URI for Learn More Links.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.Moniker.WWWPASS

Public internet vendor URI for accessing support account.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.Moniker.WWWPRV

Public internet vendor URI for privacy policy statement.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.Moniker.WWWQSPEC

Public internet vendor URI for Quick Specs.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.Moniker.WWWRESTDOC

Public internet vendor URI for REST API documentation.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.Moniker.WWWSUP

Public internet vendor URI for management processor and product support.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.Moniker.WWWSWLIC

Public internet vendor URI for vendor software licensing.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.Sessions.CertCommonName

The name of the management processor as it appears in the digital certificate when a secure web GUI session is established to the management processor.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.Sessions.CertificateLoginEnabled

Specifies whether Certificate login is enabled.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### Oem.Hpe.Sessions.KerberosEnabled

Specifies whether Kerberos login is enabled.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### Oem.Hpe.Sessions.LDAPAuthLicenced

Specifies whether a valid license is installed for LDAP use.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### Oem.Hpe.Sessions.LDAPEnabled

Specifies whether LDAP login is enabled.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### Oem.Hpe.Sessions.LocalLoginEnabled

Specifies whether local users can log in.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### Oem.Hpe.Sessions.LoginFailureDelay

The delay (seconds) when a management processor login attempt has failed.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Oem.Hpe.Sessions.LoginHint.Hint

The information on how to log in to the management processor.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.Sessions.LoginHint.HintPOSTData.Password

The password for logging in to the management processor.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.Sessions.LoginHint.HintPOSTData.UserName

The user name for logging in to the management processor.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.Sessions.SecurityMessage

The login security banner message that is displayed on the management processor Login page.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.Sessions.SecurityOverride

Specifies whether the security override switch is enabled.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### Oem.Hpe.Sessions.ServerName

The name of the server that this management processor is managing.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.Time

The current Redfish service time.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### RedfishVersion

The version of the Redfish service


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### UUID

Unique identifier for a service instance.  This value should be an exact match of the UUID value returned in a 200OK from an SSDP M-SEARCH request during discovery.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
## Session
```@odata.type: "#Session.v1_0_0.Session"```

> **Resource Instances of this Type**:  

> * `https://{iLO}/redfish/v1/sessionservice/sessions/{item}/`

### Oem.Hpe.AccessTime

User session last-access time


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.LoginTime

User session login time


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.MySession

Indicates whether this is a session I own.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### Oem.Hpe.Privileges.HostBIOSConfigPriv

This privilege enables a user to configure Host Bios Settings.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### Oem.Hpe.Privileges.HostNICConfigPriv

This privilege enables a user to configure Host NIC Settings.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### Oem.Hpe.Privileges.HostStorageConfigPriv

This privilege enables a user to configure Host Storage Settings.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### Oem.Hpe.Privileges.LoginPriv

This privilege enables a user to log in to the management processor. All local accounts have the login privilege. This privilege is added automatically if it is not specified.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### Oem.Hpe.Privileges.RemoteConsolePriv

This privilege enables a user to remotely access the host system Remote Console, including video, keyboard, and mouse control.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### Oem.Hpe.Privileges.SystemRecoveryConfigPriv

This privilege enables a user to manage the critical recovery firmware images on iLO Drive.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### Oem.Hpe.Privileges.UserConfigPriv

This privilege enables a user to add, edit, and delete local management processor user accounts. A user with this privilege can change privileges for all users.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### Oem.Hpe.Privileges.VirtualMediaPriv

This privilege enables a user to use the Virtual Media feature on the host system.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### Oem.Hpe.Privileges.VirtualPowerAndResetPriv

This privilege enables a user to power-cycle or reset the host system. These activities interrupt system availability. A user with this privilege can diagnose the system by using the Generate NMI to System button.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### Oem.Hpe.Privileges.iLOConfigPriv

This privilege enables a user to configure most management processor settings, including security settings, and to remotely update the management processor firmware. This privilege does not enable local user account administration.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### Oem.Hpe.UserAccount

Login details of the user


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.UserDistinguishedName

LDAP user is identified by its distinguished name (DN).


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.UserExpires

User session expire time


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.UserIP

IP address of the user


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.UserTag

Session source


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Oem/Hpe/UserTag` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Web UI`|
|`RBSU`|
|`Remote Console`|
|`SSH`|
|`IPMI/RMCP`|
|`SM-CLP`|
|`RIBCL`|
|`REST`|
|`Unknown`|
### Oem.Hpe.UserType

User type


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Oem/Hpe/UserType` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Local`|
|`Directory`|
|`Single Sign On`|
|`Kerberos`|
|`Trusted Key`|
|`Security Override`|
|`System`|
|`Federation`|
### UserName

Name to use to log in to the management processor.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
## SessionService
```@odata.type: "#SessionService.v1_0_0.SessionService"```

This is the schema definition for the Session Service.  It represents the properties for the service itself and has links to the actual list of sessions.

> **Resource Instances of this Type**:  

> * `https://{iLO}/redfish/v1/sessionservice/`

### ServiceEnabled

This indicates whether this service is enabled.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
### SessionTimeout

This is the number of seconds of inactivity that a session may have before the session service closes the session due to inactivity.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"SessionTimeout": &lt;integer-value&gt;}

### Status.Health

This represents the health state of this resource in the absence of its dependent resources.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Status/Health` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`OK`|
|`Warning`|
|`Critical`|
### Status.HealthRollup

This represents the overall health state from the view of this resource.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Status/HealthRollup` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`OK`|
|`Warning`|
|`Critical`|
### Status.State

This indicates the known state of the resource, such as if it is enabled.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Status/State` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`Enabled`|
|`Disabled`|
|`Offline`|
|`InTest`|
|`Starting`|
|`Absent`|
## SoftwareInventory
```@odata.type: "#SoftwareInventory.v1_0_0.SoftwareInventory"```

> **Resource Instances of this Type**:  

> * `https://{iLO}/redfish/v1/updateservice/firmwareinventory/{item}/`

> * `https://{iLO}/redfish/v1/updateservice/softwareinventory/{item}/`

### Oem.Hpe.DeviceClass

DeviceType GUID rendered by iLO for certain items iLO knows how to flash, and omitted for all other items.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.DeviceContext

Friendly text string - same as 'Location' in Gen9 fw inventory - omitted if not available.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.DeviceInstance

UEFI Device Path if a PCI Device - omitted otherwise.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Status.Health

This represents the health state of this resource in the absence of its dependent resources.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Status/Health` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`OK`|
|`Warning`|
|`Critical`|
### Status.HealthRollup

This represents the overall health state from the view of this resource.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Status/HealthRollup` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`OK`|
|`Warning`|
|`Critical`|
### Status.State

This indicates the known state of the resource, such as if it is enabled.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Status/State` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`Enabled`|
|`Disabled`|
|`Offline`|
|`InTest`|
|`Starting`|
|`Absent`|
### Updateable

This is true if the item is updatable.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### Version

same as 'VersionString' in existing FwSwVersionInventory


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
## Storage
```@odata.type: "#Storage.v1_0_0.Storage"```

> **Resource Instances of this Type**:  

> * `https://{iLO}/redfish/v1/systems/{item}/storage/{item}/`

### Status.Health

This represents the health state of this resource in the absence of its dependent resources.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Status/Health` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`OK`|
|`Warning`|
|`Critical`|
### Status.HealthRollup

This represents the overall health state from the view of this resource.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Status/HealthRollup` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`OK`|
|`Warning`|
|`Critical`|
### Status.State

This indicates the known state of the resource, such as if it is enabled.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Status/State` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`Enabled`|
|`Disabled`|
|`Offline`|
|`InTest`|
|`Starting`|
|`Absent`|
### StorageControllers[array-item].Manufacturer

Controller Manufacturer name.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
### StorageControllers[array-item].Model

Controller model name.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
### StorageControllers[array-item].SerialNumber

Controller serial number.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
### StorageControllers[array-item].Status.Health

This represents the health state of this resource in the absence of its dependent resources.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`StorageControllers[]/Status/Health` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`OK`|
|`Warning`|
|`Critical`|
### StorageControllers[array-item].Status.HealthRollup

This represents the overall health state from the view of this resource.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`StorageControllers[]/Status/HealthRollup` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`OK`|
|`Warning`|
|`Critical`|
### StorageControllers[array-item].Status.State

This indicates the known state of the resource, such as if it is enabled.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`StorageControllers[]/Status/State` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`Enabled`|
|`Disabled`|
|`Offline`|
|`InTest`|
|`Starting`|
|`Absent`|
### StorageControllers[array-item].UEFIDevicePath

UEFI Device Path of the storage controller.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
## Thermal
```@odata.type: "#Thermal.v1_1_0.Thermal"```

The schema definition for the Thermal Metrics. It represents the properties for temperature and cooling.

> **Resource Instances of this Type**:  

> * `https://{iLO}/redfish/v1/chassis/{item}/thermal/`

### Fans[array-item].CorrelatableID

The CorrelatableID for this fan.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Fans[array-item].LowerThresholdCritical

Below normal range but not yet fatal.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Fans[array-item].LowerThresholdFatal

Below normal range and is fatal.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Fans[array-item].LowerThresholdNonCritical

Below normal range.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Fans[array-item].MaximumValue

Maximum value for CurrentReading.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Fans[array-item].MinimumValue

Minimum value for CurrentReading.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Fans[array-item].Oem.Hpe.HotPluggable

Indicates if the fan can be replaced while server is running.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### Fans[array-item].Oem.Hpe.Location

Indicates the component (i.e. CPU, Memory, and Storage) that the fan is being used to cool.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Fans[]/Oem/Hpe/Location` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`System`|
|`System Board`|
|`I/O Board`|
|`CPU`|
|`Memory`|
|`Storage`|
|`Removable Media`|
|`Power Supply`|
|`Ambient`|
|`Chassis`|
|`Bridge Board`|
|`Exhaust`|
|`Processor Bay`|
|`IO Bay`|
|`Blade Slot`|
|`Virtual`|
### Fans[array-item].Oem.Hpe.Redundant

Indicates if the fan is in a redundant configuration.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### Fans[array-item].PhysicalContext


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`Fans[]/PhysicalContext` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Room`|
|`Intake`|
|`Exhaust`|
|`Front`|
|`Back`|
|`Upper`|
|`Lower`|
|`CPU`|
|`GPU`|
|`Backplane`|
|`SystemBoard`|
|`PowerSupply`|
|`VoltageRegulator`|
|`StorageDevice`|
|`NetworkingDevice`|
|`ComputeBay`|
|`StorageBay`|
|`NetworkBay`|
|`ExpansionBay`|
|`PowerSupplyBay`|
### Fans[array-item].Reading

The current speed of the fan.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Fans[array-item].ReadingUnits

Units for the CurrentReading.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Fans[]/ReadingUnits` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`Percent`|
### Fans[array-item].Status.Health

This represents the health state of this resource in the absence of its dependent resources.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Fans[]/Status/Health` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`OK`|
|`Warning`|
|`Critical`|
### Fans[array-item].Status.HealthRollup

This represents the overall health state from the view of this resource.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Fans[]/Status/HealthRollup` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`OK`|
|`Warning`|
|`Critical`|
### Fans[array-item].Status.State

This indicates the known state of the resource, such as if it is enabled.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Fans[]/Status/State` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`Enabled`|
|`Disabled`|
|`Offline`|
|`InTest`|
|`Starting`|
|`Absent`|
### Fans[array-item].UpperThresholdCritical

Above normal range but not yet fatal.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Fans[array-item].UpperThresholdFatal

Above normal range and is fatal.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Fans[array-item].UpperThresholdNonCritical

Above normal range.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Oem.Hpe.FanPercentAdjust

System-wide setting for fan +/- percentage adjustment.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Oem": {"Hpe": {"FanPercentAdjust": &lt;integer-value&gt;}}}

### Status.Health

This represents the health state of this resource in the absence of its dependent resources.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Status/Health` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`OK`|
|`Warning`|
|`Critical`|
### Status.HealthRollup

This represents the overall health state from the view of this resource.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Status/HealthRollup` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`OK`|
|`Warning`|
|`Critical`|
### Status.State

This indicates the known state of the resource, such as if it is enabled.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Status/State` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`Enabled`|
|`Disabled`|
|`Offline`|
|`InTest`|
|`Starting`|
|`Absent`|
### Temperatures[array-item].CorrelatableID

The CorrelatableID for this temperature sensor.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Temperatures[array-item].LowerThresholdCritical

Below normal range but not yet fatal.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Temperatures[array-item].LowerThresholdFatal

Below normal range and is fatal.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Temperatures[array-item].LowerThresholdNonCritical

Below normal range.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Temperatures[array-item].MaximumValue

Maximum value for CurrentReading.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Temperatures[array-item].MinimumValue

Minimum value for CurrentReading.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Temperatures[array-item].Oem.Hpe.LocationXmm

The location of the sensor, in millimeters, along the X axis from the logical reference point.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Temperatures[array-item].Oem.Hpe.LocationYmm

The location of the sensor, in millimeters, along the Y axis from the logical reference point.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Temperatures[array-item].Oem.Hpe.LocationZmm

The location of the sensor, in millimeters, along the Z axis from the logical reference point.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Temperatures[array-item].PhysicalContext


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`Temperatures[]/PhysicalContext` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Room`|
|`Intake`|
|`Exhaust`|
|`Front`|
|`Back`|
|`Upper`|
|`Lower`|
|`CPU`|
|`GPU`|
|`Backplane`|
|`SystemBoard`|
|`PowerSupply`|
|`VoltageRegulator`|
|`StorageDevice`|
|`NetworkingDevice`|
|`ComputeBay`|
|`StorageBay`|
|`NetworkBay`|
|`ExpansionBay`|
|`PowerSupplyBay`|
### Temperatures[array-item].ReadingCelsius

The current reading of the temperature sensor.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Temperatures[array-item].SensorNumber

A numerical identifier to represent the temperature sensor.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Temperatures[array-item].Status.Health

This represents the health state of this resource in the absence of its dependent resources.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Temperatures[]/Status/Health` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`OK`|
|`Warning`|
|`Critical`|
### Temperatures[array-item].Status.HealthRollup

This represents the overall health state from the view of this resource.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Temperatures[]/Status/HealthRollup` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`OK`|
|`Warning`|
|`Critical`|
### Temperatures[array-item].Status.State

This indicates the known state of the resource, such as if it is enabled.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Temperatures[]/Status/State` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`Enabled`|
|`Disabled`|
|`Offline`|
|`InTest`|
|`Starting`|
|`Absent`|
### Temperatures[array-item].UpperThresholdCritical

Above normal range but not yet fatal.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Temperatures[array-item].UpperThresholdFatal

Above normal range and is fatal.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Temperatures[array-item].UpperThresholdNonCritical

The noncritical temperature threshold.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
## UpdateService
```@odata.type: "#UpdateService.v1_1_0.UpdateService"```

> **Resource Instances of this Type**:  

> * `https://{iLO}/redfish/v1/updateservice/`

### HttpPushUri

The URI to which a client may POST an update image.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.CurrentTime

ISO 8601 Redfish-style time string of the current iLO time (the reference for all scheduling)


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.FirmwareIntegrity.EnableBackgroundScan

Enables or disables background scan of critical firmware.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Oem": {"Hpe": {"FirmwareIntegrity": {"EnableBackgroundScan": true}}}}

### Oem.Hpe.FirmwareIntegrity.LastFailedImageUri

This is a link to the binary image of the firmware that failed an integrity check and is intended for diagnostic purposes.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.FirmwareIntegrity.LastScanResult

The firmware integrity scan engine status.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Oem/Hpe/FirmwareIntegrity/LastScanResult` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`OK`|
|`Repaired`|
|`Failure`|
|`Stopped`|
### Oem.Hpe.FirmwareIntegrity.LastScanTime

The time stamp of the last firmware integrity scan.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.FirmwareIntegrity.OnIntegrityFailure

Sets the policy for how the firmware integrity check handles integrity failures.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Oem": {"Hpe": {"FirmwareIntegrity": {"OnIntegrityFailure": "LogAndRepairAutomatically"}}}}

`Oem/Hpe/FirmwareIntegrity/OnIntegrityFailure` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`LogOnly`|
|`LogAndRepairAutomatically`|
### Oem.Hpe.FirmwareIntegrity.ScanEveryDays

Sets the interval between firmware integrity scans in 24 hour increments.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Oem": {"Hpe": {"FirmwareIntegrity": {"ScanEveryDays": &lt;integer-value&gt;}}}}

### Oem.Hpe.FlashProgressPercent

This is the percent complete for an iLO flash operation.  It is only valid when State is Updating.


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|No (read only)
### Oem.Hpe.Result.MessageId

The key for this message that can be used to look up the message in a message registry.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Oem": {"Hpe": {"Result": {"MessageId": "&lt;string-value&gt;"}}}}

### Oem.Hpe.State


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Oem/Hpe/State` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`Idle`|
|`Uploading`|
|`Verifying`|
|`Writing`|
|`Updating`|
|`Complete`|
|`Error`|
### Oem.Hpe.UploadCurrentEtag

client-supplied etag (during component upload) indicating to what UploadStatus is reporting upon.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.actions.actions.HpeiLOUpdateServiceExt.AddFromUri.Action


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Oem/Hpe/actions/actions/HpeiLOUpdateServiceExt.AddFromUri/Action` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`HpeiLOUpdateServiceExt.AddFromUri`|
### Oem.Hpe.actions.actions.HpeiLOUpdateServiceExt.AddFromUri.CompSigURI


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.actions.actions.HpeiLOUpdateServiceExt.AddFromUri.ImageURI


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Oem.Hpe.actions.actions.HpeiLOUpdateServiceExt.AddFromUri.TPMOverrideFlag


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### Oem.Hpe.actions.actions.HpeiLOUpdateServiceExt.AddFromUri.UpdateRepository


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### Oem.Hpe.actions.actions.HpeiLOUpdateServiceExt.AddFromUri.UpdateTarget


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### Oem.Hpe.actions.actions.HpeiLOUpdateServiceExt.AddFromUri.UploadCurrentEtag

client-supplied etag (during component upload) indicating to what UploadStatus is reporting upon.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Oem": {"Hpe": {"actions": {"actions": {"HpeiLOUpdateServiceExt.AddFromUri": {"UploadCurrentEtag": "&lt;string-value&gt;"}}}}}}

### Oem.Hpe.actions.actions.HpeiLOUpdateServiceExt.StartFirmwareIntegrityCheck.Action


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Oem/Hpe/actions/actions/HpeiLOUpdateServiceExt.StartFirmwareIntegrityCheck/Action` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`HpeiLOUpdateServiceExt.StartFirmwareIntegrityCheck`|
### ServiceEnabled

Indicates if the Update Service is enabled.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### POST Action "UpdateService.SimpleUpdate"

Parameters:

"**ImageURI**" (string) with the value **"<uri>"**

"**TransferProtocol**" (string) with one of the following value(s):

* CIFS
* FTP
* HTTP
* HTTPS
* NSF
* SCP
* TFTP
* OEM

> example "UpdateService.SimpleUpdate" action:

```
POST <target-uri>
Content-Type: application/json
OData-Version: 4.0

{
    "ImageURI": "<uri>", 
    "TransferProtocol": "CIFS"
}
```

## VirtualMedia
```@odata.type: "#VirtualMedia.v1_0_0.VirtualMedia"```

This is the schema definition for the Virtual Media service.

> **Resource Instances of this Type**:  

> * `https://{iLO}/redfish/v1/managers/{item}/virtualmedia/{item}/`

### ConnectedVia

Specifies how the virtual media is connected to the server.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`ConnectedVia` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`NotConnected`|
|`URI`|
|`Applet`|
### Image

The valid URI indicating the image that is mounted on this server. A null value indicates that no image exists.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Image": "&lt;string-value&gt;"}

### ImageName

The name of the image that is mounted on this server. This is usually provided when a URL image is mounted through scripted virtual media.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|No (read only)
### Inserted

Indicates whether the virtual media is mounted on the server.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
### Oem.Hpe.BootOnNextServerReset

If set to true, the server will boot to this image on the next server reboot. The image will be ejected automatically on the second server reboot so that the server does not boot to this image twice.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Oem": {"Hpe": {"BootOnNextServerReset": true}}}

### Oem.Hpe.actions.actions.HpeiLOVirtualMedia.EjectVirtualMedia.Action


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`Oem/Hpe/actions/actions/HpeiLOVirtualMedia.EjectVirtualMedia/Action` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`HpeiLOVirtualMedia.EjectVirtualMedia`|
### Oem.Hpe.actions.actions.HpeiLOVirtualMedia.EjectVirtualMedia.Intent

A text description of the reason for this action invocation.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Oem": {"Hpe": {"actions": {"actions": {"HpeiLOVirtualMedia.EjectVirtualMedia": {"Intent": "&lt;string-value&gt;"}}}}}}

### Oem.Hpe.actions.actions.HpeiLOVirtualMedia.EjectVirtualMedia.Signature

A RSA2048 SHA-256 signature validating the provided Intent (Base64 encoded).


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Oem": {"Hpe": {"actions": {"actions": {"HpeiLOVirtualMedia.EjectVirtualMedia": {"Signature": "&lt;string-value&gt;"}}}}}}

### Oem.Hpe.actions.actions.HpeiLOVirtualMedia.InsertVirtualMedia.Action


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`Oem/Hpe/actions/actions/HpeiLOVirtualMedia.InsertVirtualMedia/Action` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`HpeiLOVirtualMedia.InsertVirtualMedia`|
### Oem.Hpe.actions.actions.HpeiLOVirtualMedia.InsertVirtualMedia.Image

A URL for an ISO, BIN, or IMG file locating the virtual media image.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Oem": {"Hpe": {"actions": {"actions": {"HpeiLOVirtualMedia.InsertVirtualMedia": {"Image": "&lt;string-value&gt;"}}}}}}

### Oem.Hpe.actions.actions.HpeiLOVirtualMedia.InsertVirtualMedia.Intent

A text description of the reason for this action invocation.


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Oem": {"Hpe": {"actions": {"actions": {"HpeiLOVirtualMedia.InsertVirtualMedia": {"Intent": "&lt;string-value&gt;"}}}}}}

### Oem.Hpe.actions.actions.HpeiLOVirtualMedia.InsertVirtualMedia.Signature

A RSA2048 SHA-256 signature validating the provided Intent (Base64 encoded).


| | |
|---|---|
|JSON type|string|
|HTTP PATCH|Yes (if resource allows PATCH)
> example PATCH: {"Oem": {"Hpe": {"actions": {"actions": {"HpeiLOVirtualMedia.InsertVirtualMedia": {"Signature": "&lt;string-value&gt;"}}}}}}

### WriteProtected

Indicates whether the virtual media is protected against write operations.


| | |
|---|---|
|JSON type|boolean|
|HTTP PATCH|No (read only)
## Volume
```@odata.type: "#Volume.v1_0_0.Volume"```

> **Resource Instances of this Type**:  

> * `https://{iLO}/redfish/v1/systems/{item}/storage/{item}/volumes/{item}/`

### CapacityBytes

The size in bytes of this Volume


| | |
|---|---|
|JSON type|integer|
|HTTP PATCH|Yes (if resource allows PATCH)
### Status.Health

This represents the health state of this resource in the absence of its dependent resources.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Status/Health` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`OK`|
|`Warning`|
|`Critical`|
### Status.HealthRollup

This represents the overall health state from the view of this resource.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Status/HealthRollup` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`OK`|
|`Warning`|
|`Critical`|
### Status.State

This indicates the known state of the resource, such as if it is enabled.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|No (read only)
`Status/State` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`null`|the value is temporarily unavailable
|`Enabled`|
|`Disabled`|
|`Offline`|
|`InTest`|
|`Starting`|
|`Absent`|
### VolumeType

The type of this volume.


| | |
|---|---|
|JSON type|enumeration|
|HTTP PATCH|Yes (if resource allows PATCH)
`VolumeType` can take one of the following values (note the some implementations may support a subset of these):

|Value| |
|---|---|
|`RawDevice`|
