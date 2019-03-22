# Example Use Cases

NOTE:  The examples in this section use a pseudo-code syntax for clarity. JSON pointer syntax is used to indicate specific properties.

## Reading BIOS Current Settings
<blockquote class="lang-specific python">
    <a href="https://github.com/HewlettPackard/python-ilorest-library/blob/master/examples/Rest/restobject.py">RestObject source code</a>
</blockquote>

```shell
curl https://{iLO}/rest/v1/systems/1/bios/settings -i --insecure -u username:password -L
```

```python
import sys
from restobject import RestObject

# When running remotely connect using the iLO address, iLO account name, 
# and password to send https requests
iLO_host = "https://{iLO}"
iLO_account = "admin"
iLO_password = "password"

#Create a REST object
REST_OBJ = RestObject(iLO_host, iLO_account, iLO_password)
instances = REST_OBJ.search_for_type("HpBios.")

for instance in instances:
	response = REST_OBJ.rest_get(instance["href"])
	print response
```

> Response

```json
{
	"AcpiRootBridgePxm": "Enabled",
	"AcpiSlit": "Enabled",
	"AdjSecPrefetch": "Enabled",
	"AdminEmail": "",
	"AdminName": "",
	...
	
	...
	"WakeOnLan": "Enabled",
	"links": {
		"self": {
			"href": "/rest/v1/systems/1/bios/Settings"
		}
	}
}
```

To GET the current BIOS configuration:

The iLO RESTful API enables UEFI BIOS configuration. The link to the BIOS configuration is from the computer system object.

## Changing Pending Settings and understanding "SettingsResults"
The current configuration object for BIOS is read only. This object contains a link to a Settings resource that you can perform a PATCH operation on.  This is the "pending settings." If you GET the Settings resource, you will see that it allows PATCH commands. You can change properties and then PATCH them back to the Settings URI. Changes to pending settings do not take effect until the server is reset. Before the server is reset, the current and pending settings are independently available. After the server is reset, the pending settings are applied and you can view any errors in the SettingsResults property on the main object.

There are benefits to handling BIOS settings in this way:

* Enables offline components (for example, BIOS) to process changes to settings in a deferred
manner.
* Allows current and pending values to remain available for review until the offline component
processes the pending settings.
* Avoids the need for complex job queues.

### Updating the BIOS settings example
```shell
curl -H "Content-Type: application/json" -X PATCH --data "@data.json" https://{iLO}/rest/v1/Systems/1/bios/settings -u username:password --insecure
```

<blockquote class="lang-specific shell">
	<p>Contents of data.json</p>
    <p>{"AdminName": "NewName"}</p>
</blockquote>

<blockquote class="lang-specific python">
    <b>For a full Redfish example click here: <a href="https://github.com/HewlettPackard/python-ilorest-library/blob/master/examples/Redfish/ex03_change_bios_setting.py">ex03_change_bios_setting.py</a></b>
	</br></br>
    <b>For a full Rest example click here: <a href="https://github.com/HewlettPackard/python-ilorest-library/blob/master/examples/Rest/ex03_change_bios_setting.py">ex03_change_bios_setting.py</a></b>
</blockquote>
The minimum required session ID privileges is `Configure.`

1. Iterate through `/rest/v1/Systems` and choose a member ComputerSystem. 
Result = `{ilo-ip-address}/rest/v1/Systems/1/BIOS`
2. Find a link in the `Oem/Hp/links` called `Bios` and note the `BiosURI`.
3. `GET BiosObj` from `BiosURI` and note that it only allows `GET` (this is the current settings).
4. Find a link in `BiosObj` called `Settings` and note this URI.
5. Obtain the BIOS settings using the URI from step 4.
  * `GET {ilo-ip-address}/rest/v1/Systems/1/BIOS/Settings`
6. Create a new JSON object with the `AdminName` property changed to `{"AdminName":"Joe
Smith"}`.
7. Update the BIOS settings. You only need to send the updated `AdminName` property in the
request body.
  * `PATCH {ilo-ip-address}/rest/v1/Systems/1/BIOS/Settings`
8. Obtain the BIOS settings to verify you made the change to the AdminName property.
  * `GET {ilo-ip-address}/rest/v1/Systems/1/BIOS/Settings`
When the server is reset, the BIOS settings are validated and adopted.


## Reading BIOS Defaults example
```shell
curl https://{iLO}/rest/v1/systems/1/bios/BaseConfigs/ -i --insecure -u username:password -L
```

```python
import sys
import ilorest

# When running remotely connect using the iLO address, iLO account name, 
# and password to send https requests
iLO_host = "https://{iLO}"
login_account = "admin"
login_password = "password"

## Create a REDFISH object
REDFISH_OBJ = ilorest.redfish_client(base_url=iLO_host,username=login_account, \
                          password=login_password, default_prefix='/redfish/v1')

# Login into the server and create a session
REDFISH_OBJ.login(auth="session")

# Do a GET on a given path
response = REDFISH_OBJ.get("/rest/v1/systems/1/bios/BaseConfigs/", None)

# Print out the response
sys.stdout.write("%s\n" % response)

# Logout of the current session
REDFISH_OBJ.logout()
```

