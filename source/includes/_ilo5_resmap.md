# Resource Map
|URI|Type|PATCH|POST|DELETE|
|:---|:---|:---:|:---:|:---:|
|`/redfish/v1/`|`ServiceRoot`|. |. |. 
|`/redfish/v1/accountservice/`|`AccountService`|X|. |. 
|`/redfish/v1/accountservice/accounts/`|`ManagerAccountCollection`|. |X|. 
|`/redfish/v1/accountservice/accounts/{item}/`|`ManagerAccount`|X|. |X
|`/redfish/v1/chassis/`|`ChassisCollection`|. |. |. 
|`/redfish/v1/chassis/{item}/`|`Chassis`|. |. |. 
|`/redfish/v1/chassis/{item}/drives/{item}/`|`Drive`|. |. |. 
|`/redfish/v1/chassis/{item}/power/`|`Power`|X|. |. 
|`/redfish/v1/chassis/{item}/power/fastpowermeter/`|`HpePowerMeter`|. |. |. 
|`/redfish/v1/chassis/{item}/power/federatedgroupcapping/`|`HpeiLOFederatedGroupCapping`|X|. |. 
|`/redfish/v1/chassis/{item}/power/powermeter/`|`HpePowerMeter`|. |. |. 
|`/redfish/v1/chassis/{item}/thermal/`|`Thermal`|. |. |. 
|`/redfish/v1/eventservice/`|`EventService`|. |X|. 
|`/redfish/v1/eventservice/eventsubscriptions/`|`EventDestinationCollection`|. |X|. 
|`/redfish/v1/managers/`|`ManagerCollection`|. |. |. 
|`/redfish/v1/managers/{item}/`|`Manager`|X|X|. 
|`/redfish/v1/managers/{item}/activehealthsystem/`|`HpeiLOActiveHealthSystem`|X|X|. 
|`/redfish/v1/managers/{item}/datetime/`|`HpeiLODateTime`|X|. |. 
|`/redfish/v1/managers/{item}/embeddedmedia/`|`HpeiLOEmbeddedMedia`|. |. |. 
|`/redfish/v1/managers/{item}/ethernetinterfaces/`|`EthernetInterfaceCollection`|. |. |. 
|`/redfish/v1/managers/{item}/ethernetinterfaces/{item}/`|`EthernetInterface`|X|. |. 
|`/redfish/v1/managers/{item}/federationgroups/`|`HpeiLOFederationGroupCollection`|. |X|. 
|`/redfish/v1/managers/{item}/federationgroups/{item}/`|`HpeiLOFederationGroup`|X|. |X
|`/redfish/v1/managers/{item}/federationpeers/`|`HpeiLOFederationPeersCollection`|. |. |. 
|`/redfish/v1/managers/{item}/federationpeers/{item}/`|`HpeiLOFederationPeers`|. |. |. 
|`/redfish/v1/managers/{item}/licenseservice/`|`HpeiLOLicenseCollection`|. |X|. 
|`/redfish/v1/managers/{item}/licenseservice/{item}/`|`HpeiLOLicense`|. |. |X
|`/redfish/v1/managers/{item}/logservices/`|`LogServiceCollection`|. |. |. 
|`/redfish/v1/managers/{item}/logservices/iel/`|`LogService`|. |X|. 
|`/redfish/v1/managers/{item}/logservices/iel/entries/`|`LogEntryCollection`|. |. |. 
|`/redfish/v1/managers/{item}/logservices/iel/entries/{item}/`|`LogEntry`|. |. |. 
|`/redfish/v1/managers/{item}/networkservice/`|`ManagerNetworkProtocol`|X|X|. 
|`/redfish/v1/managers/{item}/securityservice/`|`HpeSecurityService`|X|. |. 
|`/redfish/v1/managers/{item}/securityservice/certificateauthentication/`|`HpeCertAuth`|X|X|. 
|`/redfish/v1/managers/{item}/securityservice/eskm/`|`HpeESKM`|X|X|. 
|`/redfish/v1/managers/{item}/securityservice/httpscert/`|`HpeHttpsCert`|. |X|. 
|`/redfish/v1/managers/{item}/securityservice/sso/`|`HpeiLOSSO`|X|X|. 
|`/redfish/v1/managers/{item}/snmpservice/`|`HpeiLOSnmpService`|X|X|. 
|`/redfish/v1/managers/{item}/virtualmedia/`|`VirtualMediaCollection`|. |. |. 
|`/redfish/v1/managers/{item}/virtualmedia/{item}/`|`VirtualMedia`|X|X|. 
|`/redfish/v1/registries/`|`JsonSchemaFileCollection`|. |. |. 
|`/redfish/v1/registries/{item}/`|`JsonSchemaFile`|. |. |. 
|`/redfish/v1/resourcedirectory/`|`HpeiLOResourceDirectory`|. |. |. 
|`/redfish/v1/schemas/`|`JsonSchemaFileCollection`|. |. |. 
|`/redfish/v1/schemas/{item}/`|`JsonSchemaFile`|. |. |. 
|`/redfish/v1/sessionservice/`|`SessionService`|X|. |. 
|`/redfish/v1/sessionservice/sessions/`|`SessionCollection`|. |X|. 
|`/redfish/v1/sessionservice/sessions/{item}/`|`Session`|. |. |X
|`/redfish/v1/systems/`|`ComputerSystemCollection`|. |. |. 
|`/redfish/v1/systems/{item}/`|`ComputerSystem`|X|X|. 
|`/redfish/v1/systems/{item}/bios/`|`Bios`|. |. |. 
|`/redfish/v1/systems/{item}/bios/baseconfigs/`|`HpeBaseConfigs`|. |. |. 
|`/redfish/v1/systems/{item}/bios/boot/`|`HpeServerBootSettings`|. |. |. 
|`/redfish/v1/systems/{item}/bios/boot/baseconfigs/`|`HpeBaseConfigs`|. |. |. 
|`/redfish/v1/systems/{item}/bios/boot/settings/`|`HpeServerBootSettings`|X|. |. 
|`/redfish/v1/systems/{item}/bios/hpescalablepmem/`|`HpeScalablePmem`|. |. |. 
|`/redfish/v1/systems/{item}/bios/hpescalablepmem/settings/`|`HpeScalablePmem`|X|. |. 
|`/redfish/v1/systems/{item}/bios/iscsi/`|`HpeiSCSISoftwareInitiator`|. |. |. 
|`/redfish/v1/systems/{item}/bios/iscsi/baseconfigs/`|`HpeBaseConfigs`|. |. |. 
|`/redfish/v1/systems/{item}/bios/iscsi/settings/`|`HpeiSCSISoftwareInitiator`|X|. |. 
|`/redfish/v1/systems/{item}/bios/mappings/`|`HpeBiosMapping`|. |. |. 
|`/redfish/v1/systems/{item}/bios/settings/`|`Bios`|X|X|. 
|`/redfish/v1/systems/{item}/bios/tlsconfig/`|`HpeTlsConfig`|. |. |. 
|`/redfish/v1/systems/{item}/bios/tlsconfig/baseconfigs/`|`HpeBaseConfigs`|. |. |. 
|`/redfish/v1/systems/{item}/bios/tlsconfig/settings/`|`HpeTlsConfig`|X|. |. 
|`/redfish/v1/systems/{item}/logservices/`|`LogServiceCollection`|. |. |. 
|`/redfish/v1/systems/{item}/logservices/iml/`|`LogService`|. |X|. 
|`/redfish/v1/systems/{item}/logservices/iml/entries/`|`LogEntryCollection`|. |X|. 
|`/redfish/v1/systems/{item}/logservices/iml/entries/{item}/`|`LogEntry`|X|. |. 
|`/redfish/v1/systems/{item}/memory/`|`MemoryCollection`|. |. |. 
|`/redfish/v1/systems/{item}/memory/{item}/`|`Memory`|. |. |. 
|`/redfish/v1/systems/{item}/networkadapters/`|`HpeBaseNetworkAdapterCollection`|. |. |. 
|`/redfish/v1/systems/{item}/networkadapters/{item}/`|`HpeBaseNetworkAdapter`|. |. |. 
|`/redfish/v1/systems/{item}/pcidevices/`|`HpeServerPciDeviceCollection`|. |. |. 
|`/redfish/v1/systems/{item}/pcidevices/{item}/`|`HpeServerPciDevice`|. |. |. 
|`/redfish/v1/systems/{item}/pcislots/`|`HpeServerPCISlotCollection`|. |. |. 
|`/redfish/v1/systems/{item}/pcislots/{item}/`|`HpeServerPCISlot`|. |. |. 
|`/redfish/v1/systems/{item}/processors/`|`ProcessorCollection`|. |. |. 
|`/redfish/v1/systems/{item}/processors/{item}/`|`Processor`|. |. |. 
|`/redfish/v1/systems/{item}/secureboot/`|`SecureBoot`|X|X|. 
|`/redfish/v1/systems/{item}/smartstorage/`|`HpeSmartStorage`|. |. |. 
|`/redfish/v1/systems/{item}/smartstorage/arraycontrollers/`|`HpeSmartStorageArrayControllerCollection`|. |. |. 
|`/redfish/v1/systems/{item}/smartstorage/arraycontrollers/{item}/`|`HpeSmartStorageArrayController`|. |. |. 
|`/redfish/v1/systems/{item}/smartstorage/arraycontrollers/{item}/diskdrives/`|`HpeSmartStorageDiskDriveCollection`|. |. |. 
|`/redfish/v1/systems/{item}/smartstorage/arraycontrollers/{item}/diskdrives/{item}/`|`HpeSmartStorageDiskDrive`|. |. |. 
|`/redfish/v1/systems/{item}/smartstorage/arraycontrollers/{item}/logicaldrives/`|`HpeSmartStorageLogicalDriveCollection`|. |. |. 
|`/redfish/v1/systems/{item}/smartstorage/arraycontrollers/{item}/logicaldrives/{item}/`|`HpeSmartStorageLogicalDrive`|. |. |. 
|`/redfish/v1/systems/{item}/smartstorage/arraycontrollers/{item}/logicaldrives/{item}/datadrives/`|`HpeSmartStorageDiskDriveCollection`|. |. |. 
|`/redfish/v1/systems/{item}/smartstorage/arraycontrollers/{item}/storageenclosures/`|`HpeSmartStorageStorageEnclosureCollection`|. |. |. 
|`/redfish/v1/systems/{item}/smartstorage/arraycontrollers/{item}/storageenclosures/{item}/`|`HpeSmartStorageStorageEnclosure`|. |. |. 
|`/redfish/v1/systems/{item}/smartstorage/arraycontrollers/{item}/unconfigureddrives/`|`HpeSmartStorageDiskDriveCollection`|. |. |. 
|`/redfish/v1/systems/{item}/smartstorage/hostbusadapters/`|`HpeSmartStorageHostBusAdapterCollection`|. |. |. 
|`/redfish/v1/systems/{item}/smartstorage/hostbusadapters/{item}/`|`HpeSmartStorageHostBusAdapter`|. |. |. 
|`/redfish/v1/systems/{item}/smartstorage/hostbusadapters/{item}/diskdrives/`|`HpeSmartStorageDiskDriveCollection`|. |. |. 
|`/redfish/v1/systems/{item}/smartstorageconfig/`|`SmartStorageConfig`|. |. |. 
|`/redfish/v1/systems/{item}/smartstorageconfig/settings/`|`SmartStorageConfig`|X|. |. 
|`/redfish/v1/systems/{item}/storage/`|`StorageCollection`|. |. |. 
|`/redfish/v1/systems/{item}/storage/{item}/`|`Storage`|. |. |. 
|`/redfish/v1/systems/{item}/storage/{item}/volumes/{item}/`|`Volume`|. |. |. 
|`/redfish/v1/systems/{item}/usbports/`|`HpeUSBPortsCollection`|. |. |. 
|`/redfish/v1/systems/{item}/usbports/{item}/`|`HpeUSBPort`|. |. |. 
|`/redfish/v1/updateservice/`|`UpdateService`|X|X|. 
|`/redfish/v1/updateservice/componentrepository/`|`HpeComponentCollection`|. |. |. 
|`/redfish/v1/updateservice/componentrepository/{item}/`|`HpeComponent`|X|. |X
|`/redfish/v1/updateservice/firmwareinventory/`|`SoftwareInventoryCollection`|. |. |. 
|`/redfish/v1/updateservice/firmwareinventory/{item}/`|`SoftwareInventory`|. |. |. 
|`/redfish/v1/updateservice/installsets/`|`HpeComponentInstallSetCollection`|. |X|. 
|`/redfish/v1/updateservice/installsets/{item}/`|`HpeComponentInstallSet`|X|X|X
|`/redfish/v1/updateservice/softwareinventory/`|`SoftwareInventoryCollection`|. |. |. 
|`/redfish/v1/updateservice/softwareinventory/{item}/`|`SoftwareInventory`|. |. |. 
|`/redfish/v1/updateservice/updatetaskqueue/`|`HpeComponentUpdateTaskQueueCollection`|. |. |. 
|`/redfish/v1/updateservice/updatetaskqueue/{item}/`|`HpeComponentUpdateTask`|. |. |. 