The results looks something like this:

>Response

```json
{
	"BaseConfigs": [{
		"default": {
			"AcpiRootBridgePxm": "Enabled",
			"AcpiSlit": "Enabled",
			...
			
			...
			"VlanPriority": 0,
			"WakeOnLan": "Enabled"
		}
	}],
	"Capabilities": {
		"BaseConfig": true,
		"BaseConfigs": false
	},
	"Modified": "2016-04-21T01:52:17+00:00",
	"Name": "BIOS Default Settings",
	"Type": "HpBaseConfigs.0.10.0",
	"links": {
		"self": {
			"href": "/rest/v1/systems/1/bios/BaseConfigs"
		}
	}
}
```

The BIOS current configuration object contains a link to a separate read-only object, the `BaseConfigs`, which list the BIOS default settings. To get the BIOS `BaseConfigs` resource:

Notice that `BaseConfigs` contains an array of default sets (or base configuration sets). Each base config set contains a list of BIOS properties and their default values. The default base config set contains the BIOS manufacturing defaults. It is possible for `BaseConfigs` to contain other sets, like `default.user` for user custom defaults.

### BIOS resources and attribute registry overview
The BIOS resources are formatted differently than most other resources. BIOS resources do conform to a schema type as all objects do. However, BIOS settings vary widely across server types and BIOS revisions, so it is  extremely difficult to publish a standard schema defining all the possible BIOS setting properties. Furthermore, it is not possible to communicate some of the advanced settings such as inter-setting dependencies, and menu structure in json-schema. Therefore, BIOS uses an *Attribute Registry.*

### Attribute registry
The BIOS Current Configuration resource has a property called `AttributeRegistry`. This property indicates the name and version of a registry file that defines the properties in the BIOS configuration.  It also includes information about interdependencies between settings.

Due to their size, BIOS Attribute Registries are compressed JSON resources (gzip), so the returned HTTP headers indicate a content-encoding of `gzip.` The REST client will need to decompress the resource. This is done automatically in many web clients (like the Postman
plugin).

### BIOS attribute registry structure
The BIOS attribute registries contains three top-level arrays:

- **Menus:** Array containing the BIOS attributes menus and their hierarchy. This can be used
(for instance) to build a user interface that resembles the local BIOS Setup, or to group
properties that are related such as `ProcessorOptions` and `UsbOptions.`
- **Dependencies:** Array containing a list of dependencies of BIOS attributes on this server.
This includes inter-setting dependencies that might cause one BIOS setting to change its
value or its `ReadOnly` property based on the value of another BIOS setting.
- **BaseConfigs:** Array containing a list of default manufacturing settings of BIOS attributes.
This is equivalent to reading the BaseConfigs resource and parsing the object named
`default.`

### BIOS attributes
Each BIOS attribute in the attribute registry includes:

- Type of each BIOS attribute (enum, string, numeric, or Boolean).
- Possible values for enum type attributes.
- Display strings (localized to the registry language) for the attributes and their possible values.
- Help text and warning text (localized).
- Location and display order information, including menu hierarchy for an attribute.
BIOS 25
- Value limits, including maximum, minimum, and step values for numeric attributes, and
minimum and maximum character lengths, as well as regular expressions for string attributes.
- And other meta-data.

## Setting or Changing the BIOS Administrator and Setup Password
```shell
curl -H "Content-Type: application/json" -X PATCH --data "@data.json" https://{iLO}/rest/v1/Systems/1/bios/settings -u username:password --insecure
```

<blockquote class="lang-specific shell">
	<p>Contents of data.json</p>
    <p>{"OldAdminPassword": "oldpassword", "AdminPassword": "newpassword"}</p>
</blockquote>

<blockquote class="lang-specific python">
    <b>For a full Redfish example click here: <a href="https://github.com/HewlettPackard/python-ilorest-library/blob/master/examples/Redfish/ex03_change_bios_setting.py">ex03_change_bios_setting.py</a></b>
	</br></br>
    <b>For a full Rest example click here: <a href="https://github.com/HewlettPackard/python-ilorest-library/blob/master/examples/Rest/ex03_change_bios_setting.py">ex03_change_bios_setting.py</a></b>
</blockquote>

To change the Administrator and Power On passwords, you must change two properties for each password in the Pending Settings resource:
* **Administrator password**: Set `AdminPassword` to the new password and `OldAdminPassword` to the old password.
* **Power On password**: Set `PowerOnPassword` to the new password and
`OldPowerOnPassword` with the old password.

If you the old password is not set, you must use a blank string ("") for the old password property.

1. Iterate through `/redfish/v1/Systems` and choose a member ComputerSystem.
  * Result = `{ilo-ip-address}/redfish/v1/Systems/1/BIOS`
2. Find a link in the `Oem/Hp/links` called `Bios` and note the `BiosURI`.
3. `GET BiosObj` from `BiosURI` and note that it only allows `GET` (this is the current settings).
4. Find a link in `BiosObj` called `Settings` and note this URI.
5. Create a new JSON object with the `AdminPassword` and `OldAdminPassword` property
changed to `{"AdminPassword":"@Pa$$w0rd", "OldAdminPassword":""}.`
6. Update the BIOS settings. You only need to send the updated `AdminName` property in the
request body.
  * `PATCH {ilo-ip-address}/rest/v1/Systems/1/BIOS/Settings`

When the server is reset, the BIOS settings are validated and adopted.

## Updating the Administrator BIOS password example
```shell
curl -H "Content-Type: application/json" -H "X-HPRESTFULAPI-AuthToken: <hash of password>" -X PATCH --data "@data.json" https://{iLO}/rest/v1/Systems/1/bios/settings -u username:password --insecure
```

<blockquote class="lang-specific shell">
	<p>Contents of data.json</p>
    <p>{"OldAdminPassword": "oldpassword", "AdminPassword": "newpassword"}</p>
</blockquote>

<blockquote class="lang-specific python">
    <b>For a full Redfish example click here: <a href="https://github.com/HewlettPackard/python-ilorest-library/blob/master/examples/Redfish/ex03_change_bios_setting.py">ex03_change_bios_setting.py</a></b>
	</br></br>
    <b>For a full Rest example click here: <a href="https://github.com/HewlettPackard/python-ilorest-library/blob/master/examples/Rest/ex03_change_bios_setting.py">ex03_change_bios_setting.py</a></b>
</blockquote>
To change the Administrator and Power On passwords, you must change two properties for each password:

| HTTP Header Name | Value |
| ------------- | ------------- |
| `X-HPRESTFULAPI-AuthToken` | A string consisting of the uppercase SHA256 hex digest of the administrator password. In Python this is `hashlib.sha256(bios_password.encode()).hexdigest().upper().` |


## Example reset all BIOS and boot order settings to factory defaults
1. Iterate through `/rest/v1/Systems` and choose a member `ComputerSystem.` Find a child resource of type
`HpBios` that allows `PATCH` operations (there might be more than one but for this exercise, just choose the first
one).
  * `{ilo-ip-address}/rest/v1/Systems/1/BIOS/Settings`
2. Obtain the BIOS and boot order settings.
  * `GET {ilo-ip-address}/rest/v1/Systems/1/BIOS`
3. Create a new JSON object with the `RestoreManufacturingDefaults` property and change the value to yes.
4. Reset the BIOS and boot order settings. You only need to send the updated `RestoreManufacturingDefaults`
property in the request body.
  * `PATCH {ilo-ip-address}/rest/v1/Systems/1/BIOS`

### Reverting BIOS UEFI settings to default example
```shell
curl -H "Content-Type: application/json" -X POST --data "@data.json" https://{iLO}/rest/v1/Systems/1/bios/settings -u username:password --insecure
```

<blockquote class="lang-specific shell">
	<p>Contents of data.json</p>
    <p>{"BaseConfig": "default"}</p>
</blockquote>

<blockquote class="lang-specific python">
    <b>For a full Redfish example click here: <a href="https://github.com/HewlettPackard/python-ilorest-library/blob/master/examples/Redfish/ex06_bios_revert_default.py">ex06_bios_revert_default.py</a></b>
	</br></br>
    <b>For a full Rest example click here: <a href="https://github.com/HewlettPackard/python-ilorest-library/blob/master/examples/Rest/ex06_bios_revert_default.py">ex06_bios_revert_default.py</a></b>
</blockquote>
The BIOS Settings resource supports a special feature that allows you to revert BIOS settings
to default for the selected resource. This is accomplished by performing the PATCH or PUT
operation on a special property in the BIOS settings object: {"BaseConfig": "default"}.
This can be combined with other property sets to first set default values and then set specific
settings all in one operation.

**NOTE:** The `BaseConfig` property might not already exist in the BIOS or BIOS Settings
resources. To determine if the BIOS resource supports reverting the settings to default, `GET` the
BIOS `BaseConfigs` resource, and view the `Capabilities` property.

1. Iterate through `/rest/v1/Systems` and choose a member `ComputerSystem`. Find a
child resource of type `HpBios` that allows `PUT` operations (there might be more than one
but for this exercise, just choose the first one).
  * `{ilo-ip-address}/rest/v1/Systems/1/BIOS/Settings`
2. Obtain the BIOS UEFI settings.
  * `GET {ilo-ip-address}/rest/v1/Systems/1/BIOS/Settings`
3. Change or add the BaseConfig property to `{"BaseConfig":"default"}` in the response
body.
4. Update the BIOS UEFI settings.
  * `PUT {ilo-ip-address}/rest/v1/Systems/1/BIOS/Settings`
When the sever is reset, the BIOS UEFI settings are reverted to default.

**NOTE:**

* You might also view the default values for BIOS settings by finding the resource type
`HpBaseConfigs.`
  * `{ilo-ip-address}/rest/v1/Systems/1/BIOS/BaseConfigs`
* `BaseConfig` can be combined with other property values to first reset everything to default
and then apply some specific settings in one operation.

## Enabling BIOS UEFI Secure Boot example
```shell
curl -H "Content-Type: application/json" -X PATCH --data "@data.json" https://{iLO}/rest/v1/Systems/1/SecureBoot -u username:password --insecure
```

<blockquote class="lang-specific shell">
	<p>Contents of data.json</p>
    <p>{"SecureBootEnable":true}</p>
</blockquote>

<blockquote class="lang-specific python">
    <b>For a full Redfish example click here: <a href="https://github.com/HewlettPackard/python-ilorest-library/blob/master/examples/Redfish/ex05_enable_secure_boot.py">ex05_enable_secure_boot.py</a></b>
	</br></br>
    <b>For a full Rest example click here: <a href="https://github.com/HewlettPackard/python-ilorest-library/blob/master/examples/Redfish/ex05_enable_secure_boot.py">ex05_enable_secure_boot.py</a></b>
</blockquote>
The minimum required session ID privileges is `Configure.`

1. Iterate through `/rest/v1/Systems` and choose a member ComputerSystem. Find a child
resource of type `HpSecureBoot` that allows `PATCH` operations (there might be more than
one but for this exercise, just choose the first one).
  * `{ilo-ip-address}/rest/v1/Systems/1/SecureBoot`
2. Obtain the secure boot settings.
  * `GET {ilo-ip-address}/rest/v1/Systems/1/SecureBoot`
3. Create a new JSON object with the `SecureBootEnable` property changed to
`{"SecureBootEnable":true}.`
4. Update the secure boot settings. You only need to send the updated `SecureBootEnable`
property in the request body.
  * `PATCH {ilo-ip-address}/rest/v1/Systems/1/SecureBoot`

When the sever is reset, the boot settings are validated and adopted.

## Example iSCSI Software Initiator configuration

>Existing example resource:

```json
{
    "iSCSIBootSources": [
        {
             "iSCSIBootAttemptInstance": 1,
             ...
        },
        {
             "iSCSIBootAttemptInstance": 2,
             ...
        },
        {
             "iSCSIBootAttemptInstance": 0,
             ...
        },
        {
             "iSCSIBootAttemptInstance": 0,
             ...
        }
    ],
    ...
}
```

```json
{
	"iSCSIBootSources": [
		{}, 
		{
			"iSCSIConnectRetry": 2
		}, 
		{
			"iSCSIBootAttemptInstance": 3,
			"iSCSIBootAttemptName": "Name",
			"iSCSINicSource": "NicBootX"
			...
		}, 
		{}
	]
}
```

The iSCSI Software Initiator allows you to configure an iSCSI target device to be used as a boot
source. The BIOS current configuration object contains a link to a separate resource of type
`HpiSCSISoftwareInitiator.` The BIOS current configuration resource and the iSCSI Software
Initiator current configuration resources are read-only. To change iSCSI settings, you need to
follow another link to the `Settings` resource, which allows `PUT` and `PATCH` operations.

The iSCSI target configurations are represented in an `iSCSIBootSources` property, that is an
array of objects, each containing the settings for a single target. The size of the array represents
the total number of iSCSI boot sources that can be configured at the same time. Many mutable
properties exist, including `iSCSIBootAttemptInstance,` which can be set to a unique integer
in the range [1, *N*], where N is the boot sources array size. By default, this *instance number* is 0
for all objects, indicating that the object should be ignored when configuring iSCSI.

Each object also contains two read-only properties—`StructuredBootString` and
`UEFIDevicePath`, which are only populated after the target has been successfully configured
as a boot source. More information about each property is available in the corresponding schema.
The iSCSI initiator name is represented by the `iSCSIInitiatorName` property.

An additional read-only property, `iSCSINicSources,` is only shown in the iSCSI current
configuration resource. This property is an array of strings representing the possible NIC instances
that can be used as targets for iSCSI boot configuration. To confirm which NIC device each string
corresponds to, it is recommended to cross-reference two other resources:

* A resource of type `HpBiosMapping` can be found through a `Mappings` link in the BIOS
current configurations resource. Within its `BiosPciSettingsMappings` property is an
array of mappings between BIOS-specific device strings (such as the `NIC` source string)
and a `CorrelatableID` string that can be used to refer to the same device in non-BIOS
contexts.
* A collection of `HpServerPciDevices` may be found through a PCIDevices link in the
`ComputerSystem` resource. The specific PCI device corresponding to the NIC instance
can be found by searching for the `CorrelatableID` that will usually match a
`UEFIDevicePath.` Once the `HpServerPciDevice` resource is found, you have access
to all the human-readable properties useful for describing a NIC source.

Changing the `iSCSIBootSources` and `iSCSIInitiatorName` settings can be done through
`PATCH` operations, very similar to how `HpBios` settings are changed. However, whereas all BIOS
settings are located in a single flat object, iSCSI settings are nested into arrays and sub-objects.
When doing a `PATCH` operation, use empty objects (`{}`) in place of those boot source objects
that you do not want to alter.

The following example covers a situation where you have configured two iSCSI boot sources,
and you would like to edit some existing settings, and add a third source.

1. Iterate through `/rest/v1/Systems` and choose a member `ComputerSystem.` Find a
child resource of type `HpiSCSISoftwareInitiator` that allows PATCH operations.
  * `{ilo-address}/rest/v1/Systems/1/BIOS/iSCSI/Settings`
2. Inspect the existing `iSCSIBootSources` array. You need to inspect the
`iSCSIBootAttemptInstance` property of each object to find the boot sources you are
prefer to change.

3. Create a new JSON object with the iSCSIBootSources property.
  *  Use an empty object in the position of instance 1 to indicate that it should not be modified.
Use an object in the position of instance 2 containing the properties that should be
modified—all omitted properties will remain unmodified.
  * To add a new boot source, find any position of instance 0 and replace it with an object
containing all the new settings, and most importantly, a new unique value of
iSCSIBootAttemptInstance.

4. Change the iSCSI software initiator settings.
  * `PATCH {ilo-address}/rest/v1/Systems/1/BIOS/iSCSI/Settings` 




## Changing Boot Settings
### UEFI boot structured name string
This UEFI boot structured name string is unique and represents each UEFI boot option in the
system. Software can identify and manipulate devices using the string’s fixed format as defined
in this specification. Software can assume that the string unique for each boot device in the UEFI
BootOrder.

The UEFI boot structured name string is divided into sections separated by ‘.’ characters, using
the following format:

*<DeviceType>.<Location>.<Instance>.<Sub-instance>.<Qualifier>*

* DeviceType: The first section describes the device type (For example, `HD,` `CD,` `NIC,` and
`PCI.`).
* **Location:** The second and the third section together describes the location of the device
(For example, `Slot.7` or `Emb.4`).
* **Instance:** The third section is used with the `Location` section to describe the device location
(for example, the slot number or embedded instance number).
* **Sub-instance:** The fourth section is optional, and is used as a sub-instance number in case
of multiple boot options using the same instance. For example, this can be the port number
for a multi-port NIC.
* **Qualifier:** The fifth section is optional, and describes the logical protocol (for example, IPv4,
IPv6, and iSCSI).

The Structured Boot String information is part of the `BootSources[]property` in the
`HpServerBootSettings` object and the `StructuredName` property in the
`HpServerPciDevice` object.

### UEFI boot structured name string examples
**Table 1 Examples**

        Name | Description
------------ | -------------
**HD.Emb.4.2** | The second instance of a hard drive in embedded SA controller bay 4
**NIC.Slot.7.2.IPv4** | Port 2 of a NIC in PCIe slot 7, which is enabled for PXE IPv4
**NIC.FlexLOM.1.1.IPv6** | Port 1 of an embedded NIC FlexLOM, which is enabled for PXE IPv6
**PCI.Slot.6.1** | PCIe card in slot 6
**HD.FrontUSB.2.2** | Second partition of a flash drive in front USB port 2


**Table 2 Examples of currently supported Structured Boot Strings** 

       Device Type | Location | Instance | Sub instance | Qualifier | Structure Boot String Examples 
------------ | ------------- | ------------- | ------------- | ------------- | -------------
Smart Array Hard Drive | Embedded | Bay number | Incremental by LUN |  | HD.Emb.1.1
                       | Slot | Slot number | Incremental by LUN |  | HD.Slot.1.1
Smart Arrary Controller | Embedded | Controller Instance | 1 |  | RAID.Emb.1.1
                       | Slot | Slot number | 1 |  | RAID.Slot.1.1
Dynamic Smart Array Controller (Software RAID) | Embedded | 1 | 1 |  | Storage.Emb.1.1
                       | Slot | Controller Instance | 1 |  | Storage.Slot.1.1
SATA Hard Drive | Embedded | SATA port # 1 |  |  | HD.Emb.1.1
SATA Controller | Embedded | Controller Instance | 1 |  | SATA.Emb.1.1
All other storage controllers (FC, SAS, etc…) | Embedded | 1 | 1 |  | Storage.Emb.1.1
         | Slot | Slot # | 1 |  | Storage.Slot.1.1
Network Adapter | LOM | NIC number, 1 for 1st NIC, 2 for 2nd NIC | Port number | IPv4 or IPv6 or iSCSI or FCoE | NIC.LOM.1.2.IPv4, NIC.LOM.1.2.IPv6
         | FlexibleLOM | FlexibleLOM number, 1 for 1st FlexLOM, 2 for 2nd FlexLOM | Port Number | IPv4 or IPv6 or iSCSI or FCoE | NIC.FlexLOM.2.1.IPv4, NIC.FlexLOM.2.1.IPv6
         | Slot | Slot Number | Port number | IPv4 or IPv6 or iSCSI or FCoE | NIC.Slot.3.2.Ipv4
Fiber Channel Adapter | Slot | Slot number | Port number | IPv4 or IPv6 or iSCSI or FCoE | PCI.Slot.3.1
OS Boot entry (such as Embedded HD.Slot.1.2 “Windows Boot Manager”) | Slot  | Embedded |  | Incremental | HD.Emb.1.2, HD.Slot.1.2
USB Key | Front USB | USB Port # | Incremental by LUN |  | HD.FrontUSB.1.1
        | Rear USB | USB Port # | Incremental by LUN |  | HD.RearUSB.1.1
        | Internal USB | USB Port # |  |  | HD.InternalUSB.1.1
        | iLO virtual media |  |  |  | HD.Virtual.1.1
ISO image | iLO virtual media |  |  |  | CD.Virtual.2.1
Virtual Install Disk (VID) | Embedded store | USB Port # |  |  | HD.VirtualUSB.1.1
Embedded User Partition | Embedded store | USB Port # |  |  | HD.VirtualUSB.2.1
USB CD/DVD | Front USB | USB Port # |  |  | CD.FrontUSB.1.1
           | Rear USB | USB Port # |  |  | CD.RearUSB.1.1
           | Internal USB | USB Port # |  |  | xxxxxxxx
SD card | SD slot | USB Port # |  |  | HD.SD.1.1
Floppy | Front USB, Rear USB | USB Port # |  |  | FD.FrontUSB.1.1, FD.RearUSB.1.1 
Embedded UEFI Shell | Embedded | 1 | 1 |  | Shell.Emb.1.1
UEFI applications (embedded in the ROM firmware) (Diag, System Utility, etc..) | Embedded | 1 | Incremental |  | App.Emb.1.1, App.Emb.1.2, App.Emb.1.3
File | URL | Different URL Increased by 1 | 1 |  | File.URL.1.1
HPE RAM Disk Device | RAM Memory | 1 | Port Number |  | RAMDisk.Emb.1.1
Special USB device class with Device Path: UsbClass(0xFFFF, 0xFFFF, 0xFF, 0xFF, 0xFF) | Any USB device in the system | 1 |  |  | Generic.USB.1.1
Empty slot, no device | Slot | Slot number | 1 |  | PCI.Slot.2.1
Unknown device | Embedded Slot Unknown location | Slot number or 1 | Incremental |  | Unknown.Slot.1.1, Unknown.Unknown.1.1 
NVMe | Slot | Slot number | NVMe drive number (The number is based on bus enumeration sequence). |  | NVMe.Slot.1.1
NVMe | Embedded | Bay number | 1 (Each drive bay has 1 NVMe drive.) |  | NVMe.Emb.1.1

### Change UEFI boot order example
<blockquote class="lang-specific shell">
	<p>For more information click on the python tab.</p>
</blockquote>

<blockquote class="lang-specific python">
    <b>For a full Redfish example click here: <a href="https://github.com/HewlettPackard/python-ilorest-library/blob/master/examples/Redfish/ex07_change_boot_order.py">ex07_change_boot_order.py</a></b>
	</br></br>
    <b>For a full Rest example click here: <a href="https://github.com/HewlettPackard/python-ilorest-library/blob/master/examples/Redfish/ex07_change_boot_order.py">ex07_change_boot_order.py</a></b>
</blockquote>
The BIOS current configuration object contains a link to a separate read-only resource of type
`HpServerBootSettings` that lists the UEFI Boot Order current configuration. This is the system
boot order when the system is configured in the UEFI Boot Mode. The UEFI Boot Order current
configuration resource contains a `BootSources` property, which is an array of UEFI boot sources.
Each object in that array has a unique `StructuredBootString,` among other properties that
identify that boot source.

The UEFI boot order list itself is represented in a separate `PersistentBootConfigOrder`
property that is an ordered array of boot sources, each referenced by its
`StructuredBootString.` In addition, a `DesiredBootDevices` property lists a separate
ordered list of desired boot sources that might not be listed in the `BootSources` property. This
is useful for configuring boot from a specific SCSI or FC LUN or iSCSI target that might have not
been configured (and discovered by BIOS) yet.

As with the BIOS current configuration resource, the UEFI Boot Order current configuration
resource is read only (as evident by the allow header, which do not list `PATCH` as an allowed
operation). To change the UEFI Boot Order, you need to follow the link to a separate Settings
resource that you can perform a `PATCH` operation on that contains the pending UEFI Boot Order
settings, and update that `PersistentBootConfigOrder` and/or the `DesiredBootDevices`
properties in that Settings resource. The settings remain pending until next reboot, and the results
are reflected back in the `SettingsResults` property in the UEFI Boot Order current configuration
resource.

**Prerequisites:** Minimum required session ID privileges: Configure

1. Iterate through `/rest/v1/Systems` and choose a member `ComputerSystem.` Find a child resource of type
`HpServerBootSettings` that allows `PATCH` operations (there might be more than one but for this exercise,
just choose the first one).
  * `{ilo-ip-address}/rest/v1/Systems/1/BIOS/Boot/Settings`
2. Obtain the UEFI boot order.
  * `GET {ilo-ip-address}/rest/v1/Systems/1/BIOS/Boot/Settings`
3. Create a new JSON object with the `PersistentBootConfigOrder` property and change the boot order.
4. Change the UEFI boot order. You only need to send the updated `PersistentBootConfigOrder` property in
the request body.
  * `PATCH {ilo-ip-address}/rest/v1/Systems/1/BIOS/Boot/Settings`

When the sever is reset, the new boot order is validated and used.
      
## Reset a Server
Server power control is a system-node-level entity, not a chassis-level control. For example, you
can turn on one node in a multi-node chassis. You control power by performing an HTTP operation
on a computer system node object.

Some operations in the interface are not truly RESTful `GET,` `PUT,` `POST,` `DELETE,` or `PATCH.` They
are called custom actions and are performed with an HTTP `POST` containing a specific request
payload. Typically, actions are defined when the action you want to perform is not adequately
represented by the properties available in the type. For example, a power button is not readable,
so you cannot `GET` the status of the power button. In this case, pressing the power button is an
action.

Actions are `POST` operations with an `Action` property that names the action to perform and zero
or more parameter properties.

### Reset a server example
```shell
curl -H "Content-Type: application/json" -X POST --data "@data.json" https://{iLO}/rest/v1/systems/1 -u username:password --insecure
```

<blockquote class="lang-specific shell">
	<p>Contents of data.json</p>
    <p>{"Action":"Reset"}</p>
</blockquote>

<blockquote class="lang-specific python">
    <b>For a full Redfish example click here: <a href="https://github.com/HewlettPackard/python-ilorest-library/blob/master/examples/Redfish/ex04_reset_server.py">ex04_reset_server.py</a></b>
	</br></br>
    <b>For a full Rest example click here: <a href="https://github.com/HewlettPackard/python-ilorest-library/blob/master/examples/Redfish/ex04_reset_server.py">ex04_reset_server.py</a></b>
</blockquote>
**Prerequisites** 

Minimum required session ID privileges: Configure

1. Iterate through `/rest/v1/Systems` and choose a member `ComputerSystem` that allows `POST` operations.
  * `{ilo-ip-address}/rest/v1/Systems/1`
2. Construct an Action object to submit to iLO.
  * `{"Action":"Reset","ResetType":"ForceRestart"}`
3. Change the `Action` and `ResetType` properties to `{"Action":"Reset","ResetType":"ForceRestart"}.`
4. Reset the server.
  * `POST {ilo-ip-address}/rest/v1/Systems/1`

The server resets and reboots.

## Download Active Health System Data
<blockquote class="lang-specific shell">
	<p>For more information click on the python tab.</p>
</blockquote>

<blockquote class="lang-specific python">
    <b>For a full Redfish example click here: <a href="https://github.com/HewlettPackard/python-ilorest-library/blob/master/examples/Redfish/ex46_get_ahs_data.py">ex46_get_ahs_data.py</a></b>
	</br></br>
    <b>For a full Rest example click here: <a href="https://github.com/HewlettPackard/python-ilorest-library/blob/master/examples/Rest/ex46_get_ahs_data.py">ex46_get_ahs_data.py</a></b>
</blockquote>

Active Health System (AHS) data may be accessed by first discovering the resource of type `HpiLOActiveHealthSystem`.  This is typically at `https://{iLO}/redfish/v1/managers/{item}/activehealthsystem`.  Refer to the section on Iterating Collections for details on how to navigate the data model.

1.  Iterate the Managers collection at `https://{iLO}/redfish/v1/managers/`.  For traditional iLO-based server architectures there is a single manager representing iLO 4 itself.

2.  Find the `Link` property referring to the `HpiLOActiveHealthSystem` and follow that link.

3.  GET the `HpiLOActiveHealthSystem` resource and look for the URI indicated by `Links.AHSLocation.extref`.

4.  Perform a GET to this URI with the following query parameters to define the download time range and embed customer case information:

* `from`:  the starting date of the download range (in YYYY-MM-DD format)
* `to`:    the ending date of the download range (in YYYY-MM-DD format)
* `case_no`:  case identification string
* `co_name`:  company or organization name
* `contact`:  contact name
* `email`:  contact email address
* `phone`:  contact phone number

If successful, the response is an HTTP 200 level status code and a binary download which can be saved to a file.

## Finding the iLO mac address
<blockquote class="lang-specific shell">
	<p>For more information click on the python tab.</p>
</blockquote>

<blockquote class="lang-specific python">
    <b>For a full Redfish example click here: <a href="https://github.com/HewlettPackard/python-ilorest-library/blob/master/examples/Redfish/ex09_find_ilo_mac_address.py">ex09_find_ilo_mac_address.py</a></b>
	</br></br>
    <b>For a full Rest example click here: <a href="https://github.com/HewlettPackard/python-ilorest-library/blob/master/examples/Rest/ex09_find_ilo_mac_address.py">ex09_find_ilo_mac_address.py</a></b>
</blockquote>
Before you search for the iLO mac address, you must create an instance of a `RestObject` or `RedfishObject`. The class constructor takes the iLO hostname/IP address, iLO login username, and password as arguments. The class also initializes a login session, gets systems resources, and message registries.

iLO implements two `EthernetInterface` resources under `/redfish/v1/managers/{item}/ethernetinterfaces`—the iLO dedicated network interface resource and the shared network interface resource. Only one resource can be enabled at a time. The shared network port has additional options under `SharedNetworkPortOptions`.  Clients should look for the `SharedNetworkPortOptions` property to identify the shared interface. The number or order of Ethernet interfaces might change in the future.

## Adding an iLO user account
<blockquote class="lang-specific shell">
	<p>For more information click on the python tab.</p>
</blockquote>

<blockquote class="lang-specific python">
    <b>For a full Redfish example click here: <a href="https://github.com/HewlettPackard/python-ilorest-library/blob/master/examples/Redfish/ex10_add_ilo_user_account.py">ex10_add_ilo_user_account.py</a></b>
	</br></br>
    <b>For a full Rest example click here: <a href="https://github.com/HewlettPackard/python-ilorest-library/blob/master/examples/Rest/ex10_add_ilo_user_account.py">ex10_add_ilo_user_account.py</a></b>
</blockquote>
Before you add an iLO user account, you must create an instance of a `RestObject` or `RedfishObject`. The class constructor takes the iLO hostname/IP address, iLO login username, and password as arguments. The class also initializes a login session, gets systems resources, and message registries.

## Setting a license key
```shell
curl -H "Content-Type: application/json" -X POST --data "@data.json" https://{iLO}/rest/v1/Managers/1/LicenseService -u username:password --insecure
```

<blockquote class="lang-specific shell">
	<p>Contents of data.json</p>
    <p>{"LicenseKey": "xxxxx-xxxxx-xxxxx-xxxxx-xxxxx"}</p>
</blockquote>

<blockquote class="lang-specific python">
    <b>For a full Redfish example click here: <a href="https://github.com/HewlettPackard/python-ilorest-library/blob/master/examples/Redfish/ex31_set_license_key.py">ex31_set_license_key.py</a></b>
	</br></br>
    <b>For a full Rest example click here: <a href="https://github.com/HewlettPackard/python-ilorest-library/blob/master/examples/Rest/ex31_set_license_key.py">ex31_set_license_key.py</a></b>
</blockquote>
Before you set a license key, you must create an instance of a `RestObject` or `RedfishObject`. The class constructor takes the iLO hostname/IP address, iLO login username, and password as arguments. The class also initializes a login session, gets systems resources, and message registries.




## Changing an iLO user account
<blockquote class="lang-specific shell">
	<p>For more information click on the python tab.</p>
</blockquote>

<blockquote class="lang-specific python">
    <b>For full Redfish examples click here: <a href="https://github.com/HewlettPackard/python-ilorest-library/blob/master/examples/Redfish/ex11_modify_ilo_user_account.py">ex11_modify_ilo_user_account.py</a>, <a href="https://github.com/HewlettPackard/python-ilorest-library/blob/master/examples/Redfish/ex12_remove_ilo_account.py ">ex12_remove_ilo_account.py</a></b>
	</br></br>
    <b>For full Rest examples click here: <a href="https://github.com/HewlettPackard/python-ilorest-library/blob/master/examples/Rest/ex11_modify_ilo_user_account.py">ex11_modify_ilo_user_account.py</a>, <a href="https://github.com/HewlettPackard/python-ilorest-library/blob/master/examples/Rest/ex12_remove_ilo_account.py">ex12_remove_ilo_account.py</a></b>
</blockquote>

Before you change an iLO user account, you must create an instance of a `RestObject` or `RedfishObject`. The class constructor takes the iLO hostname/IP address, iLO login username, and password as arguments. The class also initializes a login session, gets systems resources, and message registries.

## Enabling and Downloading Serial Over LAN Log
To obtain serial over LAN log information from iLO, you must enable the Virtual Serial Port (VSP) Download and the Serial Over LAN Logging features (SOL).

1. In the Manager resource (`/redfish/v1/managers/{item}`), use the PATCH operation to set `VSPLogDownloadEnabled` to true. `VSPLogDownloadEnabled` is in the OEM section of the Manager resource.
2. In the ManagerNetworkProtocol resource (`/redfish/v1/managers/{item}/networkservice`), use the PATCH operation to set `SerialOverLanLogging` to true. `SerialOverLanLogging` is in the OEM section of the Manager resource.
3. Wait until the log content is captured.
4. Find the URI of the serial over LAN binary download. This is called `VSPLogLocation` in the OEM section of the Manager resource (`/redfish/v1/managers/{item}`).
5. Perform the GET operation on the URI indicated to download the log (GZIP file).

