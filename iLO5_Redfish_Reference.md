# Resource Map
|URI|Type|
|:---|:---|
|`/redfish/v1/`|[ServiceRoot](#serviceroot-v1_1_0-serviceroot)|
|`/redfish/v1/accountservice/`|[AccountService](#accountservice-v1_0_2-accountservice)|
|`/redfish/v1/accountservice/accounts/`|Collection of [ManagerAccount](#manageraccount-v1_0_0-manageraccount)|
|`/redfish/v1/accountservice/accounts/{item}/`|[ManagerAccount](#manageraccount-v1_0_0-manageraccount)|
|`/redfish/v1/accountservice/usercertificatemapping/`|Collection of [HpeiLOAccountCertificateMap](#hpeiloaccountcertificatemap-v1_0_1-hpeiloaccountcertificatemap)|
|`/redfish/v1/accountservice/usercertificatemapping/{item}/`|[HpeiLOAccountCertificateMap](#hpeiloaccountcertificatemap-v1_0_1-hpeiloaccountcertificatemap)|
|`/redfish/v1/chassis/`|Collection of [Chassis](#chassis-v1_2_0-chassis)|
|`/redfish/v1/chassis/{item}/`|[Chassis](#chassis-v1_2_0-chassis)|
|`/redfish/v1/chassis/{item}/Power/accpowerservice/calibration/`|[HpeServerAccPowerCalibration](#hpeserveraccpowercalibration-v1_0_0-hpeserveraccpowercalibration)|
|`/redfish/v1/chassis/{item}/acchddservice/`|[HpeServerAccHddService](#hpeserveracchddservice-v1_0_0-hpeserveracchddservice)|
|`/redfish/v1/chassis/{item}/acchddservice/zone/`|[HpeServerAccHddZone](#hpeserveracchddzone-v1_0_0-hpeserveracchddzone)|
|`/redfish/v1/chassis/{item}/devices/`|Collection of [HpeServerDevice](#hpeserverdevice-v2_0_0-hpeserverdevice)|
|`/redfish/v1/chassis/{item}/devices/{item}/`|[HpeServerDevice](#hpeserverdevice-v2_0_0-hpeserverdevice)|
|`/redfish/v1/chassis/{item}/drives/{interface}/{item}/`|[Drive](#drive-v1_0_0-drive)|
|`/redfish/v1/chassis/{item}/networkadapters/`|Collection of [NetworkAdapter](#networkadapter-v1_0_1-networkadapter)|
|`/redfish/v1/chassis/{item}/networkadapters/{item}/`|[NetworkAdapter](#networkadapter-v1_0_1-networkadapter)|
|`/redfish/v1/chassis/{item}/networkadapters/{item}/Settings/`|[NetworkAdapter](#networkadapter-v1_0_1-networkadapter)|
|`/redfish/v1/chassis/{item}/networkadapters/{item}/networkdevicefunctions/`|Collection of [NetworkDeviceFunction](#networkdevicefunction-v1_1_0-networkdevicefunction)|
|`/redfish/v1/chassis/{item}/networkadapters/{item}/networkdevicefunctions/{item}/`|[NetworkDeviceFunction](#networkdevicefunction-v1_1_0-networkdevicefunction)|
|`/redfish/v1/chassis/{item}/networkadapters/{item}/networkdevicefunctions/{item}/settings/`|[NetworkDeviceFunction](#networkdevicefunction-v1_1_0-networkdevicefunction)|
|`/redfish/v1/chassis/{item}/networkadapters/{item}/networkports/`|Collection of [NetworkPort](#networkport-v1_1_0-networkport)|
|`/redfish/v1/chassis/{item}/networkadapters/{item}/networkports/{item}/`|[NetworkPort](#networkport-v1_1_0-networkport)|
|`/redfish/v1/chassis/{item}/networkadapters/{item}/networkports/{item}/hpeevb/`|[HpeNetworkPortEVB](#hpenetworkportevb-v1_0_0-hpenetworkportevb)|
|`/redfish/v1/chassis/{item}/networkadapters/{item}/networkports/{item}/hpelldp/`|[HpeNetworkPortLLDP](#hpenetworkportlldp-v1_0_0-hpenetworkportlldp)|
|`/redfish/v1/chassis/{item}/networkadapters/{item}/networkports/{item}/settings/`|[NetworkPort](#networkport-v1_1_0-networkport)|
|`/redfish/v1/chassis/{item}/power/`|[Power](#power-v1_2_1-power)|
|`/redfish/v1/chassis/{item}/power/accpowerservice/`|[HpeServerAccPowerService](#hpeserveraccpowerservice-v1_0_0-hpeserveraccpowerservice)|
|`/redfish/v1/chassis/{item}/power/accpowerservice/nodesinfo/`|[HpeServerAccPowerNodesInfo](#hpeserveraccpowernodesinfo-v1_0_0-hpeserveraccpowernodesinfo)|
|`/redfish/v1/chassis/{item}/power/accpowerservice/powerlimit/`|[HpeServerAccPowerLimit](#hpeserveraccpowerlimit-v1_0_0-hpeserveraccpowerlimit)|
|`/redfish/v1/chassis/{item}/power/accpowerservice/zone/`|[HpeServerAccPowerZone](#hpeserveraccpowerzone-v1_0_0-hpeserveraccpowerzone)|
|`/redfish/v1/chassis/{item}/power/fastpowermeter/`|[HpePowerMeter](#hpepowermeter-v2_0_0-hpepowermeter)|
|`/redfish/v1/chassis/{item}/power/federatedgroupcapping/`|[HpeiLOFederatedGroupCapping](#hpeilofederatedgroupcapping-v2_0_0-hpeilofederatedgroupcapping)|
|`/redfish/v1/chassis/{item}/power/powermeter/`|[HpePowerMeter](#hpepowermeter-v2_0_0-hpepowermeter)|
|`/redfish/v1/chassis/{item}/thermal/`|[Thermal](#thermal-v1_1_0-thermal)|
|`/redfish/v1/eventservice/`|[EventService](#eventservice-v1_0_1-eventservice)|
|`/redfish/v1/eventservice/cacertificates/`|Collection of [HpeCertificate](#hpecertificate-v1_0_0-hpecertificate)|
|`/redfish/v1/eventservice/cacertificates/{item}/`|[HpeCertificate](#hpecertificate-v1_0_0-hpecertificate)|
|`/redfish/v1/eventservice/eventsubscriptions/`|Collection of [EventDestination](#eventdestination-v1_0_0-eventdestination)|
|`/redfish/v1/eventservice/eventsubscriptions/{item}/`|[EventDestination](#eventdestination-v1_0_0-eventdestination)|
|`/redfish/v1/managers/`|Collection of [Manager](#manager-v1_1_0-manager)|
|`/redfish/v1/managers/{item}/`|[Manager](#manager-v1_1_0-manager)|
|`/redfish/v1/managers/{item}/activehealthsystem/`|[HpeiLOActiveHealthSystem](#hpeiloactivehealthsystem-v2_2_0-hpeiloactivehealthsystem)|
|`/redfish/v1/managers/{item}/backuprestoreservice/`|[HpeiLOBackupRestoreService](#hpeilobackuprestoreservice-v2_1_0-hpeilobackuprestoreservice)|
|`/redfish/v1/managers/{item}/datetime/`|[HpeiLODateTime](#hpeilodatetime-v2_0_0-hpeilodatetime)|
|`/redfish/v1/managers/{item}/embeddedmedia/`|[HpeiLOEmbeddedMedia](#hpeiloembeddedmedia-v2_0_0-hpeiloembeddedmedia)|
|`/redfish/v1/managers/{item}/ethernetinterfaces/`|Collection of [EthernetInterface](#ethernetinterface-v1_0_3-ethernetinterface)|
|`/redfish/v1/managers/{item}/ethernetinterfaces/{item}/`|[EthernetInterface](#ethernetinterface-v1_0_3-ethernetinterface)|
|`/redfish/v1/managers/{item}/federationgroups/`|Collection of [HpeiLOFederationGroup](#hpeilofederationgroup-v2_0_0-hpeilofederationgroup)|
|`/redfish/v1/managers/{item}/federationgroups/{item}/`|[HpeiLOFederationGroup](#hpeilofederationgroup-v2_0_0-hpeilofederationgroup)|
|`/redfish/v1/managers/{item}/federationpeers/`|Collection of [HpeiLOFederationPeers](#hpeilofederationpeers-v2_0_0-hpeilofederationpeers)|
|`/redfish/v1/managers/{item}/federationpeers/{item}/`|[HpeiLOFederationPeers](#hpeilofederationpeers-v2_0_0-hpeilofederationpeers)|
|`/redfish/v1/managers/{item}/licenseservice/`|Collection of [HpeiLOLicense](#hpeilolicense-v2_1_0-hpeilolicense)|
|`/redfish/v1/managers/{item}/licenseservice/{item}/`|[HpeiLOLicense](#hpeilolicense-v2_1_0-hpeilolicense)|
|`/redfish/v1/managers/{item}/logservices/`|Collection of [LogService](#logservice-v1_0_0-logservice)|
|`/redfish/v1/managers/{item}/logservices/iel/`|[LogService](#logservice-v1_0_0-logservice)|
|`/redfish/v1/managers/{item}/logservices/iel/entries/`|Collection of [LogEntry](#logentry-v1_0_0-logentry)|
|`/redfish/v1/managers/{item}/logservices/iel/entries/{item}/`|[LogEntry](#logentry-v1_0_0-logentry)|
|`/redfish/v1/managers/{item}/networkservice/`|[ManagerNetworkProtocol](#managernetworkprotocol-v1_0_0-managernetworkprotocol)|
|`/redfish/v1/managers/{item}/remotesupportservice/`|[HpeRemoteSupport](#hperemotesupport-v2_2_0-hperemotesupport)|
|`/redfish/v1/managers/{item}/remotesupportservice/serviceeventlogs/`|Collection of [LogEntry](#logentry-v1_0_0-logentry)|
|`/redfish/v1/managers/{item}/remotesupportservice/serviceeventlogs/{item}/`|[LogEntry](#logentry-v1_0_0-logentry)|
|`/redfish/v1/managers/{item}/securityservice/`|[HpeSecurityService](#hpesecurityservice-v2_2_0-hpesecurityservice)|
|`/redfish/v1/managers/{item}/securityservice/certificateauthentication/`|[HpeCertAuth](#hpecertauth-v1_1_0-hpecertauth)|
|`/redfish/v1/managers/{item}/securityservice/certificateauthentication/cacertificates/`|Collection of [HpeCertificate](#hpecertificate-v1_0_0-hpecertificate)|
|`/redfish/v1/managers/{item}/securityservice/certificateauthentication/cacertificates/{item}/`|[HpeCertificate](#hpecertificate-v1_0_0-hpecertificate)|
|`/redfish/v1/managers/{item}/securityservice/eskm/`|[HpeESKM](#hpeeskm-v2_0_0-hpeeskm)|
|`/redfish/v1/managers/{item}/securityservice/httpscert/`|[HpeHttpsCert](#hpehttpscert-v2_0_0-hpehttpscert)|
|`/redfish/v1/managers/{item}/securityservice/sso/`|[HpeiLOSSO](#hpeilosso-v2_0_0-hpeilosso)|
|`/redfish/v1/managers/{item}/snmpservice/`|[HpeiLOSnmpService](#hpeilosnmpservice-v2_1_0-hpeilosnmpservice)|
|`/redfish/v1/managers/{item}/snmpservice/snmpalertdestinations/`|Collection of [HpeSNMPAlertDestination](#hpesnmpalertdestination-v2_0_0-hpesnmpalertdestination)|
|`/redfish/v1/managers/{item}/snmpservice/snmpalertdestinations/{item}/`|[HpeSNMPAlertDestination](#hpesnmpalertdestination-v2_0_0-hpesnmpalertdestination)|
|`/redfish/v1/managers/{item}/snmpservice/snmpusers/`|Collection of [HpeSNMPUser](#hpesnmpuser-v2_0_0-hpesnmpuser)|
|`/redfish/v1/managers/{item}/snmpservice/snmpusers/{item}/`|[HpeSNMPUser](#hpesnmpuser-v2_0_0-hpesnmpuser)|
|`/redfish/v1/managers/{item}/virtualmedia/`|Collection of [VirtualMedia](#virtualmedia-v1_0_0-virtualmedia)|
|`/redfish/v1/managers/{item}/virtualmedia/{item}/`|[VirtualMedia](#virtualmedia-v1_0_0-virtualmedia)|
|`/redfish/v1/registries/`|Collection of [MessageRegistryFile](#messageregistryfile-v1_0_4-messageregistryfile)|
|`/redfish/v1/registries/{item}/`|[MessageRegistryFile](#messageregistryfile-v1_0_4-messageregistryfile)|
|`/redfish/v1/resourcedirectory/`|[HpeiLOResourceDirectory](#hpeiloresourcedirectory-v2_0_0-hpeiloresourcedirectory)|
|`/redfish/v1/schemas/`|Collection of [JsonSchemaFile](#jsonschemafile-v1_0_4-jsonschemafile)|
|`/redfish/v1/schemas/{item}/`|[JsonSchemaFile](#jsonschemafile-v1_0_4-jsonschemafile)|
|`/redfish/v1/sessionservice/`|[SessionService](#sessionservice-v1_0_0-sessionservice)|
|`/redfish/v1/sessionservice/sessions/`|Collection of [Session](#session-v1_0_0-session)|
|`/redfish/v1/sessionservice/sessions/{item}/`|[Session](#session-v1_0_0-session)|
|`/redfish/v1/systems/`|Collection of [ComputerSystem](#computersystem-v1_4_0-computersystem)|
|`/redfish/v1/systems/{item}/`|[ComputerSystem](#computersystem-v1_4_0-computersystem)|
|`/redfish/v1/systems/{item}/basenetworkadapters/`|Collection of [HpeBaseNetworkAdapter](#hpebasenetworkadapter-v2_0_0-hpebasenetworkadapter)|
|`/redfish/v1/systems/{item}/basenetworkadapters/{item}/`|[HpeBaseNetworkAdapter](#hpebasenetworkadapter-v2_0_0-hpebasenetworkadapter)|
|`/redfish/v1/systems/{item}/bios/`|[Bios](#bios-v1_0_0-bios)|
|`/redfish/v1/systems/{item}/bios/baseconfigs/`|[HpeBaseConfigs](#hpebaseconfigs-v2_0_0-hpebaseconfigs)|
|`/redfish/v1/systems/{item}/bios/boot/`|[HpeServerBootSettings](#hpeserverbootsettings-v2_0_0-hpeserverbootsettings)|
|`/redfish/v1/systems/{item}/bios/boot/baseconfigs/`|[HpeBaseConfigs](#hpebaseconfigs-v2_0_0-hpebaseconfigs)|
|`/redfish/v1/systems/{item}/bios/boot/settings/`|[HpeServerBootSettings](#hpeserverbootsettings-v2_0_0-hpeserverbootsettings)|
|`/redfish/v1/systems/{item}/bios/hpescalablepmem/`|[HpeScalablePmem](#hpescalablepmem-v1_0_0-hpescalablepmem)|
|`/redfish/v1/systems/{item}/bios/hpescalablepmem/settings/`|[HpeScalablePmem](#hpescalablepmem-v1_0_0-hpescalablepmem)|
|`/redfish/v1/systems/{item}/bios/iscsi/`|[HpeiSCSISoftwareInitiator](#hpeiscsisoftwareinitiator-v2_0_0-hpeiscsisoftwareinitiator)|
|`/redfish/v1/systems/{item}/bios/iscsi/baseconfigs/`|[HpeBaseConfigs](#hpebaseconfigs-v2_0_0-hpebaseconfigs)|
|`/redfish/v1/systems/{item}/bios/iscsi/settings/`|[HpeiSCSISoftwareInitiator](#hpeiscsisoftwareinitiator-v2_0_0-hpeiscsisoftwareinitiator)|
|`/redfish/v1/systems/{item}/bios/mappings/`|[HpeBiosMapping](#hpebiosmapping-v2_0_0-hpebiosmapping)|
|`/redfish/v1/systems/{item}/bios/settings/`|[Bios](#bios-v1_0_0-bios)|
|`/redfish/v1/systems/{item}/bios/tlsconfig/`|[HpeTlsConfig](#hpetlsconfig-v1_0_0-hpetlsconfig)|
|`/redfish/v1/systems/{item}/bios/tlsconfig/baseconfigs/`|[HpeBaseConfigs](#hpebaseconfigs-v2_0_0-hpebaseconfigs)|
|`/redfish/v1/systems/{item}/bios/tlsconfig/settings/`|[HpeTlsConfig](#hpetlsconfig-v1_0_0-hpetlsconfig)|
|`/redfish/v1/systems/{item}/ethernetinterfaces/`|Collection of [EthernetInterface](#ethernetinterface-v1_0_3-ethernetinterface)|
|`/redfish/v1/systems/{item}/ethernetinterfaces/{item}/`|[EthernetInterface](#ethernetinterface-v1_0_3-ethernetinterface)|
|`/redfish/v1/systems/{item}/logservices/`|Collection of [LogService](#logservice-v1_0_0-logservice)|
|`/redfish/v1/systems/{item}/logservices/iml/`|[LogService](#logservice-v1_0_0-logservice)|
|`/redfish/v1/systems/{item}/logservices/iml/entries/`|Collection of [LogEntry](#logentry-v1_0_0-logentry)|
|`/redfish/v1/systems/{item}/logservices/iml/entries/{item}/`|[LogEntry](#logentry-v1_0_0-logentry)|
|`/redfish/v1/systems/{item}/memory/`|Collection of [Memory](#memory-v1_1_0-memory)|
|`/redfish/v1/systems/{item}/memory/{item}/`|[Memory](#memory-v1_1_0-memory)|
|`/redfish/v1/systems/{item}/networkinterfaces/`|Collection of [NetworkInterface](#networkinterface-v1_1_0-networkinterface)|
|`/redfish/v1/systems/{item}/networkinterfaces/{item}/`|[NetworkInterface](#networkinterface-v1_1_0-networkinterface)|
|`/redfish/v1/systems/{item}/networkinterfaces/{item}/networkports/`|Collection of [NetworkPort](#networkport-v1_1_0-networkport)|
|`/redfish/v1/systems/{item}/networkinterfaces/{item}/networkports/{item}/`|[NetworkPort](#networkport-v1_1_0-networkport)|
|`/redfish/v1/systems/{item}/networkinterfaces/{item}/networkports/{item}/hpeevb/`|[HpeNetworkPortEVB](#hpenetworkportevb-v1_0_0-hpenetworkportevb)|
|`/redfish/v1/systems/{item}/networkinterfaces/{item}/networkports/{item}/hpelldp/`|[HpeNetworkPortLLDP](#hpenetworkportlldp-v1_0_0-hpenetworkportlldp)|
|`/redfish/v1/systems/{item}/networkinterfaces/{item}/networkports/{item}/settings/`|[NetworkPort](#networkport-v1_1_0-networkport)|
|`/redfish/v1/systems/{item}/pcidevices/`|Collection of [HpeServerPciDevice](#hpeserverpcidevice-v2_0_0-hpeserverpcidevice)|
|`/redfish/v1/systems/{item}/pcidevices/{item}/`|[HpeServerPciDevice](#hpeserverpcidevice-v2_0_0-hpeserverpcidevice)|
|`/redfish/v1/systems/{item}/pcislots/`|Collection of [HpeServerPCISlot](#hpeserverpcislot-v2_1_0-hpeserverpcislot)|
|`/redfish/v1/systems/{item}/pcislots/{item}/`|[HpeServerPCISlot](#hpeserverpcislot-v2_1_0-hpeserverpcislot)|
|`/redfish/v1/systems/{item}/processors/`|Collection of [Processor](#processor-v1_0_0-processor)|
|`/redfish/v1/systems/{item}/processors/{item}/`|[Processor](#processor-v1_0_0-processor)|
|`/redfish/v1/systems/{item}/secureboot/`|[SecureBoot](#secureboot-v1_0_0-secureboot)|
|`/redfish/v1/systems/{item}/smartstorage/`|[HpeSmartStorage](#hpesmartstorage-v2_0_0-hpesmartstorage)|
|`/redfish/v1/systems/{item}/smartstorage/arraycontrollers/`|Collection of [HpeSmartStorageArrayController](#hpesmartstoragearraycontroller-v2_1_0-hpesmartstoragearraycontroller)|
|`/redfish/v1/systems/{item}/smartstorage/arraycontrollers/{item}/`|[HpeSmartStorageArrayController](#hpesmartstoragearraycontroller-v2_1_0-hpesmartstoragearraycontroller)|
|`/redfish/v1/systems/{item}/smartstorage/arraycontrollers/{item}/diskdrives/`|Collection of [HpeSmartStorageDiskDrive](#hpesmartstoragediskdrive-v2_0_0-hpesmartstoragediskdrive)|
|`/redfish/v1/systems/{item}/smartstorage/arraycontrollers/{item}/diskdrives/{item}/`|[HpeSmartStorageDiskDrive](#hpesmartstoragediskdrive-v2_0_0-hpesmartstoragediskdrive)|
|`/redfish/v1/systems/{item}/smartstorage/arraycontrollers/{item}/logicaldrives/`|Collection of [HpeSmartStorageLogicalDrive](#hpesmartstoragelogicaldrive-v2_1_0-hpesmartstoragelogicaldrive)|
|`/redfish/v1/systems/{item}/smartstorage/arraycontrollers/{item}/logicaldrives/{item}/`|[HpeSmartStorageLogicalDrive](#hpesmartstoragelogicaldrive-v2_1_0-hpesmartstoragelogicaldrive)|
|`/redfish/v1/systems/{item}/smartstorage/arraycontrollers/{item}/logicaldrives/{item}/datadrives/`|Collection of [HpeSmartStorageDiskDrive](#hpesmartstoragediskdrive-v2_0_0-hpesmartstoragediskdrive)|
|`/redfish/v1/systems/{item}/smartstorage/arraycontrollers/{item}/storageenclosures/`|Collection of [HpeSmartStorageStorageEnclosure](#hpesmartstoragestorageenclosure-v2_0_0-hpesmartstoragestorageenclosure)|
|`/redfish/v1/systems/{item}/smartstorage/arraycontrollers/{item}/storageenclosures/{item}/`|[HpeSmartStorageStorageEnclosure](#hpesmartstoragestorageenclosure-v2_0_0-hpesmartstoragestorageenclosure)|
|`/redfish/v1/systems/{item}/smartstorage/arraycontrollers/{item}/unconfigureddrives/`|Collection of [HpeSmartStorageDiskDrive](#hpesmartstoragediskdrive-v2_0_0-hpesmartstoragediskdrive)|
|`/redfish/v1/systems/{item}/smartstorage/arraycontrollers/{item}/unconfigureddrives/{item}/`|[HpeSmartStorageDiskDrive](#hpesmartstoragediskdrive-v2_0_0-hpesmartstoragediskdrive)|
|`/redfish/v1/systems/{item}/smartstorage/hostbusadapters/`|Collection of [HpeSmartStorageHostBusAdapter](#hpesmartstoragehostbusadapter-v2_0_0-hpesmartstoragehostbusadapter)|
|`/redfish/v1/systems/{item}/smartstorage/hostbusadapters/{item}/`|[HpeSmartStorageHostBusAdapter](#hpesmartstoragehostbusadapter-v2_0_0-hpesmartstoragehostbusadapter)|
|`/redfish/v1/systems/{item}/smartstorage/hostbusadapters/{item}/diskdrives/`|Collection of [HpeSmartStorageDiskDrive](#hpesmartstoragediskdrive-v2_0_0-hpesmartstoragediskdrive)|
|`/redfish/v1/systems/{item}/smartstorage/hostbusadapters/{item}/diskdrives/{item}/`|[HpeSmartStorageDiskDrive](#hpesmartstoragediskdrive-v2_0_0-hpesmartstoragediskdrive)|
|`/redfish/v1/systems/{item}/smartstorageconfig/`|[SmartStorageConfig](#smartstorageconfig-v2_0_0-smartstorageconfig)|
|`/redfish/v1/systems/{item}/smartstorageconfig/settings/`|[SmartStorageConfig](#smartstorageconfig-v2_0_0-smartstorageconfig)|
|`/redfish/v1/systems/{item}/storage/`|Collection of [Storage](#storage-v1_0_0-storage)|
|`/redfish/v1/systems/{item}/storage/{interface}/{item}/`|[Storage](#storage-v1_0_0-storage)|
|`/redfish/v1/systems/{item}/storage/{interface}/{item}/volumes/`|Collection of [Volume](#volume-v1_0_0-volume)|
|`/redfish/v1/systems/{item}/storage/{interface}/{item}/volumes/{item}/`|[Volume](#volume-v1_0_0-volume)|
|`/redfish/v1/systems/{item}/usbdevices/`|Collection of [HpeUSBDevice](#hpeusbdevice-v2_0_0-hpeusbdevice)|
|`/redfish/v1/systems/{item}/usbdevices/{item}/`|[HpeUSBDevice](#hpeusbdevice-v2_0_0-hpeusbdevice)|
|`/redfish/v1/systems/{item}/usbports/`|Collection of [HpeUSBPort](#hpeusbport-v2_0_0-hpeusbport)|
|`/redfish/v1/systems/{item}/usbports/{item}/`|[HpeUSBPort](#hpeusbport-v2_0_0-hpeusbport)|
|`/redfish/v1/updateservice/`|[UpdateService](#updateservice-v1_1_0-updateservice)|
|`/redfish/v1/updateservice/componentrepository/`|Collection of [HpeComponent](#hpecomponent-v1_0_0-hpecomponent)|
|`/redfish/v1/updateservice/componentrepository/{item}/`|[HpeComponent](#hpecomponent-v1_0_0-hpecomponent)|
|`/redfish/v1/updateservice/firmwareinventory/`|Collection of [SoftwareInventory](#softwareinventory-v1_0_0-softwareinventory)|
|`/redfish/v1/updateservice/firmwareinventory/{item}/`|[SoftwareInventory](#softwareinventory-v1_0_0-softwareinventory)|
|`/redfish/v1/updateservice/installsets/`|Collection of [HpeComponentInstallSet](#hpecomponentinstallset-v1_0_1-hpecomponentinstallset)|
|`/redfish/v1/updateservice/installsets/{item}/`|[HpeComponentInstallSet](#hpecomponentinstallset-v1_0_1-hpecomponentinstallset)|
|`/redfish/v1/updateservice/softwareinventory/`|Collection of [SoftwareInventory](#softwareinventory-v1_0_0-softwareinventory)|
|`/redfish/v1/updateservice/softwareinventory/{item}/`|[SoftwareInventory](#softwareinventory-v1_0_0-softwareinventory)|
|`/redfish/v1/updateservice/updatetaskqueue/`|Collection of [HpeComponentUpdateTask](#hpecomponentupdatetask-v1_0_1-hpecomponentupdatetask)|
|`/redfish/v1/updateservice/updatetaskqueue/{item}/`|[HpeComponentUpdateTask](#hpecomponentupdatetask-v1_0_1-hpecomponentupdatetask)|
## AccountService.v1_0_2.AccountService
```@odata.type: "#AccountService.v1_0_2.AccountService"```

This is the schema definition for the Account service. It represents the properties for this service and has links to the list of accounts.

### Managing User Accounts with the Accounts Collection

**JSONPath**: `/Accounts/@odata.id`

The destination of this link is a collection of user accounts (see ManagerAccount).

* You may create a new user account by POSTing a new account description the the Accounts collection.  See ManagerAccount for details.
> e.g. `POST https://{iLO}/redfish/v1/accountservice/accounts/ with new account description`
* You may modify an existing user by PATCHing properties to the user account resource.  See ManagerAccount for details.
> e.g. `PATCH https://{iLO}/redfish/v1/accountservice/accounts/{item} with different properties`
* You may remove a user account by DELETEing the resources representing the user
> e.g. `DELETE https://{iLO}/redfish/v1/accountservice/accounts/{item}`

### Resource Instances
|Uri|HTTP Allow|
|---|---|
|```/redfish/v1/accountservice/```|GET PATCH |

### Links to other Resources
|Link Name|Destination type
|---|---|
|```Accounts```|Collection of [ManagerAccount](#manageraccount-v1_0_0-manageraccount)|

### Accounts
This property references a resource of type Collection with a MemberType of ManagerAccount.
### Oem.Hpe.AuthFailureDelayTimeSeconds
Member of [AccountService.v1_0_2.AccountService](#accountservice-v1_0_2-accountservice)

| | |
|---|---|
|Description|The time in seconds to delay for each failure after AuthFailuresBeforeDelay authentication attempts have failed.  Values of 2, 5, 10, and 30 seconds are valid.|
|Type|integer|
|Read Only|False|

The following are the supported values:

|Value|
|---|
|```2```|
|```5```|
|```10```|
|```30```|

### Oem.Hpe.AuthFailureLoggingThreshold
Member of [AccountService.v1_0_2.AccountService](#accountservice-v1_0_2-accountservice)

| | |
|---|---|
|Description|This property enables you to view and configure logging criteria for failed authentications. A failed login log entry is recorded after the configured number of attempts. 0 = feature disabled; 1-3 and 5 are allowable values.|
|Type|integer|
|Read Only|False|

The following are the supported values:

|Value|
|---|
|```Null```|
|```1```|
|```2```|
|```3```|
|```5```|

### Oem.Hpe.AuthFailuresBeforeDelay
Member of [AccountService.v1_0_2.AccountService](#accountservice-v1_0_2-accountservice)

| | |
|---|---|
|Description|The number of failed authentication attempts allowed before authentication is delayed by AuthFailureDelayTimeSeconds. Values of  0, 1, 3, and 5 are valid, with 0 indicating delay after every authentication failure.|
|Type|integer|
|Read Only|False|

The following are the supported values:

|Value|
|---|
|```Null```|
|```1```|
|```3```|
|```5```|

### Oem.Hpe.DefaultPassword
Member of [AccountService.v1_0_2.AccountService](#accountservice-v1_0_2-accountservice)

| | |
|---|---|
|Description|The default password used to log in to the management processor when factory reset is performed.|
|Type|string or null|
|Read Only|False|

### Oem.Hpe.DefaultUserName
Member of [AccountService.v1_0_2.AccountService](#accountservice-v1_0_2-accountservice)

| | |
|---|---|
|Description|The default name used to log in to the management processor when factory reset is performed.|
|Type|string or null|
|Read Only|False|

### Oem.Hpe.MinPasswordLength
Member of [AccountService.v1_0_2.AccountService](#accountservice-v1_0_2-accountservice)

| | |
|---|---|
|Description|This property specifies the minimum number of characters allowed when a user password is set or changed. It must be a value from 0 to 39.|
|Type|integer|
|Read Only|False|

## Bios.v1_0_0.Bios
```@odata.type: "#Bios.v1_0_0.Bios"```

Bios contains properties surrounding a BIOS Attribute Registry (where the system-specific BIOS attributes are described) and the Actions needed to perform changes to BIOS settings, which typically require a system reset to apply.
### Resource Instances
|Uri|HTTP Allow|
|---|---|
|```/redfish/v1/systems/{item}/bios/```|GET |
|```/redfish/v1/systems/{item}/bios/settings/```|GET POST PATCH |

### Links to other Resources
|Link Name|Destination type
|---|---|
|```Oem/Hpe/Links/Boot```|[HpeServerBootSettings](#hpeserverbootsettings-v2_0_0-hpeserverbootsettings)|
|```Oem/Hpe/Links/ScalablePmem```|[HpeScalablePmem](#hpescalablepmem-v1_0_0-hpescalablepmem)|
|```@Redfish.Settings/SettingsObject```|[Bios](#bios-v1_0_0-bios)|
|```Oem/Hpe/Links/TlsConfig```|[HpeTlsConfig](#hpetlsconfig-v1_0_0-hpetlsconfig)|
|```Oem/Hpe/Links/BaseConfigs```|[HpeBaseConfigs](#hpebaseconfigs-v2_0_0-hpebaseconfigs)|
|```Oem/Hpe/Links/Mappings```|[HpeBiosMapping](#hpebiosmapping-v2_0_0-hpebiosmapping)|
|```Oem/Hpe/Links/iScsi```|[HpeiSCSISoftwareInitiator](#hpeiscsisoftwareinitiator-v2_0_0-hpeiscsisoftwareinitiator)|

### @Redfish.Settings
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)
See the Redfish standard schema and specification for information on common @Redfish properties.

### AttributeRegistry
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|The Resource ID of the Attribute Registry for the BIOS Attributes resource.|
|Type|string or null|
|Read Only|True|

### Attributes
**AcpiHpet (High Precision Event Timer (HPET) ACPI Support)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to disable the High Precision Event Timer (HPET) table and device object in ACPI. When disabled, the HPET is not available to an operating system that supports the HPET through the industry standard ACPI name space.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Enabled```|Enabled|
|```Disabled```|Disabled|

**AcpiRootBridgePxm (Memory Proximity Reporting for I/O)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|When enabled, the System BIOS reports the proximity relationship between I/O devices and system memory to the operating system. Most operating systems can use this information to efficiently assign memory resources for devices, such as network controllers and storage devices. Additionally, certain I/O devices might not be able to take advantage of I/O handling benefits if their OS drivers are not properly optimized to support this feature. See your operating system and I/O device documentation for more details.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Enabled```|Enabled|
|```Disabled```|Disabled|

**AcpiSlit (ACPI SLIT)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|The ACPI SLIT (System Locality Information Table) defines the relative access times between processors, memory subsystems, and I/O subsystems. Operating systems that support the SLIT can use this information to improve performance by allocating resources and workloads more efficiently.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Enabled```|Enabled|
|```Disabled```|Disabled|

**AdjSecPrefetch (Adjacent Sector Prefetch)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to disable the processor Adjacent Sector Prefetch feature. In some cases, setting this option to disabled can improve performance. Typically, setting this option to enabled provides better performance. Only disable this option after performing application benchmarking to verify improved performance in the environment.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Enabled```|Enabled|
|```Disabled```|Disabled|

**AdminEmail (Administrator E-mail Address)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Enter the server administrator's e-mail address.|
|Type|String|
|Read Only|False|

**AdminName (Administrator Name)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Enter the server administrator's name text.|
|Type|String|
|Read Only|False|

**AdminOtherInfo (Administrator Other Information)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Enter the server administrator's information text.|
|Type|String|
|Read Only|False|

**AdminPassword (Set Admin Password)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to enter the administrator password to protect the server configuration. When this option is enabled, you are prompted for this password before being allowed to modify the configuration.|
|Type|Password|
|Read Only|False|

**AdminPhone (Administrator Phone Number)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Enter the server administrator's phone number text.|
|Type|String|
|Read Only|False|

**AdvancedMemProtection (Advanced Memory Protection)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to configure additional memory protection with ECC (Error Checking and Correcting). Options and support vary per system.
Advanced ECC keeps all installed memory available for use while still protecting the system against all single-bit failures and certain multi-bit failures.
Online Spare Memory enables a system to automatically map out a group of memory that is detected to be at an increased risk of receiving uncorrected memory errors based on an advanced analysis of corrected memory errors. The mapped out memory is automatically replaced by a spare group of memory without interrupting the system.
Mirrored Memory provides the maximum protection against uncorrected memory errors that might otherwise result in a system failure.
Fault Tolerant Advanced Double Device Data Correction (ADDDC) enables the system to correct memory errors and continue to operate in cases of multiple DRAM device failures on a DIMM. This provides protection against uncorrectable memory errors beyond what is available with Advanced ECC.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```FastFaultTolerantADDDC```|Fast Fault Tolerant Memory (ADDDC)|
|```AdvancedEcc```|Advanced ECC Support|
|```OnlineSpareAdvancedEcc```|Online Spare with Advanced ECC Support|
|```MirroredAdvancedEcc```|Mirrored Memory with Advanced ECC Support|

**AsrStatus (ASR Status)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to configure the Automatic Server Recovery option, which enables the system to automatically reboot if the server locks up.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Enabled```|Enabled|
|```Disabled```|Disabled|

**AsrTimeoutMinutes (ASR Timeout)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|When Automatic Server Recovery is enabled, you can use this option to set the time to wait before rebooting the server in the event of an operating system crash or server lockup.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Timeout10```|10 Minutes|
|```Timeout15```|15 Minutes|
|```Timeout20```|20 Minutes|
|```Timeout30```|30 Minutes|
|```Timeout5```|5 Minutes|

**AssetTagProtection (Asset Tag Protection)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to lock Asset Tag information. When set to lock, the Asset Tag is not erased if the default system settings are restored.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Locked```|Locked|
|```Unlocked```|Unlocked|

**AutoPowerOn (Automatic Power-On)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to configure the server power state when AC power is applied to the system. By default, the system returns to its previous power state when AC power is restored after an AC power loss. Always Power On and Always Power Off cause the system to always return to the "on" and "off" state, respectively, whenever power is applied, even if the system is in the "off" state when power is lost.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```AlwaysPowerOn```|Always Power On|
|```AlwaysPowerOff```|Always Power Off|
|```RestoreLastState```|Restore Last Power State|

**BootMode (Boot Mode)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to select the boot mode of the system. Selecting UEFI Mode configures the system to boot Unified Extensible Firmware Interface (UEFI) compatible operating systems. Selecting Legacy BIOS Mode configures the system to boot traditional operating systems in Legacy BIOS compatibility mode. The operating system can only boot in the mode in which it is installed. The following options require booting in UEFI Mode: Secure Boot, IPv6 PXE Boot, boot > 2.2 TB Disks in AHCI SATA Mode, and Smart Array SW RAID.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Uefi```|UEFI Mode|
|```LegacyBios```|Legacy BIOS Mode|

**BootOrderPolicy (Boot Order Policy)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to configure how the system attempts to boot devices per the Boot Order list when no bootable device is found. If configured to 'Retry Boot Order Indefinitely,' the system continuously attempts to process the Boot Order list until a bootable device is found. If configured to 'Attempt Boot Order Once,' the system attempts to process all items in the Boot Order list once, and if unsuccessful, waits for user input to proceed. If configured for 'Reset After Failed Boot Attempt,' the system attempts to process all items in the Boot Order list once, and then reboots the system.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```RetryIndefinitely```|Retry Boot Order Indefinitely|
|```AttemptOnce```|Attempt Boot Order Once|
|```ResetAfterFailed```|Reset After Failed Boot Attempt|

**ChannelInterleaving (Channel Interleaving)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|You can only configure this option if the Workload Profile is set to Custom. Use this option to modify the level of interleaving for which the memory system is configured. Typically, higher levels of memory interleaving result in maximum performance. However, reducing the level of interleaving can result in power savings.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Enabled```|Enabled|
|```Disabled```|Disabled|

**Chipset_TpmFeatureType (Chipset-TPM feature type)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Information: Use this option to enable chipset based TPM 2.0 feature|
|Type|Enumeration|
|Read Only|True|

|Value|Description|
|---|---|
|```Chipset-TpmFeature:NONE```|Chipset-TPM feature: NONE|
|```Chipset-TpmFeature:PTT```|Chipset-TPM feature: PTT|
|```Chipset-TpmFeature:OTHER```|Chipset-TPM feature: OTHER|

**CollabPowerControl (Collaborative Power Control)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|For operating systems that support the Processor Clocking Control (PCC) Interface, enabling this option enables the Operating System to request processor frequency changes even if the Power Regulator option on the server are configured for Dynamic Power Savings Mode. For Operating Systems that do not support the PCC Interface, or when the Power Regulator Mode is not configured for Dynamic Power Savings Mode, this option has no effect on system operation.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Enabled```|Enabled|
|```Disabled```|Disabled|

**ConfigurationEnabled (Configuration)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|When enabled, the persistent memory regions may be re-configured. A reconfiguration will not be allowed if the current Backup state is 'Pending'.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Enabled```|Enabled|
|```Disabled```|Disabled|

**ConfigurationRestoration (Restore Configuration)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|When enabled, the persistent memory configuration contained on the storage devices will be restored.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Enabled```|Enabled|
|```Disabled```|Disabled|

**ConsistentDevNaming (Consistent Device Naming)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to select the level of Consistent Device Naming. On supported operating systems, NIC ports are named based on their location in the system. CDN Support for LOMs Only names Embedded NICs and FlexibleLOMs. Existing NIC connections retain their names until reinstalled under the OS environment.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```LomsAndSlots```|CDN Support for LOMs and Slots|
|```LomsOnly```|CDN Support for LOMs Only|
|```Disabled```|Disabled|

**CoreBoosting (Core Boosting)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to enable the Core Boosting technology to increase processor performance on qualified processors. |
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Disabled```|Disabled|
|```Enabled```|Enabled|

**CustomPostMessage (Custom POST Message)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Enter a message to be displayed on POST screen during system startup. This feature limits POST screen messaging to 62 characters, special characters are also accepted.|
|Type|String|
|Read Only|False|

**DaylightSavingsTime (Daylight Savings Time)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|This option controls the Daylight Savings Time (DST) adjustment to the displayed local time.  If this option is disabled, the displayed local time will not be adjusted for DST.  If this option is enabled, the displayed local time will be advanced by one hour.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Disabled```|Disabled|
|```Enabled```|Enabled|

**DcuIpPrefetcher (DCU IP Prefetcher)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to disable the processor DCU IP Prefetcher feature. In some cases, setting this option to disabled can improve performance. In most cases, the default value of enabled provides optimal performance. Only disable this option after performing application benchmarking to verify improved performance in the environment. |
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Enabled```|Enabled|
|```Disabled```|Disabled|

**DcuStreamPrefetcher (DCU Stream Prefetcher)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to disable the processor DCU Stream Prefetcher feature. In some cases, setting this option to disabled can improve performance. Typically, setting this option to enabled provides better performance. Only disable this option after performing application benchmarking to verify improved performance in your environment.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Enabled```|Enabled|
|```Disabled```|Disabled|

**Dhcpv4 (DHCPv4)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|When enabled, this option enables obtaining the pre-boot network IPv4 configuration from a DHCP server. Individual settings are not available. When disabled, you must configure static IP address settings individually.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Enabled```|Enabled|
|```Disabled```|Disabled|

**DynamicPowerCapping (Dynamic Power Capping Functionality)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to configure when the System BIOS executes power calibration during the boot process. In Auto mode, calibration is run the first time the server is booted, and is then only run again when the server's hardware configuration or configuration settings change. When disabled, the calibration does not run, and Dynamic Power Capping is not supported. When enabled, the calibration is run on every boot.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Auto```|Auto|
|```Enabled```|Enabled|
|```Disabled```|Disabled|

**EmbNicAspm (PCIe Power Management(ASPM))**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to configure the PCIe Link Power Management (ASPM) support for the selected device. When configured for L0s Enabled, the selected device's link enters a standby energy savings state. When configured for L1 Enabled, the selected device's link enters a lower power standby state at the expense of a longer exit latency. When configured for L1 and L0s Enabled, the selected device's link enters either power savings mode, depending on link utilization, and provides the highest energy savings.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Auto```|Auto|
|```Disabled```|Disabled|
|```AspmL1Enabled```|L1 Enabled|

**EmbNicEnable (PCIe Device Disable)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Select this option to enable or disable PCI devices.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Auto```|Auto|
|```Disabled```|Disabled|

**EmbNicLinkSpeed (PCIe Link Speed)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to configure the PCIe Link Speed for the selected device. When configured for Auto, the selected device trains at the maximum supported speed of the PCIe link. When configured for PCIe Generation 2 Link Speed, the selected device trains at a maximum of PCIe Generation 2 speed. When configured for PCIe Generation  Link 1 speed, the selected device trains at a maximum of PCIe Generation 1 speed.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Auto```|Auto|
|```PcieGen1```|PCIe Generation 1.0|

**EmbNicPCIeOptionROM (PCIe Option ROM)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to enable or disable Device Option ROM |
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Enabled```|Enabled|
|```Disabled```|Disabled|

**EmbSas1Aspm (PCIe Power Management(ASPM))**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to configure the PCIe Link Power Management (ASPM) support for the selected device. When configured for L0s Enabled, the selected device's link enters a standby energy savings state. When configured for L1 Enabled, the selected device's link enters a lower power standby state at the expense of a longer exit latency. When configured for L1 and L0s Enabled, the selected device's link enters either power savings mode, depending on link utilization, and provides the highest energy savings.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Auto```|Auto|
|```Disabled```|Disabled|
|```AspmL1Enabled```|L1 Enabled|

**EmbSas1Boot (Embedded SAS Controller 1)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|When Boot All Targets is selected, all valid boot targets attached to the storage controller are made available in the UEFI Boot Order list. If Boot No Targets is selected, no boot targets from this storage controller are made available in the UEFI Boot Order list.If Boot Limit to 24 Targets is selected, 24 boot targets attached to the storage controller are made available in the UEFI Boot Order list.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```AllTargets```|Boot All Targets|
|```TwentyFourTargets```|Boot Limit to 24 Targets|
|```NoTargets```|Boot No Targets|

**EmbSas1Enable (PCIe Device Disable)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Select this option to enable or disable PCI devices.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Auto```|Auto|
|```Disabled```|Disabled|

**EmbSas1LinkSpeed (PCIe Link Speed)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to configure the PCIe Link Speed for the selected device. When configured for Auto, the selected device trains at the maximum supported speed of the PCIe link. When configured for PCIe Generation 2 Link Speed, the selected device trains at a maximum of PCIe Generation 2 speed. When configured for PCIe Generation  Link 1 speed, the selected device trains at a maximum of PCIe Generation 1 speed.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Auto```|Auto|
|```PcieGen1```|PCIe Generation 1.0|
|```PcieGen2```|PCIe Generation 2.0|

**EmbSas1PcieOptionROM (PCIe Option ROM)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to enable or disable Device Option ROM |
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Enabled```|Enabled|
|```Disabled```|Disabled|

**EmbSata1Aspm (SATA Power Management(SALP))**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to enable or disable Aggressive Link Power Management(SALP).|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Disabled```|Disabled|
|```Enabled```|Enabled|

**EmbSata1Enable (SATA Device Disable)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Select this option to enable or disable SATA devices.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Auto```|Auto|
|```Disabled```|Disabled|

**EmbSata1PCIeOptionROM (PCIe Option ROM)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to enable or disable Device Option ROM |
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Enabled```|Enabled|
|```Disabled```|Disabled|

**EmbSata2Aspm (SATA Power Management(SALP))**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to enable or disable Aggressive Link Power Management(SALP).|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Disabled```|Disabled|
|```Enabled```|Enabled|

**EmbSata2Enable (SATA Device Disable)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Select this option to enable or disable PCI devices.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Auto```|Auto|
|```Disabled```|Disabled|

**EmbSata2PCIeOptionROM (PCIe Option ROM)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to enable or disable Device Option ROM |
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Enabled```|Enabled|
|```Disabled```|Disabled|

**EmbVideoConnection (Embedded Video Connection)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|When configured for Auto mode, the external video connection to the embedded video controller is automatically disabled to save power when a monitor is not attached. It is automatically enabled when a monitor is attached, including when the server is operating. When configured for Always Disabled, the external video connection to the embedded video controller is disabled, and a monitor connected to this port does not display except during system boot. This can be used for security reasons. When configured for Always Enabled, the external video connection to the embedded video controller is always enabled. This option is only required if a monitor is attached with a monitor detection that does not function properly (making AUTO mode not work properly). Note: This option does not affect Integrated Remote Console video. Also, if you press F9 or F11 during system boot, the configured video connector behavior is overridden, and the video console remains enabled. This lets you reconfigure the Embedded Video Connection option even if the video is disabled.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Auto```|Auto|
|```AlwaysDisabled```|Always Disabled|
|```AlwaysEnabled```|Always Enabled|

**EmbeddedSata (Embedded SATA Configuration)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Important: Smart Array SW RAID is not supported when Boot Mode is set to Legacy BIOS Mode. 

Use this option to configure the embedded chipset SATA controller. When selecting the Advanced Host Controller Interface (AHCI) or RAID (if supported), make sure the proper operating system drivers are used for proper operation.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Ahci```|SATA AHCI Support|
|```Raid```|Smart Array SW RAID Support|

**EmbeddedSerialPort (Embedded Serial Port)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Select this option to assign the logical COM port address and associated default resources to the selected physical serial port. The operating system can overwrite this setting.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Com1Irq4```|COM 1; IRQ4; I/O: 3F8h-3FFh|
|```Com2Irq3```|COM 2; IRQ3; I/O: 2F8h-2FFh|
|```Disabled```|Disabled|

**EmbeddedUefiShell (Embedded UEFI Shell)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to enable or disable the Embedded UEFI Shell. When enabled, you can launch the Embedded UEFI Shell from the pre-boot environment. When enabled and the Boot Mode is configured for UEFI Mode, you can add the Embedded UEFI Shell to the UEFI Boot Order list  by selecting the option entitled 'Add Embedded UEFI Shell to Boot Order'. When disabled, the Embedded UEFI Shell is not available in the pre-boot environment, and you cannot add it to the UEFI Boot Order list. The Embedded UEFI Shell is a pre-boot command line environment that you can use for scripting and running UEFI applications. It provides CLI-based commands to configure the server, update the System BIOS and other firmware, and obtain system information and error logs.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Enabled```|Enabled|
|```Disabled```|Disabled|

**EmsConsole (EMS Console)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to configure the ACPI serial port settings, which include the ability to redirect the Windows Server Emergency Management console (EMS) through either the physical or virtual serial port.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Disabled```|Disabled|
|```Physical```|Physical Serial Port|
|```Virtual```|Virtual Serial Port|

**EnabledCoresPerProc (Enabled Cores per Processor)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|This option enables limiting the number of enabled processor cores per physical processor. You can set the number of enabled cores to a value supported by the physical processor. Setting the value to 0 or a value larger than the number of supported cores of the installed processor will result in all processor cores in the socket being enabled.|
|Type|Integer|
|Read Only|False|

**EnergyEfficientTurbo (Energy Efficient Turbo)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|This option controls whether the processor uses an energy efficiency based policy when engaging turbo range frequencies. This option is only applicable when Turbo Mode is enabled.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Enabled```|Enabled|
|```Disabled```|Disabled|

**EnergyPerfBias (Energy/Performance Bias)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|You can only configure this option if the Workload Profile is set to Custom. Use this option to configure several processor subsystems to optimize the performance and power usage of the processor. Balanced Performance provides optimum power efficiency, and is recommended for most environments. Maximum Performance Mode is recommended for environments that require the highest performance and lowest latency but are not sensitive to power consumption. Only use Power Savings Mode in environments that are power sensitive and can accept reduced performance.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```MaxPerf```|Maximum Performance|
|```BalancedPerf```|Balanced Performance|
|```BalancedPower```|Balanced Power|
|```PowerSavingsMode```|Power Savings Mode|

**EraseUserDefaults (Erase User Defaults)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Select this option to erase the user defaults backup.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```No```|No, Cancel|
|```Yes```|Yes, erase the current settings.|

**ExtendedAmbientTemp (Extended Ambient Temperature Support)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to enable the server to operate at higher ambient temperatures than normally supported. These options are only supported with specific hardware configurations. See your server documentation before configuring the server to enable extended ambient temperature support. Improper system operation or damage to hardware components can result from enabling these options in unsupported configurations. Selecting Enabled for 40c Ambient (ASHRAE 3) enables the server to operate in environments with ambient temperatures up to 40 degrees Celsius. Selecting Enabled for 45c Ambient (ASHRAE 4) enables the server to operate in environments with ambient temperatures up to 45 degrees Celsius. Not all servers support both 40c Ambient (ASHRAE 3) and 45c Ambient (ASHRAE 4).|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Disabled```|Disabled|
|```ASHRAE3```|Enabled for 40c Ambient (ASHRAE 3)|
|```ASHRAE4```|Enabled for 45c Ambient (ASHRAE 4)|

**ExtendedMemTest (Extended Memory Test)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|When enabled, the system validates memory during the memory initialization process. If uncorrectable memory errors are detected, the memory is mapped out, and the failed DIMMs are logged to the Integrated Management Log (IML). Enabling this option can result in a significant increase in the server boot time.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Enabled```|Enabled|
|```Disabled```|Disabled|

**F11BootMenu (One-Time Boot Menu (F11 Prompt))**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to disable the POST One-Time Boot F11 Prompt.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Enabled```|Enabled|
|```Disabled```|Disabled|

**FCScanPolicy (Fibre Channel/FCoE Scan Policy)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to change the default Fibre Channel or FCoE policy for scanning for boot targets. When configured for Scan All Targets, each installed FC/FCoE adapter scans all available targets. When configured for Scan Configured Targets Only, the FC/FCoE adapters only scan targets that are preconfigured in the devices settings. This option overrides any individual device settings configured in the device-specific setup.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```AllTargets```|Scan All Targets|
|```CardConfig```|Scan Configured Targets Only|

**FanFailPolicy (Fan Failure Policy)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to configure how the server reacts when fans fail, resulting in the server not having required fans in operation. When configured for "Shutdown/Halt on Critical Fan Failures," the server cannot boot or operate when it does not have required fans operating due to one or more fan failures.  When configured for "Allow Operation with Critical Fan Failures," the server can boot and operate if it does not have required fans operating due to one or more fan failures. It is recommended that you configure the Fan Failure Policy to the default state of "Shutdown/Halt on Critical Fan Failures." Operating without the required fans operating can result in damage to hardware components.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Shutdown```|Shutdown/Halt on Critical Fan Failures|
|```Allow```|Allow Operation with Critical Fan Failures|

**FanInstallReq (Fan Installation Requirements)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to configure how the server reacts when all required fans are not installed. When configured for Enable Messaging, the server displays messages and log events to the Integrated Management Log (IML) when required fans are not installed. The server can still boot and operate. When configured for Disable Messaging, the server does not display messages and log events when required fans are not installed. All indications that the server is operating without required fans are removed. It is recommended that you leave Fan Installation Requirements in the default state of Enable Messaging. Operating without the required fans can result in damage to hardware components.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```EnableMessaging```|Enable Messaging|
|```DisableMessaging```|Disable Messaging|

**FlexLom1Aspm (PCIe Power Management(ASPM))**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to configure the PCIe Link Power Management (ASPM) support for the selected device. When configured for L0s Enabled, the selected device's link enters a standby energy savings state. When configured for L1 Enabled, the selected device's link enters a lower power standby state at the expense of a longer exit latency. When configured for L1 and L0s Enabled, the selected device's link enters either power savings mode, depending on link utilization, and provides the highest energy savings.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Auto```|Auto|
|```Disabled```|Disabled|
|```AspmL1Enabled```|L1 Enabled|

**FlexLom1Enable (PCIe Device Disable)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Select this option to enable or disable PCI devices.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Auto```|Auto|
|```Disabled```|Disabled|

**FlexLom1LinkSpeed (PCIe Link Speed)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to configure the PCIe Link Speed for the selected device. When configured for Auto, the selected device trains at the maximum supported speed of the PCIe link. When configured for PCIe Generation 2 Link Speed, the selected device trains at a maximum of PCIe Generation 2 speed. When configured for PCIe Generation  Link 1 speed, the selected device trains at a maximum of PCIe Generation 1 speed.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Auto```|Auto|
|```PcieGen1```|PCIe Generation 1.0|
|```PcieGen2```|PCIe Generation 2.0|

**FlexLom1PCIeOptionROM (PCIe Option ROM)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to enable or disable Device Option ROM |
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Enabled```|Enabled|
|```Disabled```|Disabled|

**FunctionalityEnabled (Functionality)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|When enabled, data in the persistent memory regions will be saved to non-volatile storage upon power loss and power events. Note that enabling this option will disable the following options: Node Interleaving, Extended Memory Test, Memory Clear on Warm Reset, Memory Mirroring, Online Spare Memory, Fault Tolerant Memory, and Sub-NUMA Clustering. |
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Enabled```|Enabled|
|```Disabled```|Disabled|

**HttpSupport (HTTP Support)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to control the UEFI HTTP(s) boot support when in UEFI Mode, and the 'Discover Shell Auto-Start Script using DHCP' option under 'Embedded UEFI Shell' settings.
When 'Auto' is selected, the system automatically adds HTTP(S) boot options to the UEFI Boot Order list for every network port that is enabled for Network Boot. Selecting this option enables the system to boot to the HTTP or HTTPS URLs provided by the DHCP server. Any other URLs provided by the DHCP server are ignored. 
When 'HTTP only' is selected, the system automatically adds HTTP boot options to the UEFI Boot Order list for every network port that is enabled for Network Boot. Selecting this option enables the system to boot to the HTTP URLs provided by the DHCP server, and to ignore any HTTPS or other URLs that are provided. 
When 'HTTPS only' is selected, the system automatically adds HTTPS boot options to the UEFI Boot Order list for every network port that is enabled for Network Boot. Selecting this option enables the system to boot to the HTTPS URLs provided by the DHCP server, and to ignore any HTTP or other URLs that are provided. 
To enable HTTPS boot either by selecting 'Auto' or 'HTTPS only', you must enroll the respective TLS certificate of the HTTPS server under Server Security > TLS(HTTPS) Options. 
Note: This setting only affects the HTTP boot options added for the network ports, and the Discover Shell Auto-Start Script provided by the DHCP server. Other settings, such as Boot from URL, are not affected by this setting.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Auto```|Auto|
|```HttpsOnly```|HTTPS only|
|```HttpOnly```|HTTP only|
|```Disabled```|Disabled|

**HwPrefetcher (HW Prefetcher)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to disable the processor HW prefetch feature. In some cases, setting this option to disabled can improve performance. Typically, setting this option to enabled provides better performance. Only disable this option after performing application benchmarking to verify improved performance in the environment.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Enabled```|Enabled|
|```Disabled```|Disabled|

**IntelDmiLinkFreq (Intel DMI Link Frequency)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to force the link speed between the processor and the southbridge to run at slower speeds to save power.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Auto```|Auto|
|```DmiGen1```|Gen 1 Speed|
|```DmiGen2```|Gen 2 Speed|

**IntelNicDmaChannels (Intel NIC DMA Channels (IOAT))**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to select the Intel NIC DMA Channels support. This is a NIC acceleration option that only runs on Intel-based NICs.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Enabled```|Enabled|
|```Disabled```|Disabled|

**IntelPerfMonitoring (Intel Performance Monitoring Support)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|This option does not impact performance. When enabled, this option exposes certain chipset devices that can be used with the Intel Performance Monitoring Toolkit.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Disabled```|Disabled|
|```Enabled```|Enabled|

**IntelProcVtd (Intel(R) VT-d)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|If enabled, a hypervisor or operating system supporting this option can use hardware capabilities provided by Intel VT for Directed I/O. You can leave this set to enabled even if you are not using a hypervisor or an operating system that uses this option.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Enabled```|Enabled|
|```Disabled```|Disabled|

**IntelTxt (Intel(R) TXT Support)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to modify Intel TXT support.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Enabled```|Enabled|
|```Disabled```|Disabled|

**IntelUpiFreq (Intel UPI Link Frequency)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to set the UPI Link frequency to a lower speed. Running at a lower frequency can reduce power consumption, but can also affect system performance. You can only configure this option if two or more CPUs are present and the Workload Profile is set to custom.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Auto```|Auto|
|```MinUpiSpeed```|Min UPI Speed|

**IntelUpiLinkEn (Intel UPI Link Enablement)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to configure the UPI topology to use fewer links between processors, when available. Changing from the default can reduce UPI bandwidth performance in exchange for less power consumption.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Auto```|Auto|
|```SingleLink```|Single Link Operation|

**IntelUpiPowerManagement (Intel UPI Link Power Management)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to place the Quick Path Interconnect (UPI) links into a low power state when the links are not being used. This lowers power usage with minimal effect on performance. You can only configure this option if two or more CPUs are present and the Workload Profile is set to custom.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Enabled```|Enabled|
|```Disabled```|Disabled|

**IntelligentProvisioning (Intelligent Provisioning (F10 Prompt))**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to enable or disable the Intelligent Provisioning functionality. When disabled, you are prevented from entering the Intelligent Provisioning environment by pressing F10 during server boot. You must set this option to enabled to use Intelligent Provisioning functionality.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Enabled```|Enabled|
|```Disabled```|Disabled|

**InternalSDCardSlot (Internal SD Card Slot)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to enable or disable the Internal SD Card Slot. When set to disabled, the SD card slot is disabled, regardless of whether an SD Card is installed or not. The SD Card will not be visible in the pre-boot environment or under the operating system.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Enabled```|Enabled|
|```Disabled```|Disabled|

**Ipv4Address (IPv4 Address)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to specify the pre-boot network IPv4 address. Enter a static IP address using dotted-decimal notation (for example, 127.0.0.1). If DHCP is used (the DHCPv4 option is enabled), this setting is unavailable because the value is supplied automatically.|
|Type|String|
|Read Only|False|

**Ipv4Gateway (IPv4 Gateway)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to specify the pre-boot network gateway IPv4 address. Enter a static IP address using dotted-decimal notation (for example, 127.0.0.1). If DHCP is used (the DHCPv4 option is enabled), this setting is unavailable because the value is supplied automatically.|
|Type|String|
|Read Only|False|

**Ipv4PrimaryDNS (IPv4 Primary DNS)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to specify the pre-boot network Primary DNS Server IPv4 address. Enter a static IP address using dotted-decimal notation (for example, 127.0.0.1). If DHCP is used (the DHCPv4 option is enabled), this setting is unavailable because the value is supplied automatically.|
|Type|String|
|Read Only|False|

**Ipv4SecondaryDNS (IPv4 Secondary DNS)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to specify the pre-boot network Secondary DNS Server IPv4 address. Enter a static IP address using dotted-decimal notation (for example, 127.0.0.1). If DHCP is used (the DHCPv4 option is enabled), this setting is unavailable because the value is supplied automatically.|
|Type|String|
|Read Only|False|

**Ipv4SubnetMask (IPv4 Subnet Mask)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to specify the pre-boot network subnet mask. Enter a static IP address using dotted-decimal notation (for example, 255.255.255.0). If DHCP is used (the DHCPv4 option is enabled), this setting is unavailable because the value is supplied automatically.|
|Type|String|
|Read Only|False|

**Ipv6Address (IPv6 Address)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to specify the pre-boot network IPv6 address. Enter a static IP address in the standard colon seperated format (for example, 1234::1000). If IPv6 Config Policy is set to Automatic, this setting is unavailable because the value is supplied automatically.|
|Type|String|
|Read Only|False|

**Ipv6ConfigPolicy (IPv6 Config Policy)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|When set to Automatic, this option enables obtaining the pre-boot network IPv6 configuration automatically. Individual settings are not available. When set to Manual, you must configure static IP address settings individually.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Automatic```|Automatic|
|```Manual```|Manual|

**Ipv6Duid (IPv6 DHCP Unique Identifier)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to control the IPv6 DHCP Unique Identifier (DUID). If configured for Auto, the DUID is set using the Universal Unique Identifier (UUID) of the server, or using the DUID-LLT method if the server UUID is not available. If configured for DUID-LLT, the DUID is set based on the Link-layer Address Plus Time [DUID-LLT] method. |
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Auto```|Auto|
|```DuidLlt```|DUID-LLT|

**Ipv6Gateway (IPv6 Gateway)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to specify the pre-boot network gateway IPv6 address. Enter a static IP address in the standard colon seperated format (for example, 1234::1000). If IPv6 Config Policy is set to Automatic, this setting is unavailable because the value is supplied automatically.|
|Type|String|
|Read Only|False|

**Ipv6PrimaryDNS (IPv6 Primary DNS)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to specify the pre-boot network Primary DNS Server IPv6 address. Enter a static IP address in the standard colon seperated format (for example, 1234::1000). If IPv6 Config Policy is set to Automatic, this setting is unavailable because the value is supplied automatically.|
|Type|String|
|Read Only|False|

**Ipv6SecondaryDNS (IPv6 Secondary DNS)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to specify the pre-boot network Secondary DNS Server IPv6 address. Enter a static IP address in the standard colon seperated format (for example, 1234::1000). If IPv6 Config Policy is set to Automatic, this setting is unavailable because the value is supplied automatically.|
|Type|String|
|Read Only|False|

**LLCDeadLineAllocation (LLC Dead Line Allocation)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Enable  - Opportunistically fill dead lines in LLC. Disable - Never fill dead lines in LLC.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Enabled```|Enabled|
|```Disabled```|Disabled|

**LlcPrefetch (LLC Prefetch)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to configure the processor Last Level Cache (LLC) prefetch feature. In some cases, setting this option to disabled can improve performance. Typically, setting this option to enabled provides better performance. Only disable this option after performing application benchmarking to verify improved performance in the environment.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Enabled```|Enabled|
|```Disabled```|Disabled|

**LocalRemoteThreshold (Local/Remote Threshold)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Local/Remote Threshold setting.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Auto```|Auto|
|```Low```|Low|
|```Medium```|Medium|
|```High```|High|
|```Disabled```|Disabled|

**MaxMemBusFreqMHz (Maximum Memory Bus Frequency)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to configure the memory system to run memory at a lower maximum speed than that supported by the installed processor and DIMM configuration. Setting this option to Auto configures the system to run memory at the maximum speed supported.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Auto```|Auto|
|```MaxMemBusFreq2667```|2667 MHz|
|```MaxMemBusFreq2400```|2400 MHz|
|```MaxMemBusFreq2133```|2133 MHz|
|```MaxMemBusFreq1867```|1867 MHz|

**MaxPcieSpeed (Maximum PCI Express Speed)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|You can only configure this option if the Workload Profile is set to Custom. If a PCI Express device does not run properly at its optimal speed, lowering the speed at which the device is running can address this issue. This option enables you to lower the maximum PCI Express speed at which the server allows PCI Express devices to operate. You can also use it to address issues with problematic PCI Express devices. Setting this value to Maximum Supported configures the platform to run at the maximum speed supported by the platform or the PCIe device, whichever is lower.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```PerPortCtrl```|Per Port Control|
|```PcieGen1```|PCIe Generation 1.0|

**MemClearWarmReset (Memory Clear on Warm Reset)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to configure when memory is cleared on warm resets. When disabled, the contents of memory are only cleared on a warm reset if requested by the operating system. When enabled, memory is cleared on all reboots. Disabling this option can save boot time by skipping the clearing of memory on warm resets.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Enabled```|Enabled|
|```Disabled```|Disabled|

**MemFastTraining (Memory Fast Training)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|This option enables a boot time reduction by controlling when the BIOS bypasses the full memory training. When enabled, the server bypasses the full memory training during boot, and uses memory parameters determined on a previous boot to decrease boot time. Note that even when enabled, the BIOS performs a full memory training if the DIMM configuration or processor configuration changes, or if there is a change in any BIOS setting related to memory or processor configuration. When disabled, the server performs a full memory training on every server boot.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Enabled```|Enabled|
|```Disabled```|Disabled|

**MemMirrorMode (Memory Mirroring Mode)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to select from the available Memory Mirroring modes. Full Mirror - reserves 50% of the total available memory for mirroring. Partial Mirror (20% above 4GB) - reserves 20% of the total available Memory above 4GB for Mirroring. Partial Mirror (10% above 4GB) - reserves 10% of the total available Memory above 4GB for Mirroring. Partial Mirror (Memory below 4GB) - depending on the memory configuration, sets up 2GB or 3GB of lower memory below 4GB for Mirroring. Partial Mirror (OS Configured) - sets up the system to configure Partial Mirroring at OS level. |
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Full```|Full Mirror|
|```PartialOsConfig```|Partial Mirror (OS Configured)|
|```PartialFirst4GB```|Partial Mirror (Memory below 4GB)|
|```Partial10PercentAbove4GB```|Partial Mirror (10% above 4GB)|
|```Partial20PercentAbove4GB```|Partial Mirror (20% above 4GB)|

**MemPatrolScrubbing (Memory Patrol Scrubbing)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|This option corrects memory soft errors so that, over the length of the system runtime, the risk of producing multi-bit and uncorrectable errors is reduced.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Enabled```|Enabled|
|```Disabled```|Disabled|

**MemRefreshRate (Memory Refresh Rate)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|This option controls the refresh rate of the memory controller and might affect the performance and resiliency of the server memory. It is recommended that you leave this setting in the default state unless indicated in other documentation for this server.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Refreshx1```|1x Refresh|
|```Refreshx2```|2x Refresh|

**MemoryRemap (Memory Remap)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to remap memory that may have been previously disabled from the system due to a failure event, such as an uncorrectable memory error. The Remap All Memory Option causes the system to make all memory in the system available again on the next boot. The No Action option leaves any affected memory unavailable to the system.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```NoAction```|No Action|
|```AllMemory```|All Memory|

**MinProcIdlePkgState (Minimum Processor Idle Power Package C-State)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|You can configure this option only if the Workload Profile is set to Custom. Use this option to select the lowest idle package power state (C-state) of the processor. The processor automatically transitions into package C-states based on the Core C-states in which cores on the processor have transitioned. The higher the package C-state, the lower the power usage of that idle package state. (Package C6 (retention) is the lowest power idle package state supported by the processor).|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```C6Retention```|Package C6 (retention) State|
|```C6NonRetention```|Package C6 (non-retention) State|
|```NoState```|No Package State|

**MinProcIdlePower (Minimum Processor Idle Power Core C-State)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|You can only configure this option if Workload Profile is set to Custom. Use this option to select the lowest idle power state (C-state) of the processor that the operating system uses. The higher the C-state, the lower the power usage of that idle state. (C6 is the lowest power idle state supported by the processor).|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```C6```|C6 State|
|```C1E```|C1E State|
|```NoCStates```|No C-states|

**MixedPowerSupplyReporting (Mixed Power Supply Reporting)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|When enabled, the server logs a message that a mixed power supply configuration is present. When disabled, the server no longer logs messages that a mixed power supply configuration is present.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Enabled```|Enabled|
|```Disabled```|Disabled|

**NetworkBootRetry (Network Boot Retry Support)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to configure the Network Boot Retry Support. When enabled, the system BIOS attempts to boot the network device up to the number of times configured in the Network Boot Retry Count option before attempting to boot the next network device. This setting only takes effect when attempting to boot a network device from the F12 function key and one-time boot options.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Enabled```|Enabled|
|```Disabled```|Disabled|

**NetworkBootRetryCount (Network Boot Retry Count)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to control the number of times the system BIOS attempts to boot a network device.|
|Type|Integer|
|Read Only|False|

**NicBoot1 (Embedded NIC 1 Boot)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to enable or disable network boot (PXE, iSCSI, FCoE or UEFI HTTP) for the selected NIC. You might need to configure the NIC firmware for the boot option to be active.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```NetworkBoot```|Network Boot|
|```Disabled```|Disabled|

**NicBoot10 (Embedded NIC 10 Boot)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to enable or disable network boot (PXE, iSCSI, FCoE or UEFI HTTP) for the selected NIC. You might need to configure the NIC firmware for the boot option to be active.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```NetworkBoot```|Network Boot|
|```Disabled```|Disabled|

**NicBoot11 (Embedded NIC 11 Boot)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to enable or disable network boot (PXE, iSCSI, FCoE or UEFI HTTP) for the selected NIC. You might need to configure the NIC firmware for the boot option to be active.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```NetworkBoot```|Network Boot|
|```Disabled```|Disabled|

**NicBoot12 (Embedded NIC 12 Boot)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to enable or disable network boot (PXE, iSCSI, FCoE or UEFI HTTP) for the selected NIC. You might need to configure the NIC firmware for the boot option to be active.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```NetworkBoot```|Network Boot|
|```Disabled```|Disabled|

**NicBoot2 (Embedded NIC 2 Boot)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to enable or disable network boot (PXE, iSCSI, FCoE or UEFI HTTP) for the selected NIC. You might need to configure the NIC firmware for the boot option to be active.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```NetworkBoot```|Network Boot|
|```Disabled```|Disabled|

**NicBoot3 (Embedded NIC 3 Boot)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to enable or disable network boot (PXE, iSCSI, FCoE or UEFI HTTP) for the selected NIC. You might need to configure the NIC firmware for the boot option to be active.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```NetworkBoot```|Network Boot|
|```Disabled```|Disabled|

**NicBoot4 (Embedded NIC 4 Boot)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to enable or disable network boot (PXE, iSCSI, FCoE or UEFI HTTP) for the selected NIC. You might need to configure the NIC firmware for the boot option to be active.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```NetworkBoot```|Network Boot|
|```Disabled```|Disabled|

**NicBoot5 (Embedded NIC 5 Boot)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to enable or disable network boot (PXE, iSCSI, FCoE or UEFI HTTP) for the selected NIC. You might need to configure the NIC firmware for the boot option to be active.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```NetworkBoot```|Network Boot|
|```Disabled```|Disabled|

**NicBoot6 (Embedded NIC 6 Boot)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to enable or disable network boot (PXE, iSCSI, FCoE or UEFI HTTP) for the selected NIC. You might need to configure the NIC firmware for the boot option to be active.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```NetworkBoot```|Network Boot|
|```Disabled```|Disabled|

**NicBoot7 (Embedded NIC 7 Boot)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to enable or disable network boot (PXE, iSCSI, FCoE or UEFI HTTP) for the selected NIC. You might need to configure the NIC firmware for the boot option to be active.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```NetworkBoot```|Network Boot|
|```Disabled```|Disabled|

**NicBoot8 (Embedded NIC 8 Boot)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to enable or disable network boot (PXE, iSCSI, FCoE or UEFI HTTP) for the selected NIC. You might need to configure the NIC firmware for the boot option to be active.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```NetworkBoot```|Network Boot|
|```Disabled```|Disabled|

**NicBoot9 (Embedded NIC 9 Boot)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to enable or disable network boot (PXE, iSCSI, FCoE or UEFI HTTP) for the selected NIC. You might need to configure the NIC firmware for the boot option to be active.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```NetworkBoot```|Network Boot|
|```Disabled```|Disabled|

**NodeInterleaving (Node Interleaving)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to disable the NUMA architecture properties for the system. All operating system platforms support NUMA architectures. In most cases, optimum performance is obtained by disabling the Node Interleaving option. When this option is enabled, memory addresses are interleaved across the memory installed for each processor. Some workloads might experience improved performance when this option is enabled. Node Interleaving cannot be enabled when NVDIMMs are present in the system.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Enabled```|Enabled|
|```Disabled```|Disabled|

**NumaGroupSizeOpt (NUMA Group Size Optimization)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to configure how the System BIOS reports the size of a NUMA node (number of logical processors), which assists the Operating System in grouping processors for application use (referred to as Kgroups). The default setting of Clustered provides better performance due to optimizing the resulting groups along NUMA boundaries. However, some applications might not be optimized to take advantage of processors spanning multiple groups. In such cases, selecting the Flat option might be necessary in order for those applications to utilize more logical processors.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Flat```|Flat|
|```Clustered```|Clustered|

**NvmeDrive1 (NVMe Drive 1)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to configure different NVM Express Drives Usage. When NVMe is selected, NVM Express Drive is used as storage device. When Scalable PMEM is selected, NVM Express Drive is used as Logical NVDIMM Backup/Restore device.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Nvme```|NVMe|
|```ScalablePMEM```|Scalable PMEM|

**NvmeDrive10 (NVMe Drive 10)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to configure different NVM Express Drives Usage. When NVMe is selected, NVM Express Drive is used as storage device. When Scalable PMEM is selected, NVM Express Drive is used as Logical NVDIMM Backup/Restore device.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Nvme```|NVMe|
|```ScalablePMEM```|Scalable PMEM|

**NvmeDrive11 (NVMe Drive 11)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to configure different NVM Express Drives Usage. When NVMe is selected, NVM Express Drive is used as storage device. When Scalable PMEM is selected, NVM Express Drive is used as Logical NVDIMM Backup/Restore device.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Nvme```|NVMe|
|```ScalablePMEM```|Scalable PMEM|

**NvmeDrive12 (NVMe Drive 12)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to configure different NVM Express Drives Usage. When NVMe is selected, NVM Express Drive is used as storage device. When Scalable PMEM is selected, NVM Express Drive is used as Logical NVDIMM Backup/Restore device.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Nvme```|NVMe|
|```ScalablePMEM```|Scalable PMEM|

**NvmeDrive13 (NVMe Drive 13)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to configure different NVM Express Drives Usage. When NVMe is selected, NVM Express Drive is used as storage device. When Scalable PMEM is selected, NVM Express Drive is used as Logical NVDIMM Backup/Restore device.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Nvme```|NVMe|
|```ScalablePMEM```|Scalable PMEM|

**NvmeDrive14 (NVMe Drive 14)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to configure different NVM Express Drives Usage. When NVMe is selected, NVM Express Drive is used as storage device. When Scalable PMEM is selected, NVM Express Drive is used as Logical NVDIMM Backup/Restore device.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Nvme```|NVMe|
|```ScalablePMEM```|Scalable PMEM|

**NvmeDrive15 (NVMe Drive 15)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to configure different NVM Express Drives Usage. When NVMe is selected, NVM Express Drive is used as storage device. When Scalable PMEM is selected, NVM Express Drive is used as Logical NVDIMM Backup/Restore device.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Nvme```|NVMe|
|```ScalablePMEM```|Scalable PMEM|

**NvmeDrive16 (NVMe Drive 16)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to configure different NVM Express Drives Usage. When NVMe is selected, NVM Express Drive is used as storage device. When Scalable PMEM is selected, NVM Express Drive is used as Logical NVDIMM Backup/Restore device.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Nvme```|NVMe|
|```ScalablePMEM```|Scalable PMEM|

**NvmeDrive17 (NVMe Drive 17)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to configure different NVM Express Drives Usage. When NVMe is selected, NVM Express Drive is used as storage device. When Scalable PMEM is selected, NVM Express Drive is used as Logical NVDIMM Backup/Restore device.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Nvme```|NVMe|
|```ScalablePMEM```|Scalable PMEM|

**NvmeDrive18 (NVMe Drive 18)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to configure different NVM Express Drives Usage. When NVMe is selected, NVM Express Drive is used as storage device. When Scalable PMEM is selected, NVM Express Drive is used as Logical NVDIMM Backup/Restore device.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Nvme```|NVMe|
|```ScalablePMEM```|Scalable PMEM|

**NvmeDrive19 (NVMe Drive 19)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to configure different NVM Express Drives Usage. When NVMe is selected, NVM Express Drive is used as storage device. When Scalable PMEM is selected, NVM Express Drive is used as Logical NVDIMM Backup/Restore device.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Nvme```|NVMe|
|```ScalablePMEM```|Scalable PMEM|

**NvmeDrive2 (NVMe Drive 2)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to configure different NVM Express Drives Usage. When NVMe is selected, NVM Express Drive is used as storage device. When Scalable PMEM is selected, NVM Express Drive is used as Logical NVDIMM Backup/Restore device.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Nvme```|NVMe|
|```ScalablePMEM```|Scalable PMEM|

**NvmeDrive20 (NVMe Drive 20)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to configure different NVM Express Drives Usage. When NVMe is selected, NVM Express Drive is used as storage device. When Scalable PMEM is selected, NVM Express Drive is used as Logical NVDIMM Backup/Restore device.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Nvme```|NVMe|
|```ScalablePMEM```|Scalable PMEM|

**NvmeDrive21 (NVMe Drive 21)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to configure different NVM Express Drives Usage. When NVMe is selected, NVM Express Drive is used as storage device. When Scalable PMEM is selected, NVM Express Drive is used as Logical NVDIMM Backup/Restore device.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Nvme```|NVMe|
|```ScalablePMEM```|Scalable PMEM|

**NvmeDrive22 (NVMe Drive 22)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to configure different NVM Express Drives Usage. When NVMe is selected, NVM Express Drive is used as storage device. When Scalable PMEM is selected, NVM Express Drive is used as Logical NVDIMM Backup/Restore device.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Nvme```|NVMe|
|```ScalablePMEM```|Scalable PMEM|

**NvmeDrive23 (NVMe Drive 23)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to configure different NVM Express Drives Usage. When NVMe is selected, NVM Express Drive is used as storage device. When Scalable PMEM is selected, NVM Express Drive is used as Logical NVDIMM Backup/Restore device.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Nvme```|NVMe|
|```ScalablePMEM```|Scalable PMEM|

**NvmeDrive24 (NVMe Drive 24)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to configure different NVM Express Drives Usage. When NVMe is selected, NVM Express Drive is used as storage device. When Scalable PMEM is selected, NVM Express Drive is used as Logical NVDIMM Backup/Restore device.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Nvme```|NVMe|
|```ScalablePMEM```|Scalable PMEM|

**NvmeDrive25 (NVMe Drive 25)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to configure different NVM Express Drives Usage. When NVMe is selected, NVM Express Drive is used as storage device. When Scalable PMEM is selected, NVM Express Drive is used as Logical NVDIMM Backup/Restore device.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Nvme```|NVMe|
|```ScalablePMEM```|Scalable PMEM|

**NvmeDrive26 (NVMe Drive 26)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to configure different NVM Express Drives Usage. When NVMe is selected, NVM Express Drive is used as storage device. When Scalable PMEM is selected, NVM Express Drive is used as Logical NVDIMM Backup/Restore device.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Nvme```|NVMe|
|```ScalablePMEM```|Scalable PMEM|

**NvmeDrive27 (NVMe Drive 27)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to configure different NVM Express Drives Usage. When NVMe is selected, NVM Express Drive is used as storage device. When Scalable PMEM is selected, NVM Express Drive is used as Logical NVDIMM Backup/Restore device.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Nvme```|NVMe|
|```ScalablePMEM```|Scalable PMEM|

**NvmeDrive28 (NVMe Drive 28)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to configure different NVM Express Drives Usage. When NVMe is selected, NVM Express Drive is used as storage device. When Scalable PMEM is selected, NVM Express Drive is used as Logical NVDIMM Backup/Restore device.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Nvme```|NVMe|
|```ScalablePMEM```|Scalable PMEM|

**NvmeDrive29 (NVMe Drive 29)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to configure different NVM Express Drives Usage. When NVMe is selected, NVM Express Drive is used as storage device. When Scalable PMEM is selected, NVM Express Drive is used as Logical NVDIMM Backup/Restore device.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Nvme```|NVMe|
|```ScalablePMEM```|Scalable PMEM|

**NvmeDrive3 (NVMe Drive 3)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to configure different NVM Express Drives Usage. When NVMe is selected, NVM Express Drive is used as storage device. When Scalable PMEM is selected, NVM Express Drive is used as Logical NVDIMM Backup/Restore device.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Nvme```|NVMe|
|```ScalablePMEM```|Scalable PMEM|

**NvmeDrive30 (NVMe Drive 30)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to configure different NVM Express Drives Usage. When NVMe is selected, NVM Express Drive is used as storage device. When Scalable PMEM is selected, NVM Express Drive is used as Logical NVDIMM Backup/Restore device.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Nvme```|NVMe|
|```ScalablePMEM```|Scalable PMEM|

**NvmeDrive31 (NVMe Drive 31)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to configure different NVM Express Drives Usage. When NVMe is selected, NVM Express Drive is used as storage device. When Scalable PMEM is selected, NVM Express Drive is used as Logical NVDIMM Backup/Restore device.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Nvme```|NVMe|
|```ScalablePMEM```|Scalable PMEM|

**NvmeDrive32 (NVMe Drive 32)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to configure different NVM Express Drives Usage. When NVMe is selected, NVM Express Drive is used as storage device. When Scalable PMEM is selected, NVM Express Drive is used as Logical NVDIMM Backup/Restore device.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Nvme```|NVMe|
|```ScalablePMEM```|Scalable PMEM|

**NvmeDrive33 (NVMe Drive 33)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to configure different NVM Express Drives Usage. When NVMe is selected, NVM Express Drive is used as storage device. When Scalable PMEM is selected, NVM Express Drive is used as Logical NVDIMM Backup/Restore device.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Nvme```|NVMe|
|```ScalablePMEM```|Scalable PMEM|

**NvmeDrive34 (NVMe Drive 34)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to configure different NVM Express Drives Usage. When NVMe is selected, NVM Express Drive is used as storage device. When Scalable PMEM is selected, NVM Express Drive is used as Logical NVDIMM Backup/Restore device.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Nvme```|NVMe|
|```ScalablePMEM```|Scalable PMEM|

**NvmeDrive35 (NVMe Drive 35)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to configure different NVM Express Drives Usage. When NVMe is selected, NVM Express Drive is used as storage device. When Scalable PMEM is selected, NVM Express Drive is used as Logical NVDIMM Backup/Restore device.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Nvme```|NVMe|
|```ScalablePMEM```|Scalable PMEM|

**NvmeDrive36 (NVMe Drive 36)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to configure different NVM Express Drives Usage. When NVMe is selected, NVM Express Drive is used as storage device. When Scalable PMEM is selected, NVM Express Drive is used as Logical NVDIMM Backup/Restore device.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Nvme```|NVMe|
|```ScalablePMEM```|Scalable PMEM|

**NvmeDrive37 (NVMe Drive 37)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to configure different NVM Express Drives Usage. When NVMe is selected, NVM Express Drive is used as storage device. When Scalable PMEM is selected, NVM Express Drive is used as Logical NVDIMM Backup/Restore device.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Nvme```|NVMe|
|```ScalablePMEM```|Scalable PMEM|

**NvmeDrive38 (NVMe Drive 38)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to configure different NVM Express Drives Usage. When NVMe is selected, NVM Express Drive is used as storage device. When Scalable PMEM is selected, NVM Express Drive is used as Logical NVDIMM Backup/Restore device.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Nvme```|NVMe|
|```ScalablePMEM```|Scalable PMEM|

**NvmeDrive39 (NVMe Drive 39)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to configure different NVM Express Drives Usage. When NVMe is selected, NVM Express Drive is used as storage device. When Scalable PMEM is selected, NVM Express Drive is used as Logical NVDIMM Backup/Restore device.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Nvme```|NVMe|
|```ScalablePMEM```|Scalable PMEM|

**NvmeDrive4 (NVMe Drive 4)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to configure different NVM Express Drives Usage. When NVMe is selected, NVM Express Drive is used as storage device. When Scalable PMEM is selected, NVM Express Drive is used as Logical NVDIMM Backup/Restore device.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Nvme```|NVMe|
|```ScalablePMEM```|Scalable PMEM|

**NvmeDrive40 (NVMe Drive 40)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to configure different NVM Express Drives Usage. When NVMe is selected, NVM Express Drive is used as storage device. When Scalable PMEM is selected, NVM Express Drive is used as Logical NVDIMM Backup/Restore device.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Nvme```|NVMe|
|```ScalablePMEM```|Scalable PMEM|

**NvmeDrive41 (NVMe Drive 41)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to configure different NVM Express Drives Usage. When NVMe is selected, NVM Express Drive is used as storage device. When Scalable PMEM is selected, NVM Express Drive is used as Logical NVDIMM Backup/Restore device.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Nvme```|NVMe|
|```ScalablePMEM```|Scalable PMEM|

**NvmeDrive42 (NVMe Drive 42)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to configure different NVM Express Drives Usage. When NVMe is selected, NVM Express Drive is used as storage device. When Scalable PMEM is selected, NVM Express Drive is used as Logical NVDIMM Backup/Restore device.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Nvme```|NVMe|
|```ScalablePMEM```|Scalable PMEM|

**NvmeDrive43 (NVMe Drive 43)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to configure different NVM Express Drives Usage. When NVMe is selected, NVM Express Drive is used as storage device. When Scalable PMEM is selected, NVM Express Drive is used as Logical NVDIMM Backup/Restore device.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Nvme```|NVMe|
|```ScalablePMEM```|Scalable PMEM|

**NvmeDrive44 (NVMe Drive 44)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to configure different NVM Express Drives Usage. When NVMe is selected, NVM Express Drive is used as storage device. When Scalable PMEM is selected, NVM Express Drive is used as Logical NVDIMM Backup/Restore device.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Nvme```|NVMe|
|```ScalablePMEM```|Scalable PMEM|

**NvmeDrive45 (NVMe Drive 45)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to configure different NVM Express Drives Usage. When NVMe is selected, NVM Express Drive is used as storage device. When Scalable PMEM is selected, NVM Express Drive is used as Logical NVDIMM Backup/Restore device.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Nvme```|NVMe|
|```ScalablePMEM```|Scalable PMEM|

**NvmeDrive46 (NVMe Drive 46)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to configure different NVM Express Drives Usage. When NVMe is selected, NVM Express Drive is used as storage device. When Scalable PMEM is selected, NVM Express Drive is used as Logical NVDIMM Backup/Restore device.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Nvme```|NVMe|
|```ScalablePMEM```|Scalable PMEM|

**NvmeDrive47 (NVMe Drive 47)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to configure different NVM Express Drives Usage. When NVMe is selected, NVM Express Drive is used as storage device. When Scalable PMEM is selected, NVM Express Drive is used as Logical NVDIMM Backup/Restore device.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Nvme```|NVMe|
|```ScalablePMEM```|Scalable PMEM|

**NvmeDrive48 (NVMe Drive 48)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to configure different NVM Express Drives Usage. When NVMe is selected, NVM Express Drive is used as storage device. When Scalable PMEM is selected, NVM Express Drive is used as Logical NVDIMM Backup/Restore device.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Nvme```|NVMe|
|```ScalablePMEM```|Scalable PMEM|

**NvmeDrive49 (NVMe Drive 49)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to configure different NVM Express Drives Usage. When NVMe is selected, NVM Express Drive is used as storage device. When Scalable PMEM is selected, NVM Express Drive is used as Logical NVDIMM Backup/Restore device.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Nvme```|NVMe|
|```ScalablePMEM```|Scalable PMEM|

**NvmeDrive5 (NVMe Drive 5)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to configure different NVM Express Drives Usage. When NVMe is selected, NVM Express Drive is used as storage device. When Scalable PMEM is selected, NVM Express Drive is used as Logical NVDIMM Backup/Restore device.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Nvme```|NVMe|
|```ScalablePMEM```|Scalable PMEM|

**NvmeDrive50 (NVMe Drive 50)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to configure different NVM Express Drives Usage. When NVMe is selected, NVM Express Drive is used as storage device. When Scalable PMEM is selected, NVM Express Drive is used as Logical NVDIMM Backup/Restore device.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Nvme```|NVMe|
|```ScalablePMEM```|Scalable PMEM|

**NvmeDrive6 (NVMe Drive 6)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to configure different NVM Express Drives Usage. When NVMe is selected, NVM Express Drive is used as storage device. When Scalable PMEM is selected, NVM Express Drive is used as Logical NVDIMM Backup/Restore device.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Nvme```|NVMe|
|```ScalablePMEM```|Scalable PMEM|

**NvmeDrive7 (NVMe Drive 7)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to configure different NVM Express Drives Usage. When NVMe is selected, NVM Express Drive is used as storage device. When Scalable PMEM is selected, NVM Express Drive is used as Logical NVDIMM Backup/Restore device.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Nvme```|NVMe|
|```ScalablePMEM```|Scalable PMEM|

**NvmeDrive8 (NVMe Drive 8)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to configure different NVM Express Drives Usage. When NVMe is selected, NVM Express Drive is used as storage device. When Scalable PMEM is selected, NVM Express Drive is used as Logical NVDIMM Backup/Restore device.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Nvme```|NVMe|
|```ScalablePMEM```|Scalable PMEM|

**NvmeDrive9 (NVMe Drive 9)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to configure different NVM Express Drives Usage. When NVMe is selected, NVM Express Drive is used as storage device. When Scalable PMEM is selected, NVM Express Drive is used as Logical NVDIMM Backup/Restore device.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Nvme```|NVMe|
|```ScalablePMEM```|Scalable PMEM|

**NvmeOptionRom (Embedded NVM Express Option ROM)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to enable or disable embedded NVM Express Option ROM. When enabled, the system loads the NVM Express Option ROM provided by the system BIOS. When disabled, the system loads the NVM Express Option ROM provided by the adapter.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Enabled```|Enabled|
|```Disabled```|Disabled|

**OldAdminPassword (Enter previous Admin Password)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|In order to set a new Admin Password, the previous Admin Password must be specified.|
|Type|Password|
|Read Only|False|

**OldPowerOnPassword (Enter previous Power On Password)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|In order to set a new Power On Password, the previous Power On Password must be specified.|
|Type|Password|
|Read Only|False|

**PciResourcePadding (NVMe PCIe Resource Padding)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to configure PCIe resources to support PCIe hot-add for NVMe drives. When Normal is selected, PCIe resources are only allocated to devices installed at boot time, and PCIe hot-add is not supported. When Medium is selected, additional PCIe resources are allocated for each PCIe Root Port, which might enable a PCIe hot-add event to work without requiring a system reboot to enumerate the device. When High is selected, a maximum amount of PCIe resources are set aside to allow for the best chance of supporting a PCIe hot-add event.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Normal```|Normal|
|```Medium```|Medium|
|```High```|High|

**PciSlot1Aspm (PCIe Power Management(ASPM))**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to configure the PCIe Link Power Management (ASPM) support for the selected device. When configured for L0s Enabled, the selected device's link enters a standby energy savings state. When configured for L1 Enabled, the selected device's link enters a lower power standby state at the expense of a longer exit latency. When configured for L1 and L0s Enabled, the selected device's link enters either power savings mode, depending on link utilization, and provides the highest energy savings.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Auto```|Auto|
|```Disabled```|Disabled|
|```AspmL1Enabled```|L1 Enabled|

**PciSlot1Enable (PCIe Device Disable)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Select this option to enable or disable PCI devices.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Auto```|Auto|
|```Disabled```|Disabled|

**PciSlot1LinkSpeed (PCIe Link Speed)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to configure the PCIe Link Speed for the selected device. When configured for Auto, the selected device trains at the maximum supported speed of the PCIe link. When configured for PCIe Generation 2 Link Speed, the selected device trains at a maximum of PCIe Generation 2 speed. When configured for PCIe Generation  Link 1 speed, the selected device trains at a maximum of PCIe Generation 1 speed.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Auto```|Auto|
|```PcieGen1```|PCIe Generation 1.0|
|```PcieGen2```|PCIe Generation 2.0|

**PciSlot1OptionROM (PCIe Option ROM)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to enable or disable Device Option ROM |
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Enabled```|Enabled|
|```Disabled```|Disabled|

**PciSlot2Aspm (PCIe Power Management(ASPM))**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to configure the PCIe Link Power Management (ASPM) support for the selected device. When configured for L0s Enabled, the selected device's link enters a standby energy savings state. When configured for L1 Enabled, the selected device's link enters a lower power standby state at the expense of a longer exit latency. When configured for L1 and L0s Enabled, the selected device's link enters either power savings mode, depending on link utilization, and provides the highest energy savings.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Auto```|Auto|
|```Disabled```|Disabled|
|```AspmL1Enabled```|L1 Enabled|

**PciSlot2Enable (PCIe Device Disable)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Select this option to enable or disable PCI devices.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Auto```|Auto|
|```Disabled```|Disabled|

**PciSlot2LinkSpeed (PCIe Link Speed)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to configure the PCIe Link Speed for the selected device. When configured for Auto, the selected device trains at the maximum supported speed of the PCIe link. When configured for PCIe Generation 2 Link Speed, the selected device trains at a maximum of PCIe Generation 2 speed. When configured for PCIe Generation  Link 1 speed, the selected device trains at a maximum of PCIe Generation 1 speed.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Auto```|Auto|
|```PcieGen1```|PCIe Generation 1.0|
|```PcieGen2```|PCIe Generation 2.0|

**PciSlot2OptionROM (PCIe Option ROM)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to enable or disable Device Option ROM |
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Enabled```|Enabled|
|```Disabled```|Disabled|

**PciSlot3Aspm (PCIe Power Management(ASPM))**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to configure the PCIe Link Power Management (ASPM) support for the selected device. When configured for L0s Enabled, the selected device's link enters a standby energy savings state. When configured for L1 Enabled, the selected device's link enters a lower power standby state at the expense of a longer exit latency. When configured for L1 and L0s Enabled, the selected device's link enters either power savings mode, depending on link utilization, and provides the highest energy savings.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Auto```|Auto|
|```Disabled```|Disabled|
|```AspmL1Enabled```|L1 Enabled|

**PciSlot3Enable (PCIe Device Disable)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Select this option to enable or disable PCI devices.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Auto```|Auto|
|```Disabled```|Disabled|

**PciSlot3LinkSpeed (PCIe Link Speed)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to configure the PCIe Link Speed for the selected device. When configured for Auto, the selected device trains at the maximum supported speed of the PCIe link. When configured for PCIe Generation 2 Link Speed, the selected device trains at a maximum of PCIe Generation 2 speed. When configured for PCIe Generation  Link 1 speed, the selected device trains at a maximum of PCIe Generation 1 speed.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Auto```|Auto|
|```PcieGen1```|PCIe Generation 1.0|
|```PcieGen2```|PCIe Generation 2.0|

**PciSlot3OptionROM (PCIe Option ROM)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to enable or disable Device Option ROM |
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Enabled```|Enabled|
|```Disabled```|Disabled|

**PciSlot4Aspm (PCIe Power Management(ASPM))**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to configure the PCIe Link Power Management (ASPM) support for the selected device. When configured for L0s Enabled, the selected device's link enters a standby energy savings state. When configured for L1 Enabled, the selected device's link enters a lower power standby state at the expense of a longer exit latency. When configured for L1 and L0s Enabled, the selected device's link enters either power savings mode, depending on link utilization, and provides the highest energy savings.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Auto```|Auto|
|```Disabled```|Disabled|
|```AspmL1Enabled```|L1 Enabled|

**PciSlot4Enable (PCIe Device Disable)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Select this option to enable or disable PCI devices.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Auto```|Auto|
|```Disabled```|Disabled|

**PciSlot4LinkSpeed (PCIe Link Speed)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to configure the PCIe Link Speed for the selected device. When configured for Auto, the selected device trains at the maximum supported speed of the PCIe link. When configured for PCIe Generation 2 Link Speed, the selected device trains at a maximum of PCIe Generation 2 speed. When configured for PCIe Generation  Link 1 speed, the selected device trains at a maximum of PCIe Generation 1 speed.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Auto```|Auto|
|```PcieGen1```|PCIe Generation 1.0|
|```PcieGen2```|PCIe Generation 2.0|

**PciSlot4OptionROM (PCIe Option ROM)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to enable or disable Device Option ROM |
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Enabled```|Enabled|
|```Disabled```|Disabled|

**PciSlot5Aspm (PCIe Power Management(ASPM))**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to configure the PCIe Link Power Management (ASPM) support for the selected device. When configured for L0s Enabled, the selected device's link enters a standby energy savings state. When configured for L1 Enabled, the selected device's link enters a lower power standby state at the expense of a longer exit latency. When configured for L1 and L0s Enabled, the selected device's link enters either power savings mode, depending on link utilization, and provides the highest energy savings.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Auto```|Auto|
|```Disabled```|Disabled|
|```AspmL1Enabled```|L1 Enabled|

**PciSlot5Enable (PCIe Device Disable)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Select this option to enable or disable PCI devices.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Auto```|Auto|
|```Disabled```|Disabled|

**PciSlot5LinkSpeed (PCIe Link Speed)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to configure the PCIe Link Speed for the selected device. When configured for Auto, the selected device trains at the maximum supported speed of the PCIe link. When configured for PCIe Generation 2 Link Speed, the selected device trains at a maximum of PCIe Generation 2 speed. When configured for PCIe Generation  Link 1 speed, the selected device trains at a maximum of PCIe Generation 1 speed.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Auto```|Auto|
|```PcieGen1```|PCIe Generation 1.0|
|```PcieGen2```|PCIe Generation 2.0|

**PciSlot5OptionROM (PCIe Option ROM)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to enable or disable Device Option ROM |
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Enabled```|Enabled|
|```Disabled```|Disabled|

**PciSlot6Aspm (PCIe Power Management(ASPM))**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to configure the PCIe Link Power Management (ASPM) support for the selected device. When configured for L0s Enabled, the selected device's link enters a standby energy savings state. When configured for L1 Enabled, the selected device's link enters a lower power standby state at the expense of a longer exit latency. When configured for L1 and L0s Enabled, the selected device's link enters either power savings mode, depending on link utilization, and provides the highest energy savings.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Auto```|Auto|
|```Disabled```|Disabled|
|```AspmL1Enabled```|L1 Enabled|

**PciSlot6Enable (PCIe Device Disable)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Select this option to enable or disable PCI devices.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Auto```|Auto|
|```Disabled```|Disabled|

**PciSlot6LinkSpeed (PCIe Link Speed)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to configure the PCIe Link Speed for the selected device. When configured for Auto, the selected device trains at the maximum supported speed of the PCIe link. When configured for PCIe Generation 2 Link Speed, the selected device trains at a maximum of PCIe Generation 2 speed. When configured for PCIe Generation  Link 1 speed, the selected device trains at a maximum of PCIe Generation 1 speed.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Auto```|Auto|
|```PcieGen1```|PCIe Generation 1.0|
|```PcieGen2```|PCIe Generation 2.0|

**PciSlot6OptionROM (PCIe Option ROM)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to enable or disable Device Option ROM |
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Enabled```|Enabled|
|```Disabled```|Disabled|

**PciSlot7Aspm (PCIe Power Management(ASPM))**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to configure the PCIe Link Power Management (ASPM) support for the selected device. When configured for L0s Enabled, the selected device's link enters a standby energy savings state. When configured for L1 Enabled, the selected device's link enters a lower power standby state at the expense of a longer exit latency. When configured for L1 and L0s Enabled, the selected device's link enters either power savings mode, depending on link utilization, and provides the highest energy savings.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Auto```|Auto|
|```Disabled```|Disabled|
|```AspmL1Enabled```|L1 Enabled|

**PciSlot7Enable (PCIe Device Disable)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Select this option to enable or disable PCI devices.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Auto```|Auto|
|```Disabled```|Disabled|

**PciSlot7LinkSpeed (PCIe Link Speed)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to configure the PCIe Link Speed for the selected device. When configured for Auto, the selected device trains at the maximum supported speed of the PCIe link. When configured for PCIe Generation 2 Link Speed, the selected device trains at a maximum of PCIe Generation 2 speed. When configured for PCIe Generation  Link 1 speed, the selected device trains at a maximum of PCIe Generation 1 speed.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Auto```|Auto|
|```PcieGen1```|PCIe Generation 1.0|
|```PcieGen2```|PCIe Generation 2.0|

**PciSlot7OptionROM (PCIe Option ROM)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to enable or disable Device Option ROM |
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Enabled```|Enabled|
|```Disabled```|Disabled|

**PciSlot8Aspm (PCIe Power Management(ASPM))**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to configure the PCIe Link Power Management (ASPM) support for the selected device. When configured for L0s Enabled, the selected device's link enters a standby energy savings state. When configured for L1 Enabled, the selected device's link enters a lower power standby state at the expense of a longer exit latency. When configured for L1 and L0s Enabled, the selected device's link enters either power savings mode, depending on link utilization, and provides the highest energy savings.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Auto```|Auto|
|```Disabled```|Disabled|
|```AspmL1Enabled```|L1 Enabled|

**PciSlot8Enable (PCIe Device Disable)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Select this option to enable or disable PCI devices.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Auto```|Auto|
|```Disabled```|Disabled|

**PciSlot8LinkSpeed (PCIe Link Speed)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to configure the PCIe Link Speed for the selected device. When configured for Auto, the selected device trains at the maximum supported speed of the PCIe link. When configured for PCIe Generation 2 Link Speed, the selected device trains at a maximum of PCIe Generation 2 speed. When configured for PCIe Generation  Link 1 speed, the selected device trains at a maximum of PCIe Generation 1 speed.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Auto```|Auto|
|```PcieGen1```|PCIe Generation 1.0|
|```PcieGen2```|PCIe Generation 2.0|

**PciSlot8OptionROM (PCIe Option ROM)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to enable or disable Device Option ROM |
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Enabled```|Enabled|
|```Disabled```|Disabled|

**PersistentMemAddressRangeScrub (Persistent Memory Address Range Scrub)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to configure the NVDIMM memory Address Range Scrub support. When enabled, this option allows a supported OS to attempt recovery from an uncorrectable memory error detected in the NVDIMM memory. When disabled, the NVDIMM memory will be disabled on the following boot after detecting an uncorrectable memory error in the NVDIMM. If the NVDIMM memory Memory Interleaving option is enabled, a disabled NVDIMM will include all the modules or regions within the set.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Enabled```|Enabled|
|```Disabled```|Disabled|

**PersistentMemBackupPowerPolicy (Persistent Memory Backup Power Policy)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|This option controls whether the system waits during system boot for batteries to charge if sufficient battery backup power for the installed persistent memory is not available. If this option is configured for 'Continue Boot without Backup Power', the server boots even if sufficient battery backup power is not installed. In this case, if sufficient battery backup power is not enabled, the configured memory will NOT be used by the operating system as persistent storage or as system memory.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```WaitForBackupPower```|Wait for Backup Power on Boot|
|```BootWithoutBackupPower```|Continue Boot without Backup Power|

**PersistentMemScanMem (Persistent Memory Integrity Check)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|When this option is enabled, persistent memory will be checked during system boot to determine data integrity. Depending on the Persistent Memory Address Range Scrub setting, discovered errors during the data integrity check will either be presented to the operating system for recovery or cause the persistent memory to be mapped out and unavailable to the operating system. If this option is disabled, any persistent memory which has issues with the ability to read data or which has bad data may result in uncorrectable errors that result in a system crash. 
 If this option is disabled, Persistent Memory Address Range Scrub functionality might be impacted.For NVDIMM-N, this option will be automatically enabled if Persistent Memory Address Range Scrub functionality is enabled.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Enabled```|Enabled|
|```Disabled```|Disabled|

**PostBootProgress (POST Verbose Boot Progress)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to enable verbose boot progress messaging. Because this option displays additional debug information to the screen and serial console, it might be helpful for determining why a server became unresponsive during the boot process.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Disabled```|Disabled|
|```Serial```|Serial Only|
|```All```|All|

**PostDiscoveryMode (UEFI POST Discovery Mode)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to configure the UEFI POST Discovery Mode. When Auto is selected, the system selectively starts devices which are required for booting the devices in the UEFI Boot Order list. Note: For some situations like system configuration change, the system will change to start all devices for discovering all boot devices. When Force Full Discovery is selected, the system starts all devices in the system providing full boot target availability. Note: When Force Full Discovery is selected, boot time might significantly increase. When Force Fast Discovery is selected, the system starts as few devices as possible to get minimal boot time. Note: When Force Fast Discovery is selected, some unsupported devices may not work properly. You may need to replace the unsupported device with one that supports Fast Discovery.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Auto```|Auto|
|```ForceFullDiscovery```|Force Full Discovery|
|```ForceFastDiscovery```|Force Fast Discovery|

**PostF1Prompt (POST F1 Prompt)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to configure the system to display the F1 key on the server POST screen. If an error is encountered, you can press the F1 key to continue with the server power-up sequence. Select one of the following options: 
Delayed 20 Seconds - If an error occurs, the system pauses for 20 seconds at the F1 prompt and continues to boot the OS. 
Delayed 2 Seconds - If an error occurs, the system pauses for 2 seconds at the F1 prompt and continues to boot the OS. 
Disabled - If an error occurs, the system bypasses the F1 prompt and continues to boot the OS. 
Note: For critical errors, the system pauses for 20 seconds at the F1 prompt, regardless of how this option is configured.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Delayed20Sec```|Delayed 20 seconds|
|```Delayed2Sec```|Delayed 2 seconds|
|```Disabled```|Disabled|

**PowerButton (Power Button Mode)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Disabling this option disables the momentary power button functionality. This option does not affect the four-second power button override or the remote power control functionality.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Enabled```|Enabled|
|```Disabled```|Disabled|

**PowerOnDelay (Power-On Delay)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to delay the server from turning on for a specified time. Pressing the power button (using the Virtual Power Button), or Wake-ON LAN events, and RTC Wake-up events override the delay and power on the server without any additional delay. This enablesstaggering when servers power-up after a power loss to prevent power usage spikes.Note that the actual delay before the server is powered on will be longer than the specifiedtime because the server must always wait for iLO FW to initialize before the server attempts to power on.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```NoDelay```|No Delay|
|```Random```|Random Delay|
|```Delay15Sec```|15 Second Delay|
|```Delay30Sec```|30 Second Delay|
|```Delay45Sec```|45 Second Delay|
|```Delay60Sec```|60 Second Delay|

**PowerOnPassword (Set Power On Password)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|When the server powers on, a prompt is displayed to enter a password before continuing the boot process. In the event of an ASR reboot, the Power-On Password is bypassed, and the server boots normally.|
|Type|Password|
|Read Only|False|

**PowerRegulator (Power Regulator)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|You can only configure this option if the Workload Profile is set to Custom. Use this option to configure the following Power Regulator support: 
- Dynamic Power Savings Mode: Automatically varies processor speed and power usage based on processor utilization. Enables the reduction of overall power consumption with little or no impact on performance. Does not require OS support. 
- Static Low Power Mode: Reduces processor speed and power usage. Guarantees a lower maximum power usage for the system. Performance impacts are greater for environments with higher processor utilization. 
- Static High Performance Mode: Processors run in their maximum power/performance state at all times, regardless of the OS power management policy. 
- OS Control Mode: Processors run in their maximum power/performance state at all times unless the OS enables a power management policy.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```DynamicPowerSavings```|Dynamic Power Savings Mode|
|```StaticLowPower```|Static Low Power Mode|
|```StaticHighPerf```|Static High Performance Mode|
|```OsControl```|OS Control Mode|

**PreBootNetwork (Pre-Boot Network Interface)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to select the network interface used for pre-boot network connections. When the selection is Auto, the system uses the first available port with a network connection.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Auto```|Auto|
|```EmbNicPort1```|Embedded NIC Port 1|
|```EmbNicPort2```|Embedded NIC Port 2|
|```EmbNicPort3```|Embedded NIC Port 3|
|```EmbNicPort4```|Embedded NIC Port 4|
|```EmbNicPort5```|Embedded NIC Port 5|
|```EmbNicPort6```|Embedded NIC Port 6|
|```EmbNicPort7```|Embedded NIC Port 7|
|```EmbNicPort8```|Embedded NIC Port 8|
|```FlexLom1Port1```|Embedded FlexibleLOM 1 Port 1|
|```FlexLom1Port2```|Embedded FlexibleLOM 1 Port 2|
|```FlexLom1Port3```|Embedded FlexibleLOM 1 Port 3|
|```FlexLom1Port4```|Embedded FlexibleLOM 1 Port 4|
|```FlexLom1Port5```|Embedded FlexibleLOM 1 Port 5|
|```FlexLom1Port6```|Embedded FlexibleLOM 1 Port 6|
|```FlexLom1Port7```|Embedded FlexibleLOM 1 Port 7|
|```FlexLom1Port8```|Embedded FlexibleLOM 1 Port 8|
|```Slot1NicPort1```|Slot 1 NIC Port 1|
|```Slot1NicPort2```|Slot 1 NIC Port 2|
|```Slot1NicPort3```|Slot 1 NIC Port 3|
|```Slot1NicPort4```|Slot 1 NIC Port 4|
|```Slot1NicPort5```|Slot 1 NIC Port 5|
|```Slot1NicPort6```|Slot 1 NIC Port 6|
|```Slot1NicPort7```|Slot 1 NIC Port 7|
|```Slot1NicPort8```|Slot 1 NIC Port 8|
|```Slot2NicPort1```|Slot 2 NIC Port 1|
|```Slot2NicPort2```|Slot 2 NIC Port 2|
|```Slot2NicPort3```|Slot 2 NIC Port 3|
|```Slot2NicPort4```|Slot 2 NIC Port 4|
|```Slot2NicPort5```|Slot 2 NIC Port 5|
|```Slot2NicPort6```|Slot 2 NIC Port 6|
|```Slot2NicPort7```|Slot 2 NIC Port 7|
|```Slot2NicPort8```|Slot 2 NIC Port 8|
|```Slot3NicPort1```|Slot 3 NIC Port 1|
|```Slot3NicPort2```|Slot 3 NIC Port 2|
|```Slot3NicPort3```|Slot 3 NIC Port 3|
|```Slot3NicPort4```|Slot 3 NIC Port 4|
|```Slot3NicPort5```|Slot 3 NIC Port 5|
|```Slot3NicPort6```|Slot 3 NIC Port 6|
|```Slot3NicPort7```|Slot 3 NIC Port 7|
|```Slot3NicPort8```|Slot 3 NIC Port 8|
|```Slot4NicPort1```|Slot 4 NIC Port 1|
|```Slot4NicPort2```|Slot 4 NIC Port 2|
|```Slot4NicPort3```|Slot 4 NIC Port 3|
|```Slot4NicPort4```|Slot 4 NIC Port 4|
|```Slot4NicPort5```|Slot 4 NIC Port 5|
|```Slot4NicPort6```|Slot 4 NIC Port 6|
|```Slot4NicPort7```|Slot 4 NIC Port 7|
|```Slot4NicPort8```|Slot 4 NIC Port 8|
|```Slot5NicPort1```|Slot 5 NIC Port 1|
|```Slot5NicPort2```|Slot 5 NIC Port 2|
|```Slot5NicPort3```|Slot 5 NIC Port 3|
|```Slot5NicPort4```|Slot 5 NIC Port 4|
|```Slot5NicPort5```|Slot 5 NIC Port 5|
|```Slot5NicPort6```|Slot 5 NIC Port 6|
|```Slot5NicPort7```|Slot 5 NIC Port 7|
|```Slot5NicPort8```|Slot 5 NIC Port 8|
|```Slot6NicPort1```|Slot 6 NIC Port 1|
|```Slot6NicPort2```|Slot 6 NIC Port 2|
|```Slot6NicPort3```|Slot 6 NIC Port 3|
|```Slot6NicPort4```|Slot 6 NIC Port 4|
|```Slot6NicPort5```|Slot 6 NIC Port 5|
|```Slot6NicPort6```|Slot 6 NIC Port 6|
|```Slot6NicPort7```|Slot 6 NIC Port 7|
|```Slot6NicPort8```|Slot 6 NIC Port 8|
|```Slot7NicPort1```|Slot 7 NIC Port 1|
|```Slot7NicPort2```|Slot 7 NIC Port 2|
|```Slot7NicPort3```|Slot 7 NIC Port 3|
|```Slot7NicPort4```|Slot 7 NIC Port 4|
|```Slot7NicPort5```|Slot 7 NIC Port 5|
|```Slot7NicPort6```|Slot 7 NIC Port 6|
|```Slot7NicPort7```|Slot 7 NIC Port 7|
|```Slot7NicPort8```|Slot 7 NIC Port 8|
|```Slot8NicPort1```|Slot 8 NIC Port 1|
|```Slot8NicPort2```|Slot 8 NIC Port 2|
|```Slot8NicPort3```|Slot 8 NIC Port 3|
|```Slot8NicPort4```|Slot 8 NIC Port 4|
|```Slot8NicPort5```|Slot 8 NIC Port 5|
|```Slot8NicPort6```|Slot 8 NIC Port 6|
|```Slot8NicPort7```|Slot 8 NIC Port 7|
|```Slot8NicPort8```|Slot 8 NIC Port 8|

**PrebootNetworkEnvPolicy (Pre-Boot Network Environment)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to set the preference for Pre-Boot Network.
If configured for Auto, all the network operations initiated in the pre boot environment occur over IPv4 or IPv6. The order of the existing network boot targets is not modified in the UEFI Boot Order list. New network boot targets are added to the end of the list using the default policy of the System BIOS.
If configured for IPv4, all the network operations initiated in the pre boot environment only occur over IPv4. All existing IPv6 network boot targets are removed in the UEFI Boot Order. No new IPv6 network boot targets are added to the list.
If configured for IPv6, all the network operations initiated in the pre boot environment only occur over IPv6. All existing IPv4 network boot targets in the UEFI Boot Order are removed. No new IPv4 network boot targets are added to the list.
|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Auto```|Auto|
|```IPv4```|IPv4|
|```IPv6```|IPv6|

**PrebootNetworkProxy (Pre-Boot Network Proxy)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to configure a pre-boot network proxy. When set, network operations for 'Pre-Boot Network Interface' are attempted through the configured proxy. The proxy must be in a HTTP URL format, and can be specified as http://IPv4_address:port, http://IPv6 address:port or http://FQDN:port.|
|Type|String|
|Read Only|False|

**ProcAes (Processor AES-NI Support)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to enable or disable the Advanced Encryption Standard Instruction Set (AES-NI) in the processor.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Enabled```|Enabled|
|```Disabled```|Disabled|

**ProcHyperthreading (Intel(R) Hyper-Threading)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to enable or disable Intel Hyper-Threading. When enabled, each physical processor core operates as two logical processor cores. When disabled, each physical processor core operates as one logical processor core. Enabling this option can improve overall performance for applications that benefit from a higher processor core count.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Enabled```|Enabled|
|```Disabled```|Disabled|

**ProcTurbo (Intel(R) Turbo Boost Technology)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Turbo Boost Technology enables the processor to transition to a higher frequency than the processor's rated speed if the processor has available power and is within temperature specifications. Disabling this option reduces power usage, and also reduces the system's maximum achievable performance under some workloads.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Disabled```|Disabled|
|```Enabled```|Enabled|

**ProcVirtualization (Intel(R) Virtualization Technology (Intel VT) )**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|When enabled, a hypervisor or operating system supporting this option can use hardware capabilities provided by Intel VT. Some hypervisors require that you enable Intel VT. You can leave this set to enabled even if you are not using a hypervisor or an |
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Enabled```|Enabled|
|```Disabled```|Disabled|

**ProcX2Apic (Processor x2APIC Support)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|x2APIC support enables operating systems to run more efficiently on high core count configurations. It also optimizes interrupt distribution in virtualized environments. In most cases, set this option to enabled. This configures the operating system to optionally enable x2APIC support when it loads. Some older hypervisors and operating systems might have issues with optional x2APIC support, in which case disabling x2APIC might be necessary to address those issues. Additionally, some hypervisors and operating systems will not use X2APIC unless this option is set to Force Enabled prior to booting.  The Force Enabled option also causes the Intel(R) VT-d setting to be set to enabled.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Enabled```|Enabled|
|```ForceEnabled```|Force Enabled|
|```Disabled```|Disabled|

**Processor1LogicalNvdimm1SizeGiB (Processor 1: Logical NVDIMM 1 (GB))**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to specify the amount of regular memory, in gigabytes (1,073,741,824 bytes), to allocate for use as a logical NVDIMM for each specified region. Entries for processor pairs represent logical NVDIMMs which may span multiple processors. An attempt will be made to balance these regions across sockets. The processor-specific entries represent Logical NVDIMMs assigned to a designated socket. These regions are allocated from the top of the memory range for each domain.|
|Type|Integer|
|Read Only|False|

**Processor1LogicalNvdimm2SizeGiB (Processor 1: Logical NVDIMM 2 (GB))**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to specify the amount of regular memory, in gigabytes (1,073,741,824 bytes), to allocate for use as a logical NVDIMM for each specified region. Entries for processor pairs represent logical NVDIMMs which may span multiple processors. An attempt will be made to balance these regions across sockets. The processor-specific entries represent Logical NVDIMMs assigned to a designated socket. These regions are allocated from the top of the memory range for each domain.|
|Type|Integer|
|Read Only|False|

**Processor1ScalablePmemAvailableGiB (Processor 1: Persistent Memory Available (GB))**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Displays the maximum amount of persistent memory available in the system. The 'Total Available' value represents the amount of total system memory available for use as persistent memory.  The processor-specific values represent the amount of domain (socket) specific system memory that is available for use as logical NVDIMMs. The 'Storage' value represents the total size available on the backup device(s) for storing persistent memory.  All values are in gigabytes (1,073,741,824 bytes).|
|Type|Integer|
|Read Only|True|

**Processor2LogicalNvdimm1SizeGiB (Processor 2: Logical NVDIMM 1 (GB))**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to specify the amount of regular memory, in gigabytes (1,073,741,824 bytes), to allocate for use as a logical NVDIMM for each specified region. Entries for processor pairs represent logical NVDIMMs which may span multiple processors. An attempt will be made to balance these regions across sockets. The processor-specific entries represent Logical NVDIMMs assigned to a designated socket. These regions are allocated from the top of the memory range for each domain.|
|Type|Integer|
|Read Only|False|

**Processor2LogicalNvdimm2SizeGiB (Processor 2: Logical NVDIMM 2 (GB))**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to specify the amount of regular memory, in gigabytes (1,073,741,824 bytes), to allocate for use as a logical NVDIMM for each specified region. Entries for processor pairs represent logical NVDIMMs which may span multiple processors. An attempt will be made to balance these regions across sockets. The processor-specific entries represent Logical NVDIMMs assigned to a designated socket. These regions are allocated from the top of the memory range for each domain.|
|Type|Integer|
|Read Only|False|

**Processor2ScalablePmemAvailableGiB (Processor 2: Persistent Memory Available (GB))**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Displays the maximum amount of persistent memory available in the system. The 'Total Available' value represents the amount of total system memory available for use as persistent memory.  The processor-specific values represent the amount of domain (socket) specific system memory that is available for use as logical NVDIMMs. The 'Storage' value represents the total size available on the backup device(s) for storing persistent memory.  All values are in gigabytes (1,073,741,824 bytes).|
|Type|Integer|
|Read Only|True|

**ProcessorJitterControl (Processor Jitter Control)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Processor Jitter Control allows the customer to manage processor frequency variance to do technologies such as Turbo which vary the frequency based on power, thermals, and active cores. When configured for Auto-tuned, the platform will monitor frequency variance and automatically make adjustments to minimize variance over time. When configured for Manual-tuned, the customer can choose to attempt to operate the processor at a fixed frequency and can select lower or higher frequencies statically. |
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Disabled```|Disabled|
|```Auto-tuned```|Auto-tuned|
|```Manual-tuned```|Manual-tuned|

**ProcessorJitterControlFrequency (Processor Jitter Control Frequency)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Processor Jitter Control Frequency allows the customer to stipulate the starting frequency in the Auto-tuned mode, or the desired frequency in the Manual-tuned mode. The input frequency is in units of Megahertz. System firmware will adjust the frequency to the nearest higher intermediate frequency supported by the processor if the input frequency is not supported.|
|Type|Integer|
|Read Only|False|

**ProductId (Product ID)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to set the system product ID. This value must always match the product ID sticker located on the chassis.|
|Type|String|
|Read Only|False|

**RedundantPowerSupply (Redundant Power Supply Mode)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to configure how the system handles redundant power supply configurations. Balanced Mode shares the power delivery equally between all installed power supplies. All High Efficiency Mode options provide the most power efficient operation with redundant power supplies by keeping half of the power supplies in standby mode at lower power usage levels. The High Efficiency Mode options enable the system to select which power supply to place in standby. Auto enables the system to select between the odd or even power supply based on a semi-random distribution within a group of systems.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```BalancedMode```|Balanced Mode|
|```HighEfficiencyAuto```|High Efficiency Mode (Auto)|
|```HighEfficiencyOddStandby```|High Efficiency Mode (Odd Supply Standby)|
|```HighEfficiencyEvenStandby```|High Efficiency Mode (Even Supply Standby)|

**RemovableFlashBootSeq (Removable Flash Media Boot Sequence)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to select which USB or SD Card devices you want to search for first when enumerating boot devices. You can select whether the system boots to external USB drive keys, internal USB drive keys, or the internal SD card slot. This option does not override the device boot order in the Standard Boot Order (IPL) option. You can only configure this option when Boot Mode is set to Legacy BIOS.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```InternalSdCardFirst```|Internal SD Card First|
|```InternalKeysFirst```|Internal DriveKeys First|
|```ExternalKeysFirst```|External DriveKeys First|

**RestoreDefaults (Restore Default System Settings)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to reset all configuration settings to their default values. Changes that have been made might be lost. You must reboot the system for changes to take effect.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```No```|No, cancel the restore procedure.|
|```Yes```|Yes, restore the default settings.|

**RestoreManufacturingDefaults (Restore Default Manufacturing Settings)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to reset all configuration settings to their default manufacturing values. Changes that have been made might be lost. If Secure Boot is enabled, related security settings might be lost. You must reboot the system for changes to take effect.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```No```|No, cancel restore procedure.|
|```Yes```|Yes, restore the default settings.|

**RomSelection (ROM Selection)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to revert the server to a previous BIOS ROM image. The backup image is the BIOS ROM image that was used prior to the last flash event.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```CurrentRom```|Use Current ROM|
|```BackupRom```|Switch to Backup ROM|

**SataSecureErase (SATA Secure Erase)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to control whether Secure Erase functionality is supported. When enabled, the Security Freeze Lock command is not sent to supported SATA hard drives, enabling Secure erase to function (the Secure Erase command is supported). This option is only supported when the SATA controller is in AHCI mode. Secure Erase only operates with hard drives that support the Secure Erase command.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Enabled```|Enabled|
|```Disabled```|Disabled|

**SaveUserDefaults (Save User Defaults)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Select this option to save the current settings as the system defaults.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```No```|No, Cancel|
|```Yes```|Yes, Save|

**ScalablePmemCapacity (Scalable Persistent Memory Capacity (GB))**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Total Scalable Persistent Memory Capacity in GB.|
|Type|Integer|
|Read Only|True|

**SecStartBackupImage (Backup ROM Image Authentication)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to enable cryptographic authentication of the backup ROM image on startup. When this option is disabled, only the primary image is authenticated on each startup. Enable this option to also perform cryptographic authentication of the backup ROM image.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Enabled```|Enabled|
|```Disabled```|Disabled|

**SecureBootStatus (Secure Boot Status)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|The current state of Secure Boot configuration.|
|Type|Enumeration|
|Read Only|True|

|Value|Description|
|---|---|
|```Enabled```|Enabled|
|```Disabled```|Disabled|

**SerialConsoleBaudRate (BIOS Serial Console Baud Rate)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|This is the transfer rate at which data is transmitted through the serial port.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```BaudRate9600```|9600|
|```BaudRate19200```|19200|
|```BaudRate38400```|38400|
|```BaudRate57600```|57600|
|```BaudRate115200```|115200|

**SerialConsoleEmulation (BIOS Serial Console Emulation Mode)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to select the emulation mode type. The option you select depends on the emulation you want to use in your serial terminal program (such as HyperTerminal or PuTTy). The BIOS emulation mode must match the mode you select in your terminal program.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Vt100```|VT100|
|```Ansi```|ANSI|
|```Vt100Plus```|VT100+|
|```VtUtf8```|VT-UTF8|

**SerialConsolePort (BIOS Serial Console Port)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to re-direct video and keystrokes through the serial port to OS boot. This option can interfere with non-terminal devices attached to the serial port. In such cases, set this option to disabled. This option is only supported in English language mode when running in the UEFI pre-boot System Utilities.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Auto```|Auto|
|```Disabled```|Disabled|
|```Physical```|Physical Serial Port|
|```Virtual```|Virtual Serial Port|

**SerialNumber (Serial Number)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to set the system serial number. This value must always match the serial number sticker located on the chassis.|
|Type|String|
|Read Only|False|

**ServerAssetTag (Server Asset Tag)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Select this option to modify the Server Asset Tag text line.|
|Type|String|
|Read Only|False|

**ServerName (Server Name)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Select this option to modify the server name text line.|
|Type|String|
|Read Only|False|

**ServerOtherInfo (Server Other Information)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to modify the Other Server text line.|
|Type|String|
|Read Only|False|

**ServerPrimaryOs (Server Primary OS)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to modify the Server Primary OS text line.|
|Type|String|
|Read Only|False|

**ServiceEmail (Service Contact E-mail Address)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Enter the server service contact e-mail address.|
|Type|String|
|Read Only|False|

**ServiceName (Service Contact Name)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Enter the server service contact name text.|
|Type|String|
|Read Only|False|

**ServiceOtherInfo (Service Contact Other Information)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Enter the other server service contact information text.|
|Type|String|
|Read Only|False|

**ServicePhone (Service Contact Phone Number)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Enter the server service contact phone number text.|
|Type|String|
|Read Only|False|

**SetupBrowserSelection (Setup Browser Selection)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Select which setup browser to use: GUI or Text. Auto mode uses text when the user enters RBSU via serial console, and uses GUI via IRC or physical terminal.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```GUI```|GUI|
|```Text```|Text|
|```Auto```|Auto|

**Slot1NicBoot1 (Slot 1 NIC Port 1 Boot)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active. This is applicable only in UEFI Boot Mode.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```NetworkBoot```|Network Boot|
|```Disabled```|Disabled|

**Slot1NicBoot2 (Slot 1 NIC Port 2 Boot)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active. This is applicable only in UEFI Boot Mode.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```NetworkBoot```|Network Boot|
|```Disabled```|Disabled|

**Slot1NicBoot3 (Slot 1 NIC Port 3 Boot)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active. This is applicable only in UEFI Boot Mode.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```NetworkBoot```|Network Boot|
|```Disabled```|Disabled|

**Slot1NicBoot4 (Slot 1 NIC Port 4 Boot)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active. This is applicable only in UEFI Boot Mode.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```NetworkBoot```|Network Boot|
|```Disabled```|Disabled|

**Slot1NicBoot5 (Slot 1 NIC Port 5 Boot)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active. This is applicable only in UEFI Boot Mode.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```NetworkBoot```|Network Boot|
|```Disabled```|Disabled|

**Slot1NicBoot6 (Slot 1 NIC Port 6 Boot)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active. This is applicable only in UEFI Boot Mode.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```NetworkBoot```|Network Boot|
|```Disabled```|Disabled|

**Slot1NicBoot7 (Slot 1 NIC Port 7 Boot)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active. This is applicable only in UEFI Boot Mode.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```NetworkBoot```|Network Boot|
|```Disabled```|Disabled|

**Slot1NicBoot8 (Slot 1 NIC Port 8 Boot)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active. This is applicable only in UEFI Boot Mode.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```NetworkBoot```|Network Boot|
|```Disabled```|Disabled|

**Slot1StorageBoot (PCIe Slot 1)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|When Boot All Targets is selected, all valid boot targets attached to the storage controller are made available in the UEFI Boot Order list. If Boot No Targets is selected, no boot targets from this storage controller are made available in the UEFI Boot Order.If Boot Limit to 24 Targets is selected, 24 boot targets attached to the storage controller are made available in the UEFI Boot Order.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```AllTargets```|Boot All Targets|
|```TwentyFourTargets```|Boot Limit to 24 Targets|
|```NoTargets```|Boot No Targets|

**Slot2NicBoot1 (Slot 2 NIC Port 1 Boot)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active. This is applicable only in UEFI Boot Mode.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```NetworkBoot```|Network Boot|
|```Disabled```|Disabled|

**Slot2NicBoot2 (Slot 2 NIC Port 2 Boot)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active. This is applicable only in UEFI Boot Mode.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```NetworkBoot```|Network Boot|
|```Disabled```|Disabled|

**Slot2NicBoot3 (Slot 2 NIC Port 3 Boot)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active. This is applicable only in UEFI Boot Mode.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```NetworkBoot```|Network Boot|
|```Disabled```|Disabled|

**Slot2NicBoot4 (Slot 2 NIC Port 4 Boot)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active. This is applicable only in UEFI Boot Mode.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```NetworkBoot```|Network Boot|
|```Disabled```|Disabled|

**Slot2NicBoot5 (Slot 2 NIC Port 5 Boot)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active. This is applicable only in UEFI Boot Mode.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```NetworkBoot```|Network Boot|
|```Disabled```|Disabled|

**Slot2NicBoot6 (Slot 2 NIC Port 6 Boot)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active. This is applicable only in UEFI Boot Mode.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```NetworkBoot```|Network Boot|
|```Disabled```|Disabled|

**Slot2NicBoot7 (Slot 2 NIC Port 7 Boot)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active. This is applicable only in UEFI Boot Mode.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```NetworkBoot```|Network Boot|
|```Disabled```|Disabled|

**Slot2NicBoot8 (Slot 2 NIC Port 8 Boot)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active. This is applicable only in UEFI Boot Mode.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```NetworkBoot```|Network Boot|
|```Disabled```|Disabled|

**Slot2StorageBoot (PCIe Slot 2)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|When Boot All Targets is selected, all valid boot targets attached to the storage controller are made available in the UEFI Boot Order list. If Boot No Targets is selected, no boot targets from this storage controller are made available in the UEFI Boot Order.If Boot Limit to 24 Targets is selected, 24 boot targets attached to the storage controller are made available in the UEFI Boot Order.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```AllTargets```|Boot All Targets|
|```TwentyFourTargets```|Boot Limit to 24 Targets|
|```NoTargets```|Boot No Targets|

**Slot3NicBoot1 (Slot 3 NIC Port 1 Boot)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active. This is applicable only in UEFI Boot Mode.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```NetworkBoot```|Network Boot|
|```Disabled```|Disabled|

**Slot3NicBoot2 (Slot 3 NIC Port 2 Boot)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active. This is applicable only in UEFI Boot Mode.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```NetworkBoot```|Network Boot|
|```Disabled```|Disabled|

**Slot3NicBoot3 (Slot 3 NIC Port 3 Boot)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active. This is applicable only in UEFI Boot Mode.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```NetworkBoot```|Network Boot|
|```Disabled```|Disabled|

**Slot3NicBoot4 (Slot 3 NIC Port 4 Boot)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active. This is applicable only in UEFI Boot Mode.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```NetworkBoot```|Network Boot|
|```Disabled```|Disabled|

**Slot3NicBoot5 (Slot 3 NIC Port 5 Boot)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active. This is applicable only in UEFI Boot Mode.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```NetworkBoot```|Network Boot|
|```Disabled```|Disabled|

**Slot3NicBoot6 (Slot 3 NIC Port 6 Boot)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active. This is applicable only in UEFI Boot Mode.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```NetworkBoot```|Network Boot|
|```Disabled```|Disabled|

**Slot3NicBoot7 (Slot 3 NIC Port 7 Boot)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active. This is applicable only in UEFI Boot Mode.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```NetworkBoot```|Network Boot|
|```Disabled```|Disabled|

**Slot3NicBoot8 (Slot 3 NIC Port 8 Boot)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active. This is applicable only in UEFI Boot Mode.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```NetworkBoot```|Network Boot|
|```Disabled```|Disabled|

**Slot3StorageBoot (PCIe Slot 3)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|When Boot All Targets is selected, all valid boot targets attached to the storage controller are made available in the UEFI Boot Order list. If Boot No Targets is selected, no boot targets from this storage controller are made available in the UEFI Boot Order.If Boot Limit to 24 Targets is selected, 24 boot targets attached to the storage controller are made available in the UEFI Boot Order.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```AllTargets```|Boot All Targets|
|```TwentyFourTargets```|Boot Limit to 24 Targets|
|```NoTargets```|Boot No Targets|

**Slot4NicBoot1 (Slot 4 NIC Port 1 Boot)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active. This is applicable only in UEFI Boot Mode.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```NetworkBoot```|Network Boot|
|```Disabled```|Disabled|

**Slot4NicBoot2 (Slot 4 NIC Port 2 Boot)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active. This is applicable only in UEFI Boot Mode.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```NetworkBoot```|Network Boot|
|```Disabled```|Disabled|

**Slot4NicBoot3 (Slot 4 NIC Port 3 Boot)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active. This is applicable only in UEFI Boot Mode.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```NetworkBoot```|Network Boot|
|```Disabled```|Disabled|

**Slot4NicBoot4 (Slot 4 NIC Port 4 Boot)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active. This is applicable only in UEFI Boot Mode.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```NetworkBoot```|Network Boot|
|```Disabled```|Disabled|

**Slot4NicBoot5 (Slot 4 NIC Port 5 Boot)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active. This is applicable only in UEFI Boot Mode.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```NetworkBoot```|Network Boot|
|```Disabled```|Disabled|

**Slot4NicBoot6 (Slot 4 NIC Port 6 Boot)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active. This is applicable only in UEFI Boot Mode.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```NetworkBoot```|Network Boot|
|```Disabled```|Disabled|

**Slot4NicBoot7 (Slot 4 NIC Port 7 Boot)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active. This is applicable only in UEFI Boot Mode.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```NetworkBoot```|Network Boot|
|```Disabled```|Disabled|

**Slot4NicBoot8 (Slot 4 NIC Port 8 Boot)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active. This is applicable only in UEFI Boot Mode.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```NetworkBoot```|Network Boot|
|```Disabled```|Disabled|

**Slot4StorageBoot (PCIe Slot 4)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|When Boot All Targets is selected, all valid boot targets attached to the storage controller are made available in the UEFI Boot Order list. If Boot No Targets is selected, no boot targets from this storage controller are made available in the UEFI Boot Order.If Boot Limit to 24 Targets is selected, 24 boot targets attached to the storage controller are made available in the UEFI Boot Order.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```AllTargets```|Boot All Targets|
|```TwentyFourTargets```|Boot Limit to 24 Targets|
|```NoTargets```|Boot No Targets|

**Slot5NicBoot1 (Slot 5 NIC Port 1 Boot)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active. This is applicable only in UEFI Boot Mode.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```NetworkBoot```|Network Boot|
|```Disabled```|Disabled|

**Slot5NicBoot2 (Slot 5 NIC Port 2 Boot)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active. This is applicable only in UEFI Boot Mode.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```NetworkBoot```|Network Boot|
|```Disabled```|Disabled|

**Slot5NicBoot3 (Slot 5 NIC Port 3 Boot)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active. This is applicable only in UEFI Boot Mode.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```NetworkBoot```|Network Boot|
|```Disabled```|Disabled|

**Slot5NicBoot4 (Slot 5 NIC Port 4 Boot)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active. This is applicable only in UEFI Boot Mode.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```NetworkBoot```|Network Boot|
|```Disabled```|Disabled|

**Slot5NicBoot5 (Slot 5 NIC Port 5 Boot)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active. This is applicable only in UEFI Boot Mode.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```NetworkBoot```|Network Boot|
|```Disabled```|Disabled|

**Slot5NicBoot6 (Slot 5 NIC Port 6 Boot)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active. This is applicable only in UEFI Boot Mode.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```NetworkBoot```|Network Boot|
|```Disabled```|Disabled|

**Slot5NicBoot7 (Slot 5 NIC Port 7 Boot)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active. This is applicable only in UEFI Boot Mode.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```NetworkBoot```|Network Boot|
|```Disabled```|Disabled|

**Slot5NicBoot8 (Slot 5 NIC Port 8 Boot)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active. This is applicable only in UEFI Boot Mode.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```NetworkBoot```|Network Boot|
|```Disabled```|Disabled|

**Slot5StorageBoot (PCIe Slot 5)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|When Boot All Targets is selected, all valid boot targets attached to the storage controller are made available in the UEFI Boot Order list. If Boot No Targets is selected, no boot targets from this storage controller are made available in the UEFI Boot Order.If Boot Limit to 24 Targets is selected, 24 boot targets attached to the storage controller are made available in the UEFI Boot Order.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```AllTargets```|Boot All Targets|
|```TwentyFourTargets```|Boot Limit to 24 Targets|
|```NoTargets```|Boot No Targets|

**Slot6NicBoot1 (Slot 6 NIC Port 1 Boot)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active. This is applicable only in UEFI Boot Mode.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```NetworkBoot```|Network Boot|
|```Disabled```|Disabled|

**Slot6NicBoot2 (Slot 6 NIC Port 2 Boot)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active. This is applicable only in UEFI Boot Mode.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```NetworkBoot```|Network Boot|
|```Disabled```|Disabled|

**Slot6NicBoot3 (Slot 6 NIC Port 3 Boot)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active. This is applicable only in UEFI Boot Mode.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```NetworkBoot```|Network Boot|
|```Disabled```|Disabled|

**Slot6NicBoot4 (Slot 6 NIC Port 4 Boot)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active. This is applicable only in UEFI Boot Mode.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```NetworkBoot```|Network Boot|
|```Disabled```|Disabled|

**Slot6NicBoot5 (Slot 6 NIC Port 5 Boot)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active. This is applicable only in UEFI Boot Mode.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```NetworkBoot```|Network Boot|
|```Disabled```|Disabled|

**Slot6NicBoot6 (Slot 6 NIC Port 6 Boot)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active. This is applicable only in UEFI Boot Mode.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```NetworkBoot```|Network Boot|
|```Disabled```|Disabled|

**Slot6NicBoot7 (Slot 6 NIC Port 7 Boot)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active. This is applicable only in UEFI Boot Mode.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```NetworkBoot```|Network Boot|
|```Disabled```|Disabled|

**Slot6NicBoot8 (Slot 6 NIC Port 8 Boot)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active. This is applicable only in UEFI Boot Mode.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```NetworkBoot```|Network Boot|
|```Disabled```|Disabled|

**Slot6StorageBoot (PCIe Slot 6)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|When Boot All Targets is selected, all valid boot targets attached to the storage controller are made available in the UEFI Boot Order list. If Boot No Targets is selected, no boot targets from this storage controller are made available in the UEFI Boot Order.If Boot Limit to 24 Targets is selected, 24 boot targets attached to the storage controller are made available in the UEFI Boot Order.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```AllTargets```|Boot All Targets|
|```TwentyFourTargets```|Boot Limit to 24 Targets|
|```NoTargets```|Boot No Targets|

**Slot7NicBoot1 (Slot 7 NIC Port 1 Boot)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active. This is applicable only in UEFI Boot Mode.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```NetworkBoot```|Network Boot|
|```Disabled```|Disabled|

**Slot7NicBoot2 (Slot 7 NIC Port 2 Boot)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active. This is applicable only in UEFI Boot Mode.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```NetworkBoot```|Network Boot|
|```Disabled```|Disabled|

**Slot7NicBoot3 (Slot 7 NIC Port 3 Boot)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active. This is applicable only in UEFI Boot Mode.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```NetworkBoot```|Network Boot|
|```Disabled```|Disabled|

**Slot7NicBoot4 (Slot 7 NIC Port 4 Boot)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active. This is applicable only in UEFI Boot Mode.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```NetworkBoot```|Network Boot|
|```Disabled```|Disabled|

**Slot7StorageBoot (PCIe Slot 7)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|When Boot All Targets is selected, all valid boot targets attached to the storage controller are made available in the UEFI Boot Order list. If Boot No Targets is selected, no boot targets from this storage controller are made available in the UEFI Boot Order.If Boot Limit to 24 Targets is selected, 24 boot targets attached to the storage controller are made available in the UEFI Boot Order.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```AllTargets```|Boot All Targets|
|```TwentyFourTargets```|Boot Limit to 24 Targets|
|```NoTargets```|Boot No Targets|

**Slot8NicBoot1 (Slot 8 NIC Port 1 Boot)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active. This is applicable only in UEFI Boot Mode.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```NetworkBoot```|Network Boot|
|```Disabled```|Disabled|

**Slot8NicBoot2 (Slot 8 NIC Port 2 Boot)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active. This is applicable only in UEFI Boot Mode.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```NetworkBoot```|Network Boot|
|```Disabled```|Disabled|

**Slot8NicBoot3 (Slot 8 NIC Port 3 Boot)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active. This is applicable only in UEFI Boot Mode.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```NetworkBoot```|Network Boot|
|```Disabled```|Disabled|

**Slot8NicBoot4 (Slot 8 NIC Port 4 Boot)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to enable or disable UEFI PXE Boot, UEFI HTTP Boot and iSCSI Software Initiator for the selected NIC. You might need to configure the NIC firmware for the boot option to be active. This is applicable only in UEFI Boot Mode.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```NetworkBoot```|Network Boot|
|```Disabled```|Disabled|

**Slot8StorageBoot (PCIe Slot 8)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|When Boot All Targets is selected, all valid boot targets attached to the storage controller are made available in the UEFI Boot Order list. If Boot No Targets is selected, no boot targets from this storage controller are made available in the UEFI Boot Order.If Boot Limit to 24 Targets is selected, 24 boot targets attached to the storage controller are made available in the UEFI Boot Order.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```AllTargets```|Boot All Targets|
|```TwentyFourTargets```|Boot Limit to 24 Targets|
|```NoTargets```|Boot No Targets|

**SpannedLogicalNvdimm1AvailableMemoryGiB (Processors 1,2: Spanned Persistent Memory Available (GB))**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Displays the maximum amount of persistent memory available in the system. The 'Total Available' value represents the amount of total system memory available for use as persistent memory.  The processor-specific values represent the amount of domain (socket) specific system memory that is available for use as logical NVDIMMs. The 'Storage' value represents the total size available on the backup device(s) for storing persistent memory.  All values are in gigabytes (1,073,741,824 bytes).|
|Type|Integer|
|Read Only|True|

**SpannedLogicalNvdimm1SizeGiB (Processors 1,2: Spanned Logical NVDIMM (GB))**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to specify the amount of regular memory, in gigabytes (1,073,741,824 bytes), to allocate for use as a logical NVDIMM for each specified region. Entries for processor pairs represent logical NVDIMMs which may span multiple processors. An attempt will be made to balance these regions across sockets. The processor-specific entries represent Logical NVDIMMs assigned to a designated socket. These regions are allocated from the top of the memory range for each domain.|
|Type|Integer|
|Read Only|False|

**SpannedLogicalNvdimm1StartingDomainId (Spanned Logical NVDIMM 1 Starting Domain ID)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to specify the amount of regular memory, in gigabytes (1,073,741,824 bytes), to allocate for use as a logical NVDIMM for each specified region. Entries for processor pairs represent logical NVDIMMs which may span multiple processors. An attempt will be made to balance these regions across sockets. The processor-specific entries represent Logical NVDIMMs assigned to a designated socket. These regions are allocated from the top of the memory range for each domain.|
|Type|Integer|
|Read Only|False|

**SpannedLogicalNvdimm1StartingDomainSize (Spanned Logical NVDIMM 1 Starting Domain Size)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to specify the amount of regular memory, in gigabytes (1,073,741,824 bytes), to allocate for use as a logical NVDIMM for each specified region. Entries for processor pairs represent logical NVDIMMs which may span multiple processors. An attempt will be made to balance these regions across sockets. The processor-specific entries represent Logical NVDIMMs assigned to a designated socket. These regions are allocated from the top of the memory range for each domain.|
|Type|Integer|
|Read Only|False|

**Sriov (SR-IOV)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|If enabled, SR-IOV support enables a hypervisor to create virtual instances of a PCI-express device, potentially increasing performance. If enabled, the BIOS allocates additional resources to PCI-express devices. You can leave this option set to enabled even if you are not using a hypervisor.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Enabled```|Enabled|
|```Disabled```|Disabled|

**StaleAtoS (Stale A to S)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Stale A to S directory optimization.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Enabled```|Enabled|
|```Disabled```|Disabled|

**StorageInitialize (Initialize Backup Storage Devices)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|When enabled, the persistent memory Storage devices will be reinitialized on the next boot.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Enabled```|Enabled|
|```Disabled```|Disabled|

**SubNumaClustering (Sub-NUMA Clustering)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|When enabled, Sub-NUMA Clustering divides the processor's cores, cache, and memory into multiple NUMA domains. Enabling this feature can increase performance for workloads that are NUMA aware and optimized. 
Note: When this option is enabled, up to 1GB of system memory may become unavailable.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Enabled```|Enabled|
|```Disabled```|Disabled|

**ThermalConfig (Thermal Configuration)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to select the fan cooling solution for the system. Optimal Cooling provides the most efficient solution by configuring fan speeds to the minimum required speed to provide adequate cooling. Increased Cooling runs fans at higher speeds to provide additional cooling. Select Increased Cooling when third-party storage controllers are cabled to the embedded hard drive cage, or if the system is experiencing thermal issues that cannot be resolved. Maximum cooling provides the maximum cooling available on this platform.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```OptimalCooling```|Optimal Cooling|
|```IncreasedCooling```|Increased Cooling|
|```MaxCooling```|Maximum Cooling|

**ThermalShutdown (Thermal Shutdown)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to control the reaction of the system to caution level thermal events. When disabled, the System Management Firmware ignores thermal events, and the system immediately powers off in data-destructive situations.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Enabled```|Enabled|
|```Disabled```|Disabled|

**TimeFormat (Time Format)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|This option controls how the system time is stored in the hardware Real Time Clock (RTC). When configured to 'Coordinated Universal Time (UTC)' (default) the local time is calculated from the associated time zone value. When configured to 'Local Time' the time is stored directly as local time and the time zone option does not have meaning. Setting this option to 'Local Time' works around an issue when using Microsoft Windows operating systems in Legacy Boot Mode where the time is set incorrectly.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Utc```|Coordinated Universal Time (UTC)|
|```Local```|Local Time|

**TimeZone (Time Zone)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|This option displays the current time zone setting for the system.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```UtcM12```|UTC-12:00, International Date Line West|
|```UtcM11```|UTC-11:00, Midway Island, Samoa|
|```UtcM10```|UTC-10:00, Hawaii|
|```UtcM9```|UTC-09:00, Alaska|
|```UtcM8```|UTC-08:00, Pacific Time(US & Canada)|
|```UtcM7```|UTC-07:00, Mountain Time (US & Canada)|
|```UtcM6```|UTC-06:00, Central America, Central Time(US & Canada)|
|```UtcM5```|UTC-05:00, Eastern Time(US & Canada)|
|```UtcM430```|UTC-04:30, Caracas|
|```UtcM4```|UTC-04:00, Atlantic Time(Canada), Caracas, Santiago|
|```UtcM330```|UTC-03:30, Newfoundland|
|```UtcM3```|UTC-03:00, Brasilia, Buenos Aires, Georgetown, Greenland|
|```UtcM2```|UTC-02:00, Mid-Atlantic|
|```UtcM1```|UTC-01:00, Azores, Cape Verde Is.|
|```Utc0```|UTC-00:00, Greenwich Mean Time, Dublin, London|
|```UtcP1```|UTC+01:00, Amsterdam, Berlin, Rome, Paris, West Central Africa|
|```UtcP2```|UTC+02:00, Athens, Istanbul, Cairo, Jerusalem|
|```UtcP3```|UTC+03:00, Baghdad, Kuwait, Riyadh, Moscow, Nairobi|
|```UtcP330```|UTC+03:30, Tehran|
|```UtcP4```|UTC+04:00, Abu Dhabi, Muscat, Baku, Tbilisi, Yerevan|
|```UtcP430```|UTC+04:30, Kabul|
|```UtcP5```|UTC+05:00, Ekaterinburg, Islamabad, Karachi, Tashkent|
|```UtcP530```|UTC+05:30, Chennai, Kolkata, Mumbai, New Delhi|
|```UtcP545```|UTC+05:45, Kathmandu|
|```UtcP6```|UTC+06:00, Almaty, Novosibirsk, Astana, Dhaka|
|```UtcP630```|UTC+06:30, Rangoon|
|```UtcP7```|UTC+07:00, Bangkok, Hanoi, Jakarta, Krasnoyarsk|
|```UtcP8```|UTC+08:00, Taipei, Beijing, Chongqing, Hong Kong, Urumqi|
|```UtcP9```|UTC+09:00, Osaka, Sapporo, Tokyo, Seoul, Yakutsk|
|```UtcP930```|UTC+09:30, Adelaide, Darwin|
|```UtcP10```|UTC+10:00, Canberra, Melbourne, Sydney, Guam, Hobart, Vladivostok|
|```UtcP11```|UTC+11:00, Magadan, Solomon Is., New Caledonia|
|```UtcP12```|UTC+12:00, Auckland, Wellington, Fiji, Kamchatka, Marshall Is.|
|```UtcP13```|UTC+13:00, Nuku'alofa|
|```UtcP14```|UTC+14:00, Line Islands|
|```Unspecified```|Unspecified Time Zone|

**Tpm20SoftwareInterfaceOperation (TPM 2.0 Software Interface Operation)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|TPM 2.0 Software Interface Operation: FIFO or CRB.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```NoAction```|No Action|
|```Fifo```|FIFO interface|
|```Crb```|CRB interface|

**Tpm20SoftwareInterfaceStatus (Current TPM 2.0 Software Interface Status)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Current TPM 2.0 Software Interface Status: FIFO or CRB.|
|Type|Enumeration|
|Read Only|True|

|Value|Description|
|---|---|
|```NoAction```|No Action|
|```Fifo```|FIFO interface|
|```Crb```|CRB interface|

**Tpm2Operation (TPM 2.0 Operation)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to perform a clear operation on the TPM. Clearing the TPM can prevent the server from booting to a TPM-aware operating system if the operating system uses TPM's measurements. TPM 2.0 is only supported in UEFI Mode.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```NoAction```|No Action|
|```Clear```|Clear|

**TpmActivePcrs (Current TPM 2.0 Active PCRs)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Current TPM 2.0 Active PCRs: SHA1, SHA256 or SHA1_SHA256|
|Type|Enumeration|
|Read Only|True|

|Value|Description|
|---|---|
|```NotSpecified```|Not specified|
|```Sha1```|SHA1 only|
|```Sha256```|SHA256 only|
|```Sha1Sha256```|SHA1 and SHA256|

**TpmChipId (Current TPM Chip ID)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Current TPM Chip: STMicro, Intel PTT fTPM or Nationz TPM20|
|Type|Enumeration|
|Read Only|True|

|Value|Description|
|---|---|
|```None```|None|
|```StMicroGen10```|ST Micro Gen10|
|```IntelPttFTpm```|Intel PTT fTPM|
|```NationzTpm20```|Nationz TPM20|

**TpmFips (Current TPM FIPS mode)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Current TPM FIPS (Federal Information Processing Standard) status: Not specified; non-FIPS certified; FIPS certified.|
|Type|Enumeration|
|Read Only|True|

|Value|Description|
|---|---|
|```NotSpecified```|Not specified|
|```NonFipsMode```|Non-FIPS Mode|
|```FipsMode```|FIPS mode|

**TpmFipsModeSwitch (TPM FIPS Mode Switch)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to switch the TPM chip to FIPS mode, regular mode.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```NoAction```|No Action|
|```RegularMode```|Regular mode|
|```FipsMode```|FIPS mode|

**TpmModeSwitchOperation (TPM Mode Switch Operation)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to switch the TPM chip to TPM 1.2/2.0, FIPS mode or non-FIPS mode.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```NoAction```|No Action|
|```Tpm12```|TPM 1.2|
|```Tpm20```|TPM 2.0|

**TpmOperation (TPM 1.2 Operation)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to enable the Trusted Platform Module and BIOS secure startup. When enabled, the TPM is fully functional. When disabled, the TPM is visible; however, functionality is limited. This option also enables you to reset the TPM to factory settings, which clears any assigned passwords, keys, or ownership data. Clearing the TPM can prevent the server from booting to a TPM-aware operating system if the operating system uses TPM's measurements.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```NoAction```|No Action|
|```Enable```|Enable|
|```Disable```|Disable|
|```Clear```|Clear|

**TpmState (Current TPM State)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Current TPM device state: Not Present; Present and Disabled; Present and Enabled.|
|Type|Enumeration|
|Read Only|True|

|Value|Description|
|---|---|
|```NotPresent```|Not Present|
|```PresentDisabled```|Present and Disabled|
|```PresentEnabled```|Present and Enabled|

**TpmType (Current TPM Type)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Current TPM device type.|
|Type|Enumeration|
|Read Only|True|

|Value|Description|
|---|---|
|```NoTpm```|No TPM|
|```Tpm12```|TPM 1.2|
|```Tpm20```|TPM 2.0|

**TpmUefiOpromMeasuring (TPM UEFI Option ROM Measurement)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to enable measuring the UEFI PCI option ROMs. Disabling this option skips measuring the UEFI PCI option ROMs.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Enabled```|Enabled|
|```Disabled```|Disabled|

**TpmVisibility (TPM Visibility)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to hide the TPM from the operating system. When the TPM is hidden, BIOS secure startup is disabled, and the TPM does not respond to any commands. Intended use is for removing the TPM option from the system without removing the actual hardware.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Hidden```|Hidden|
|```Visible```|Visible|

**UefiOptimizedBoot (UEFI Optimized Boot)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|When enabled, the system BIOS boots using native UEFI graphics drivers. When disabled, the system BIOS boots using INT10 legacy video support. You cannot disable this option if Secure Boot is enabled. You can only configure this option if Boot Mode is configured to UEFI Mode. 
Set this option to disabled for compatibility with Microsoft Windows 2008 and Windows 2008 R2 operating systems on a system configured for UEFI Mode. 
Set this option to enabled for compatibility with VMWare ESXi operating systems on a system configured for UEFI Mode.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Enabled```|Enabled|
|```Disabled```|Disabled|

**UefiSerialDebugLevel (UEFI Serial Debug Message Level)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to enable the UEFI Serial Debug output and verbosity level. Selecting Verbose can impact server boot time significantly. This option is only applicable in UEFI Mode.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Disabled```|Disabled|
|```ErrorsOnly```|Errors Only|
|```Medium```|Medium|
|```Network```|Network|
|```Verbose```|Verbose|
|```Custom```|Custom|

**UefiShellBootOrder (Add Embedded UEFI Shell to Boot Order)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|When enabled, this option adds the Embedded UEFI Shell as an entry in the UEFI Boot Order list. This option is only available when the Boot Mode is configured to UEFI Mode and the Embedded UEFI Shell is enabled.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Enabled```|Enabled|
|```Disabled```|Disabled|

**UefiShellScriptVerification (Shell Script Verification)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Enable this option to allow verification of UEFI shell script files when Secure Boot is enabled. For successful execution of script, make sure that UEFI shell scripts are enrolled in the Secure Boot database (db).|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Enabled```|Enabled|
|```Disabled```|Disabled|

**UefiShellStartup (UEFI Shell Script Auto-Start)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to enable or disable automatic execution of the Embedded UEFI Shell startup script. You can store the script file on local media or access it from a network location. You must name the script file "startup.nsh" and place it on local media or a network location accessible to the server.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Enabled```|Enabled|
|```Disabled```|Disabled|

**UefiShellStartupLocation (Shell Auto-Start Script Location)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to select the location of the Embedded UEFI Shell startup script. For the 'File Systems on Attached Media' option, you must name the script file "startup.nsh" and place it on a UEFI accessible local file system, such as a FAT32 partition on a USB disk or HDD. For the 'Network Location' option, the file must end with a .nsh extension, and must be placed at an HTTP/HTTPS or FTP location accessible to the system. When you select the 'Auto' option, the system attempts to retrieve the startup script from the network location first, followed by locally attached media.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Auto```|Auto|
|```AttachedMedia```|File Systems on Attached Media|
|```NetworkLocation```|Network Location|

**UefiShellStartupUrl (Network Location for Shell Auto-Start Script)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to configure a network URL to a UEFI Shell startup script. This option is available and used only when the Auto-Start Script Location is set to 'Network Location', or 'Auto', and the Shell Auto-Start Script discovery using DHCP is set to 'Disabled'. URLs in HTTP/HTTPS are accepted using either an IPv4 or IPv6 server address, or using a host name. FTP formats are accepted using either an IPv4 server address or a host name. For example, the URLs can be in any of the following formats: http://192.168.0.1/file/file.nsh, http://example.com/file/file.nsh, https://example.com/file/file.nsh, http://[1234::1000]/file.nsh. The file must end with an .nsh extension. When configured, the Embedded UEFI Shell attempts to load and execute the startup script from the network location pointed to by this URL. When a HTTPS URL is configured, you must enroll the respective HTTPS server's TLS certificate under Server Security > TLS(HTTPS) Options.|
|Type|String|
|Read Only|False|

**UefiShellStartupUrlFromDhcp (Discover Shell Auto-Start Script using DHCP)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to let the Shell discover its startup script URL using DHCP. This option is available only if the 'HTTP Support' policy is not set to 'Disabled' and Auto-Start Script Location is set to 'Network Location', or 'Auto'. When set to 'Enabled', the Shell sends DHCP requests with the DHCP User Class option set to the string 'UEFIShell'. The DHCP server must be configured to provide HTTP/HTTPS or FTP URLs when this DHCP User Class string is present in the DHCP request. The User Class option is Option 77 when using DHCP over IPv4, and Option 15 when using DHCP over IPv6. URLs in HTTP/HTTPS must use either an IPv4 or IPv6 server address, or a host name. FTP formats are accepted using either an IPv4 server address or a host name. The URL provided by the DHCP server should match the 'HTTP Support' policy. When 'HTTP Support' policy is set to 'Auto', any HTTP/HTTPS or FTP URL provided by the DHCP server is used. When policy is set to 'HTTPS only', only HTTPS URLs are used, and other URLs are ignored. When policy is set to 'HTTP only', only HTTP or FTP URLs are used, and other URLs are ignored. When policy is set to 'Disabled', the Shell does not send any DHCP request.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Enabled```|Enabled|
|```Disabled```|Disabled|

**UncoreFreqScaling (Uncore Frequency Scaling)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|This option controls the frequency scaling of the processor's internal busses (the uncore.) Setting this option to Auto enables the processor to dynamically change frequencies based on workload. Forcing to the maximum or minimum frequency enables tuning for latency or power consumption.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Auto```|Auto|
|```Maximum```|Maximum|
|```Minimum```|Minimum|

**UpiPrefetcher (UPI Prefetcher)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to disable the processor UPI Prefetch feature. In some cases, setting this option to disabled can improve performance. Typically, setting this option to enabled provides better performance. Only disable this option after performing application benchmarking to verify improved performance in the environment. This option must be enabled when Sub-Numa Clustering (SNC) is enabled.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Enabled```|Enabled|
|```Disabled```|Disabled|

**UrlBootFile (Boot from URL 1)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to configure a network URL to a bootable ISO or EFI file. URLs in HTTP/HTTPS are accepted using either an IPv4 or IPv6 server address, or using a host name. For example, the URLs can be in any of the following formats: http://192.168.0.1/file/image.iso, http://example.com/file/image.efi, https://example.com/file/image.efi, http://[1234::1000]/image.iso. 
When configured, this URL is listed as a boot option in the UEFI boot menu. Selecting this boot option downloads the file to the system memory, and configures the system to attempt to boot from it. There is no specific ordering on this option. It can be independently ordered in the boot menu. 
This setting requires configuring the 'Pre-Boot Network Interface' option if you want to access the URL location through a specific network interface. When a HTTPS URL is configured, this setting requires enrolling the respective TLS certificate of the HTTPS server under Server Security > TLS(HTTPS) Options. 
This is only applicable in UEFI Mode. 
Note: Booting from an ISO file can involve only booting a preliminary OS environment image, such as WinPE or a mini Linux, or a complete OS install image if the OS supports the HTTP Boot feature (Old OS versions may not support this). Please check your OS documentation for the HTTP Boot feature support.|
|Type|String|
|Read Only|False|

**UrlBootFile2 (Boot from URL 2)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to configure a network URL to a bootable ISO or EFI file. URLs in HTTP/HTTPS are accepted using either an IPv4 or IPv6 server address, or using a host name. For example, the URLs can be in any of the following formats: http://192.168.0.1/file/image.iso, http://example.com/file/image.efi, https://example.com/file/image.efi, http://[1234::1000]/image.iso. 
When configured, this URL is listed as a boot option in the UEFI boot menu. Selecting this boot option downloads the file to the system memory, and configures the system to attempt to boot from it. There is no specific ordering on this option. It can be independently ordered in the boot menu. 
This setting requires configuring the 'Pre-Boot Network Interface' option if you want to access the URL location through a specific network interface. When a HTTPS URL is configured, this setting requires enrolling the respective TLS certificate of the HTTPS server under Server Security > TLS(HTTPS) Options. 
This is only applicable in UEFI Mode. 
Note: Booting from an ISO file can involve only booting a preliminary OS environment image, such as WinPE or a mini Linux, or a complete OS install image if the OS supports the HTTP Boot feature (Old OS versions may not support this). Please check your OS documentation for the HTTP Boot feature support.|
|Type|String|
|Read Only|False|

**UrlBootFile3 (Boot from URL 3)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to configure a network URL to a bootable ISO or EFI file. URLs in HTTP/HTTPS are accepted using either an IPv4 or IPv6 server address, or using a host name. For example, the URLs can be in any of the following formats: http://192.168.0.1/file/image.iso, http://example.com/file/image.efi, https://example.com/file/image.efi, http://[1234::1000]/image.iso. 
When configured, this URL is listed as a boot option in the UEFI boot menu. Selecting this boot option downloads the file to the system memory, and configures the system to attempt to boot from it. There is no specific ordering on this option. It can be independently ordered in the boot menu. 
This setting requires configuring the 'Pre-Boot Network Interface' option if you want to access the URL location through a specific network interface. When a HTTPS URL is configured, this setting requires enrolling the respective TLS certificate of the HTTPS server under Server Security > TLS(HTTPS) Options. 
This is only applicable in UEFI Mode. 
Note: Booting from an ISO file can involve only booting a preliminary OS environment image, such as WinPE or a mini Linux, or a complete OS install image if the OS supports the HTTP Boot feature (Old OS versions may not support this). Please check your OS documentation for the HTTP Boot feature support.|
|Type|String|
|Read Only|False|

**UrlBootFile4 (Boot from URL 4)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to configure a network URL to a bootable ISO or EFI file. URLs in HTTP/HTTPS are accepted using either an IPv4 or IPv6 server address, or using a host name. For example, the URLs can be in any of the following formats: http://192.168.0.1/file/image.iso, http://example.com/file/image.efi, https://example.com/file/image.efi, http://[1234::1000]/image.iso. 
When configured, this URL is listed as a boot option in the UEFI boot menu. Selecting this boot option downloads the file to the system memory, and configures the system to attempt to boot from it. There is no specific ordering on this option. It can be independently ordered in the boot menu. 
This setting requires configuring the 'Pre-Boot Network Interface' option if you want to access the URL location through a specific network interface. When a HTTPS URL is configured, this setting requires enrolling the respective TLS certificate of the HTTPS server under Server Security > TLS(HTTPS) Options. 
This is only applicable in UEFI Mode. 
Note: Booting from an ISO file can involve only booting a preliminary OS environment image, such as WinPE or a mini Linux, or a complete OS install image if the OS supports the HTTP Boot feature (Old OS versions may not support this). Please check your OS documentation for the HTTP Boot feature support.|
|Type|String|
|Read Only|False|

**UsbBoot (USB Boot Support)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Set this option to disabled to prevent the system from booting to any USB devices connected to the server. This includes preventing boot to virtual media devices, and the embedded SD or uSD card slot (if supported).|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Enabled```|Enabled|
|```Disabled```|Disabled|

**UsbControl (USB Control)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|All USB Ports Enabled: Enables all USB ports and embedded devices.All USB Ports Disabled: Disables all USB ports and embedded devices.External USB Ports Disabled: Disables only external USB ports.Internal USB Ports Disabled: Disables only internal USB ports.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```UsbEnabled```|All USB Ports Enabled|
|```UsbDisabled```|All USB Ports Disabled|
|```ExternalUsbDisabled```|External USB Ports Disabled|
|```InternalUsbDisabled```|Internal USB Ports Disabled|

**UserDefaultsState (User Defaults)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Displays whether user default settings are enabled or disabled.|
|Type|Enumeration|
|Read Only|True|

|Value|Description|
|---|---|
|```Enabled```|Enabled|
|```Disabled```|Disabled|

**UtilityLang (Utility Language)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Select this option to adjust the current language for the system.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```English```|English|
|```Japanese```|日本語|
|```Chinese```|中文（简体）|

**VideoOptions (Video Options)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to configure video settings in the system. When set to Add-in Video Enabled, Embedded Video Disabled, the system only displays video to the first discovered add-in video controller. When set to Both Add-in and Embedded Video Enabled, the system displays video to both the embedded and the first discovered add-in video controllers. In both modes, early system startup video is displayed to the embedded video controller.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```OptionalVideoOnly```|Add-in Video Enabled, Embedded Video Disabled|
|```BothVideoEnabled```|Both Add-in and Embedded Video Enabled|

**VirtualInstallDisk (Virtual Install Disk)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to control the Virtual Install Disk. The Virtual Install Disk contains drivers specific to this server that an OS can use during installation. If enabled, the Virtual Install Disk appears as a drive in the operating system.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Enabled```|Enabled|
|```Disabled```|Disabled|

**VirtualSerialPort (Virtual Serial Port)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to assign the logical COM port address and associated default resources used by the Virtual Serial Port (VSP). VSP enables the Management Processor to present an emulated serial port to support the BIOS Serial Console and operating system serial console.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Com1Irq4```|COM 1; IRQ4; I/O: 3F8h-3FFh|
|```Com2Irq3```|COM 2; IRQ3; I/O: 2F8h-2FFh|
|```Disabled```|Disabled|

**VlanControl (VLAN Control)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to enable or disable VLAN tagging on all enabled network interfaces.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Enabled```|Enabled|
|```Disabled```|Disabled|

**VlanId (VLAN ID)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to set the global VLAN ID for all enabled network interfaces. Valid values are 0 to 4094.A value of 0 sets the device to send untagged frames.|
|Type|Integer|
|Read Only|False|

**VlanPriority (VLAN Priority)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to set the priority for the VLAN tagged frames. Valid values are 0 to 7.|
|Type|Integer|
|Read Only|False|

**WakeOnLan (Wake-On LAN)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|You can configure the server to be powered on remotely when it receives a special packet. This option requires a NIC, NIC driver, and operating system that are WOL-capable.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Enabled```|Enabled|
|```Disabled```|Disabled|

**WorkloadProfile (Workload Profile)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Select this option to change the Workload Profile to accomodate your desired workload. Settings that are changed by the Workload Profile are grayed out and unchangeable unless in the 'Custom' profile. Please refer to the 'UEFI Workload-based Performance Tuning Guide' for details on which profiles affect which options. |
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```GeneralPowerEfficientCompute```|General Power Efficient Compute|
|```GeneralPeakFrequencyCompute```|General Peak Frequency Compute|
|```GeneralThroughputCompute```|General Throughput Compute|
|```Virtualization-PowerEfficient```|Virtualization - Power Efficient|
|```Virtualization-MaxPerformance```|Virtualization - Max Performance|
|```LowLatency```|Low Latency|
|```MissionCritical```|Mission Critical|
|```TransactionalApplicationProcessing```|Transactional Application Processing|
|```HighPerformanceCompute(HPC)```|High Performance Compute (HPC)|
|```DecisionSupport```|Decision Support|
|```GraphicProcessing```|Graphic Processing|
|```I/OThroughput```|I/O Throughput|
|```Custom```|Custom|

**XptPrefetcher (XPT Prefetcher)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to disable the processor XPT Prefetch feature. In some cases, setting this option to disabled can improve performance. Typically, setting this option to enabled provides better performance. Only disable this option after performing application benchmarking to verify improved performance in the environment. This option must be enabled when Sub-Numa Clustering (SNC) is enabled.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```Auto```|Auto|
|```Enabled```|Enabled|
|```Disabled```|Disabled|

**iSCSIPolicy (iSCSI Policy)**
Member of [Bios.v1_0_0.Bios](#bios-v1_0_0-bios)

| | |
|---|---|
|Description|Use this option to set the iSCSI Policy. If configured to Software Initiator, the iSCSI software initiator will be used to access iSCSI targets on any configured NIC ports. If configured to Adapter Initiator, the adapter specific iSCSI initiator will be used instead. The adapter firmware must be configured to access iSCSI targets from the adapter initiator.|
|Type|Enumeration|
|Read Only|False|

|Value|Description|
|---|---|
|```SoftwareInitiator```|Software Initiator|
|```AdapterInitiator```|Adapter Initiator|

## Chassis.v1_2_0.Chassis
```@odata.type: "#Chassis.v1_2_0.Chassis"```

The schema definition for the Chassis resource represents the properties for physical components for any system. This object represents racks, rack mount servers, blades, standalone, modular systems, enclosures, and all other containers. The non-CPU/device-centric parts of the schema are accessed either directly or indirectly through this resource.
### Resource Instances
|Uri|HTTP Allow|
|---|---|
|```/redfish/v1/chassis/{item}/```|GET POST |

### Links to other Resources
|Link Name|Destination type
|---|---|
|```Links/ComputerSystems[]```|[ComputerSystem](#computersystem-v1_4_0-computersystem)|
|```Links/ManagedBy[]```|[Manager](#manager-v1_1_0-manager)|
|```Oem/Hpe/Links/Devices```|Collection of [HpeServerDevice](#hpeserverdevice-v2_0_0-hpeserverdevice)|
|```NetworkAdapters```|Collection of [NetworkAdapter](#networkadapter-v1_0_1-networkadapter)|
|```Power```|[Power](#power-v1_2_1-power)|
|```Thermal```|[Thermal](#thermal-v1_1_0-thermal)|
|```Links/Drives[]```|[Drive](#drive-v1_0_0-drive)|

### AssetTag
Member of [Chassis.v1_2_0.Chassis](#chassis-v1_2_0-chassis)

| | |
|---|---|
|Description|The chassis user-assigned asset tag.|
|Type|string or null|
|Read Only|False|

### ChassisType
Member of [Chassis.v1_2_0.Chassis](#chassis-v1_2_0-chassis)

| | |
|---|---|
|Description|This property indicates the physical form factor type of this resource.|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```Rack```|An equipment rack, typically a 19-inch wide freestanding unit.|
|```Blade```|An enclosed or semi-enclosed, typically vertically-oriented, system chassis that must be plugged into a multi-system chassis to function normally.|
|```Enclosure```|A generic term for a chassis that does not fit any other description.|
|```StandAlone```|A single, free-standing system, commonly called a tower or desktop chassis.|
|```RackMount```|A single system chassis designed specifically for mounting in an equipment rack.|
|```Card```|A loose device or circuit board intended to be installed in a system or other enclosure.|
|```Cartridge```|A small self-contained system intended to be plugged into a multi-system chassis.|
|```Row```|A collection of equipment racks.|
|```Pod```|A collection of equipment racks in a large, likely transportable, container.|
|```Expansion```|A chassis that expands the capabilities or capacity of another chassis.|
|```Sidecar```|A chassis that mechanically connects with another chassis to expand its capabilities or capacity.|
|```Zone```|A logical division or portion of a physical chassis that contains multiple devices or systems that cannot be physically separated.|
|```Sled```|TBD|
|```Shelf```|An enclosed or semi-enclosed, typically horizontally-oriented, system chassis that must be plugged into a multi-system chassis to function normally.|
|```Other```|A chassis that does not fit any of these definitions.|

### IndicatorLED
Member of [Chassis.v1_2_0.Chassis](#chassis-v1_2_0-chassis)

| | |
|---|---|
|Description|The chassis indicator LED that is used to identify the chassis. The user can manipulate this LED.|
|Type|string or null|
|Read Only|False|

The following are the supported values:

|Value|Description|
|---|---|
|```Null```|A value is temporarily unavailable|
|```Unknown```|The state of the Indicator LED cannot be determined.|
|```Lit```|The Indicator LED is on.|
|```Blinking```|The Indicator LED is blinking.|
|```Off```|The Indicator LED is off.|

### Manufacturer
Member of [Chassis.v1_2_0.Chassis](#chassis-v1_2_0-chassis)

| | |
|---|---|
|Description|The chassis manufacturer.|
|Type|string or null|
|Read Only|True|

### Model
Member of [Chassis.v1_2_0.Chassis](#chassis-v1_2_0-chassis)

| | |
|---|---|
|Description|The chassis model number.|
|Type|string or null|
|Read Only|True|

### NetworkAdapters
The collection of network adapters contained within this chassis.
### Oem.Hpe.BayNumber
Member of [Chassis.v1_2_0.Chassis](#chassis-v1_2_0-chassis)

| | |
|---|---|
|Description|The bay number of the node or the blade.|
|Type|integer|
|Read Only|True|

### Oem.Hpe.BaysConsumedHeight
Member of [Chassis.v1_2_0.Chassis](#chassis-v1_2_0-chassis)

| | |
|---|---|
|Description|The number of enclosure bays this chassis consumes in height.|
|Type|integer|
|Read Only|True|

### Oem.Hpe.BaysConsumedWidth
Member of [Chassis.v1_2_0.Chassis](#chassis-v1_2_0-chassis)

| | |
|---|---|
|Description|The number of enclosure bays this chassis consumes in width.|
|Type|integer|
|Read Only|True|

### Oem.Hpe.Firmware
**Oem.Hpe.Firmware.PlatformDefinitionTable**
**Oem.Hpe.Firmware.PlatformDefinitionTable.Current**
**Oem.Hpe.Firmware.PlatformDefinitionTable.Current.VersionString**
Member of [Chassis.v1_2_0.Chassis](#chassis-v1_2_0-chassis)

| | |
|---|---|
|Description|The version of the Intelligent Platform Abstraction Data.|
|Type|string|
|Read Only|True|

**Oem.Hpe.Firmware.PowerManagementController**
**Oem.Hpe.Firmware.PowerManagementController.Current**
**Oem.Hpe.Firmware.PowerManagementController.Current.VersionString**
Member of [Chassis.v1_2_0.Chassis](#chassis-v1_2_0-chassis)

| | |
|---|---|
|Description|The firmware version of the Power Monitor.|
|Type|string|
|Read Only|True|

**Oem.Hpe.Firmware.PowerManagementControllerBootloader**
**Oem.Hpe.Firmware.PowerManagementControllerBootloader.Current**
**Oem.Hpe.Firmware.PowerManagementControllerBootloader.Current.Family**
Member of [Chassis.v1_2_0.Chassis](#chassis-v1_2_0-chassis)

| | |
|---|---|
|Description|The family type of the Power Monitor hardware.|
|Type|string|
|Read Only|True|

**Oem.Hpe.Firmware.PowerManagementControllerBootloader.Current.VersionString**
Member of [Chassis.v1_2_0.Chassis](#chassis-v1_2_0-chassis)

| | |
|---|---|
|Description|The firmware version of the Power Monitor boot loader.|
|Type|string|
|Read Only|True|

**Oem.Hpe.Firmware.SASProgrammableLogicDevice**
**Oem.Hpe.Firmware.SASProgrammableLogicDevice.Current**
**Oem.Hpe.Firmware.SASProgrammableLogicDevice.Current.VersionString**
Member of [Chassis.v1_2_0.Chassis](#chassis-v1_2_0-chassis)

| | |
|---|---|
|Description|The firmware version of the SAS controller.|
|Type|string|
|Read Only|True|

**Oem.Hpe.Firmware.SPSFirmwareVersionData**
**Oem.Hpe.Firmware.SPSFirmwareVersionData.Current**
**Oem.Hpe.Firmware.SPSFirmwareVersionData.Current.VersionString**
Member of [Chassis.v1_2_0.Chassis](#chassis-v1_2_0-chassis)

| | |
|---|---|
|Description|The SPS FW Version number, aka ME FW Version, AAAA.BBBB.CCCC.DDDD.E|
|Type|string|
|Read Only|True|

**Oem.Hpe.Firmware.SystemProgrammableLogicDevice**
**Oem.Hpe.Firmware.SystemProgrammableLogicDevice.Current**
**Oem.Hpe.Firmware.SystemProgrammableLogicDevice.Current.VersionString**
Member of [Chassis.v1_2_0.Chassis](#chassis-v1_2_0-chassis)

| | |
|---|---|
|Description|The firmware version of the CPLD.|
|Type|string|
|Read Only|True|

### Oem.Hpe.Images
**Oem.Hpe.Images.Front**
**Oem.Hpe.Images.Front.extref**
Member of [Chassis.v1_2_0.Chassis](#chassis-v1_2_0-chassis)

| | |
|---|---|
|Description|The URI of an external resource.|
|Type|string|
|Read Only|True|

**Oem.Hpe.Images.Model**
**Oem.Hpe.Images.Model.extref**
Member of [Chassis.v1_2_0.Chassis](#chassis-v1_2_0-chassis)

| | |
|---|---|
|Description|The URI of an external resource.|
|Type|string|
|Read Only|True|

### Oem.Hpe.Location
**Oem.Hpe.Location.GeographicLocation**
**Oem.Hpe.Location.GeographicLocation.RackName**
Member of [Chassis.v1_2_0.Chassis](#chassis-v1_2_0-chassis)

| | |
|---|---|
|Description|The name of the chassis enclosure.|
|Type|string|
|Read Only|True|

**Oem.Hpe.Location.LocationInRack**
**Oem.Hpe.Location.LocationInRack.RackLdsPartNumber**
Member of [Chassis.v1_2_0.Chassis](#chassis-v1_2_0-chassis)

| | |
|---|---|
|Description|The chassis rack part number.|
|Type|string|
|Read Only|True|

**Oem.Hpe.Location.LocationInRack.RackLdsProductDescription**
Member of [Chassis.v1_2_0.Chassis](#chassis-v1_2_0-chassis)

| | |
|---|---|
|Description| The chassis rack product description.|
|Type|string|
|Read Only|True|

**Oem.Hpe.Location.LocationInRack.RackUHeight**
Member of [Chassis.v1_2_0.Chassis](#chassis-v1_2_0-chassis)

| | |
|---|---|
|Description|The chassis rack U height.|
|Type|integer|
|Read Only|True|

**Oem.Hpe.Location.LocationInRack.RackUUID**
Member of [Chassis.v1_2_0.Chassis](#chassis-v1_2_0-chassis)

| | |
|---|---|
|Description|The chassis rack UUID.|
|Type|string|
|Read Only|True|

**Oem.Hpe.Location.LocationInRack.TagVersion**
Member of [Chassis.v1_2_0.Chassis](#chassis-v1_2_0-chassis)

| | |
|---|---|
|Description|The chassis rack tag version.|
|Type|integer|
|Read Only|True|

**Oem.Hpe.Location.LocationInRack.ULocation**
Member of [Chassis.v1_2_0.Chassis](#chassis-v1_2_0-chassis)

| | |
|---|---|
|Description|The chassis rack U location.|
|Type|string|
|Read Only|True|

**Oem.Hpe.Location.LocationInRack.UPosition**
Member of [Chassis.v1_2_0.Chassis](#chassis-v1_2_0-chassis)

| | |
|---|---|
|Description|The chassis U position in the rack.|
|Type|integer|
|Read Only|True|

**Oem.Hpe.Location.LocationOfChassis**
**Oem.Hpe.Location.LocationOfChassis.UUID**
Member of [Chassis.v1_2_0.Chassis](#chassis-v1_2_0-chassis)

| | |
|---|---|
|Description|The chassis UUID provided by SMBIOS.|
|Type|string|
|Read Only|True|

### Oem.Hpe.MCTPEnabledOnServer
Member of [Chassis.v1_2_0.Chassis](#chassis-v1_2_0-chassis)

| | |
|---|---|
|Description|Indicates if MCTP is enabled on the server or not.|
|Type|boolean|
|Read Only|True|

### Oem.Hpe.OnboardAdministrator
**Oem.Hpe.OnboardAdministrator.IPv4Address**
Member of [Chassis.v1_2_0.Chassis](#chassis-v1_2_0-chassis)

| | |
|---|---|
|Description|IPv4 address of the chassis.|
|Type|string or null|
|Read Only|True|

**Oem.Hpe.OnboardAdministrator.IPv6**
**Oem.Hpe.OnboardAdministrator.IPv6.DHCPv6Address (array)**
Member of [Chassis.v1_2_0.Chassis](#chassis-v1_2_0-chassis)
```DHCPv6Address``` is an array containing elements of:


| | |
|---|---|
|Type|string|
|Read Only|True|

**Oem.Hpe.OnboardAdministrator.IPv6.SLAACAddress (array)**
Member of [Chassis.v1_2_0.Chassis](#chassis-v1_2_0-chassis)
```SLAACAddress``` is an array containing elements of:


| | |
|---|---|
|Type|string|
|Read Only|True|

**Oem.Hpe.OnboardAdministrator.IPv6.StaticAddress (array)**
Member of [Chassis.v1_2_0.Chassis](#chassis-v1_2_0-chassis)
```StaticAddress``` is an array containing elements of:


| | |
|---|---|
|Type|string|
|Read Only|True|

**Oem.Hpe.OnboardAdministrator.MacAddress**
Member of [Chassis.v1_2_0.Chassis](#chassis-v1_2_0-chassis)

| | |
|---|---|
|Description|MAC address of the chassis.|
|Type|string or null|
|Read Only|True|

### Oem.Hpe.PowerAlertMode
**Oem.Hpe.PowerAlertMode.Activated**
Member of [Chassis.v1_2_0.Chassis](#chassis-v1_2_0-chassis)

| | |
|---|---|
|Description|The power alert mode activation state.|
|Type|boolean|
|Read Only|True|

**Oem.Hpe.PowerAlertMode.AlertPowerWatts**
Member of [Chassis.v1_2_0.Chassis](#chassis-v1_2_0-chassis)

| | |
|---|---|
|Description|The power consumption of the system when operating in alert mode.|
|Type|integer|
|Read Only|True|

### Oem.Hpe.SmartStorageBattery (array)
Member of [Chassis.v1_2_0.Chassis](#chassis-v1_2_0-chassis)
```SmartStorageBattery``` is an array containing elements of:

**SmartStorageBattery[{item}].BatteryWearLevelPercent**
Member of [Chassis.v1_2_0.Chassis](#chassis-v1_2_0-chassis)

| | |
|---|---|
|Description|The battery wear level percentage. When this value reaches 100%, the battery is completely worn out and needs to be replaced. The value is null if battery wear level cannot be determined or is not supported.|
|Type|integer or null|
|Read Only|True|

**SmartStorageBattery[{item}].ChargeLevelPercent**
Member of [Chassis.v1_2_0.Chassis](#chassis-v1_2_0-chassis)

| | |
|---|---|
|Description|State of charge of the battery.|
|Type|integer or null|
|Read Only|True|

**SmartStorageBattery[{item}].ErrorCode**
Member of [Chassis.v1_2_0.Chassis](#chassis-v1_2_0-chassis)

| | |
|---|---|
|Description|Error code of the battery.|
|Type|string or null|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```Null```|A value is temporarily unavailable|
|```GeneralFailure```|The battery has failed.|
|```HighInternalBatteryResistance```|The battery has failed due to high internal resistance.|
|```LowOpenCircuitVoltage```|The battery has failed due to a low voltage output.|
|```BatteryCellFailure```|The battery has failed.|
|```BatteryChargeTimeout```|The battery did not charge at the expected rate, indicating a faulty battery.|
|```OverTemperature```|The battery was disabled due to high ambient temperature, and will be re-enabled when the temperature is lowered.|
|```DischargeBelowMinimumVoltage```|The battery discharged below the minimum discharge voltage, and may be re-enabled upon recharging the battery.|
|```DischargeCurrentHigh```|The last backup failed due to exceeding the maximum discharge current.|
|```LoadCountExceeded```|The battery was disabled due to exceeding the maximum amount of devices supported, and will be re-enabled when the battery has been recharged or the additional devices are removed.|
|```BackupSucceeded```|The last backup succeeded within the expected time.|
|```OverCurrent```|The battery has been protected due to exceeding the output current capability. The battery should be re-enabled on the next reboot.|
|```PermanentFailure```|The battery has permanently failed.|
|```BackupTimeExceeded```|The last backup failed due to exceeding the battery discharge time limit.|

**SmartStorageBattery[{item}].FailurePredicted**
Member of [Chassis.v1_2_0.Chassis](#chassis-v1_2_0-chassis)

| | |
|---|---|
|Description|Is this battery currently predicting a failure in the near future.|
|Type|boolean or null|
|Read Only|True|

**SmartStorageBattery[{item}].FirmwareVersion**
Member of [Chassis.v1_2_0.Chassis](#chassis-v1_2_0-chassis)

| | |
|---|---|
|Description|Firmware version of the battery.|
|Type|string|
|Read Only|True|

**SmartStorageBattery[{item}].Index**
Member of [Chassis.v1_2_0.Chassis](#chassis-v1_2_0-chassis)

| | |
|---|---|
|Description|Index of the battery.|
|Type|integer|
|Read Only|True|

**SmartStorageBattery[{item}].MaximumCapWatts**
Member of [Chassis.v1_2_0.Chassis](#chassis-v1_2_0-chassis)

| | |
|---|---|
|Description|Maximum capacity of the battery in watts.|
|Type|integer|
|Read Only|True|

**SmartStorageBattery[{item}].Model**
Member of [Chassis.v1_2_0.Chassis](#chassis-v1_2_0-chassis)

| | |
|---|---|
|Description|Model of the battery.|
|Type|string|
|Read Only|True|

**SmartStorageBattery[{item}].ProductName**
Member of [Chassis.v1_2_0.Chassis](#chassis-v1_2_0-chassis)

| | |
|---|---|
|Description|Product name of the battery.|
|Type|string|
|Read Only|True|

**SmartStorageBattery[{item}].RemainingChargeTimeSeconds**
Member of [Chassis.v1_2_0.Chassis](#chassis-v1_2_0-chassis)

| | |
|---|---|
|Description|Remaining charging time of the battery in seconds.|
|Type|integer or null|
|Read Only|True|

**SmartStorageBattery[{item}].SerialNumber**
Member of [Chassis.v1_2_0.Chassis](#chassis-v1_2_0-chassis)

| | |
|---|---|
|Description|Serial number of the battery.|
|Type|string|
|Read Only|True|

**SmartStorageBattery[{item}].SparePartNumber**
Member of [Chassis.v1_2_0.Chassis](#chassis-v1_2_0-chassis)

| | |
|---|---|
|Description|Spare part number of the battery.|
|Type|string|
|Read Only|True|

**SmartStorageBattery[{item}].Status**
Member of [Chassis.v1_2_0.Chassis](#chassis-v1_2_0-chassis)
See the Redfish standard schema and specification for information on common Status object.

### Oem.Hpe.SystemMaintenanceSwitches
**Oem.Hpe.SystemMaintenanceSwitches.Sw1**
Member of [Chassis.v1_2_0.Chassis](#chassis-v1_2_0-chassis)

| | |
|---|---|
|Description|Override iLO security.|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```On```|iLO Security Override Enabled.|
|```Off```|No function (Normal).|

**Oem.Hpe.SystemMaintenanceSwitches.Sw10**
Member of [Chassis.v1_2_0.Chassis](#chassis-v1_2_0-chassis)

| | |
|---|---|
|Description|Reserved.|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```On```|Switch is on.|
|```Off```|Switch is off (Normal).|

**Oem.Hpe.SystemMaintenanceSwitches.Sw11**
Member of [Chassis.v1_2_0.Chassis](#chassis-v1_2_0-chassis)

| | |
|---|---|
|Description|Reserved.|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```On```|Switch is on.|
|```Off```|Switch is off (Normal).|

**Oem.Hpe.SystemMaintenanceSwitches.Sw12**
Member of [Chassis.v1_2_0.Chassis](#chassis-v1_2_0-chassis)

| | |
|---|---|
|Description|Reserved.|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```On```|Switch is on.|
|```Off```|Switch is off (Normal).|

**Oem.Hpe.SystemMaintenanceSwitches.Sw2**
Member of [Chassis.v1_2_0.Chassis](#chassis-v1_2_0-chassis)

| | |
|---|---|
|Description|Reserved.|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```On```|Switch is on.|
|```Off```|Switch is off (Normal).|

**Oem.Hpe.SystemMaintenanceSwitches.Sw3**
Member of [Chassis.v1_2_0.Chassis](#chassis-v1_2_0-chassis)

| | |
|---|---|
|Description|Reserved.|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```On```|Switch is on.|
|```Off```|Switch is off (Normal).|

**Oem.Hpe.SystemMaintenanceSwitches.Sw4**
Member of [Chassis.v1_2_0.Chassis](#chassis-v1_2_0-chassis)

| | |
|---|---|
|Description|Reserved.|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```On```|Switch is on.|
|```Off```|Switch is off (Normal).|

**Oem.Hpe.SystemMaintenanceSwitches.Sw5**
Member of [Chassis.v1_2_0.Chassis](#chassis-v1_2_0-chassis)

| | |
|---|---|
|Description|BIOS/UEFI Password Disable.|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```On```|Power On Password disabled.|
|```Off```|Power On Password enabled (Normal).|

**Oem.Hpe.SystemMaintenanceSwitches.Sw6**
Member of [Chassis.v1_2_0.Chassis](#chassis-v1_2_0-chassis)

| | |
|---|---|
|Description|Reset Configuration.|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```On```||
|```Off```||

**Oem.Hpe.SystemMaintenanceSwitches.Sw7**
Member of [Chassis.v1_2_0.Chassis](#chassis-v1_2_0-chassis)

| | |
|---|---|
|Description|Reserved.|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```On```|Switch is on.|
|```Off```|Switch is off (Default).|

**Oem.Hpe.SystemMaintenanceSwitches.Sw8**
Member of [Chassis.v1_2_0.Chassis](#chassis-v1_2_0-chassis)

| | |
|---|---|
|Description|Reserved.|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```On```|Switch is on.|
|```Off```|Switch is off (Default).|

**Oem.Hpe.SystemMaintenanceSwitches.Sw9**
Member of [Chassis.v1_2_0.Chassis](#chassis-v1_2_0-chassis)

| | |
|---|---|
|Description|Reserved.|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```On```|Switch is on.|
|```Off```|Switch is off (Default).|

### PartNumber
Member of [Chassis.v1_2_0.Chassis](#chassis-v1_2_0-chassis)

| | |
|---|---|
|Description|The chassis part number.|
|Type|string or null|
|Read Only|True|

### PhysicalSecurity
**PhysicalSecurity.IntrusionSensor**
Member of [Chassis.v1_2_0.Chassis](#chassis-v1_2_0-chassis)

| | |
|---|---|
|Description|This indicates the known state of the physical security sensor, such as if it is hardware intrusion detected.|
|Type|string or null|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```Normal```|No abnormal physical security conditions are detected at this time.|
|```HardwareIntrusion```|A door, lock, or other mechanism protecting the internal system hardware from being accessed is detected as being in an insecure state.|
|```TamperingDetected```|Physical tampering of the monitored entity is detected.|

**PhysicalSecurity.IntrusionSensorReArm**
Member of [Chassis.v1_2_0.Chassis](#chassis-v1_2_0-chassis)

| | |
|---|---|
|Description|This indicates how the Normal state to be restored.|
|Type|string or null|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```Manual```|This sensor would be restored to the Normal state by a manual re-arm.|
|```Automatic```|This sensor would be restored to the Normal state automatically as no abnormal physical security conditions are detected.|

### Power
A reference to the thermal metrics (power supplies, power policies, sensors) for this chassis.
### SKU
Member of [Chassis.v1_2_0.Chassis](#chassis-v1_2_0-chassis)

| | |
|---|---|
|Description|The chassis SKU.|
|Type|string or null|
|Read Only|True|

### SerialNumber
Member of [Chassis.v1_2_0.Chassis](#chassis-v1_2_0-chassis)

| | |
|---|---|
|Description|The chassis serial number.|
|Type|string or null|
|Read Only|True|

### Status
Member of [Chassis.v1_2_0.Chassis](#chassis-v1_2_0-chassis)
See the Redfish standard schema and specification for information on common Status object.

### Thermal
A reference to the thermal metrics (fans, cooling, sensors) for this chassis.
### Actions

**HpeServerChassis.DisableMCTPOnServer**
Member of [Chassis.v1_2_0.Chassis](#chassis-v1_2_0-chassis)
There are no parameters for this action.

**HpeServerChassis.FactoryResetMCTP**
Member of [Chassis.v1_2_0.Chassis](#chassis-v1_2_0-chassis)
There are no parameters for this action.
## ComputerSystem.v1_4_0.ComputerSystem
```@odata.type: "#ComputerSystem.v1_4_0.ComputerSystem"```

The schema definition of a computer system and its properties. A computer system represents a physical or virtual machine and the local resources, such as memory, CPU, and other devices that can be accessed from that machine.
### Resource Instances
|Uri|HTTP Allow|
|---|---|
|```/redfish/v1/systems/{item}/```|GET POST PATCH |

### Links to other Resources
|Link Name|Destination type
|---|---|
|```EthernetInterfaces```|Collection of [EthernetInterface](#ethernetinterface-v1_0_3-ethernetinterface)|
|```Oem/Hpe/Links/USBDevices```|Collection of [HpeUSBDevice](#hpeusbdevice-v2_0_0-hpeusbdevice)|
|```Links/Chassis[]```|[Chassis](#chassis-v1_2_0-chassis)|
|```Memory```|Collection of [Memory](#memory-v1_1_0-memory)|
|```Oem/Hpe/Links/USBPorts```|Collection of [HpeUSBPort](#hpeusbport-v2_0_0-hpeusbport)|
|```Oem/Hpe/Links/NetworkAdapters```|Collection of [HpeBaseNetworkAdapter](#hpebasenetworkadapter-v2_0_0-hpebasenetworkadapter)|
|```Oem/Hpe/SmartStorageConfig[]```|[SmartStorageConfig](#smartstorageconfig-v2_0_0-smartstorageconfig)|
|```Processors```|Collection of [Processor](#processor-v1_0_0-processor)|
|```SecureBoot```|[SecureBoot](#secureboot-v1_0_0-secureboot)|
|```Storage```|Collection of [Storage](#storage-v1_0_0-storage)|
|```Bios```|[Bios](#bios-v1_0_0-bios)|
|```Oem/Hpe/Links/EthernetInterfaces```|Collection of [EthernetInterface](#ethernetinterface-v1_0_3-ethernetinterface)|
|```LogServices```|Collection of [LogService](#logservice-v1_0_0-logservice)|
|```Oem/Hpe/Links/SmartStorage```|[HpeSmartStorage](#hpesmartstorage-v2_0_0-hpesmartstorage)|
|```Oem/Hpe/Links/PCISlots```|Collection of [HpeServerPCISlot](#hpeserverpcislot-v2_1_0-hpeserverpcislot)|
|```NetworkInterfaces```|Collection of [NetworkInterface](#networkinterface-v1_1_0-networkinterface)|
|```Links/ManagedBy[]```|[Manager](#manager-v1_1_0-manager)|
|```Oem/Hpe/Links/PCIDevices```|Collection of [HpeServerPciDevice](#hpeserverpcidevice-v2_0_0-hpeserverpcidevice)|

### AssetTag
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)

| | |
|---|---|
|Description|A user-definable tag that is used to track this system for inventory or other client purposes.|
|Type|string or null|
|Read Only|False|

### Bios
The Bios URI.
### BiosVersion
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)

| | |
|---|---|
|Description|The version of the system BIOS or primary system firmware.|
|Type|string or null|
|Read Only|True|

### Boot
**Boot.BootSourceOverrideEnabled**
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)

| | |
|---|---|
|Description|BootSourceOverrideTarget must be specified before BootSourceOverrideEnabled can be used.|
|Type|string or null|
|Read Only|False|

The following are the supported values:

|Value|Description|
|---|---|
|```Null```|A value is temporarily unavailable|
|```Disabled```|The system will boot normally.|
|```Once```|On its next boot cycle, the system will boot (one time) to the Boot Source Override Target. The value of BootSourceOverrideEnabled is then reset back to Disabled.|
|```Continuous```|The system will boot to the target specified in the BootSourceOverrideTarget until this property is set to Disabled.|

**Boot.BootSourceOverrideMode**
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)

| | |
|---|---|
|Type|string|
|Read Only|False|

The following are the supported values:

|Value|Description|
|---|---|
|```Legacy```|The system will boot in non-UEFI boot mode to the Boot Source Override Target.|
|```UEFI```|The system will boot in UEFI boot mode to the Boot Source Override Target.|

**Boot.BootSourceOverrideTarget**
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)

| | |
|---|---|
|Description|The current boot source to be used at next boot instead of the normal boot device, if BootSourceOverrideEnabled is true.|
|Type|string or null|
|Read Only|False|

**Boot.BootSourceOverrideTarget@Redfish.AllowableValues (array)**
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)
```BootSourceOverrideTarget@Redfish.AllowableValues``` is an array containing elements of:


| | |
|---|---|
|Description|The current boot source to be used at next boot instead of the normal boot device, if BootSourceOverrideEnabled is not Disabled.|
|Type|string or null|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```Null```|A value is temporarily unavailable|
|```None```|Boot from the normal boot device.|
|```Pxe```|Boot from the Pre-Boot EXecution (PXE) environment.|
|```Floppy```|Boot from the floppy disk drive.|
|```Cd```|Boot from the CD/DVD disc.|
|```Usb```|Boot from a USB device as specified by the system BIOS.|
|```Hdd```|Boot from a hard drive.|
|```BiosSetup```|Boot to the BIOS Setup Utility.|
|```Utilities```|Boot the manufacturer's Utilities program(s).|
|```Diags```|Boot the manufacturer's Diagnostics program.|
|```UefiShell```|Boot to the UEFI Shell.|
|```UefiTarget```|Boot to the UEFI Device specified in the UefiTargetBootSourceOverride property.|
|```SDCard```|Boot from an SD Card|
|```UefiHttp```|Boot from a UEFI HTTP network location|

**Boot.UefiTargetBootSourceOverride**
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)

| | |
|---|---|
|Description|This property is the UEFI Device Path of the device to boot from when BootSourceOverrideTarget is UefiTarget.|
|Type|string or null|
|Read Only|False|

**Boot.UefiTargetBootSourceOverride@Redfish.AllowableValues (array)**
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)
```UefiTargetBootSourceOverride@Redfish.AllowableValues``` is an array containing elements of:


| | |
|---|---|
|Description|An array of structured boot strings.|
|Type|string or null|
|Read Only|True|

### EthernetInterfaces
A reference to the collection of Ethernet interfaces associated with this system.
### HostName
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)

| | |
|---|---|
|Description|The DNS Host Name, without any domain information|
|Type|string or null|
|Read Only|True|

### IndicatorLED
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)

| | |
|---|---|
|Description|The state of the indicator LED.|
|Type|string or null|
|Read Only|False|

The following are the supported values:

|Value|Description|
|---|---|
|```Null```|A value is temporarily unavailable|
|```Unknown```|The state of the Indicator LED cannot be determined.|
|```Lit```|The Indicator LED is lit.|
|```Blinking```|The Indicator LED is blinking.|
|```Off```|The Indicator LED is off.|

### LogServices
The LogService collection URI for this resource.
### Manufacturer
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)

| | |
|---|---|
|Description|The manufacturer or OEM of this system.|
|Type|string or null|
|Read Only|True|

### Memory
The central memory in the system.
### MemorySummary
**MemorySummary.Status**
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)
See the Redfish standard schema and specification for information on common Status object.

**MemorySummary.TotalSystemMemoryGiB**
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)

| | |
|---|---|
|Description|This is the total amount of memory in the system measured in GiB.|
|Type|integer or null|
|Read Only|True|

### Model
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)

| | |
|---|---|
|Description|The model information that the manufacturer uses to refer to this system.|
|Type|string or null|
|Read Only|True|

### NetworkInterfaces
The collection of network interfaces partitioned to this system.
### Oem.Hpe.AggregateHealthStatus
**Oem.Hpe.AggregateHealthStatus.AgentlessManagementService**
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)

| | |
|---|---|
|Description|This indicates if the Agentless Management Service is available or not. |
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```Unavailable```|The Agentless Management Service is unavailable.|
|```Ready```|The Agentless Management Service is Ready.|

**Oem.Hpe.AggregateHealthStatus.BiosOrHardwareHealth**
**Oem.Hpe.AggregateHealthStatus.BiosOrHardwareHealth.Status**
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)
See the Redfish standard schema and specification for information on common Status object.

**Oem.Hpe.AggregateHealthStatus.FanRedundancy**
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)

| | |
|---|---|
|Description|This indicates if the Fan is redundant or not. |
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```Redundant```|The fans are Redundant.|
|```NonRedundant```|The fans are not Redundant.|
|```FailedRedundant```|The Redundant fan has failed.|
|```Unknown```|The Redundant state is unknown.|

**Oem.Hpe.AggregateHealthStatus.Fans**
**Oem.Hpe.AggregateHealthStatus.Fans.Status**
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)
See the Redfish standard schema and specification for information on common Status object.

**Oem.Hpe.AggregateHealthStatus.Memory**
**Oem.Hpe.AggregateHealthStatus.Memory.Status**
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)
See the Redfish standard schema and specification for information on common Status object.

**Oem.Hpe.AggregateHealthStatus.Network**
**Oem.Hpe.AggregateHealthStatus.Network.Status**
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)
See the Redfish standard schema and specification for information on common Status object.

**Oem.Hpe.AggregateHealthStatus.PowerSupplies**
**Oem.Hpe.AggregateHealthStatus.PowerSupplies.PowerSuppliesMismatch**
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)

| | |
|---|---|
|Description|This indicates if the there is a mismatch in the power supplies.|
|Type|boolean|
|Read Only|True|

**Oem.Hpe.AggregateHealthStatus.PowerSupplies.Status**
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)
See the Redfish standard schema and specification for information on common Status object.

**Oem.Hpe.AggregateHealthStatus.PowerSupplyRedundancy**
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)

| | |
|---|---|
|Description|This indicates if the Power Supply is redundant or not. |
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```Redundant```|The power supplies are Redundant.|
|```NonRedundant```|The power supplies are not Redundant.|
|```FailedRedundant```|The Redundant power supply has failed.|
|```Unknown```|The Redundant state is unknown.|

**Oem.Hpe.AggregateHealthStatus.Processors**
**Oem.Hpe.AggregateHealthStatus.Processors.Status**
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)
See the Redfish standard schema and specification for information on common Status object.

**Oem.Hpe.AggregateHealthStatus.SmartStorageBattery**
**Oem.Hpe.AggregateHealthStatus.SmartStorageBattery.Status**
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)
See the Redfish standard schema and specification for information on common Status object.

**Oem.Hpe.AggregateHealthStatus.Storage**
**Oem.Hpe.AggregateHealthStatus.Storage.Status**
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)
See the Redfish standard schema and specification for information on common Status object.

**Oem.Hpe.AggregateHealthStatus.Temperatures**
**Oem.Hpe.AggregateHealthStatus.Temperatures.Status**
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)
See the Redfish standard schema and specification for information on common Status object.

### Oem.Hpe.Bios
**Oem.Hpe.Bios.Backup**
**Oem.Hpe.Bios.Backup.BuildNumber**
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)

| | |
|---|---|
|Description|The build number of the firmware.|
|Type|integer|
|Read Only|True|

**Oem.Hpe.Bios.Backup.BuildNumberString**
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)

| | |
|---|---|
|Description|The string version of the build number of the firmware.|
|Type|string|
|Read Only|True|

**Oem.Hpe.Bios.Backup.Date**
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)

| | |
|---|---|
|Description|The build date of the firmware.|
|Type|string|
|Read Only|True|

**Oem.Hpe.Bios.Backup.DebugBuild**
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)

| | |
|---|---|
|Description|True if the firmware is a debug build; False if it is not.|
|Type|boolean|
|Read Only|True|

**Oem.Hpe.Bios.Backup.Family**
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)

| | |
|---|---|
|Description|The family of the firmware.|
|Type|string|
|Read Only|True|

**Oem.Hpe.Bios.Backup.MajorVersion**
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)

| | |
|---|---|
|Description|The major version of the firmware.|
|Type|integer|
|Read Only|True|

**Oem.Hpe.Bios.Backup.MinorVersion**
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)

| | |
|---|---|
|Description|The minor version of the firmware.|
|Type|integer|
|Read Only|True|

**Oem.Hpe.Bios.Backup.Time**
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)

| | |
|---|---|
|Description|The build time of the firmware.|
|Type|string|
|Read Only|True|

**Oem.Hpe.Bios.Backup.VersionString**
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)

| | |
|---|---|
|Description|The version string of the firmware. This value might be null if VersionString is unavailable.|
|Type|string or null|
|Read Only|True|

**Oem.Hpe.Bios.Bootblock**
**Oem.Hpe.Bios.Bootblock.BuildNumber**
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)

| | |
|---|---|
|Description|The build number of the firmware.|
|Type|integer|
|Read Only|True|

**Oem.Hpe.Bios.Bootblock.BuildNumberString**
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)

| | |
|---|---|
|Description|The string version of the build number of the firmware.|
|Type|string|
|Read Only|True|

**Oem.Hpe.Bios.Bootblock.Date**
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)

| | |
|---|---|
|Description|The build date of the firmware.|
|Type|string|
|Read Only|True|

**Oem.Hpe.Bios.Bootblock.DebugBuild**
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)

| | |
|---|---|
|Description|True if the firmware is a debug build; False if it is not.|
|Type|boolean|
|Read Only|True|

**Oem.Hpe.Bios.Bootblock.Family**
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)

| | |
|---|---|
|Description|The family of the firmware.|
|Type|string|
|Read Only|True|

**Oem.Hpe.Bios.Bootblock.MajorVersion**
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)

| | |
|---|---|
|Description|The major version of the firmware.|
|Type|integer|
|Read Only|True|

**Oem.Hpe.Bios.Bootblock.MinorVersion**
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)

| | |
|---|---|
|Description|The minor version of the firmware.|
|Type|integer|
|Read Only|True|

**Oem.Hpe.Bios.Bootblock.Time**
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)

| | |
|---|---|
|Description|The build time of the firmware.|
|Type|string|
|Read Only|True|

**Oem.Hpe.Bios.Bootblock.VersionString**
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)

| | |
|---|---|
|Description|The version string of the firmware. This value might be null if VersionString is unavailable.|
|Type|string or null|
|Read Only|True|

**Oem.Hpe.Bios.Current**
**Oem.Hpe.Bios.Current.BuildNumber**
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)

| | |
|---|---|
|Description|The build number of the firmware.|
|Type|integer|
|Read Only|True|

**Oem.Hpe.Bios.Current.BuildNumberString**
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)

| | |
|---|---|
|Description|The string version of the build number of the firmware.|
|Type|string|
|Read Only|True|

**Oem.Hpe.Bios.Current.Date**
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)

| | |
|---|---|
|Description|The build date of the firmware.|
|Type|string|
|Read Only|True|

**Oem.Hpe.Bios.Current.DebugBuild**
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)

| | |
|---|---|
|Description|True if the firmware is a debug build; False if it is not.|
|Type|boolean|
|Read Only|True|

**Oem.Hpe.Bios.Current.Family**
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)

| | |
|---|---|
|Description|The family of the firmware.|
|Type|string|
|Read Only|True|

**Oem.Hpe.Bios.Current.MajorVersion**
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)

| | |
|---|---|
|Description|The major version of the firmware.|
|Type|integer|
|Read Only|True|

**Oem.Hpe.Bios.Current.MinorVersion**
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)

| | |
|---|---|
|Description|The minor version of the firmware.|
|Type|integer|
|Read Only|True|

**Oem.Hpe.Bios.Current.Time**
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)

| | |
|---|---|
|Description|The build time of the firmware.|
|Type|string|
|Read Only|True|

**Oem.Hpe.Bios.Current.VersionString**
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)

| | |
|---|---|
|Description|The version string of the firmware. This value might be null if VersionString is unavailable.|
|Type|string or null|
|Read Only|True|

**Oem.Hpe.Bios.UefiClass**
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)

| | |
|---|---|
|Description|The UEFI BIOS Class value defined in the UEFI specification.|
|Type|integer|
|Read Only|True|

The following are the supported values:

|Value|
|---|
|```Null```|
|```1```|
|```2```|
|```3```|

### Oem.Hpe.CurrentPowerOnTimeSeconds
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)

| | |
|---|---|
|Description|Displays the amount of time(in seconds) that has passed since the server was last powered on. The data is reset on iLO reset.|
|Type|integer or null|
|Read Only|True|

### Oem.Hpe.DeviceDiscoveryComplete
**Oem.Hpe.DeviceDiscoveryComplete.AMSDeviceDiscovery**
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)

| | |
|---|---|
|Description|This property indicates the current AMS Device Discovery Status.|
|Type|string or null|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```Null```|A value is temporarily unavailable|
|```Busy```|The server has AMS loaded and iLO is discovering devices that require AMS to be loaded|
|```Complete```|The server has AMS loaded and iLO is finished discovering devices that require AMS to be loaded|
|```NoAMS```|The server does not have AMS loaded for device discovery.|
|```Initial```|Default state after iLO has booted.|

**Oem.Hpe.DeviceDiscoveryComplete.DeviceDiscovery**
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)

| | |
|---|---|
|Description|This property indicates the current device discovery status of devices that are not Smart Array or AMS related.|
|Type|string or null|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```Null```|A value is temporarily unavailable|
|```Busy```|iLO is discovering devices.|
|```vAuxDeviceDiscoveryComplete```|The server is off and iLO is finished discovering devices.|
|```vMainDeviceDiscoveryComplete```|The server is on and iLO is finished discovering devices.|
|```DataIncomplete```|iLO response took longer than expected while discovering devices.|
|```Initial```|Default state after iLO has booted.|

**Oem.Hpe.DeviceDiscoveryComplete.SmartArrayDiscovery**
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)

| | |
|---|---|
|Description|This property indicates the current Smart Array Storage Device Discovery Status|
|Type|string or null|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```Null```|A value is temporarily unavailable|
|```Busy```|iLO is discovering Smart Array devices.  If the server is shutdown before discovery is complete, this reflects an incomplete data set.|
|```PendingSoftwareRAID```|Pending discovery of Dynamic Smart Array.|
|```Complete```|iLO is finished discovering Smart Array storage.|
|```Initial```|Default state for Smart Array|
|```Cached```|Data is cached, server is offline or data not yet available.|

### Oem.Hpe.EndOfPostDelaySeconds
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)

| | |
|---|---|
|Description|Supported on UEFI based systems only. The number of seconds to delay before finalizing POST with the Mode action (e.g. delay before shutdown).|
|Type|integer or null|
|Read Only|False|

### Oem.Hpe.HostOS
**Oem.Hpe.HostOS.OsName**
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)

| | |
|---|---|
|Description|from cpqHoName if AMS is running|
|Type|string|
|Read Only|True|

**Oem.Hpe.HostOS.OsSysDescription**
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)

| | |
|---|---|
|Description|from cpqHosysDesc if AMS is running|
|Type|string|
|Read Only|True|

**Oem.Hpe.HostOS.OsType**
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)

| | |
|---|---|
|Description|from cpqHoOsType if AMS is running.|
|Type|integer|
|Read Only|True|

**Oem.Hpe.HostOS.OsVersion**
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)

| | |
|---|---|
|Description|from cpqHoVersion if AMS is running|
|Type|string|
|Read Only|True|

### Oem.Hpe.IntelligentProvisioningAlwaysOn
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)

| | |
|---|---|
|Description|Always on Intelligent Provisioning is available.|
|Type|boolean|
|Read Only|True|

### Oem.Hpe.IntelligentProvisioningIndex
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)

| | |
|---|---|
|Description| Index in the Firmware Version Table for Intelligent Provisioning.|
|Type|integer or null|
|Read Only|True|

### Oem.Hpe.IntelligentProvisioningLocation
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)

| | |
|---|---|
|Description| Location string of Intelligent Provisioning in Firmware Version Table.|
|Type|string|
|Read Only|True|

### Oem.Hpe.IntelligentProvisioningVersion
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)

| | |
|---|---|
|Description| Intelligent Provisioning Version.|
|Type|string|
|Read Only|True|

### Oem.Hpe.PCAPartNumber
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)

| | |
|---|---|
|Description|The PCA part number.|
|Type|string or null|
|Read Only|True|

### Oem.Hpe.PCASerialNumber
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)

| | |
|---|---|
|Description|The PCA serial number.|
|Type|string or null|
|Read Only|True|

### Oem.Hpe.PostDiscoveryCompleteTimeStamp
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)

| | |
|---|---|
|Description|Displays the last known POST Discovery Complete time|
|Type|string or null|
|Read Only|True|

### Oem.Hpe.PostDiscoveryMode
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)

| | |
|---|---|
|Description|The manner in which the system will operate during the discovery section of POST.|
|Type|string or null|
|Read Only|False|

The following are the supported values:

|Value|Description|
|---|---|
|```Null```|A value is temporarily unavailable|
|```Auto```|BIOS will automatically use ForceFastBoot if the system hardware has not changed from last time of FullDiscovery or ForceFullDiscovery if the system hardware has changed.|
|```ForceFullDiscovery```|Server makes a full discovery of all devices.|
|```ForceFastBoot```|Server uses the existing cached discovery data.|

### Oem.Hpe.PostMode
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)

| | |
|---|---|
|Description|The manner in which the system will operate during and at completion of POST.|
|Type|string or null|
|Read Only|False|

The following are the supported values:

|Value|Description|
|---|---|
|```Null```|A value is temporarily unavailable|
|```Normal```|Normal operations.|
|```PostToShutdown```|Server boots until Discovery Completes, then shuts down.|
|```PostToReboot```|Server boots until Discovery Completes, then reboots.|

### Oem.Hpe.PostState
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)

| | |
|---|---|
|Description|The current state of system POST.|
|Type|string or null|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```Null```|A value is temporarily unavailable|
|```Unknown```|iLO was unable to determine the current server state.|
|```Reset```|The server is currently in reset.|
|```PowerOff```|The server power is off.|
|```InPost```|The server is booting and has not reached discovery complete.|
|```InPostDiscoveryComplete```|The server has reached discovery complete and is now waiting for the installed OS to be booted.  Discovery complete is the point at which it has been deemed safe to read and write the BIOS configuration information.|
|```FinishedPost```|The server has booted the installed OS.|

### Oem.Hpe.PowerAllocationLimit
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)

| | |
|---|---|
|Description|The total amount of power allocated to the system.|
|Type|integer or null|
|Read Only|True|

### Oem.Hpe.PowerAutoOn
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)

| | |
|---|---|
|Description|Auto Power-On mode defines what occurs when the AC power is applied to the system.|
|Type|string|
|Read Only|False|

The following are the supported values:

|Value|
|---|
|```RemainOff```|
|```PowerOn```|
|```Restore```|

### Oem.Hpe.PowerOnDelay
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)

| | |
|---|---|
|Description|The PowerAutoOn policy delay that can also be found in the HpBios::PowerOnDelay object.  Will be null if PowerAutoOn is set to RemainOff.  Blades only support Minimum and RandomUpTo120Sec.|
|Type|string or null|
|Read Only|False|

The following are the supported values:

|Value|
|---|
|```Null```|
|```Minimum```|
|```15Sec```|
|```30Sec```|
|```45Sec```|
|```60Sec```|
|```RandomUpTo120Sec```|

### Oem.Hpe.PowerOnMinutes
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)

| | |
|---|---|
|Description|The number of lifetime minutes that the server has been powered on.|
|Type|integer or null|
|Read Only|True|

### Oem.Hpe.PowerRegulatorMode
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)

| | |
|---|---|
|Description|Power Regulator mode.  Switching to and from OS Control mode requires a server reboot to take effect.|
|Type|string|
|Read Only|False|

The following are the supported values:

|Value|
|---|
|```OSControl```|
|```Dynamic```|
|```Max```|
|```Min```|
|```Unknown```|

### Oem.Hpe.PowerRegulatorModesSupported (array)
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)
```PowerRegulatorModesSupported``` is an array containing elements of:


| | |
|---|---|
|Type|string|
|Read Only|True|

### Oem.Hpe.ProcessorJitterControl
**Oem.Hpe.ProcessorJitterControl.FrequencyLimitMHz**
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)

| | |
|---|---|
|Description|Frequency limit of the Processor in MHz.|
|Type|integer|
|Read Only|False|

**Oem.Hpe.ProcessorJitterControl.Mode**
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)

| | |
|---|---|
|Description|Provides various jitter control modes.|
|Type|string|
|Read Only|False|

The following are the supported values:

|Value|
|---|
|```Auto```|
|```Disabled```|
|```Manual```|

### Oem.Hpe.SMBIOS
**Oem.Hpe.SMBIOS.extref**
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)

| | |
|---|---|
|Description|The URI of an external resource.|
|Type|string|
|Read Only|True|

### Oem.Hpe.ServerFQDN
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)

| | |
|---|---|
|Description|The IP address or FQDN of the server. Host software like AMS is required to obtain this value from the OS.|
|Type|string|
|Read Only|True|

### Oem.Hpe.ServerSignature
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)

| | |
|---|---|
|Description| The CRC32 of:  All Device Signatures combined together, Server Slot Location in Enclosure, Enclosure UUID, and Manager Domain IP Address|
|Type|integer or null|
|Read Only|True|

### Oem.Hpe.ServerSignatureStatus
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)

| | |
|---|---|
|Description|The current state of Server Signature.|
|Type|string or null|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```Null```|A value is temporarily unavailable|
|```Initial```|The server signature calculation has not run yet.|
|```Busy```|The server signature calculation is being run.|
|```Invalid```|The server signature is invalid.  Re-compute action necessary.|
|```Complete```|The server signature calculation is complete and valid.|

### Oem.Hpe.SmartStorageConfig (array)
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)
```SmartStorageConfig``` is an array containing elements of:

### Oem.Hpe.VirtualProfile
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)

| | |
|---|---|
|Description|The current state of the systems virtual profile.  This profile is the one that, when the server is rebooted, will set the  Virtual properties.  Intent is to use this state to determine whether the server needs to be rebooted so these values are set.  Additional informaiton about the profile will be considered later.|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|
|---|
|```Active```|
|```Busy```|
|```Inactive```|
|```Unknown```|

### Oem.Hpe.VirtualUUID
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)

| | |
|---|---|
|Description|Used in conjunction with the UUID (Logical) value.|
|Type|string or null|
|Read Only|True|

### PartNumber
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)

| | |
|---|---|
|Description|The manufacturer's system part number.|
|Type|string or null|
|Read Only|True|

### PowerState
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)

| | |
|---|---|
|Description|This is the current power state of the system|
|Type|string or null|
|Read Only|True|

The following are the supported values:

|Value|
|---|
|```Null```|
|```On```|
|```Off```|
|```Unknown```|
|```Reset```|

### ProcessorSummary
**ProcessorSummary.Count**
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)

| | |
|---|---|
|Description|The number of processors in the system.|
|Type|integer or null|
|Read Only|True|

**ProcessorSummary.Model**
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)

| | |
|---|---|
|Description|The processor model for the primary or majority of processors in this system.|
|Type|string or null|
|Read Only|True|

**ProcessorSummary.Status**
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)
See the Redfish standard schema and specification for information on common Status object.

### Processors
The central processors in the system.
### SKU
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)

| | |
|---|---|
|Description|SKU for this system.|
|Type|string or null|
|Read Only|True|

### SecureBoot
A reference to the UEFI SecureBoot resource associated with this system.
### SerialNumber
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)

| | |
|---|---|
|Description|The system serial number.|
|Type|string or null|
|Read Only|True|

### Status
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)
See the Redfish standard schema and specification for information on common Status object.

### Storage
A reference to the collection of storage devices associated with this system.
### SystemType
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)

| | |
|---|---|
|Description|The type of computer system that this resource represents.|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```Physical```|A computer system|
|```Virtual```|A virtual machine instance running on this system|
|```OS```|An operating system instance|
|```PhysicallyPartitioned```|A hardware-based partition of a computer system|
|```VirtuallyPartitioned```|A virtual or software-based partition of a computer system|

### TrustedModules (array)
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)
```TrustedModules``` is an array containing elements of:

**TrustedModules[{item}].FirmwareVersion**
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)

| | |
|---|---|
|Description|The firmware version of this Trusted Module|
|Type|string or null|
|Read Only|True|

**TrustedModules[{item}].InterfaceType**
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)

| | |
|---|---|
|Description|This property indicates the interface type of the Trusted Module.|
|Type|string or null|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```TM1_0```|Trusted Module (TM) 1.0|
|```TPM1_2```|Trusted Platform Module (TPM) 1.2|
|```TPM2_0```|Trusted Platform Module (TPM) 2.0|

**TrustedModules[{item}].Oem.Hpe.VendorName**
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)

| | |
|---|---|
|Description|Trusted module vendor name.|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|
|---|
|```None```|
|```STMicro```|
|```Intel```|
|```Nationz```|
|```Unknown```|

**TrustedModules[{item}].Status**
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)
See the Redfish standard schema and specification for information on common Status object.

### UUID
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)

| | |
|---|---|
|Description|The universal unique identifier for this system.|
|Type|string or null|
|Read Only|True|

### Actions

**ComputerSystem.Reset**
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)

**Parameters:**

**ResetType (string)**

|Value|Description|
|---|---|
|On|
|ForceOff|
|ForceRestart|
|Nmi|
|PushPowerButton|

**HpeComputerSystemExt.SystemReset**
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)

**Parameters:**

**ResetType (string)**

ResetType identifies the type of Action to be performed.

|Value|Description|
|---|---|
|ColdBoot|
|AuxCycle|

**HpeComputerSystemExt.PowerButton**
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)

**Parameters:**

**PushType (string)**

PushType identifies the type of Action to be performed.

|Value|Description|
|---|---|
|Press|
|PressAndHold|

**HpeComputerSystemExt.ServerSigRecompute**
Member of [ComputerSystem.v1_4_0.ComputerSystem](#computersystem-v1_4_0-computersystem)
There are no parameters for this action.
## Drive.v1_0_0.Drive
```@odata.type: "#Drive.v1_0_0.Drive"```
### Resource Instances
|Uri|HTTP Allow|
|---|---|
|```/redfish/v1/chassis/{item}/drives/{interface}/{item}/```|GET |

### Links to other Resources
|Link Name|Destination type
|---|---|
|```Links/Volumes[]```|[Volume](#volume-v1_0_0-volume)|

### BlockSizeBytes
Member of [Drive.v1_0_0.Drive](#drive-v1_0_0-drive)

| | |
|---|---|
|Description|The size of the smallest addressible unit (Block) of this drive in bytes|
|Type|integer or null|
|Read Only|True|

### CapableSpeedGbs
Member of [Drive.v1_0_0.Drive](#drive-v1_0_0-drive)

| | |
|---|---|
|Description|The speed which this drive can communicate to a storage controller in ideal conditions in Gigabits per second|
|Type|integer or null|
|Read Only|True|

### CapacityBytes
Member of [Drive.v1_0_0.Drive](#drive-v1_0_0-drive)

| | |
|---|---|
|Description|The size in bytes of this Drive|
|Type|integer or null|
|Read Only|True|

### FailurePredicted
Member of [Drive.v1_0_0.Drive](#drive-v1_0_0-drive)

| | |
|---|---|
|Description|Is this drive currently predicting a failure in the near future|
|Type|boolean or null|
|Read Only|True|

### Identifiers
**Identifiers.DurableName**
Member of [Drive.v1_0_0.Drive](#drive-v1_0_0-drive)

| | |
|---|---|
|Description|This indicates the world wide, persistent name of the resource.|
|Type|string or null|
|Read Only|True|

**Identifiers.DurableNameFormat**
Member of [Drive.v1_0_0.Drive](#drive-v1_0_0-drive)

| | |
|---|---|
|Description|This represents the format of the DurableName property.|
|Type|string or null|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```EUI```|IEEE-defined 64-bit Extended Unique Identifier|

### Location (array)
Member of [Drive.v1_0_0.Drive](#drive-v1_0_0-drive)
```Location``` is an array containing elements of:

**Location[{item}].Info**
Member of [Drive.v1_0_0.Drive](#drive-v1_0_0-drive)

| | |
|---|---|
|Description|This indicates the location of the resource.|
|Type|string or null|
|Read Only|True|

**Location[{item}].InfoFormat**
Member of [Drive.v1_0_0.Drive](#drive-v1_0_0-drive)

| | |
|---|---|
|Description|This represents the format of the Info property.|
|Type|string or null|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```Box:Bay```|The Info is the box and bay number of the Drive.|
|```BayNumber```|The Info is the bay number of the Drive.|

### Manufacturer
Member of [Drive.v1_0_0.Drive](#drive-v1_0_0-drive)

| | |
|---|---|
|Description|This is the manufacturer of this drive.|
|Type|string or null|
|Read Only|True|

### MediaType
Member of [Drive.v1_0_0.Drive](#drive-v1_0_0-drive)

| | |
|---|---|
|Description|The type of media contained in this drive.|
|Type|string or null|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```HDD```|The drive media type is traditional magnetic platters|
|```SSD```|The drive media type is solid state or flash memory|

### Model
Member of [Drive.v1_0_0.Drive](#drive-v1_0_0-drive)

| | |
|---|---|
|Description|This is the model number for the drive.|
|Type|string or null|
|Read Only|True|

### NegotiatedSpeedGbs
Member of [Drive.v1_0_0.Drive](#drive-v1_0_0-drive)

| | |
|---|---|
|Description|The speed which this drive is currently communicating to the storage controller in Gigabits per second|
|Type|integer or null|
|Read Only|True|

### Oem.Hpe.CriticalWarning
Member of [Drive.v1_0_0.Drive](#drive-v1_0_0-drive)

| | |
|---|---|
|Description|Failure information reported by the drive.|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```AvailableSpareSpace```|Available spare space has fallen below the threshold.|
|```TemperatureTheshold```|A temperature is above an over temperature threshold or below an under temperature threshold.|
|```ReliabilityError```|The NVM subsystem reliability has been degraded due to significant media related errors or any internal error that degrades NVM subsystem reliability.|
|```ReadOnlyMode```|The media has been placed in read only mode.|
|```VolatileBackupFailure```|The volatile memory backup device has failed. This field is only valid if the controller has a volatile memory backup solution|

### Oem.Hpe.CurrentTemperatureCelsius
Member of [Drive.v1_0_0.Drive](#drive-v1_0_0-drive)

| | |
|---|---|
|Description|The current temperature of the drive|
|Type|integer|
|Read Only|True|

### Oem.Hpe.DriveStatus
**Oem.Hpe.DriveStatus.Health**
Member of [Drive.v1_0_0.Drive](#drive-v1_0_0-drive)

| | |
|---|---|
|Description|This represents the health state of this resource in the absence of its dependent resources.|
|Type|string or null|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```Null```|A value is temporarily unavailable|
|```OK```|Normal|
|```Warning```|A condition exists that requires attention|
|```Critical```|A critical condition exists that requires immediate attention|

**Oem.Hpe.DriveStatus.HealthRollup**
Member of [Drive.v1_0_0.Drive](#drive-v1_0_0-drive)

| | |
|---|---|
|Description|This represents the overall health state from the view of this resource.|
|Type|string or null|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```Null```|A value is temporarily unavailable|
|```OK```|Normal|
|```Warning```|A condition exists that requires attention|
|```Critical```|A critical condition exists that requires immediate attention|

**Oem.Hpe.DriveStatus.State**
Member of [Drive.v1_0_0.Drive](#drive-v1_0_0-drive)

| | |
|---|---|
|Description|This indicates the known state of the resource, such as if it is enabled.|
|Type|string or null|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```Null```|A value is temporarily unavailable|
|```Enabled```|This function or resource has been enabled|
|```Disabled```|This function or resource has been disabled|
|```Offline```|This function or resource is enabled, but currently unavailable|
|```InTest```|This function or resource is underdoing testing|
|```Starting```|This function or resource is starting|
|```Absent```|This function or resource is not installed|

### Oem.Hpe.HealthUpdated
Member of [Drive.v1_0_0.Drive](#drive-v1_0_0-drive)

| | |
|---|---|
|Description|Describes how drive health related data (FailurePredicted, PredictedMediaLifeLeftPercent, Status, DriveStatus, CriticalWarning, WearStatus) are updated.|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```Boot```|The health related properties are updated when the system boot and are not updated at runtime.|
|```Dynamic```|The health related properties are updated periodically at runtime.|

### Oem.Hpe.NVMeId
Member of [Drive.v1_0_0.Drive](#drive-v1_0_0-drive)

| | |
|---|---|
|Description|NVMe Identifier:  ModelName, SerialNumber, PCI-Vendor-ID.|
|Type|string|
|Read Only|True|

### Oem.Hpe.PowerOnHours
Member of [Drive.v1_0_0.Drive](#drive-v1_0_0-drive)

| | |
|---|---|
|Description|The number of lifetime hours that the drive has been powered on. The value is null if the disk power on hours cannot be determined or is not supported.|
|Type|integer or null|
|Read Only|True|

### Oem.Hpe.TemperatureStatus
**Oem.Hpe.TemperatureStatus.Health**
Member of [Drive.v1_0_0.Drive](#drive-v1_0_0-drive)

| | |
|---|---|
|Description|This represents the health state of this resource in the absence of its dependent resources.|
|Type|string or null|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```Null```|A value is temporarily unavailable|
|```OK```|Normal|
|```Warning```|A condition exists that requires attention|
|```Critical```|A critical condition exists that requires immediate attention|

**Oem.Hpe.TemperatureStatus.HealthRollup**
Member of [Drive.v1_0_0.Drive](#drive-v1_0_0-drive)

| | |
|---|---|
|Description|This represents the overall health state from the view of this resource.|
|Type|string or null|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```Null```|A value is temporarily unavailable|
|```OK```|Normal|
|```Warning```|A condition exists that requires attention|
|```Critical```|A critical condition exists that requires immediate attention|

**Oem.Hpe.TemperatureStatus.State**
Member of [Drive.v1_0_0.Drive](#drive-v1_0_0-drive)

| | |
|---|---|
|Description|This indicates the known state of the resource, such as if it is enabled.|
|Type|string or null|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```Null```|A value is temporarily unavailable|
|```Enabled```|This function or resource has been enabled|
|```Disabled```|This function or resource has been disabled|
|```Offline```|This function or resource is enabled, but currently unavailable|
|```InTest```|This function or resource is underdoing testing|
|```Starting```|This function or resource is starting|
|```Absent```|This function or resource is not installed|

### Oem.Hpe.WearStatus
Member of [Drive.v1_0_0.Drive](#drive-v1_0_0-drive)

| | |
|---|---|
|Description|The wear status of the drive, an estimation of remaining life span.|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```OK```|The SSD is not in any imminent danger of wear out.|
|```FiftySixDayThreshold```|Indicates that based upon the current workload, the solid state disk will reach the maximum usage limit for writes (wear out) within fifty-six days. You should modify your write workload or begin preparing to replace your SSD drive|
|```FivePercentThreshold```|Indicates that the solid state disk has passed the five percent threshold and is at or below five percent of reaching the maximum usage limit for writes (wear out). You should begin to prepare to replace your SSD drive.|
|```TwoPercentThreshold```|Indicates that the solid state disk has passed the two percent threshold and is at or below two percent of reaching the maximum usage limit for writes (wear out). You should begin to prepare to replace your SSD drive.|
|```SSDWearOut```|Indicates that a solid state drive is approaching the maximum usage limit for writes (wear out) and should be replaced as soon as possible.|
|```Unknown```|The SSD wear status cannot be determined.|

### PartNumber
Member of [Drive.v1_0_0.Drive](#drive-v1_0_0-drive)

| | |
|---|---|
|Description|The part number for this drive.|
|Type|string or null|
|Read Only|True|

### PredictedMediaLifeLeftPercent
Member of [Drive.v1_0_0.Drive](#drive-v1_0_0-drive)

| | |
|---|---|
|Description|The percentage of reads and writes that are predicted to still be available for the media|
|Type|integer or null|
|Read Only|True|

### Protocol
Member of [Drive.v1_0_0.Drive](#drive-v1_0_0-drive)

| | |
|---|---|
|Description|The protocol this drive is using to communicate to the storage controller|
|Type|string or null|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```NVMe```|Non-Volatile Memory Express|
|```SATA```|Serial AT Attachment|
|```USB```|Universal Serial Bus|

### Revision
Member of [Drive.v1_0_0.Drive](#drive-v1_0_0-drive)

| | |
|---|---|
|Description|The revision of this Drive|
|Type|string or null|
|Read Only|True|

### RotationSpeedRPM
Member of [Drive.v1_0_0.Drive](#drive-v1_0_0-drive)

| | |
|---|---|
|Description|The rotation speed of this Drive in Revolutions per Minute (RPM)|
|Type|integer or null|
|Read Only|True|

### SerialNumber
Member of [Drive.v1_0_0.Drive](#drive-v1_0_0-drive)

| | |
|---|---|
|Description|Serial Number of the drive.|
|Type|string or null|
|Read Only|True|

### Status
Member of [Drive.v1_0_0.Drive](#drive-v1_0_0-drive)
See the Redfish standard schema and specification for information on common Status object.

## EthernetInterface.v1_0_3.EthernetInterface
```@odata.type: "#EthernetInterface.v1_0_3.EthernetInterface"```

The schema definition of a simple Ethernet NIC resource.
### Resource Instances
|Uri|HTTP Allow|
|---|---|
|```/redfish/v1/managers/{item}/ethernetinterfaces/{item}/```|GET PATCH |
|```/redfish/v1/systems/{item}/ethernetinterfaces/{item}/```|GET |

### AutoNeg
Member of [EthernetInterface.v1_0_3.EthernetInterface](#ethernetinterface-v1_0_3-ethernetinterface)

| | |
|---|---|
|Description|This indicates if the speed and duplex is automatically configured by the NIC.|
|Type|boolean or null|
|Read Only|False|

### FQDN
Member of [EthernetInterface.v1_0_3.EthernetInterface](#ethernetinterface-v1_0_3-ethernetinterface)

| | |
|---|---|
|Description|The complete, fully qualified domain name obtained by DNS for this NIC.|
|Type|string or null|
|Read Only|True|

### FrameSize
Member of [EthernetInterface.v1_0_3.EthernetInterface](#ethernetinterface-v1_0_3-ethernetinterface)

| | |
|---|---|
|Description|The MAC frame size (bytes).|
|Type|integer or null|
|Read Only|False|

### FullDuplex
Member of [EthernetInterface.v1_0_3.EthernetInterface](#ethernetinterface-v1_0_3-ethernetinterface)

| | |
|---|---|
|Description|The connection duplex status. If AutoNeg is enabled, this property cannot be modified. AutoNeg is only applicable and modifiable for a dedicated network port and cannot be modified for blade servers.|
|Type|boolean or null|
|Read Only|False|

### HostName
Member of [EthernetInterface.v1_0_3.EthernetInterface](#ethernetinterface-v1_0_3-ethernetinterface)

| | |
|---|---|
|Description|The DNS Host Name, without any domain information.|
|Type|string or null|
|Read Only|True|

### IPv4Addresses (array)
Member of [EthernetInterface.v1_0_3.EthernetInterface](#ethernetinterface-v1_0_3-ethernetinterface)
```IPv4Addresses``` is an array containing elements of:

**IPv4Addresses[{item}].Address**
Member of [EthernetInterface.v1_0_3.EthernetInterface](#ethernetinterface-v1_0_3-ethernetinterface)

| | |
|---|---|
|Description|The IPv4 Address.|
|Type|string or null|
|Read Only|False|

**IPv4Addresses[{item}].AddressOrigin**
Member of [EthernetInterface.v1_0_3.EthernetInterface](#ethernetinterface-v1_0_3-ethernetinterface)

| | |
|---|---|
|Description|How the address was determined.|
|Type|string or null|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```Null```|A value is temporarily unavailable|
|```DHCP```|The address is provided by a DHCP service.|
|```Static```|A static address as configured by the user.|

**IPv4Addresses[{item}].Gateway**
Member of [EthernetInterface.v1_0_3.EthernetInterface](#ethernetinterface-v1_0_3-ethernetinterface)

| | |
|---|---|
|Description|The IPv4 gateway for this address.|
|Type|string or null|
|Read Only|False|

**IPv4Addresses[{item}].SubnetMask**
Member of [EthernetInterface.v1_0_3.EthernetInterface](#ethernetinterface-v1_0_3-ethernetinterface)

| | |
|---|---|
|Description|The IPv4 Subnet mask.|
|Type|string or null|
|Read Only|False|

### IPv6AddressPolicyTable (array)
Member of [EthernetInterface.v1_0_3.EthernetInterface](#ethernetinterface-v1_0_3-ethernetinterface)
```IPv6AddressPolicyTable``` is an array containing elements of:

**IPv6AddressPolicyTable[{item}].Label**
Member of [EthernetInterface.v1_0_3.EthernetInterface](#ethernetinterface-v1_0_3-ethernetinterface)

| | |
|---|---|
|Description|The label value for this table entry, as defined in RFC3484 section 2.1.|
|Type|integer or null|
|Read Only|False|

**IPv6AddressPolicyTable[{item}].Precedence**
Member of [EthernetInterface.v1_0_3.EthernetInterface](#ethernetinterface-v1_0_3-ethernetinterface)

| | |
|---|---|
|Description|The precedence value for this table entry as defined in RFC3484 section 2.1.|
|Type|integer or null|
|Read Only|False|

**IPv6AddressPolicyTable[{item}].Prefix**
Member of [EthernetInterface.v1_0_3.EthernetInterface](#ethernetinterface-v1_0_3-ethernetinterface)

| | |
|---|---|
|Description|The IPv6 Address Prefix for this table entry as defined in RFC3484 section 2.1.|
|Type|string or null|
|Read Only|False|

### IPv6Addresses (array)
Member of [EthernetInterface.v1_0_3.EthernetInterface](#ethernetinterface-v1_0_3-ethernetinterface)
```IPv6Addresses``` is an array containing elements of:

**IPv6Addresses[{item}].Address**
Member of [EthernetInterface.v1_0_3.EthernetInterface](#ethernetinterface-v1_0_3-ethernetinterface)

| | |
|---|---|
|Description|The IPv6 Address.|
|Type|string or null|
|Read Only|True|

**IPv6Addresses[{item}].AddressOrigin**
Member of [EthernetInterface.v1_0_3.EthernetInterface](#ethernetinterface-v1_0_3-ethernetinterface)

| | |
|---|---|
|Description|How the address was determined.|
|Type|string or null|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```Null```|A value is temporarily unavailable|
|```DHCP```|The address is provided by a DHCP service.|
|```Static```|A static address as configured by the user.|
|```SLAAC```|The address is provided by a Stateless Address AutoConfiguration (SLAAC) service.|

**IPv6Addresses[{item}].AddressState**
Member of [EthernetInterface.v1_0_3.EthernetInterface](#ethernetinterface-v1_0_3-ethernetinterface)

| | |
|---|---|
|Description|The current state of this address as defined in RFC 4862.|
|Type|string or null|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```Null```|A value is temporarily unavailable|
|```Preferred```|This address is currently within both its valid and preferred lifetimes as defined in RFC 4862.|
|```Deprecated```|This address is currently within its valid lifetime, but the address is now outside of its preferred lifetime as defined in RFC 4862.|
|```Tentative```|This address is currently undergoing Duplicate Address Detection testing as defined in RFC 4862 section 5.4.|
|```Failed```|This address has a problem with Duplicate Address Detection testing as defined in RFC 4862 section 5.4 and is not currently in use.|

**IPv6Addresses[{item}].PrefixLength**
Member of [EthernetInterface.v1_0_3.EthernetInterface](#ethernetinterface-v1_0_3-ethernetinterface)

| | |
|---|---|
|Description|The IPv6 Address Prefix Length.|
|Type|integer or null|
|Read Only|True|

### IPv6DefaultGateway
Member of [EthernetInterface.v1_0_3.EthernetInterface](#ethernetinterface-v1_0_3-ethernetinterface)

| | |
|---|---|
|Description|The IPv6 default gateway address that is currently in use on this interface.|
|Type|string or null|
|Read Only|True|

### IPv6StaticAddresses (array)
Member of [EthernetInterface.v1_0_3.EthernetInterface](#ethernetinterface-v1_0_3-ethernetinterface)
```IPv6StaticAddresses``` is an array containing elements of:

**IPv6StaticAddresses[{item}].Address**
Member of [EthernetInterface.v1_0_3.EthernetInterface](#ethernetinterface-v1_0_3-ethernetinterface)

| | |
|---|---|
|Description|A valid IPv6 address.|
|Type|string or null|
|Read Only|False|

**IPv6StaticAddresses[{item}].PrefixLength**
Member of [EthernetInterface.v1_0_3.EthernetInterface](#ethernetinterface-v1_0_3-ethernetinterface)

| | |
|---|---|
|Description|The Prefix Length of this IPv6 address.|
|Type|integer or null|
|Read Only|False|

### LinkStatus
Member of [EthernetInterface.v1_0_3.EthernetInterface](#ethernetinterface-v1_0_3-ethernetinterface)

| | |
|---|---|
|Description|The link status of this interface (port).|
|Type|string or null|
|Read Only|True|

The following are the supported values:

|Value|
|---|
|```LinkUp```|
|```NoLink```|
|```LinkDown```|
|```Null```|

### MACAddress
Member of [EthernetInterface.v1_0_3.EthernetInterface](#ethernetinterface-v1_0_3-ethernetinterface)

| | |
|---|---|
|Description|The effective current MAC address. If the assignable MAC address is not supported, this is a read-only alias of FactoryMacAddress.|
|Type|string or null|
|Read Only|False|

### MaxIPv6StaticAddresses
Member of [EthernetInterface.v1_0_3.EthernetInterface](#ethernetinterface-v1_0_3-ethernetinterface)

| | |
|---|---|
|Description|The maximum number of IPv6 static addresses that can be configured on this interface.|
|Type|integer or null|
|Read Only|True|

### NameServers (array)
Member of [EthernetInterface.v1_0_3.EthernetInterface](#ethernetinterface-v1_0_3-ethernetinterface)
```NameServers``` is an array containing elements of:


| | |
|---|---|
|Type|string or null|
|Read Only|True|

### Oem.Hpe.ConfigurationSettings
Member of [EthernetInterface.v1_0_3.EthernetInterface](#ethernetinterface-v1_0_3-ethernetinterface)

| | |
|---|---|
|Description|The state of the currently displayed configuration settings.|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```Current```|All configuration settings for this NIC are currently in use.|
|```SomePendingReset```|One or more configuration settings on this NIC are not yet in use.  They require a reset of this management processor in order to take effect.|

### Oem.Hpe.DHCPv4
**Oem.Hpe.DHCPv4.Enabled**
Member of [EthernetInterface.v1_0_3.EthernetInterface](#ethernetinterface-v1_0_3-ethernetinterface)

| | |
|---|---|
|Description|Determines whether DHCPv4 is enabled.|
|Type|boolean|
|Read Only|False|

**Oem.Hpe.DHCPv4.UseDNSServers**
Member of [EthernetInterface.v1_0_3.EthernetInterface](#ethernetinterface-v1_0_3-ethernetinterface)

| | |
|---|---|
|Description|Determines whether to use DHCPv4-supplied DNS servers. Can only be enabled when DHCPv4 is also enabled; otherwise, this property will be set to false and will be read-only.|
|Type|boolean|
|Read Only|False|

**Oem.Hpe.DHCPv4.UseDomainName**
Member of [EthernetInterface.v1_0_3.EthernetInterface](#ethernetinterface-v1_0_3-ethernetinterface)

| | |
|---|---|
|Description|Determines whether to use a DHCPv4-supplied domain name. Can only be enabled when DHCPv4 is also enabled; otherwis,e this property will be set to false and will be read-only.|
|Type|boolean|
|Read Only|False|

**Oem.Hpe.DHCPv4.UseGateway**
Member of [EthernetInterface.v1_0_3.EthernetInterface](#ethernetinterface-v1_0_3-ethernetinterface)

| | |
|---|---|
|Description|Determines whether to use a DHCPv4-supplied gateway. Can only be enabled when DHCPv4 is also enabled; otherwise, this property will be set to false and will be read-only.|
|Type|boolean|
|Read Only|False|

**Oem.Hpe.DHCPv4.UseNTPServers**
Member of [EthernetInterface.v1_0_3.EthernetInterface](#ethernetinterface-v1_0_3-ethernetinterface)

| | |
|---|---|
|Description|Determines whether to use DHCPv4-supplied NTP servers. Can only be enabled when DHCPv4 is also enabled; otherwise, this property will be set to false and will be read-only.|
|Type|boolean|
|Read Only|False|

**Oem.Hpe.DHCPv4.UseStaticRoutes**
Member of [EthernetInterface.v1_0_3.EthernetInterface](#ethernetinterface-v1_0_3-ethernetinterface)

| | |
|---|---|
|Description|Determines whether to use DHCPv4-supplied static routes. Can only be enabled when DHCPv4 is also enabled; otherwise, this property will be set to false and will be read-only.|
|Type|boolean|
|Read Only|False|

**Oem.Hpe.DHCPv4.UseWINSServers**
Member of [EthernetInterface.v1_0_3.EthernetInterface](#ethernetinterface-v1_0_3-ethernetinterface)

| | |
|---|---|
|Description|Determines whether to use DHCPv4-supplied WINS servers. Can only be enabled when DHCPv4 is also enabled; otherwise, this property will be set to false and will be read-only.|
|Type|boolean|
|Read Only|False|

### Oem.Hpe.DHCPv6
**Oem.Hpe.DHCPv6.StatefulModeEnabled**
Member of [EthernetInterface.v1_0_3.EthernetInterface](#ethernetinterface-v1_0_3-ethernetinterface)

| | |
|---|---|
|Description|Determines whether DHCPv6 Stateful mode is enabled.|
|Type|boolean|
|Read Only|False|

**Oem.Hpe.DHCPv6.StatelessModeEnabled**
Member of [EthernetInterface.v1_0_3.EthernetInterface](#ethernetinterface-v1_0_3-ethernetinterface)

| | |
|---|---|
|Description|Determines whether DHCPv6 Stateless mode is enabled.  Always enabled by default whenever DHCPv6 Stateful mode is also enabled.|
|Type|boolean|
|Read Only|False|

**Oem.Hpe.DHCPv6.UseDNSServers**
Member of [EthernetInterface.v1_0_3.EthernetInterface](#ethernetinterface-v1_0_3-ethernetinterface)

| | |
|---|---|
|Description|Determines whether to use DHCPv6-supplied DNS servers. Can only be enabled when DHCPv6 Stateless mode is also enabled; otherwise, this property will be set to false and will be read-only.|
|Type|boolean|
|Read Only|False|

**Oem.Hpe.DHCPv6.UseDomainName**
Member of [EthernetInterface.v1_0_3.EthernetInterface](#ethernetinterface-v1_0_3-ethernetinterface)

| | |
|---|---|
|Description|Determines whether to use a DHCPv6-supplied domain name. Can only be enabled when DHCPv6 Stateless mode is also enabled; otherwise, this property will be set to false and will be read-only.|
|Type|boolean|
|Read Only|False|

**Oem.Hpe.DHCPv6.UseNTPServers**
Member of [EthernetInterface.v1_0_3.EthernetInterface](#ethernetinterface-v1_0_3-ethernetinterface)

| | |
|---|---|
|Description|Determines whether to use DHCPv6-supplied NTP servers. Can only be enabled when DHCPv6 Stateless mode is also enabled; otherwise, this property will be set to false and will be read-only.|
|Type|boolean|
|Read Only|False|

**Oem.Hpe.DHCPv6.UseRapidCommit**
Member of [EthernetInterface.v1_0_3.EthernetInterface](#ethernetinterface-v1_0_3-ethernetinterface)

| | |
|---|---|
|Description|Determines whether to use DHCPv6 rapid commit mode. Can only be enabled when DHCPv6 Stateful mode is also enabled; otherwise, this property will be set to false and will be read-only. Do not enable in networks where more than one DHCPv6 server is configured to provide address assignments.|
|Type|boolean|
|Read Only|False|

### Oem.Hpe.DomainName
Member of [EthernetInterface.v1_0_3.EthernetInterface](#ethernetinterface-v1_0_3-ethernetinterface)

| | |
|---|---|
|Description|Domain name of the network to which this management processor belongs. This property can only be modified when the management processor is not configured to use a DHCP supplied domain name; otherwise this property is read-only indicating the value is provided by DHCP.|
|Type|string|
|Read Only|False|

### Oem.Hpe.HostName
Member of [EthernetInterface.v1_0_3.EthernetInterface](#ethernetinterface-v1_0_3-ethernetinterface)

| | |
|---|---|
|Description|The management processor host name.|
|Type|string|
|Read Only|False|

### Oem.Hpe.IPv4
**Oem.Hpe.IPv4.DDNSRegistration**
Member of [EthernetInterface.v1_0_3.EthernetInterface](#ethernetinterface-v1_0_3-ethernetinterface)

| | |
|---|---|
|Description|Determines whether DDNS registration is enabled.|
|Type|boolean|
|Read Only|False|

**Oem.Hpe.IPv4.DNSServers (array)**
Member of [EthernetInterface.v1_0_3.EthernetInterface](#ethernetinterface-v1_0_3-ethernetinterface)
```DNSServers``` is an array containing elements of:


| | |
|---|---|
|Type|string|
|Read Only|True|

**Oem.Hpe.IPv4.StaticRoutes (array)**
Member of [EthernetInterface.v1_0_3.EthernetInterface](#ethernetinterface-v1_0_3-ethernetinterface)
```StaticRoutes``` is an array containing elements of:

**StaticRoutes[{item}].Destination**
Member of [EthernetInterface.v1_0_3.EthernetInterface](#ethernetinterface-v1_0_3-ethernetinterface)

| | |
|---|---|
|Description|An IPv4 static route destination. Only writeable when use of DHCPv4-supplied static routes is disabled; otherwise this property is read-only indicating the value is provided by DHCPv4.|
|Type|string|
|Read Only|False|

**StaticRoutes[{item}].Gateway**
Member of [EthernetInterface.v1_0_3.EthernetInterface](#ethernetinterface-v1_0_3-ethernetinterface)

| | |
|---|---|
|Description|An IPv4 static route gateway. Only writeable when use of DHCPv4-supplied static routes is disabled; otherwise this property is read-only indicating the value is provided by DHCPv4.|
|Type|string|
|Read Only|False|

**StaticRoutes[{item}].SubnetMask**
Member of [EthernetInterface.v1_0_3.EthernetInterface](#ethernetinterface-v1_0_3-ethernetinterface)

| | |
|---|---|
|Description|An IPv4 static route subnet mask. Only writeable when use of DHCPv4-supplied static routes is disabled; otherwise this property is read-only indicating the value is provided by DHCPv4.|
|Type|string|
|Read Only|False|

**Oem.Hpe.IPv4.WINSRegistration**
Member of [EthernetInterface.v1_0_3.EthernetInterface](#ethernetinterface-v1_0_3-ethernetinterface)

| | |
|---|---|
|Description|Determines whether WINS registration is enabled.|
|Type|boolean|
|Read Only|False|

**Oem.Hpe.IPv4.WINSServers (array)**
Member of [EthernetInterface.v1_0_3.EthernetInterface](#ethernetinterface-v1_0_3-ethernetinterface)
```WINSServers``` is an array containing elements of:


| | |
|---|---|
|Type|string|
|Read Only|True|

### Oem.Hpe.IPv6
**Oem.Hpe.IPv6.DDNSRegistration**
Member of [EthernetInterface.v1_0_3.EthernetInterface](#ethernetinterface-v1_0_3-ethernetinterface)

| | |
|---|---|
|Description|Determines whether IPv6 DDNS registration is enabled.|
|Type|boolean|
|Read Only|False|

**Oem.Hpe.IPv6.DNSServers (array)**
Member of [EthernetInterface.v1_0_3.EthernetInterface](#ethernetinterface-v1_0_3-ethernetinterface)
```DNSServers``` is an array containing elements of:


| | |
|---|---|
|Type|string|
|Read Only|True|

**Oem.Hpe.IPv6.SLAACEnabled**
Member of [EthernetInterface.v1_0_3.EthernetInterface](#ethernetinterface-v1_0_3-ethernetinterface)

| | |
|---|---|
|Description|Determines whether StateLess Address Auto-Configuration is enabled.|
|Type|boolean|
|Read Only|False|

**Oem.Hpe.IPv6.StaticDefaultGateway**
Member of [EthernetInterface.v1_0_3.EthernetInterface](#ethernetinterface-v1_0_3-ethernetinterface)

| | |
|---|---|
|Description|The IPv6 static default gateway entry.|
|Type|string|
|Read Only|False|

**Oem.Hpe.IPv6.StaticRoutes (array)**
Member of [EthernetInterface.v1_0_3.EthernetInterface](#ethernetinterface-v1_0_3-ethernetinterface)
```StaticRoutes``` is an array containing elements of:

**StaticRoutes[{item}].Destination**
Member of [EthernetInterface.v1_0_3.EthernetInterface](#ethernetinterface-v1_0_3-ethernetinterface)

| | |
|---|---|
|Description|The IPv6 static route destination address.|
|Type|string|
|Read Only|False|

**StaticRoutes[{item}].Gateway**
Member of [EthernetInterface.v1_0_3.EthernetInterface](#ethernetinterface-v1_0_3-ethernetinterface)

| | |
|---|---|
|Description|The IPv6 static route gateway.|
|Type|string|
|Read Only|False|

**StaticRoutes[{item}].PrefixLength**
Member of [EthernetInterface.v1_0_3.EthernetInterface](#ethernetinterface-v1_0_3-ethernetinterface)

| | |
|---|---|
|Description|The prefix length of the IPv6 static route destination address.|
|Type|integer or null|
|Read Only|False|

**StaticRoutes[{item}].Status**
Member of [EthernetInterface.v1_0_3.EthernetInterface](#ethernetinterface-v1_0_3-ethernetinterface)
See the Redfish standard schema and specification for information on common Status object.

### Oem.Hpe.InterfaceType
Member of [EthernetInterface.v1_0_3.EthernetInterface](#ethernetinterface-v1_0_3-ethernetinterface)

| | |
|---|---|
|Description|Describes the network interface type.|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|
|---|
|```Dedicated```|
|```Shared```|

### Oem.Hpe.NICEnabled
Member of [EthernetInterface.v1_0_3.EthernetInterface](#ethernetinterface-v1_0_3-ethernetinterface)

| | |
|---|---|
|Description|Determines whether this NIC is enabled or disabled. Enabling one NIC will disable the others. If no NIC is enabled, this management processor is not accessible over the network.|
|Type|boolean|
|Read Only|False|

### Oem.Hpe.NICSupportsIPv6
Member of [EthernetInterface.v1_0_3.EthernetInterface](#ethernetinterface-v1_0_3-ethernetinterface)

| | |
|---|---|
|Description|Indicates whether or not this NIC can support the IPv6 protocol.|
|Type|boolean|
|Read Only|True|

### Oem.Hpe.PingGatewayOnStartup
Member of [EthernetInterface.v1_0_3.EthernetInterface](#ethernetinterface-v1_0_3-ethernetinterface)

| | |
|---|---|
|Description|Determines whether to ping the IPv4 gateway on startup.|
|Type|boolean|
|Read Only|False|

### Oem.Hpe.SharedNetworkPortOptions
**Oem.Hpe.SharedNetworkPortOptions.NIC**
Member of [EthernetInterface.v1_0_3.EthernetInterface](#ethernetinterface-v1_0_3-ethernetinterface)

| | |
|---|---|
|Description|Selects the system NIC that is to be shared with this management processor.|
|Type|string|
|Read Only|False|

The following are the supported values:

|Value|Description|
|---|---|
|```LOM```|The LOM NIC is configured to be shared.|
|```FlexibleLOM```|The FlexibleLOM NIC is configured to be shared.|

**Oem.Hpe.SharedNetworkPortOptions.Port**
Member of [EthernetInterface.v1_0_3.EthernetInterface](#ethernetinterface-v1_0_3-ethernetinterface)

| | |
|---|---|
|Description|The network adapter port number that is used for sharing. This feature is only applicable on systems and network adapters that support it.|
|Type|integer|
|Read Only|False|

### Oem.Hpe.SupportsFlexibleLOM
Member of [EthernetInterface.v1_0_3.EthernetInterface](#ethernetinterface-v1_0_3-ethernetinterface)

| | |
|---|---|
|Description|Indicates whether this system supports FlexibleLOM. Only applies to Shared Network Port.|
|Type|boolean|
|Read Only|True|

### Oem.Hpe.SupportsLOM
Member of [EthernetInterface.v1_0_3.EthernetInterface](#ethernetinterface-v1_0_3-ethernetinterface)

| | |
|---|---|
|Description|Indicates whether this system supports LOM. Only applies to Shared Network Port.|
|Type|boolean|
|Read Only|True|

### PermanentMACAddress
Member of [EthernetInterface.v1_0_3.EthernetInterface](#ethernetinterface-v1_0_3-ethernetinterface)

| | |
|---|---|
|Description|This is the MAC address assigned to this NIC at the factory.|
|Type|string or null|
|Read Only|True|

### SettingsResult
**SettingsResult.ETag**
Member of [EthernetInterface.v1_0_3.EthernetInterface](#ethernetinterface-v1_0_3-ethernetinterface)

| | |
|---|---|
|Description|The ETag of the resource to which the settings were applied, after the application.|
|Type|string or null|
|Read Only|True|

**SettingsResult.Operation**
Member of [EthernetInterface.v1_0_3.EthernetInterface](#ethernetinterface-v1_0_3-ethernetinterface)

| | |
|---|---|
|Description|Last operation detail.|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|
|---|
|```SettingsApply```|

**SettingsResult.Time**
Member of [EthernetInterface.v1_0_3.EthernetInterface](#ethernetinterface-v1_0_3-ethernetinterface)

| | |
|---|---|
|Description|Indicates the time the settings were applied.|
|Type|string or null|
|Read Only|True|

### SpeedMbps
Member of [EthernetInterface.v1_0_3.EthernetInterface](#ethernetinterface-v1_0_3-ethernetinterface)

| | |
|---|---|
|Description|The link speed of the Ethernet interface in megabits per second. If AutoNeg is enabled, this property cannot be modified. This property can only be modified on a dedicated network port. It cannot be modified for blade servers.|
|Type|integer or null|
|Read Only|False|

The following are the supported values:

|Value|
|---|
|```Null```|
|```5000```|
|```2500```|
|```1000```|
|```100```|
|```10```|

### Status
Member of [EthernetInterface.v1_0_3.EthernetInterface](#ethernetinterface-v1_0_3-ethernetinterface)
See the Redfish standard schema and specification for information on common Status object.

### UefiDevicePath
Member of [EthernetInterface.v1_0_3.EthernetInterface](#ethernetinterface-v1_0_3-ethernetinterface)

| | |
|---|---|
|Description|The UEFI device path for this NIC.|
|Type|string or null|
|Read Only|True|

### VLAN
**VLAN.VLANEnable**
Member of [EthernetInterface.v1_0_3.EthernetInterface](#ethernetinterface-v1_0_3-ethernetinterface)

| | |
|---|---|
|Description|This indicates if this VLAN is enabled.|
|Type|boolean or null|
|Read Only|False|

**VLAN.VLANId**
Member of [EthernetInterface.v1_0_3.EthernetInterface](#ethernetinterface-v1_0_3-ethernetinterface)

| | |
|---|---|
|Description|This indicates the VLAN identifier for this VLAN.|
|Type|integer or null|
|Read Only|False|

### VLANs
**VLANs.Members (array)**
Member of [EthernetInterface.v1_0_3.EthernetInterface](#ethernetinterface-v1_0_3-ethernetinterface)
```Members``` is an array containing elements of:

**VLANs.Members@odata.count**
Member of [EthernetInterface.v1_0_3.EthernetInterface](#ethernetinterface-v1_0_3-ethernetinterface)

| | |
|---|---|
|Description|The total number of collection members.|
|Type|integer|
|Read Only|True|

## EventService.v1_0_1.EventService
```@odata.type: "#EventService.v1_0_1.EventService"```

This is the schema definition for the Event Service.  It represents the properties for the service itself and has links to the actual list of subscriptions.
### Resource Instances
|Uri|HTTP Allow|
|---|---|
|```/redfish/v1/eventservice/```|GET POST |

### Links to other Resources
|Link Name|Destination type
|---|---|
|```Subscriptions```|Collection of [EventDestination](#eventdestination-v1_0_0-eventdestination)|
|```Oem/Hpe/CACertificates```|Collection of [HpeCertificate](#hpecertificate-v1_0_0-hpecertificate)|

### DeliveryRetryAttempts
Member of [EventService.v1_0_1.EventService](#eventservice-v1_0_1-eventservice)

| | |
|---|---|
|Description|This is the number of attempts an event posting is retried before the subscription is terminated.|
|Type|integer|
|Read Only|True|

### DeliveryRetryIntervalSeconds
Member of [EventService.v1_0_1.EventService](#eventservice-v1_0_1-eventservice)

| | |
|---|---|
|Description|This represents the number of seconds between retry attempts for sending any given Event|
|Type|integer|
|Read Only|True|

### EventTypesForSubscription (array)
Member of [EventService.v1_0_1.EventService](#eventservice-v1_0_1-eventservice)
```EventTypesForSubscription``` is an array containing elements of:


| | |
|---|---|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```StatusChange```|The status of this resource has changed|
|```ResourceUpdated```|The value of this resource has been updated|
|```ResourceAdded```|A resource has been added|
|```ResourceRemoved```|A resource has been removed|
|```Alert```|A condition exists which requires attention|

### Oem.Hpe.CACertificates
The value of this property shall be a reference to a Collection of HpeCertificate resources.
### Oem.Hpe.RequestedMaxEventsToQueueDefault
Member of [EventService.v1_0_1.EventService](#eventservice-v1_0_1-eventservice)

| | |
|---|---|
|Description|This represents the default number of events the service should queue.|
|Type|integer|
|Read Only|True|

### Oem.Hpe.RetireOldEventInMinutesDefault
Member of [EventService.v1_0_1.EventService](#eventservice-v1_0_1-eventservice)

| | |
|---|---|
|Description|This represents the default number of minutes until an event is expired.|
|Type|integer|
|Read Only|True|

### Oem.Hpe.TTLCountDefault
Member of [EventService.v1_0_1.EventService](#eventservice-v1_0_1-eventservice)

| | |
|---|---|
|Description|The default number of TTLUnits until this listener destination subscription expires.  It may be renewed prior to expire to reset the Time to Live counter.  The value 999999 is reserved to mean a perpetual subscription.|
|Type|integer|
|Read Only|True|

### Oem.Hpe.TTLUnitsDefault
Member of [EventService.v1_0_1.EventService](#eventservice-v1_0_1-eventservice)

| | |
|---|---|
|Description|The default time unit used to measure the subscription time of this listener destination.  This is the units for TTLCount and is used to express the subscription lifetime of the listener destination.|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```seconds```|Time to Live (TTL) in Seconds|
|```minutes```|Time to Live (TTL) in Minutes|
|```days```|Time to Live (TTL) in Days|

### Status
Member of [EventService.v1_0_1.EventService](#eventservice-v1_0_1-eventservice)
See the Redfish standard schema and specification for information on common Status object.

### Subscriptions
This is a reference to a collection of ListenerDestination resources.
### Actions

**EventService.SubmitTestEvent**
Member of [EventService.v1_0_1.EventService](#eventservice-v1_0_1-eventservice)

**Parameters:**

**EventID (string)**

**Severity (string)**

|Value|Description|
|---|---|
|OK|
|Warning|
|Critical|

**EventType (string)**

|Value|Description|
|---|---|
|StatusChange|
|ResourceUpdated|
|ResourceAdded|
|ResourceRemoved|
|Alert|

**OriginOfCondition (string)**

**EventTimestamp (string)**

**MessageID (string)**

**Message (string)**

**MessageArgs (array)**

**HpeEventService.ImportCACertificate**
Member of [EventService.v1_0_1.EventService](#eventservice-v1_0_1-eventservice)
Imports a Trusted CA Certificate


**Parameters:**

**Certificate (string)**

Contains PEM formatted X509 certificate or PKCS7 certificate chain (Base64 encoded).
## HpeBaseConfigs.v2_0_0.HpeBaseConfigs
```@odata.type: "#HpeBaseConfigs.v2_0_0.HpeBaseConfigs"```
### Resource Instances
|Uri|HTTP Allow|
|---|---|
|```/redfish/v1/systems/{item}/bios/baseconfigs/```|GET |
|```/redfish/v1/systems/{item}/bios/boot/baseconfigs/```|GET |
|```/redfish/v1/systems/{item}/bios/iscsi/baseconfigs/```|GET |
|```/redfish/v1/systems/{item}/bios/tlsconfig/baseconfigs/```|GET |

### BaseConfigs (array)
Member of [HpeBaseConfigs.v2_0_0.HpeBaseConfigs](#hpebaseconfigs-v2_0_0-hpebaseconfigs)
```BaseConfigs``` is an array containing elements of:

### Capabilities
**Capabilities.BaseConfig**
Member of [HpeBaseConfigs.v2_0_0.HpeBaseConfigs](#hpebaseconfigs-v2_0_0-hpebaseconfigs)

| | |
|---|---|
|Type|boolean|
|Read Only|True|

**Capabilities.BaseConfigs**
Member of [HpeBaseConfigs.v2_0_0.HpeBaseConfigs](#hpebaseconfigs-v2_0_0-hpebaseconfigs)

| | |
|---|---|
|Type|boolean|
|Read Only|True|

## HpeBaseNetworkAdapter.v2_0_0.HpeBaseNetworkAdapter
```@odata.type: "#HpeBaseNetworkAdapter.v2_0_0.HpeBaseNetworkAdapter"```
### Resource Instances
|Uri|HTTP Allow|
|---|---|
|```/redfish/v1/systems/{item}/basenetworkadapters/{item}/```|GET |

### FcPorts (array)
Member of [HpeBaseNetworkAdapter.v2_0_0.HpeBaseNetworkAdapter](#hpebasenetworkadapter-v2_0_0-hpebasenetworkadapter)
```FcPorts``` is an array containing elements of:

**FcPorts[{item}].PortNumber**
Member of [HpeBaseNetworkAdapter.v2_0_0.HpeBaseNetworkAdapter](#hpebasenetworkadapter-v2_0_0-hpebasenetworkadapter)

| | |
|---|---|
|Description|Port Number.|
|Type|integer or null|
|Read Only|True|

**FcPorts[{item}].WWNN**
Member of [HpeBaseNetworkAdapter.v2_0_0.HpeBaseNetworkAdapter](#hpebasenetworkadapter-v2_0_0-hpebasenetworkadapter)

| | |
|---|---|
|Description|World Wide Node Name.|
|Type|string or null|
|Read Only|True|

**FcPorts[{item}].WWPN**
Member of [HpeBaseNetworkAdapter.v2_0_0.HpeBaseNetworkAdapter](#hpebasenetworkadapter-v2_0_0-hpebasenetworkadapter)

| | |
|---|---|
|Description|World Wide Port Name.|
|Type|string or null|
|Read Only|True|

### Firmware
**Firmware.Current**
**Firmware.Current.VersionString**
Member of [HpeBaseNetworkAdapter.v2_0_0.HpeBaseNetworkAdapter](#hpebasenetworkadapter-v2_0_0-hpebasenetworkadapter)

| | |
|---|---|
|Description|This string represents the version of the firmware image.|
|Type|string or null|
|Read Only|True|

### PartNumber
Member of [HpeBaseNetworkAdapter.v2_0_0.HpeBaseNetworkAdapter](#hpebasenetworkadapter-v2_0_0-hpebasenetworkadapter)

| | |
|---|---|
|Description|The device part number.|
|Type|string or null|
|Read Only|True|

### PhysicalPorts (array)
Member of [HpeBaseNetworkAdapter.v2_0_0.HpeBaseNetworkAdapter](#hpebasenetworkadapter-v2_0_0-hpebasenetworkadapter)
```PhysicalPorts``` is an array containing elements of:

**PhysicalPorts[{item}].FullDuplex**
Member of [HpeBaseNetworkAdapter.v2_0_0.HpeBaseNetworkAdapter](#hpebasenetworkadapter-v2_0_0-hpebasenetworkadapter)

| | |
|---|---|
|Description|Full-duplex data transmission means that data can be transmitted in both directions on a signal carrier at the same time.|
|Type|boolean or null|
|Read Only|True|

**PhysicalPorts[{item}].IPv4Addresses (array)**
Member of [HpeBaseNetworkAdapter.v2_0_0.HpeBaseNetworkAdapter](#hpebasenetworkadapter-v2_0_0-hpebasenetworkadapter)
```IPv4Addresses``` is an array containing elements of:

**IPv4Addresses[{item}].Address**
Member of [HpeBaseNetworkAdapter.v2_0_0.HpeBaseNetworkAdapter](#hpebasenetworkadapter-v2_0_0-hpebasenetworkadapter)

| | |
|---|---|
|Description|This is the IPv4 Address.|
|Type|string or null|
|Read Only|True|

**PhysicalPorts[{item}].IPv6Addresses (array)**
Member of [HpeBaseNetworkAdapter.v2_0_0.HpeBaseNetworkAdapter](#hpebasenetworkadapter-v2_0_0-hpebasenetworkadapter)
```IPv6Addresses``` is an array containing elements of:

**IPv6Addresses[{item}].Address**
Member of [HpeBaseNetworkAdapter.v2_0_0.HpeBaseNetworkAdapter](#hpebasenetworkadapter-v2_0_0-hpebasenetworkadapter)

| | |
|---|---|
|Description|This is the IPv6 Address.|
|Type|string or null|
|Read Only|True|

**PhysicalPorts[{item}].LinkStatus**
Member of [HpeBaseNetworkAdapter.v2_0_0.HpeBaseNetworkAdapter](#hpebasenetworkadapter-v2_0_0-hpebasenetworkadapter)

| | |
|---|---|
|Description|The link status of this interface (port).|
|Type|string or null|
|Read Only|True|

The following are the supported values:

|Value|
|---|
|```LinkUp```|
|```NoLink```|
|```LinkDown```|
|```Null```|

**PhysicalPorts[{item}].MacAddress**
Member of [HpeBaseNetworkAdapter.v2_0_0.HpeBaseNetworkAdapter](#hpebasenetworkadapter-v2_0_0-hpebasenetworkadapter)

| | |
|---|---|
|Description|The port MAC address.|
|Type|string or null|
|Read Only|True|

**PhysicalPorts[{item}].Oem.Hpe.BadReceives**
Member of [HpeBaseNetworkAdapter.v2_0_0.HpeBaseNetworkAdapter](#hpebasenetworkadapter-v2_0_0-hpebasenetworkadapter)

| | |
|---|---|
|Description|A count of frames that were received by the adapter but which had an error.  This counter is the sum of mib items cpqNicIfPhysAdapterAlignmentErrors, cpqNicIfPhysAdapterFCSErrors, cpqNicIfPhysAdapterFrameTooLongs, and cpqNicIfPhysAdapterInternalMacReceiveErrors. If this counter increments frequently, check the more detailed error statistics and take appropriate action.|
|Type|integer or null|
|Read Only|True|

**PhysicalPorts[{item}].Oem.Hpe.BadTransmits**
Member of [HpeBaseNetworkAdapter.v2_0_0.HpeBaseNetworkAdapter](#hpebasenetworkadapter-v2_0_0-hpebasenetworkadapter)

| | |
|---|---|
|Description|A count of frames that were not transmitted by the adapter because of an error.  This counter is the sum of MIB items cpqNicIfPhysAdapterDeferredTransmissions, cpqNicIfPhysAdapterLateCollisions, cpqNicIfPhysAdapterExcessiveCollisions, cpqNicIfPhysAdapterCarrierSenseErrors, and cpqNicIfPhysAdapterInternalMacTransmitErrors. If this counter increments frequently, check the more detailed error statistics and take appropriate action.|
|Type|integer or null|
|Read Only|True|

**PhysicalPorts[{item}].Oem.Hpe.GoodReceives**
Member of [HpeBaseNetworkAdapter.v2_0_0.HpeBaseNetworkAdapter](#hpebasenetworkadapter-v2_0_0-hpebasenetworkadapter)

| | |
|---|---|
|Description|A count of frames successfully received by the physical adapter.|
|Type|integer or null|
|Read Only|True|

**PhysicalPorts[{item}].Oem.Hpe.GoodTransmits**
Member of [HpeBaseNetworkAdapter.v2_0_0.HpeBaseNetworkAdapter](#hpebasenetworkadapter-v2_0_0-hpebasenetworkadapter)

| | |
|---|---|
|Description|A count of frames successfully transmitted by the physical adapter.|
|Type|integer or null|
|Read Only|True|

**PhysicalPorts[{item}].Oem.Hpe.StructuredName**
Member of [HpeBaseNetworkAdapter.v2_0_0.HpeBaseNetworkAdapter](#hpebasenetworkadapter-v2_0_0-hpebasenetworkadapter)

| | |
|---|---|
|Description|PCI device structured name in UTF-8 format (e.g. 'NIC.LOM.1.1' - see PCIDevices in /rest/v1/Systems/x/PCIDevices - this comes from SMBIOS|
|Type|string or null|
|Read Only|True|

**PhysicalPorts[{item}].Oem.Hpe.Team**
Member of [HpeBaseNetworkAdapter.v2_0_0.HpeBaseNetworkAdapter](#hpebasenetworkadapter-v2_0_0-hpebasenetworkadapter)

| | |
|---|---|
|Description|If a port is configured for NIC teaming, the name of the configured link between the physical ports that form a logical network adapter. This value is displayed for system NICs only (embedded and stand-up).|
|Type|string or null|
|Read Only|True|

**PhysicalPorts[{item}].SpeedMbps**
Member of [HpeBaseNetworkAdapter.v2_0_0.HpeBaseNetworkAdapter](#hpebasenetworkadapter-v2_0_0-hpebasenetworkadapter)

| | |
|---|---|
|Description|An estimate of the interface's current bandwidth in Megabits per second.  For interfaces which do not vary in bandwidth or for those where no accurate estimation can be made, this object should contain the nominal bandwidth.|
|Type|integer or null|
|Read Only|True|

**PhysicalPorts[{item}].Status**
Member of [HpeBaseNetworkAdapter.v2_0_0.HpeBaseNetworkAdapter](#hpebasenetworkadapter-v2_0_0-hpebasenetworkadapter)
See the Redfish standard schema and specification for information on common Status object.

**PhysicalPorts[{item}].UEFIDevicePath**
Member of [HpeBaseNetworkAdapter.v2_0_0.HpeBaseNetworkAdapter](#hpebasenetworkadapter-v2_0_0-hpebasenetworkadapter)

| | |
|---|---|
|Description|UEFIDevice Path for correlation purposes|
|Type|string or null|
|Read Only|True|

### SerialNumber
Member of [HpeBaseNetworkAdapter.v2_0_0.HpeBaseNetworkAdapter](#hpebasenetworkadapter-v2_0_0-hpebasenetworkadapter)

| | |
|---|---|
|Description|The device serial number.|
|Type|string or null|
|Read Only|True|

### Status
Member of [HpeBaseNetworkAdapter.v2_0_0.HpeBaseNetworkAdapter](#hpebasenetworkadapter-v2_0_0-hpebasenetworkadapter)
See the Redfish standard schema and specification for information on common Status object.

### StructuredName
Member of [HpeBaseNetworkAdapter.v2_0_0.HpeBaseNetworkAdapter](#hpebasenetworkadapter-v2_0_0-hpebasenetworkadapter)

| | |
|---|---|
|Description|PCI device structured name in UTF-8 format (e.g. 'NIC.LOM.1.1' - see PCIDevices in /rest/v1/Systems/x/PCIDevices - this comes from SMBIOS|
|Type|string or null|
|Read Only|True|

### UEFIDevicePath
Member of [HpeBaseNetworkAdapter.v2_0_0.HpeBaseNetworkAdapter](#hpebasenetworkadapter-v2_0_0-hpebasenetworkadapter)

| | |
|---|---|
|Description|UEFIDevice Path for correlation purposes|
|Type|string or null|
|Read Only|True|

## HpeBiosMapping.v2_0_0.HpeBiosMapping
```@odata.type: "#HpeBiosMapping.v2_0_0.HpeBiosMapping"```

This is the schema definition for the BIOS Attributes Mappings resource.
### Resource Instances
|Uri|HTTP Allow|
|---|---|
|```/redfish/v1/systems/{item}/bios/mappings/```|GET |

### AttributeRegistry
Member of [HpeBiosMapping.v2_0_0.HpeBiosMapping](#hpebiosmapping-v2_0_0-hpebiosmapping)

| | |
|---|---|
|Description|The Resource ID of the Attribute Registry for the BIOS Attributes resource.|
|Type|string or null|
|Read Only|True|

### BiosPciSettingsMappings (array)
Member of [HpeBiosMapping.v2_0_0.HpeBiosMapping](#hpebiosmapping-v2_0_0-hpebiosmapping)
```BiosPciSettingsMappings``` is an array containing elements of:

**BiosPciSettingsMappings[{item}].Associations (array)**
Member of [HpeBiosMapping.v2_0_0.HpeBiosMapping](#hpebiosmapping-v2_0_0-hpebiosmapping)
```Associations``` is an array containing elements of:

**BiosPciSettingsMappings[{item}].CorrelatableID**
Member of [HpeBiosMapping.v2_0_0.HpeBiosMapping](#hpebiosmapping-v2_0_0-hpebiosmapping)

| | |
|---|---|
|Description|Contains any CorrelatableIDs that represent this PCI device. The CorrelatableID values can be JSON Pointers or UEFI identifiers.|
|Type|string|
|Read Only|True|

**BiosPciSettingsMappings[{item}].Instance**
Member of [HpeBiosMapping.v2_0_0.HpeBiosMapping](#hpebiosmapping-v2_0_0-hpebiosmapping)

| | |
|---|---|
|Description|The instance number of the parent PCI device for this association set.|
|Type|integer|
|Read Only|True|

**BiosPciSettingsMappings[{item}].Subinstances (array)**
Member of [HpeBiosMapping.v2_0_0.HpeBiosMapping](#hpebiosmapping-v2_0_0-hpebiosmapping)
```Subinstances``` is an array containing elements of:

**Subinstances[{item}].Associations (array)**
Member of [HpeBiosMapping.v2_0_0.HpeBiosMapping](#hpebiosmapping-v2_0_0-hpebiosmapping)
```Associations``` is an array containing elements of:


| | |
|---|---|
|Type|string|
|Read Only|True|

**Subinstances[{item}].CorrelatableID**
Member of [HpeBiosMapping.v2_0_0.HpeBiosMapping](#hpebiosmapping-v2_0_0-hpebiosmapping)

| | |
|---|---|
|Description|Contains any CorrelatableIDs that represent this PCI device. The CorrelatableID values can be JSON Pointers or UEFI identifiers.|
|Type|string|
|Read Only|True|

**Subinstances[{item}].Subinstance**
Member of [HpeBiosMapping.v2_0_0.HpeBiosMapping](#hpebiosmapping-v2_0_0-hpebiosmapping)

| | |
|---|---|
|Description|The sub-instance number of the child PCI device for this association set.|
|Type|integer|
|Read Only|True|

## HpeCertAuth.v1_1_0.HpeCertAuth
```@odata.type: "#HpeCertAuth.v1_1_0.HpeCertAuth"```

This is the schema definition for certificate based authentication configuration.
### Resource Instances
|Uri|HTTP Allow|
|---|---|
|```/redfish/v1/managers/{item}/securityservice/certificateauthentication/```|GET POST PATCH |

### Links to other Resources
|Link Name|Destination type
|---|---|
|```CACertificates```|Collection of [HpeCertificate](#hpecertificate-v1_0_0-hpecertificate)|
|```Links/UserCertificateMapping```|Collection of [HpeiLOAccountCertificateMap](#hpeiloaccountcertificatemap-v1_0_1-hpeiloaccountcertificatemap)|

### CACertificates
The value of this property shall be a reference to a Collection of HpeCertificate resources.
### CRLIssuer
Member of [HpeCertAuth.v1_1_0.HpeCertAuth](#hpecertauth-v1_1_0-hpecertauth)

| | |
|---|---|
|Description|Issuer of the installed CRL, if present.|
|Type|string or null|
|Read Only|True|

### CRLSerial
Member of [HpeCertAuth.v1_1_0.HpeCertAuth](#hpecertauth-v1_1_0-hpecertauth)

| | |
|---|---|
|Description|Serial Number of the installed CRL, if present.|
|Type|string or null|
|Read Only|True|

### CertificateLoginEnabled
Member of [HpeCertAuth.v1_1_0.HpeCertAuth](#hpecertauth-v1_1_0-hpecertauth)

| | |
|---|---|
|Description|Specifies whether Certificate login is enabled.|
|Type|boolean|
|Read Only|False|

### LDAPCertificateNameMapping
Member of [HpeCertAuth.v1_1_0.HpeCertAuth](#hpecertauth-v1_1_0-hpecertauth)

| | |
|---|---|
|Description|The method used to map a certificate to its associated LDAP user account.|
|Type|string|
|Read Only|False|

The following are the supported values:

|Value|Description|
|---|---|
|```SubjectCN```|The CN portion of the certificate subject will be used as the LDAP username.|
|```SubjectDN```|The fully qualified DN of the certificate subject will be used as the LDAP username.|
|```SANRFC822```|The RFC822 name from the certificate's subjectAlternativeName extension will be used as the LDAP username.|
|```SANUPN```|The UserPrincipalName from the certificate's subjectAlternativeName extension will be used as the LDAP username.|

### OCSPUri
Member of [HpeCertAuth.v1_1_0.HpeCertAuth](#hpecertauth-v1_1_0-hpecertauth)

| | |
|---|---|
|Description|URL to use for OCSP certificate checking.|
|Type|string or null|
|Read Only|False|

### StrictCACModeEnabled
Member of [HpeCertAuth.v1_1_0.HpeCertAuth](#hpecertauth-v1_1_0-hpecertauth)

| | |
|---|---|
|Description|Whether or not Strict CAC Mode is enabled.|
|Type|boolean|
|Read Only|False|

### Actions

**HpeCertAuth.DeleteCRL**
Member of [HpeCertAuth.v1_1_0.HpeCertAuth](#hpecertauth-v1_1_0-hpecertauth)
Remove an installed Certificate Revocation List (CRL).

There are no parameters for this action.

**HpeCertAuth.ImportCRL**
Member of [HpeCertAuth.v1_1_0.HpeCertAuth](#hpecertauth-v1_1_0-hpecertauth)
Imports a Certificate Revocation List (CRL).


**Parameters:**

**ImportUri (string)**

Contains URI of PEM formatted certificate revocation list (CRL) (Base64 encoded).

**HpeCertAuth.ImportCACertificate**
Member of [HpeCertAuth.v1_1_0.HpeCertAuth](#hpecertauth-v1_1_0-hpecertauth)
Imports a Trusted Certificate


**Parameters:**

**Certificate (string)**

Contains PEM formatted X509 certificate or PKCS7 certificate chain (Base64 encoded).
## HpeComponent.v1_0_0.HpeComponent
```@odata.type: "#HpeComponent.v1_0_0.HpeComponent"```
### Resource Instances
|Uri|HTTP Allow|
|---|---|
|```/redfish/v1/updateservice/componentrepository/{item}/```|GET PATCH DELETE |

### Activates
Member of [HpeComponent.v1_0_0.HpeComponent](#hpecomponent-v1_0_0-hpecomponent)

| | |
|---|---|
|Description|Indicates when a component becomes active after being updated.|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```Immediately```|The update activates immediately.|
|```AfterReboot```|The update activates after a host server reboot.|
|```AfterDeviceReset```|The update activates after a device reset.|
|```AfterHardPowerCycle```|The update activates after a full power supply disconnect or E-Fuse reset.|

### ComponentType
Member of [HpeComponent.v1_0_0.HpeComponent](#hpecomponent-v1_0_0-hpecomponent)

| | |
|---|---|
|Description|HTTP-style content-type of binary|
|Type|string|
|Read Only|True|

### ComponentUri
Member of [HpeComponent.v1_0_0.HpeComponent](#hpecomponent-v1_0_0-hpecomponent)

| | |
|---|---|
|Description|URI of the component binary.|
|Type|string|
|Read Only|True|

### Configuration
Member of [HpeComponent.v1_0_0.HpeComponent](#hpecomponent-v1_0_0-hpecomponent)

| | |
|---|---|
|Description|string defining customized parameters for some components provided by client at upload time and given to the component at execution time (Type D only).|
|Type|string|
|Read Only|False|

### Created
Member of [HpeComponent.v1_0_0.HpeComponent](#hpecomponent-v1_0_0-hpecomponent)

| | |
|---|---|
|Description|ISO 8601 time string indicating when this component was added to the NAND.|
|Type|string|
|Read Only|True|

### Criticality
Member of [HpeComponent.v1_0_0.HpeComponent](#hpecomponent-v1_0_0-hpecomponent)
### Criticality
Member of [HpeComponent.v1_0_0.HpeComponent](#hpecomponent-v1_0_0-hpecomponent)
### Criticality
Member of [HpeComponent.v1_0_0.HpeComponent](#hpecomponent-v1_0_0-hpecomponent)

| | |
|---|---|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|
|---|
|```Optional```|
|```Recommended```|
|```Critical```|

### DeviceClass
Member of [HpeComponent.v1_0_0.HpeComponent](#hpecomponent-v1_0_0-hpecomponent)

| | |
|---|---|
|Description|Device type GUID from iLO secure flash header|
|Type|string|
|Read Only|True|

### ExecutionParameters
Member of [HpeComponent.v1_0_0.HpeComponent](#hpecomponent-v1_0_0-hpecomponent)

| | |
|---|---|
|Description|Client supplied execution parameters.  These are supplied at upload time and given to the component at execution time (Type D only).|
|Type|string|
|Read Only|False|

### Filename
Member of [HpeComponent.v1_0_0.HpeComponent](#hpecomponent-v1_0_0-hpecomponent)

| | |
|---|---|
|Description|The unique filename of the component.|
|Type|string|
|Read Only|True|

### Filepath
Member of [HpeComponent.v1_0_0.HpeComponent](#hpecomponent-v1_0_0-hpecomponent)

| | |
|---|---|
|Description|Path of file on the USB LUN if you mount the repo as USB.|
|Type|string|
|Read Only|True|

### Locked
Member of [HpeComponent.v1_0_0.HpeComponent](#hpecomponent-v1_0_0-hpecomponent)

| | |
|---|---|
|Description|If true, this component cannot be removed with DELETE because it is referenced by an Install Set|
|Type|boolean|
|Read Only|True|

### SizeBytes
Member of [HpeComponent.v1_0_0.HpeComponent](#hpecomponent-v1_0_0-hpecomponent)

| | |
|---|---|
|Description|Size of the component file in bytes.|
|Type|integer or null|
|Read Only|True|

### Targets (array)
Member of [HpeComponent.v1_0_0.HpeComponent](#hpecomponent-v1_0_0-hpecomponent)
```Targets``` is an array containing elements of:


| | |
|---|---|
|Description|Target GUIDs from secure flash header or sidecar file.|
|Type|string|
|Read Only|True|

### UpdatableBy (array)
Member of [HpeComponent.v1_0_0.HpeComponent](#hpecomponent-v1_0_0-hpecomponent)
```UpdatableBy``` is an array containing elements of:


| | |
|---|---|
|Description|Describes which types of update agents may apply this component.|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```Uefi```|This component may be scheduled for update by UEFI BIOS.|
|```RuntimeAgent```|This component may be scheduled for update by a runtime update agent such as Smart Update Manager or Smart Update Tool.|
|```Bmc```|This component may be scheduled for update by iLO.|

### Version
Member of [HpeComponent.v1_0_0.HpeComponent](#hpecomponent-v1_0_0-hpecomponent)

| | |
|---|---|
|Description|Version of the component from secure flash header or sidecar file.|
|Type|string|
|Read Only|True|

## HpeComponentInstallSet.v1_0_1.HpeComponentInstallSet
```@odata.type: "#HpeComponentInstallSet.v1_0_1.HpeComponentInstallSet"```
### Resource Instances
|Uri|HTTP Allow|
|---|---|
|```/redfish/v1/updateservice/installsets/{item}/```|GET POST PATCH DELETE |

### Created
Member of [HpeComponentInstallSet.v1_0_1.HpeComponentInstallSet](#hpecomponentinstallset-v1_0_1-hpecomponentinstallset)

| | |
|---|---|
|Description|ISO-time of install set creation.|
|Type|string or null|
|Read Only|True|

### IsRecovery
Member of [HpeComponentInstallSet.v1_0_1.HpeComponentInstallSet](#hpecomponentinstallset-v1_0_1-hpecomponentinstallset)

| | |
|---|---|
|Description|If true, this install set is reserved to hold only critical firmware recovery updatable by iLO.  Additionally the 'Administrate Recovery Set' iLO privilege is required to modify or remove this install set.|
|Type|boolean|
|Read Only|False|

### Modified
Member of [HpeComponentInstallSet.v1_0_1.HpeComponentInstallSet](#hpecomponentinstallset-v1_0_1-hpecomponentinstallset)

| | |
|---|---|
|Description|ISO-time of install modification.|
|Type|string or null|
|Read Only|True|

### Sequence (array)
Member of [HpeComponentInstallSet.v1_0_1.HpeComponentInstallSet](#hpecomponentinstallset-v1_0_1-hpecomponentinstallset)
```Sequence``` is an array containing elements of:

**Sequence[{item}].Command**
Member of [HpeComponentInstallSet.v1_0_1.HpeComponentInstallSet](#hpecomponentinstallset-v1_0_1-hpecomponentinstallset)

| | |
|---|---|
|Description|Command to execute.|
|Type|string|
|Read Only|False|

The following are the supported values:

|Value|Description|
|---|---|
|```ApplyUpdate```|Apply an update using the specified component.|
|```ResetServer```|Reset the server.|
|```ResetBmc```|Reset the BMC.|
|```Wait```|Wait for the WaitTimeSeconds number of seconds.|

**Sequence[{item}].Component**
Member of [HpeComponentInstallSet.v1_0_1.HpeComponentInstallSet](#hpecomponentinstallset-v1_0_1-hpecomponentinstallset)

| | |
|---|---|
|Type|string|
|Read Only|True|

**Sequence[{item}].Filename**
Member of [HpeComponentInstallSet.v1_0_1.HpeComponentInstallSet](#hpecomponentinstallset-v1_0_1-hpecomponentinstallset)

| | |
|---|---|
|Description|The unique filename of the component.  This correlates to 'Filename' in the HpeComponent.|
|Type|string|
|Read Only|False|

**Sequence[{item}].UpdatableBy (array)**
Member of [HpeComponentInstallSet.v1_0_1.HpeComponentInstallSet](#hpecomponentinstallset-v1_0_1-hpecomponentinstallset)
```UpdatableBy``` is an array containing elements of:


| | |
|---|---|
|Type|string|
|Read Only|False|

The following are the supported values:

|Value|Description|
|---|---|
|```Bmc```|This component may be scheduled for update by iLO.|
|```Uefi```|This component may be scheduled for update by UEFI BIOS.|
|```RuntimeAgent```|This component may be scheduled for update by a runtime update agent such as Smart Update Manager or Smart Update Tool.|

**Sequence[{item}].WaitTimeSeconds**
Member of [HpeComponentInstallSet.v1_0_1.HpeComponentInstallSet](#hpecomponentinstallset-v1_0_1-hpecomponentinstallset)

| | |
|---|---|
|Description|The number of seconds to pause if the command is 'Wait'.  Ignored otherwise.|
|Type|integer|
|Read Only|False|

### Actions

**HpeComponentInstallSet.Invoke**
Member of [HpeComponentInstallSet.v1_0_1.HpeComponentInstallSet](#hpecomponentinstallset-v1_0_1-hpecomponentinstallset)

**Parameters:**

**UpdateRecoverySet (boolean)**

If true then the components in the flash operations are used to replace matching contents in the Recovery Set.
## HpeComponentUpdateTask.v1_0_1.HpeComponentUpdateTask
```@odata.type: "#HpeComponentUpdateTask.v1_0_1.HpeComponentUpdateTask"```
### Resource Instances
|Uri|HTTP Allow|
|---|---|
|```/redfish/v1/updateservice/updatetaskqueue/{item}/```||

### Command
Member of [HpeComponentUpdateTask.v1_0_1.HpeComponentUpdateTask](#hpecomponentupdatetask-v1_0_1-hpecomponentupdatetask)

| | |
|---|---|
|Description|Command to execute.|
|Type|string|
|Read Only|False|

The following are the supported values:

|Value|Description|
|---|---|
|```ApplyUpdate```|Apply an update using the specified component.|
|```ResetServer```|Reset the server.|
|```ResetBmc```|Reset the BMC.|
|```Wait```|Wait for the WaitTimeSeconds number of seconds.|

### Component
Member of [HpeComponentUpdateTask.v1_0_1.HpeComponentUpdateTask](#hpecomponentupdatetask-v1_0_1-hpecomponentupdatetask)

| | |
|---|---|
|Type|string|
|Read Only|True|

### Created
Member of [HpeComponentUpdateTask.v1_0_1.HpeComponentUpdateTask](#hpecomponentupdatetask-v1_0_1-hpecomponentupdatetask)

| | |
|---|---|
|Description|ISO-time of task creation (by whomever created this thing)|
|Type|string|
|Read Only|True|

### Expire
Member of [HpeComponentUpdateTask.v1_0_1.HpeComponentUpdateTask](#hpecomponentupdatetask-v1_0_1-hpecomponentupdatetask)

| | |
|---|---|
|Description|ISO 8601 Redfish-style time string after which we will automatically change state to Expired - null for no expire time|
|Type|string|
|Read Only|False|

### Filename
Member of [HpeComponentUpdateTask.v1_0_1.HpeComponentUpdateTask](#hpecomponentupdatetask-v1_0_1-hpecomponentupdatetask)

| | |
|---|---|
|Description|The unique filename of the component.  This correlates to 'Filename' in the HpeComponent.|
|Type|string|
|Read Only|False|

### Modified
Member of [HpeComponentUpdateTask.v1_0_1.HpeComponentUpdateTask](#hpecomponentupdatetask-v1_0_1-hpecomponentupdatetask)

| | |
|---|---|
|Description|ISO-time of last task queue item update by updater (not client)|
|Type|string|
|Read Only|True|

### Result
**Result.MessageArgs (array)**
Member of [HpeComponentUpdateTask.v1_0_1.HpeComponentUpdateTask](#hpecomponentupdatetask-v1_0_1-hpecomponentupdatetask)
```MessageArgs``` is an array containing elements of:


| | |
|---|---|
|Type|string|
|Read Only|True|

**Result.MessageId**
Member of [HpeComponentUpdateTask.v1_0_1.HpeComponentUpdateTask](#hpecomponentupdatetask-v1_0_1-hpecomponentupdatetask)

| | |
|---|---|
|Description|The key for this message that can be used to look up the message in a message registry.|
|Type|string|
|Read Only|False|

### ResultLog
Member of [HpeComponentUpdateTask.v1_0_1.HpeComponentUpdateTask](#hpecomponentupdatetask-v1_0_1-hpecomponentupdatetask)

| | |
|---|---|
|Description|base64 encoded entry to capture component log.  Estimated to be generally 1-2KB. written by updater|
|Type|string or null|
|Read Only|False|

### StartAfter
Member of [HpeComponentUpdateTask.v1_0_1.HpeComponentUpdateTask](#hpecomponentupdatetask-v1_0_1-hpecomponentupdatetask)

| | |
|---|---|
|Description|ISO 8601 Redfish-style time string of earliest execution - null for no start time specified|
|Type|string|
|Read Only|False|

### State
Member of [HpeComponentUpdateTask.v1_0_1.HpeComponentUpdateTask](#hpecomponentupdatetask-v1_0_1-hpecomponentupdatetask)

| | |
|---|---|
|Description|The current state of the update task.|
|Type|string|
|Read Only|False|

The following are the supported values:

|Value|Description|
|---|---|
|```Pending```|The task is pending execution.|
|```InProgress```|The task is executing.|
|```Complete```|The task was completed and the results are available in the Results.|
|```Expired```|The task will not execute because the current time is after the 'Expire' time.|
|```Exception```|The task was unsuccessful because of an exception condition.|
|```Canceled```|The task is no longer scheduled to run.|

### TPMOverride
Member of [HpeComponentUpdateTask.v1_0_1.HpeComponentUpdateTask](#hpecomponentupdatetask-v1_0_1-hpecomponentupdatetask)

| | |
|---|---|
|Description|If true then the TPMOverrideFlag is passed in on the associated flash operations.|
|Type|boolean|
|Read Only|False|

### UpdatableBy (array)
Member of [HpeComponentUpdateTask.v1_0_1.HpeComponentUpdateTask](#hpecomponentupdatetask-v1_0_1-hpecomponentupdatetask)
```UpdatableBy``` is an array containing elements of:


| | |
|---|---|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```Bmc```|This component may be scheduled for update by iLO.|
|```Uefi```|This component may be scheduled for update by UEFI BIOS.|
|```RuntimeAgent```|This component may be scheduled for update by a runtime update agent such as Smart Update Manager or Smart Update Tool.|

### UpdateRecoverySet
Member of [HpeComponentUpdateTask.v1_0_1.HpeComponentUpdateTask](#hpecomponentupdatetask-v1_0_1-hpecomponentupdatetask)

| | |
|---|---|
|Description|Update Recovery Set with this component if the command is 'ApplyUpdate'.  Ignored otherwise.|
|Type|boolean|
|Read Only|False|

### WaitTimeSeconds
Member of [HpeComponentUpdateTask.v1_0_1.HpeComponentUpdateTask](#hpecomponentupdatetask-v1_0_1-hpecomponentupdatetask)

| | |
|---|---|
|Description|The number of seconds to pause if the command is 'Wait'.  Ignored otherwise.|
|Type|integer|
|Read Only|False|

## HpeESKM.v2_0_0.HpeESKM
```@odata.type: "#HpeESKM.v2_0_0.HpeESKM"```

ESKM (Enterprise Security Key Manager) object enables user to connect to an operational key manager, change redundancy settings, view the key manager connection settings, test the connection, and view key management events.
### Resource Instances
|Uri|HTTP Allow|
|---|---|
|```/redfish/v1/managers/{item}/securityservice/eskm/```|GET POST PATCH |

### ESKMEvents (array)
Member of [HpeESKM.v2_0_0.HpeESKM](#hpeeskm-v2_0_0-hpeeskm)
```ESKMEvents``` is an array containing elements of:

**ESKMEvents[{item}].Event**
Member of [HpeESKM.v2_0_0.HpeESKM](#hpeeskm-v2_0_0-hpeeskm)

| | |
|---|---|
|Description|ESKM event description.|
|Type|string or null|
|Read Only|True|

**ESKMEvents[{item}].Timestamp**
Member of [HpeESKM.v2_0_0.HpeESKM](#hpeeskm-v2_0_0-hpeeskm)

| | |
|---|---|
|Description|Time of ESKM event.|
|Type|string or null|
|Read Only|True|

### KeyManagerConfig
**KeyManagerConfig.AccountGroup**
Member of [HpeESKM.v2_0_0.HpeESKM](#hpeeskm-v2_0_0-hpeeskm)

| | |
|---|---|
|Description|Account group on ESKM.|
|Type|string or null|
|Read Only|False|

**KeyManagerConfig.AccountName**
Member of [HpeESKM.v2_0_0.HpeESKM](#hpeeskm-v2_0_0-hpeeskm)

| | |
|---|---|
|Description|Account name on ESKM.|
|Type|string|
|Read Only|True|

**KeyManagerConfig.ESKMLocalCACertificateName**
Member of [HpeESKM.v2_0_0.HpeESKM](#hpeeskm-v2_0_0-hpeeskm)

| | |
|---|---|
|Description|This is the name of Local CA (Certificate Authority) in ESKM that is used to sign the ESKM server certificate. iLO will retrieve this certificate from the ESKM server.|
|Type|string or null|
|Read Only|False|

**KeyManagerConfig.ImportedCertificateIssuer**
Member of [HpeESKM.v2_0_0.HpeESKM](#hpeeskm-v2_0_0-hpeeskm)

| | |
|---|---|
|Description|Imported certificate issuer.|
|Type|string|
|Read Only|True|

**KeyManagerConfig.ImportedCertificateSubject**
Member of [HpeESKM.v2_0_0.HpeESKM](#hpeeskm-v2_0_0-hpeeskm)

| | |
|---|---|
|Description|Imported certificate subject.|
|Type|string|
|Read Only|True|

**KeyManagerConfig.LoginName**
Member of [HpeESKM.v2_0_0.HpeESKM](#hpeeskm-v2_0_0-hpeeskm)

| | |
|---|---|
|Description|ESKM administrator account login name. This property always returns null on GET.|
|Type|string or null|
|Read Only|False|

**KeyManagerConfig.Password**
Member of [HpeESKM.v2_0_0.HpeESKM](#hpeeskm-v2_0_0-hpeeskm)

| | |
|---|---|
|Description|ESKM administrator account password. This property always returns null on GET.|
|Type|string or null|
|Read Only|False|

### KeyServerRedundancyReq
Member of [HpeESKM.v2_0_0.HpeESKM](#hpeeskm-v2_0_0-hpeeskm)

| | |
|---|---|
|Description|If true encryption keys will be maintained on both the configured key servers. When this option is disabled, iLO will not verify that encryption keys are copied to both of the configured key servers.|
|Type|boolean|
|Read Only|False|

### PrimaryKeyServerAddress
Member of [HpeESKM.v2_0_0.HpeESKM](#hpeeskm-v2_0_0-hpeeskm)

| | |
|---|---|
|Description|Primary key server IP address or FQDN. Set to null to clear the value.|
|Type|string or null|
|Read Only|False|

### PrimaryKeyServerPort
Member of [HpeESKM.v2_0_0.HpeESKM](#hpeeskm-v2_0_0-hpeeskm)

| | |
|---|---|
|Description|Primary key server port number. Set to null to clear the value.|
|Type|integer or null|
|Read Only|False|

### SecondaryKeyServerAddress
Member of [HpeESKM.v2_0_0.HpeESKM](#hpeeskm-v2_0_0-hpeeskm)

| | |
|---|---|
|Description|Secondary key server IP address or FQDN. Set to null to clear the value.|
|Type|string or null|
|Read Only|False|

### SecondaryKeyServerPort
Member of [HpeESKM.v2_0_0.HpeESKM](#hpeeskm-v2_0_0-hpeeskm)

| | |
|---|---|
|Description|Secondary key server port number. Set to null to clear the value.|
|Type|integer or null|
|Read Only|False|

### Actions

**HpeESKM.ClearESKMLog**
Member of [HpeESKM.v2_0_0.HpeESKM](#hpeeskm-v2_0_0-hpeeskm)
Clears ESKM log.

There are no parameters for this action.

**HpeESKM.TestESKMConnections**
Member of [HpeESKM.v2_0_0.HpeESKM](#hpeeskm-v2_0_0-hpeeskm)
Test ESKM connections.

There are no parameters for this action.
## HpeHttpsCert.v2_0_0.HpeHttpsCert
```@odata.type: "#HpeHttpsCert.v2_0_0.HpeHttpsCert"```

This is the schema definition for the X509 Certificate.
### Resource Instances
|Uri|HTTP Allow|
|---|---|
|```/redfish/v1/managers/{item}/securityservice/httpscert/```|GET POST DELETE |

### CertificateSigningRequest
Member of [HpeHttpsCert.v2_0_0.HpeHttpsCert](#hpehttpscert-v2_0_0-hpehttpscert)

| | |
|---|---|
|Description|GenerateCSR action, wait few minutes (upto 10), perform GET operation, fills CSR. Contains a public and private key pair.|
|Type|string or null|
|Read Only|True|

### X509CertificateInformation
**X509CertificateInformation.Issuer**
Member of [HpeHttpsCert.v2_0_0.HpeHttpsCert](#hpehttpscert-v2_0_0-hpehttpscert)

| | |
|---|---|
|Description|The Certificate Authority that issued the certificate.|
|Type|string|
|Read Only|True|

**X509CertificateInformation.SerialNumber**
Member of [HpeHttpsCert.v2_0_0.HpeHttpsCert](#hpehttpscert-v2_0_0-hpehttpscert)

| | |
|---|---|
|Description|The serial number that the Certificate Authority assigned to the certificate.|
|Type|string|
|Read Only|True|

**X509CertificateInformation.Subject**
Member of [HpeHttpsCert.v2_0_0.HpeHttpsCert](#hpehttpscert-v2_0_0-hpehttpscert)

| | |
|---|---|
|Description|The entity to which the certificate was issued.|
|Type|string|
|Read Only|True|

**X509CertificateInformation.ValidNotAfter**
Member of [HpeHttpsCert.v2_0_0.HpeHttpsCert](#hpehttpscert-v2_0_0-hpehttpscert)

| | |
|---|---|
|Description|The date on which the certificate validity period ends.|
|Type|string|
|Read Only|True|

**X509CertificateInformation.ValidNotBefore**
Member of [HpeHttpsCert.v2_0_0.HpeHttpsCert](#hpehttpscert-v2_0_0-hpehttpscert)

| | |
|---|---|
|Description|The date on which the certificate validity period begins.|
|Type|string|
|Read Only|True|

### Actions

**HpeHttpsCert.ImportCertificate**
Member of [HpeHttpsCert.v2_0_0.HpeHttpsCert](#hpehttpscert-v2_0_0-hpehttpscert)
Imports a Trusted Certificate and iLO is reset.


**Parameters:**

**Certificate (string)**

Contains PEM formatted X509 certificate (Base64 encoded).

**HpeHttpsCert.GenerateCSR**
Member of [HpeHttpsCert.v2_0_0.HpeHttpsCert](#hpehttpscert-v2_0_0-hpehttpscert)

**Parameters:**

**City (string)**

The city or locality where the company or organization that owns this iLO subsystem is located.

**OrgName (string)**

The name of the company or organization that owns this iLO subsystem.

**Country (string)**

The two-character country code where the company or organization that owns this Manager subsystem is located. Eg: US

**CommonName (string)**

The FQDN of this iLO subsystem.

**IncludeIP (boolean)**

Include the IP Addresses in the CSR.

**OrgUnit (string)**

The unit within the company or organization that owns this iLO subsystem.

**State (string)**

The state where the company or organization that owns this iLO subsystem is located.
## HpeiLOActiveHealthSystem.v2_2_0.HpeiLOActiveHealthSystem
```@odata.type: "#HpeiLOActiveHealthSystem.v2_2_0.HpeiLOActiveHealthSystem"```
### Resource Instances
|Uri|HTTP Allow|
|---|---|
|```/redfish/v1/managers/{item}/activehealthsystem/```|GET POST PATCH |

### AHSEnabled
Member of [HpeiLOActiveHealthSystem.v2_2_0.HpeiLOActiveHealthSystem](#hpeiloactivehealthsystem-v2_2_0-hpeiloactivehealthsystem)

| | |
|---|---|
|Description|Determines whether HPE Active Health System logging is enabled or disabled.|
|Type|boolean|
|Read Only|False|

### AHSFileEnd
Member of [HpeiLOActiveHealthSystem.v2_2_0.HpeiLOActiveHealthSystem](#hpeiloactivehealthsystem-v2_2_0-hpeiloactivehealthsystem)

| | |
|---|---|
|Description|The end of the AHS log.|
|Type|string or null|
|Read Only|True|

### AHSFileStart
Member of [HpeiLOActiveHealthSystem.v2_2_0.HpeiLOActiveHealthSystem](#hpeiloactivehealthsystem-v2_2_0-hpeiloactivehealthsystem)

| | |
|---|---|
|Description|The start of the AHS log.|
|Type|string or null|
|Read Only|True|

### AHSStatus
**AHSStatus.HardwareEnabled**
Member of [HpeiLOActiveHealthSystem.v2_2_0.HpeiLOActiveHealthSystem](#hpeiloactivehealthsystem-v2_2_0-hpeiloactivehealthsystem)

| | |
|---|---|
|Description|Determines whether HPE Active Health System logging in hardware is enabled or not.|
|Type|boolean|
|Read Only|True|

**AHSStatus.SoftwareEnabled**
Member of [HpeiLOActiveHealthSystem.v2_2_0.HpeiLOActiveHealthSystem](#hpeiloactivehealthsystem-v2_2_0-hpeiloactivehealthsystem)

| | |
|---|---|
|Description|Determines whether HPE Active Health System logging in software is enabled or not.|
|Type|boolean|
|Read Only|True|

**AHSStatus.TemporaryHoldEnabled**
Member of [HpeiLOActiveHealthSystem.v2_2_0.HpeiLOActiveHealthSystem](#hpeiloactivehealthsystem-v2_2_0-hpeiloactivehealthsystem)

| | |
|---|---|
|Description|Determines whether HPE Active Health System logging access is temporarily disabled.|
|Type|boolean|
|Read Only|True|

### LocationParameters
**LocationParameters.case_no**
Member of [HpeiLOActiveHealthSystem.v2_2_0.HpeiLOActiveHealthSystem](#hpeiloactivehealthsystem-v2_2_0-hpeiloactivehealthsystem)

| | |
|---|---|
|Description|This query parameter may be added to the AHS location URI to insert the case number into the AHS log header. For example, http://iloname.example.net/ahsdata/HPE_xxxxxxxxxx_20140821.ahs?downloadAll=1&&case_no=abc123.|
|Type|string|
|Read Only|True|

**LocationParameters.co_name**
Member of [HpeiLOActiveHealthSystem.v2_2_0.HpeiLOActiveHealthSystem](#hpeiloactivehealthsystem-v2_2_0-hpeiloactivehealthsystem)

| | |
|---|---|
|Description|This query parameter may be added to the AHS location URI to insert the company name into the AHS log header. For example, http://iloname.example.net/ahsdata/HPE_xxxxxxxxxx_20140821.ahs?downloadAll=1&&co_name=myCompany.|
|Type|string|
|Read Only|True|

**LocationParameters.contact_name**
Member of [HpeiLOActiveHealthSystem.v2_2_0.HpeiLOActiveHealthSystem](#hpeiloactivehealthsystem-v2_2_0-hpeiloactivehealthsystem)

| | |
|---|---|
|Description|This query parameter may be added to the AHS location URI to insert the contact name into the AHS log header. For example, http://iloname.example.net/ahsdata/HPE_xxxxxxxxxx_20140821.ahs?downloadAll=1&&contact_name=JohnDoe.|
|Type|string|
|Read Only|True|

**LocationParameters.days**
Member of [HpeiLOActiveHealthSystem.v2_2_0.HpeiLOActiveHealthSystem](#hpeiloactivehealthsystem-v2_2_0-hpeiloactivehealthsystem)

| | |
|---|---|
|Description|This query parameter should be used to download the most recent N days of the AHS log. For example, http://iloname.example.net/ahsdata/HPE_xxxxxxxxxx_20140821.ahs?days=7. Will retrive logs made within the last 7 days.|
|Type|string|
|Read Only|True|

**LocationParameters.downloadAll**
Member of [HpeiLOActiveHealthSystem.v2_2_0.HpeiLOActiveHealthSystem](#hpeiloactivehealthsystem-v2_2_0-hpeiloactivehealthsystem)

| | |
|---|---|
|Description|This query parameter should be used to download entire AHS log. For example, http://iloname.example.net/ahsdata/HPE_xxxxxxxxxx_20140821.ahs?downloadAll=1.|
|Type|string|
|Read Only|True|

**LocationParameters.email**
Member of [HpeiLOActiveHealthSystem.v2_2_0.HpeiLOActiveHealthSystem](#hpeiloactivehealthsystem-v2_2_0-hpeiloactivehealthsystem)

| | |
|---|---|
|Description|This query parameter may be added to the AHS location URI to insert the contacts email address into the AHS log header. For example, http://iloname.example.net/ahsdata/HPE_xxxxxxxxxx_20140821.ahs?downloadAll=1&&email=abc@xyz.com.|
|Type|string|
|Read Only|True|

**LocationParameters.from**
Member of [HpeiLOActiveHealthSystem.v2_2_0.HpeiLOActiveHealthSystem](#hpeiloactivehealthsystem-v2_2_0-hpeiloactivehealthsystem)

| | |
|---|---|
|Description|This query parameter must be added with the 'to' query parameter to the AHS location URI to limit the range of data returned. 'downloadAll' parameter should not be used with this query parameter. For example, http://iloname.example.net/ahsdata/HPE_xxxxxxxxxx_20140821.ahs?from=2014-03-01&&to=2014-03-30.|
|Type|string|
|Read Only|True|

**LocationParameters.phone**
Member of [HpeiLOActiveHealthSystem.v2_2_0.HpeiLOActiveHealthSystem](#hpeiloactivehealthsystem-v2_2_0-hpeiloactivehealthsystem)

| | |
|---|---|
|Description|This query parameter may be added to the AHS location URI to insert the contacts phone number into the AHS log header. For example, http://iloname.example.net/ahsdata/HPE_xxxxxxxxxx_20140821.ahs?downloadAll=1&&contact_name=JohnDoe&&phone=555-555-5555.|
|Type|string|
|Read Only|True|

**LocationParameters.to**
Member of [HpeiLOActiveHealthSystem.v2_2_0.HpeiLOActiveHealthSystem](#hpeiloactivehealthsystem-v2_2_0-hpeiloactivehealthsystem)

| | |
|---|---|
|Description|This query parameter must be added with the 'from' query parameter to the AHS location URI to limit the range of data returned.'downloadAll' parameter should not be used with this query parameter. For example, http://iloname.example.net/ahsdata/HPE_xxxxxxxxxx_20140821.ahs?from=2014-03-01&&to=2014-03-30.|
|Type|string|
|Read Only|True|

### Actions

**HpeiLOActiveHealthSystem.ClearLog**
Member of [HpeiLOActiveHealthSystem.v2_2_0.HpeiLOActiveHealthSystem](#hpeiloactivehealthsystem-v2_2_0-hpeiloactivehealthsystem)
There are no parameters for this action.
## HpeiLOBackupRestoreService.v2_1_0.HpeiLOBackupRestoreService
```@odata.type: "#HpeiLOBackupRestoreService.v2_1_0.HpeiLOBackupRestoreService"```
### Resource Instances
|Uri|HTTP Allow|
|---|---|
|```/redfish/v1/managers/{item}/backuprestoreservice/```|GET |

### BackupFileLocation
Member of [HpeiLOBackupRestoreService.v2_1_0.HpeiLOBackupRestoreService](#hpeilobackuprestoreservice-v2_1_0-hpeilobackuprestoreservice)

| | |
|---|---|
|Description|The URI to which a client may POST to create and download a file for a subsequent restore operation.|
|Type|string|
|Read Only|True|

### HttpPushUri
Member of [HpeiLOBackupRestoreService.v2_1_0.HpeiLOBackupRestoreService](#hpeilobackuprestoreservice-v2_1_0-hpeilobackuprestoreservice)

| | |
|---|---|
|Description|The URI to which a client may POST a file for a subsequent restore operation.|
|Type|string|
|Read Only|True|

## HpeiLODateTime.v2_0_0.HpeiLODateTime
```@odata.type: "#HpeiLODateTime.v2_0_0.HpeiLODateTime"```

The management processor date and time.
### Resource Instances
|Uri|HTTP Allow|
|---|---|
|```/redfish/v1/managers/{item}/datetime/```|GET PATCH |

### Links to other Resources
|Link Name|Destination type
|---|---|
|```Links/EthernetNICs```|Collection of [EthernetInterface](#ethernetinterface-v1_0_3-ethernetinterface)|

### ConfigurationSettings
Member of [HpeiLODateTime.v2_0_0.HpeiLODateTime](#hpeilodatetime-v2_0_0-hpeilodatetime)

| | |
|---|---|
|Description|The state of the currently displayed configuration settings.|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|
|---|
|```Current```|
|```SomePendingReset```|

### DateTime
Member of [HpeiLODateTime.v2_0_0.HpeiLODateTime](#hpeilodatetime-v2_0_0-hpeilodatetime)

| | |
|---|---|
|Description|The date and time used by management processor.|
|Type|string|
|Read Only|True|

### NTPServers (array)
Member of [HpeiLODateTime.v2_0_0.HpeiLODateTime](#hpeilodatetime-v2_0_0-hpeilodatetime)
```NTPServers``` is an array containing elements of:


| | |
|---|---|
|Description|The current NTP server's IPv4 address, IPv6 address, or FQDN. The value either comes from DHCP or is static depending on the DHCP settings.|
|Type|string|
|Read Only|True|

### PropagateTimeToHost
Member of [HpeiLODateTime.v2_0_0.HpeiLODateTime](#hpeilodatetime-v2_0_0-hpeilodatetime)

| | |
|---|---|
|Description|Determines whether the server time is synchronized with the management processor time during the first POST after AC power is applied.|
|Type|boolean|
|Read Only|False|

### StaticNTPServers (array)
Member of [HpeiLODateTime.v2_0_0.HpeiLODateTime](#hpeilodatetime-v2_0_0-hpeilodatetime)
```StaticNTPServers``` is an array containing elements of:


| | |
|---|---|
|Description|The static NTP server's IPv4 address, IPv6 address, or FQDN. To set this property, management processor must not be configured to use NTP servers provided by DHCPv4 or DHCPv6.|
|Type|string|
|Read Only|True|

### TimeZone
**TimeZone.Index**
Member of [HpeiLODateTime.v2_0_0.HpeiLODateTime](#hpeilodatetime-v2_0_0-hpeilodatetime)

| | |
|---|---|
|Description|The index of the current time zone. To set a new time zone, specify a different time zone index. This property can be set only when DHCPv4 or DHCPv6 supplied time settings are disabled. Since the time zone list might vary from one firmware version to another (which often leads to differences in time zone indices), setting the time zone by name is recommended over setting by index, for better compatibility.|
|Type|number|
|Read Only|False|

**TimeZone.UtcOffset**
Member of [HpeiLODateTime.v2_0_0.HpeiLODateTime](#hpeilodatetime-v2_0_0-hpeilodatetime)

| | |
|---|---|
|Description|The UTC offset of the current time zone, in the format {+/-}hh:mm|
|Type|string|
|Read Only|True|

**TimeZone.Value**
Member of [HpeiLODateTime.v2_0_0.HpeiLODateTime](#hpeilodatetime-v2_0_0-hpeilodatetime)

| | |
|---|---|
|Description|The environment variable value.|
|Type|string|
|Read Only|True|

### TimeZoneList (array)
Member of [HpeiLODateTime.v2_0_0.HpeiLODateTime](#hpeilodatetime-v2_0_0-hpeilodatetime)
```TimeZoneList``` is an array containing elements of:

**TimeZoneList[{item}].Index**
Member of [HpeiLODateTime.v2_0_0.HpeiLODateTime](#hpeilodatetime-v2_0_0-hpeilodatetime)

| | |
|---|---|
|Description|The time zone index.|
|Type|number|
|Read Only|True|

**TimeZoneList[{item}].UtcOffset**
Member of [HpeiLODateTime.v2_0_0.HpeiLODateTime](#hpeilodatetime-v2_0_0-hpeilodatetime)

| | |
|---|---|
|Description|The UTC offset of the time zone, in the format {+/-}hh:mm|
|Type|string|
|Read Only|True|

**TimeZoneList[{item}].Value**
Member of [HpeiLODateTime.v2_0_0.HpeiLODateTime](#hpeilodatetime-v2_0_0-hpeilodatetime)

| | |
|---|---|
|Description|The environment variable value.|
|Type|string|
|Read Only|True|

## HpeiLOEmbeddedMedia.v2_0_0.HpeiLOEmbeddedMedia
```@odata.type: "#HpeiLOEmbeddedMedia.v2_0_0.HpeiLOEmbeddedMedia"```
### Resource Instances
|Uri|HTTP Allow|
|---|---|
|```/redfish/v1/managers/{item}/embeddedmedia/```|GET |

### Controller
**Controller.Firmware**
**Controller.Firmware.Current**
**Controller.Firmware.Current.VersionString**
Member of [HpeiLOEmbeddedMedia.v2_0_0.HpeiLOEmbeddedMedia](#hpeiloembeddedmedia-v2_0_0-hpeiloembeddedmedia)

| | |
|---|---|
|Description|The current version of the embedded media controller.|
|Type|string|
|Read Only|True|

**Controller.Status**
Member of [HpeiLOEmbeddedMedia.v2_0_0.HpeiLOEmbeddedMedia](#hpeiloembeddedmedia-v2_0_0-hpeiloembeddedmedia)
See the Redfish standard schema and specification for information on common Status object.

### SDCard
**SDCard.SizeMB**
Member of [HpeiLOEmbeddedMedia.v2_0_0.HpeiLOEmbeddedMedia](#hpeiloembeddedmedia-v2_0_0-hpeiloembeddedmedia)

| | |
|---|---|
|Description|The size of the SD card present in the server, in MB.|
|Type|integer|
|Read Only|True|

**SDCard.Status**
Member of [HpeiLOEmbeddedMedia.v2_0_0.HpeiLOEmbeddedMedia](#hpeiloembeddedmedia-v2_0_0-hpeiloembeddedmedia)
See the Redfish standard schema and specification for information on common Status object.

## HpeiLOFederatedGroupCapping.v2_0_0.HpeiLOFederatedGroupCapping
```@odata.type: "#HpeiLOFederatedGroupCapping.v2_0_0.HpeiLOFederatedGroupCapping"```
### Resource Instances
|Uri|HTTP Allow|
|---|---|
|```/redfish/v1/chassis/{item}/power/federatedgroupcapping/```|GET PATCH |

### CapWatts
Member of [HpeiLOFederatedGroupCapping.v2_0_0.HpeiLOFederatedGroupCapping](#hpeilofederatedgroupcapping-v2_0_0-hpeilofederatedgroupcapping)

| | |
|---|---|
|Description|The configured power cap for all servers in a group. This value is 0 if the power cap is not configured.|
|Type|integer|
|Read Only|True|

### CapacityWatts
Member of [HpeiLOFederatedGroupCapping.v2_0_0.HpeiLOFederatedGroupCapping](#hpeilofederatedgroupcapping-v2_0_0-hpeilofederatedgroupcapping)

| | |
|---|---|
|Description|The total power supply capacity for all servers in a group.|
|Type|integer|
|Read Only|True|

### Groups
### Throttle
Member of [HpeiLOFederatedGroupCapping.v2_0_0.HpeiLOFederatedGroupCapping](#hpeilofederatedgroupcapping-v2_0_0-hpeilofederatedgroupcapping)

| | |
|---|---|
|Description|High, Med, or Low based on the percentage of power usage.|
|Type|string|
|Read Only|True|

## HpeiLOFederationGroup.v2_0_0.HpeiLOFederationGroup
```@odata.type: "#HpeiLOFederationGroup.v2_0_0.HpeiLOFederationGroup"```
### Resource Instances
|Uri|HTTP Allow|
|---|---|
|```/redfish/v1/managers/{item}/federationgroups/{item}/```|GET PATCH DELETE |

### Key
Member of [HpeiLOFederationGroup.v2_0_0.HpeiLOFederationGroup](#hpeilofederationgroup-v2_0_0-hpeilofederationgroup)

| | |
|---|---|
|Description|The password used by the Federation Group.|
|Type|string or null|
|Read Only|False|

### Privileges
**Privileges.HostBIOSConfigPriv**
Member of [HpeiLOFederationGroup.v2_0_0.HpeiLOFederationGroup](#hpeilofederationgroup-v2_0_0-hpeilofederationgroup)

| | |
|---|---|
|Description|Host BIOS configuration privileges.|
|Type|boolean|
|Read Only|False|

**Privileges.HostNICConfigPriv**
Member of [HpeiLOFederationGroup.v2_0_0.HpeiLOFederationGroup](#hpeilofederationgroup-v2_0_0-hpeilofederationgroup)

| | |
|---|---|
|Description|Host NIC configuration privileges.|
|Type|boolean|
|Read Only|False|

**Privileges.HostStorageConfigPriv**
Member of [HpeiLOFederationGroup.v2_0_0.HpeiLOFederationGroup](#hpeilofederationgroup-v2_0_0-hpeilofederationgroup)

| | |
|---|---|
|Description|Host Storage configuration privileges.|
|Type|boolean|
|Read Only|False|

**Privileges.LoginPriv**
Member of [HpeiLOFederationGroup.v2_0_0.HpeiLOFederationGroup](#hpeilofederationgroup-v2_0_0-hpeilofederationgroup)

| | |
|---|---|
|Description|Login privileges.|
|Type|boolean|
|Read Only|False|

**Privileges.RemoteConsolePriv**
Member of [HpeiLOFederationGroup.v2_0_0.HpeiLOFederationGroup](#hpeilofederationgroup-v2_0_0-hpeilofederationgroup)

| | |
|---|---|
|Description|Remote console privileges.|
|Type|boolean|
|Read Only|False|

**Privileges.SystemRecoveryConfigPriv**
Member of [HpeiLOFederationGroup.v2_0_0.HpeiLOFederationGroup](#hpeilofederationgroup-v2_0_0-hpeilofederationgroup)

| | |
|---|---|
|Description|System Recovery configuration privileges.|
|Type|boolean|
|Read Only|False|

**Privileges.UserConfigPriv**
Member of [HpeiLOFederationGroup.v2_0_0.HpeiLOFederationGroup](#hpeilofederationgroup-v2_0_0-hpeilofederationgroup)

| | |
|---|---|
|Description|User configuration privileges.|
|Type|boolean|
|Read Only|False|

**Privileges.VirtualMediaPriv**
Member of [HpeiLOFederationGroup.v2_0_0.HpeiLOFederationGroup](#hpeilofederationgroup-v2_0_0-hpeilofederationgroup)

| | |
|---|---|
|Description|Virtual media privileges.|
|Type|boolean|
|Read Only|False|

**Privileges.VirtualPowerAndResetPriv**
Member of [HpeiLOFederationGroup.v2_0_0.HpeiLOFederationGroup](#hpeilofederationgroup-v2_0_0-hpeilofederationgroup)

| | |
|---|---|
|Description|Virtual power and reset privileges.|
|Type|boolean|
|Read Only|False|

**Privileges.iLOConfigPriv**
Member of [HpeiLOFederationGroup.v2_0_0.HpeiLOFederationGroup](#hpeilofederationgroup-v2_0_0-hpeilofederationgroup)

| | |
|---|---|
|Description|The management processor configuration privileges.|
|Type|boolean|
|Read Only|False|

## HpeiLOFederationPeers.v2_0_0.HpeiLOFederationPeers
```@odata.type: "#HpeiLOFederationPeers.v2_0_0.HpeiLOFederationPeers"```
### Resource Instances
|Uri|HTTP Allow|
|---|---|
|```/redfish/v1/managers/{item}/federationpeers/{item}/```|GET |

### Peers (array)
Member of [HpeiLOFederationPeers.v2_0_0.HpeiLOFederationPeers](#hpeilofederationpeers-v2_0_0-hpeilofederationpeers)
```Peers``` is an array containing elements of:

**Peers[{item}].HttpErrorCode**
Member of [HpeiLOFederationPeers.v2_0_0.HpeiLOFederationPeers](#hpeilofederationpeers-v2_0_0-hpeilofederationpeers)

| | |
|---|---|
|Description|Error code for success or failure.|
|Type|integer|
|Read Only|True|

**Peers[{item}].ManagerIPAddress**
Member of [HpeiLOFederationPeers.v2_0_0.HpeiLOFederationPeers](#hpeilofederationpeers-v2_0_0-hpeilofederationpeers)

| | |
|---|---|
|Description|Manager IP address of the federation peer.|
|Type|string|
|Read Only|True|

**Peers[{item}].Time**
Member of [HpeiLOFederationPeers.v2_0_0.HpeiLOFederationPeers](#hpeilofederationpeers-v2_0_0-hpeilofederationpeers)

| | |
|---|---|
|Description|Time when the federation peer was added.|
|Type|string|
|Read Only|True|

**Peers[{item}].URL**
Member of [HpeiLOFederationPeers.v2_0_0.HpeiLOFederationPeers](#hpeilofederationpeers-v2_0_0-hpeilofederationpeers)

| | |
|---|---|
|Description|URL of the federation peer.|
|Type|string|
|Read Only|True|

**Peers[{item}].UUID**
Member of [HpeiLOFederationPeers.v2_0_0.HpeiLOFederationPeers](#hpeilofederationpeers-v2_0_0-hpeilofederationpeers)

| | |
|---|---|
|Description|UUID peers that are part of the federation group.|
|Type|string|
|Read Only|True|

## HpeiLOLicense.v2_1_0.HpeiLOLicense
```@odata.type: "#HpeiLOLicense.v2_1_0.HpeiLOLicense"```
### Resource Instances
|Uri|HTTP Allow|
|---|---|
|```/redfish/v1/managers/{item}/licenseservice/{item}/```|GET DELETE |

### Confirmation
**Confirmation.Code**
Member of [HpeiLOLicense.v2_1_0.HpeiLOLicense](#hpeilolicense-v2_1_0-hpeilolicense)

| | |
|---|---|
|Description|Confirmation service response code.|
|Type|string|
|Read Only|True|

**Confirmation.Message**
Member of [HpeiLOLicense.v2_1_0.HpeiLOLicense](#hpeilolicense-v2_1_0-hpeilolicense)

| | |
|---|---|
|Description|User-friendly confirmation information for the current managment processor license.|
|Type|string|
|Read Only|True|

**Confirmation.Service**
Member of [HpeiLOLicense.v2_1_0.HpeiLOLicense](#hpeilolicense-v2_1_0-hpeilolicense)

| | |
|---|---|
|Description|Confirmation service URI.|
|Type|string|
|Read Only|True|

**Confirmation.Status**
Member of [HpeiLOLicense.v2_1_0.HpeiLOLicense](#hpeilolicense-v2_1_0-hpeilolicense)
See the Redfish standard schema and specification for information on common Status object.

### ConfirmationRequest
**ConfirmationRequest.EON**
**ConfirmationRequest.EON.License**
Member of [HpeiLOLicense.v2_1_0.HpeiLOLicense](#hpeilolicense-v2_1_0-hpeilolicense)

| | |
|---|---|
|Description|The current license of this management processor.|
|Type|string|
|Read Only|True|

**ConfirmationRequest.EON.LicenseKey**
Member of [HpeiLOLicense.v2_1_0.HpeiLOLicense](#hpeilolicense-v2_1_0-hpeilolicense)

| | |
|---|---|
|Description|The license key installed on this management processor.|
|Type|string|
|Read Only|True|

**ConfirmationRequest.EON.Quantity**
Member of [HpeiLOLicense.v2_1_0.HpeiLOLicense](#hpeilolicense-v2_1_0-hpeilolicense)

| | |
|---|---|
|Description|The number of entitlements licensed.|
|Type|integer|
|Read Only|True|

**ConfirmationRequest.EON.State**
Member of [HpeiLOLicense.v2_1_0.HpeiLOLicense](#hpeilolicense-v2_1_0-hpeilolicense)

| | |
|---|---|
|Description|The current licensing state and behavior of the management processor.  This is affected by license installation, activation and confirmation.|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```unlicensed```|standard baseline functionality|
|```evaluation```|evaluation / demonstration temporary licensed functionality|
|```nfr```|not for resale experimental functionality|
|```expired```|standard baseline functionality and evaluation licenses no longer accepted|
|```unconfirmed```|licensed functionality that has not been confirmed|
|```timeout```|licensed functionality is disabled until the license is confirmed|
|```confirmed```|licensed functionality has been confirmed for use|
|```static```|system has active built-in licensed functionality that does not require confirmation|
|```err```|error|

**ConfirmationRequest.Signer**
Member of [HpeiLOLicense.v2_1_0.HpeiLOLicense](#hpeilolicense-v2_1_0-hpeilolicense)

| | |
|---|---|
|Description|Source of confirmation request.|
|Type|string|
|Read Only|True|

**ConfirmationRequest.System**
**ConfirmationRequest.System.ChipId**
Member of [HpeiLOLicense.v2_1_0.HpeiLOLicense](#hpeilolicense-v2_1_0-hpeilolicense)

| | |
|---|---|
|Description|Management processor unique chip identifier.|
|Type|string|
|Read Only|True|

**ConfirmationRequest.System.Product**
Member of [HpeiLOLicense.v2_1_0.HpeiLOLicense](#hpeilolicense-v2_1_0-hpeilolicense)

| | |
|---|---|
|Description|System housing management processor.|
|Type|string|
|Read Only|True|

**ConfirmationRequest.System.SerialNumber**
Member of [HpeiLOLicense.v2_1_0.HpeiLOLicense](#hpeilolicense-v2_1_0-hpeilolicense)

| | |
|---|---|
|Description|System serial number.|
|Type|string|
|Read Only|True|

### License
Member of [HpeiLOLicense.v2_1_0.HpeiLOLicense](#hpeilolicense-v2_1_0-hpeilolicense)

| | |
|---|---|
|Description|The current license of this management processor.|
|Type|string|
|Read Only|True|

### LicenseClass
Member of [HpeiLOLicense.v2_1_0.HpeiLOLicense](#hpeilolicense-v2_1_0-hpeilolicense)

| | |
|---|---|
|Description|The class of current license on this management processor.|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|
|---|
|```FQL```|
|```BETA```|
|```EVAULATION```|
|```AKA```|
|```DL```|
|```FFQL```|
|```SL```|
|```SITE```|
|```BETA```|
|```EVAL```|
|```MLA```|

### LicenseErr
Member of [HpeiLOLicense.v2_1_0.HpeiLOLicense](#hpeilolicense-v2_1_0-hpeilolicense)

| | |
|---|---|
|Description|Error information from the most recent attempt to alter the installed management processor license.|
|Type|string|
|Read Only|True|

### LicenseExpire
Member of [HpeiLOLicense.v2_1_0.HpeiLOLicense](#hpeilolicense-v2_1_0-hpeilolicense)

| | |
|---|---|
|Description|User-friendly expiration information of the installed management processor license. For example, for demo license, Evaluation period 2 months 5 days 6 hours remain.|
|Type|string|
|Read Only|True|

### LicenseFeatures
**LicenseFeatures.DirectoryAuth**
Member of [HpeiLOLicense.v2_1_0.HpeiLOLicense](#hpeilolicense-v2_1_0-hpeilolicense)

| | |
|---|---|
|Description|Directory integrated authentication.|
|Type|boolean|
|Read Only|True|

**LicenseFeatures.EmailAlert**
Member of [HpeiLOLicense.v2_1_0.HpeiLOLicense](#hpeilolicense-v2_1_0-hpeilolicense)

| | |
|---|---|
|Description|Email based alerting.|
|Type|boolean|
|Read Only|True|

**LicenseFeatures.FWScan**
Member of [HpeiLOLicense.v2_1_0.HpeiLOLicense](#hpeilolicense-v2_1_0-hpeilolicense)

| | |
|---|---|
|Description|Runtime FW Integrity check.|
|Type|boolean|
|Read Only|True|

**LicenseFeatures.Federation**
Member of [HpeiLOLicense.v2_1_0.HpeiLOLicense](#hpeilolicense-v2_1_0-hpeilolicense)

| | |
|---|---|
|Description|Distributed peer to peer management.|
|Type|boolean|
|Read Only|True|

**LicenseFeatures.Jitter**
Member of [HpeiLOLicense.v2_1_0.HpeiLOLicense](#hpeilolicense-v2_1_0-hpeilolicense)

| | |
|---|---|
|Description|Jitter Control.|
|Type|boolean|
|Read Only|True|

**LicenseFeatures.KD**
Member of [HpeiLOLicense.v2_1_0.HpeiLOLicense](#hpeilolicense-v2_1_0-hpeilolicense)

| | |
|---|---|
|Description|Kernel Debugging (VSP raw mode).|
|Type|boolean|
|Read Only|True|

**LicenseFeatures.KeyMgr**
Member of [HpeiLOLicense.v2_1_0.HpeiLOLicense](#hpeilolicense-v2_1_0-hpeilolicense)

| | |
|---|---|
|Description|Store and retrieve keys from an external key manager.|
|Type|boolean|
|Read Only|True|

**LicenseFeatures.MURC**
Member of [HpeiLOLicense.v2_1_0.HpeiLOLicense](#hpeilolicense-v2_1_0-hpeilolicense)

| | |
|---|---|
|Description|Shared Multi-User Remote Console.|
|Type|boolean|
|Read Only|True|

**LicenseFeatures.PowerReg**
Member of [HpeiLOLicense.v2_1_0.HpeiLOLicense](#hpeilolicense-v2_1_0-hpeilolicense)

| | |
|---|---|
|Description|Power Regulator.|
|Type|boolean|
|Read Only|True|

**LicenseFeatures.RC**
Member of [HpeiLOLicense.v2_1_0.HpeiLOLicense](#hpeilolicense-v2_1_0-hpeilolicense)

| | |
|---|---|
|Description|Graphical Remote Console.|
|Type|boolean|
|Read Only|True|

**LicenseFeatures.Recovery**
Member of [HpeiLOLicense.v2_1_0.HpeiLOLicense](#hpeilolicense-v2_1_0-hpeilolicense)

| | |
|---|---|
|Description|OS Recovery Event.|
|Type|boolean|
|Read Only|True|

**LicenseFeatures.RemoteSyslog**
Member of [HpeiLOLicense.v2_1_0.HpeiLOLicense](#hpeilolicense-v2_1_0-hpeilolicense)

| | |
|---|---|
|Description|Remote Syslog.|
|Type|boolean|
|Read Only|True|

**LicenseFeatures.Scrncap**
Member of [HpeiLOLicense.v2_1_0.HpeiLOLicense](#hpeilolicense-v2_1_0-hpeilolicense)

| | |
|---|---|
|Description|Video Capture.|
|Type|boolean|
|Read Only|True|

**LicenseFeatures.SecureErase**
Member of [HpeiLOLicense.v2_1_0.HpeiLOLicense](#hpeilolicense-v2_1_0-hpeilolicense)

| | |
|---|---|
|Description|Secure Erase of embedded media.|
|Type|boolean|
|Read Only|True|

**LicenseFeatures.SmartCard**
Member of [HpeiLOLicense.v2_1_0.HpeiLOLicense](#hpeilolicense-v2_1_0-hpeilolicense)

| | |
|---|---|
|Description|2-Factor Authentication (Smart Card).|
|Type|boolean|
|Read Only|True|

**LicenseFeatures.SuiteB**
Member of [HpeiLOLicense.v2_1_0.HpeiLOLicense](#hpeilolicense-v2_1_0-hpeilolicense)

| | |
|---|---|
|Description|SuiteB/CNSA mode support.|
|Type|boolean|
|Read Only|True|

**LicenseFeatures.TextCons**
Member of [HpeiLOLicense.v2_1_0.HpeiLOLicense](#hpeilolicense-v2_1_0-hpeilolicense)

| | |
|---|---|
|Description|Text Console.|
|Type|boolean|
|Read Only|True|

**LicenseFeatures.VM**
Member of [HpeiLOLicense.v2_1_0.HpeiLOLicense](#hpeilolicense-v2_1_0-hpeilolicense)

| | |
|---|---|
|Description|Remote Console based Virtual Media.|
|Type|boolean|
|Read Only|True|

**LicenseFeatures.VMScript**
Member of [HpeiLOLicense.v2_1_0.HpeiLOLicense](#hpeilolicense-v2_1_0-hpeilolicense)

| | |
|---|---|
|Description|Scripted Virtual Media.|
|Type|boolean|
|Read Only|True|

**LicenseFeatures.VSPLogging**
Member of [HpeiLOLicense.v2_1_0.HpeiLOLicense](#hpeilolicense-v2_1_0-hpeilolicense)

| | |
|---|---|
|Description|Virtual Serial Port Logging and Playback.|
|Type|boolean|
|Read Only|True|

### LicenseInstallDate
Member of [HpeiLOLicense.v2_1_0.HpeiLOLicense](#hpeilolicense-v2_1_0-hpeilolicense)

| | |
|---|---|
|Description|User-friendly installation date information of the installed management processor license. For example, 19 May 2017|
|Type|string|
|Read Only|True|

### LicenseKey
Member of [HpeiLOLicense.v2_1_0.HpeiLOLicense](#hpeilolicense-v2_1_0-hpeilolicense)

| | |
|---|---|
|Description|User-visible license key installed on this management processor. License keys are 25 or 29 characters and contain letters, numbers and hypens. Use POST method to collection of membertype HpeiLOLicense to install / update the license.|
|Type|string|
|Read Only|True|

### LicenseTier
Member of [HpeiLOLicense.v2_1_0.HpeiLOLicense](#hpeilolicense-v2_1_0-hpeilolicense)

| | |
|---|---|
|Description|The licensed feature-set of the management processor.|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|
|---|
|```STD```|
|```BLSTD```|
|```ADV```|
|```BLADV```|
|```ESS```|
|```SCALEOUT```|
|```APSE```|

### LicenseType
Member of [HpeiLOLicense.v2_1_0.HpeiLOLicense](#hpeilolicense-v2_1_0-hpeilolicense)

| | |
|---|---|
|Description|The type of current license activation on this management processor.|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|
|---|
|```Unlicensed```|
|```Evaluation```|
|```Perpetual```|
|```Subscription```|
|```Internal```|
|```Duration```|
|```Expired```|

## HpeiLOResourceDirectory.v2_0_0.HpeiLOResourceDirectory
```@odata.type: "#HpeiLOResourceDirectory.v2_0_0.HpeiLOResourceDirectory"```
### Resource Instances
|Uri|HTTP Allow|
|---|---|
|```/redfish/v1/resourcedirectory/```|GET |

### Instances (array)
Member of [HpeiLOResourceDirectory.v2_0_0.HpeiLOResourceDirectory](#hpeiloresourcedirectory-v2_0_0-hpeiloresourcedirectory)
```Instances``` is an array containing elements of:

**Instances[{item}].ETag**
Member of [HpeiLOResourceDirectory.v2_0_0.HpeiLOResourceDirectory](#hpeiloresourcedirectory-v2_0_0-hpeiloresourcedirectory)

| | |
|---|---|
|Description|This is the last known etag of the resource. The property is omitted if not known.|
|Type|string|
|Read Only|True|

**Instances[{item}].HttpMethods (array)**
Member of [HpeiLOResourceDirectory.v2_0_0.HpeiLOResourceDirectory](#hpeiloresourcedirectory-v2_0_0-hpeiloresourcedirectory)
```HttpMethods``` is an array containing elements of:


| | |
|---|---|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|
|---|
|```GET```|
|```HEAD```|
|```POST```|
|```PUT```|
|```PATCH```|
|```DELETE```|

**Instances[{item}].MemberType**
Member of [HpeiLOResourceDirectory.v2_0_0.HpeiLOResourceDirectory](#hpeiloresourcedirectory-v2_0_0-hpeiloresourcedirectory)

| | |
|---|---|
|Description|This property has the type of members for collection resources.|
|Type|string|
|Read Only|True|

## HpeiLOSnmpService.v2_1_0.HpeiLOSnmpService
```@odata.type: "#HpeiLOSnmpService.v2_1_0.HpeiLOSnmpService"```
### Resource Instances
|Uri|HTTP Allow|
|---|---|
|```/redfish/v1/managers/{item}/snmpservice/```|GET POST PATCH |

### Links to other Resources
|Link Name|Destination type
|---|---|
|```SNMPUsers```|Collection of [HpeSNMPUser](#hpesnmpuser-v2_0_0-hpesnmpuser)|
|```SNMPAlertDestinations```|Collection of [HpeSNMPAlertDestination](#hpesnmpalertdestination-v2_0_0-hpesnmpalertdestination)|

### AlertDestinationAssociations (array)
Member of [HpeiLOSnmpService.v2_1_0.HpeiLOSnmpService](#hpeilosnmpservice-v2_1_0-hpeilosnmpservice)
```AlertDestinationAssociations``` is an array containing elements of:

**AlertDestinationAssociations[{item}].SNMPAlertProtocol**
Member of [HpeiLOSnmpService.v2_1_0.HpeiLOSnmpService](#hpeilosnmpservice-v2_1_0-hpeilosnmpservice)

| | |
|---|---|
|Description|Indicate the SNMP protocol associated with the AlertDestination.|
|Type|string or null|
|Read Only|False|

The following are the supported values:

|Value|Description|
|---|---|
|```SNMPv1Trap```|Indicate SNMPv1 trap is enabled for the destination.|
|```SNMPv3Trap```|Indicate SNMPv3 trap is enabled for the destination. Needs to fill the SecurityName as well.|
|```SNMPv3Inform```|Indicate SNMPv3 Inform is enabled for the destination. Needs to fill the SecurityName as well.|
|```Null```|A value is temporarily unavailable|

**AlertDestinationAssociations[{item}].SecurityName**
Member of [HpeiLOSnmpService.v2_1_0.HpeiLOSnmpService](#hpeilosnmpservice-v2_1_0-hpeilosnmpservice)

| | |
|---|---|
|Description|Provides the SNMPv3 security name associated with the destination when SNMP alert protocol is SNMPv3 trap or inform.|
|Type|string or null|
|Read Only|False|

### AlertDestinations (array)
Member of [HpeiLOSnmpService.v2_1_0.HpeiLOSnmpService](#hpeilosnmpservice-v2_1_0-hpeilosnmpservice)
```AlertDestinations``` is an array containing elements of:


| | |
|---|---|
|Type|string or null|
|Read Only|True|

### AlertsEnabled
Member of [HpeiLOSnmpService.v2_1_0.HpeiLOSnmpService](#hpeilosnmpservice-v2_1_0-hpeilosnmpservice)

| | |
|---|---|
|Description|The alert conditions that the management processor detects independently of the host operating system can be sent to specified SNMP alert destinations.|
|Type|boolean|
|Read Only|False|

### Contact
Member of [HpeiLOSnmpService.v2_1_0.HpeiLOSnmpService](#hpeilosnmpservice-v2_1_0-hpeilosnmpservice)

| | |
|---|---|
|Description|The string of up to 49 characters that specifies the system administrator or server owner. The string can include a name, email address, or phone number.|
|Type|string or null|
|Read Only|False|

### Location
Member of [HpeiLOSnmpService.v2_1_0.HpeiLOSnmpService](#hpeilosnmpservice-v2_1_0-hpeilosnmpservice)

| | |
|---|---|
|Description|The string of up to 49 characters that specifies the physical location of the server.|
|Type|string or null|
|Read Only|False|

### Oem.Hpe.SNMPColdStartTrapBroadcast
Member of [HpeiLOSnmpService.v2_1_0.HpeiLOSnmpService](#hpeilosnmpservice-v2_1_0-hpeilosnmpservice)

| | |
|---|---|
|Description|If set to true, the Cold Start Trap will be enabled. The Cold Start Trap is broadcast to a subnet broadcast address if there are no trap destinations configured in the SNMP Alert Destination(s) boxes.|
|Type|boolean|
|Read Only|False|

### PeriodicHSATrapConfig
Member of [HpeiLOSnmpService.v2_1_0.HpeiLOSnmpService](#hpeilosnmpservice-v2_1_0-hpeilosnmpservice)

| | |
|---|---|
|Description|If there are any component in health status array(HSA) Trap are in degraded or failed condition then HSA trap will be sent periodically till the component status becomes ok or fine condition. This setting is disabled by default.|
|Type|string|
|Read Only|False|

The following are the supported values:

|Value|
|---|
|```Disabled```|
|```Daily```|
|```Weekly```|
|```Monthly```|

### ReadCommunities (array)
Member of [HpeiLOSnmpService.v2_1_0.HpeiLOSnmpService](#hpeilosnmpservice-v2_1_0-hpeilosnmpservice)
```ReadCommunities``` is an array containing elements of:


| | |
|---|---|
|Type|string|
|Read Only|True|

### Role
Member of [HpeiLOSnmpService.v2_1_0.HpeiLOSnmpService](#hpeilosnmpservice-v2_1_0-hpeilosnmpservice)

| | |
|---|---|
|Description|The string of up to 64 characters that describes the server role or function.|
|Type|string or null|
|Read Only|False|

### RoleDetail
Member of [HpeiLOSnmpService.v2_1_0.HpeiLOSnmpService](#hpeilosnmpservice-v2_1_0-hpeilosnmpservice)

| | |
|---|---|
|Description|The string of up to 512 characters that describes specific tasks that the server might perform.|
|Type|string or null|
|Read Only|False|

### SNMPAlertDestinations
SNMP Alert Destination details.
### SNMPUsers
SNMPv3 User details.
### SNMPv1Traps
Member of [HpeiLOSnmpService.v2_1_0.HpeiLOSnmpService](#hpeilosnmpservice-v2_1_0-hpeilosnmpservice)

| | |
|---|---|
|Description|When enabled, SNMPv1 traps are sent to the remote management systems configured in the SNMP Alert Destination(s) boxes.|
|Type|boolean|
|Read Only|False|

### SNMPv3EngineID
Member of [HpeiLOSnmpService.v2_1_0.HpeiLOSnmpService](#hpeilosnmpservice-v2_1_0-hpeilosnmpservice)

| | |
|---|---|
|Description|The SNMPv3 Engine ID is the unique identifier of an SNMP engine that belongs to an SNMP agent entity. This value must be a hexadecimal string with an even number of 6 to 32 characters, excluding the first two characters, 0x (for example, 0x01020304abcdef).|
|Type|string or null|
|Read Only|False|

### SNMPv3InformRetryAttempt
Member of [HpeiLOSnmpService.v2_1_0.HpeiLOSnmpService](#hpeilosnmpservice-v2_1_0-hpeilosnmpservice)

| | |
|---|---|
|Description|Specifies the number of retries to be used in SNMPv3 inform.|
|Type|integer|
|Read Only|False|

### SNMPv3InformRetryIntervalSeconds
Member of [HpeiLOSnmpService.v2_1_0.HpeiLOSnmpService](#hpeilosnmpservice-v2_1_0-hpeilosnmpservice)

| | |
|---|---|
|Description|Specifies the interval in seconds between SNMPv3 inform retries.|
|Type|integer|
|Read Only|False|

### Status
Member of [HpeiLOSnmpService.v2_1_0.HpeiLOSnmpService](#hpeilosnmpservice-v2_1_0-hpeilosnmpservice)
See the Redfish standard schema and specification for information on common Status object.

### TrapCommunities (array)
Member of [HpeiLOSnmpService.v2_1_0.HpeiLOSnmpService](#hpeilosnmpservice-v2_1_0-hpeilosnmpservice)
```TrapCommunities``` is an array containing elements of:


| | |
|---|---|
|Type|string|
|Read Only|True|

### TrapSourceHostname
Member of [HpeiLOSnmpService.v2_1_0.HpeiLOSnmpService](#hpeilosnmpservice-v2_1_0-hpeilosnmpservice)

| | |
|---|---|
|Description|Determines the host name that is used in the SNMP-defined sysName variable when the management processor generates SNMP traps.|
|Type|string|
|Read Only|False|

The following are the supported values:

|Value|
|---|
|```Manager```|
|```System```|

### Users (array)
Member of [HpeiLOSnmpService.v2_1_0.HpeiLOSnmpService](#hpeilosnmpservice-v2_1_0-hpeilosnmpservice)
```Users``` is an array containing elements of:

**Users[{item}].AuthPassphrase**
Member of [HpeiLOSnmpService.v2_1_0.HpeiLOSnmpService](#hpeilosnmpservice-v2_1_0-hpeilosnmpservice)

| | |
|---|---|
|Description|Sets the passphrase to use for sign operations. Enter a value of 8 to 49 characters.|
|Type|string or null|
|Read Only|False|

**Users[{item}].AuthProtocol**
Member of [HpeiLOSnmpService.v2_1_0.HpeiLOSnmpService](#hpeilosnmpservice-v2_1_0-hpeilosnmpservice)

| | |
|---|---|
|Description|Sets the message digest algorithm to use for encoding the authorization passphrase. The message digest is calculated over an appropriate portion of an SNMP message, and is included as part of the message sent to the recipient. Select MD5 (Message Digest) or SHA (Secure Hash Algorithm).|
|Type|string or null|
|Read Only|False|

The following are the supported values:

|Value|Description|
|---|---|
|```MD5```|Indicate Message Digest Algorithm.|
|```SHA```|Indicate Secure Hash Algorithm.|
|```Null```|A value is temporarily unavailable|

**Users[{item}].PrivacyPassphrase**
Member of [HpeiLOSnmpService.v2_1_0.HpeiLOSnmpService](#hpeilosnmpservice-v2_1_0-hpeilosnmpservice)

| | |
|---|---|
|Description|Sets the passphrase to use for encrypt operations. Enter a value of 8 to 49 characters.|
|Type|string or null|
|Read Only|False|

**Users[{item}].PrivacyProtocol**
Member of [HpeiLOSnmpService.v2_1_0.HpeiLOSnmpService](#hpeilosnmpservice-v2_1_0-hpeilosnmpservice)

| | |
|---|---|
|Description|Sets the encryption algorithm to use for encoding the privacy passphrase. A portion of an SNMP message is encrypted before transmission. Select AES (Advanced Encryption Standard) or DES (Data Encryption Standard).|
|Type|string or null|
|Read Only|False|

The following are the supported values:

|Value|Description|
|---|---|
|```AES```|Indicate Advanced Encryption Standard Algorithm.|
|```DES```|Indicate Data Encryption Standard Algorithm.|
|```Null```|A value is temporarily unavailable|

**Users[{item}].SecurityName**
Member of [HpeiLOSnmpService.v2_1_0.HpeiLOSnmpService](#hpeilosnmpservice-v2_1_0-hpeilosnmpservice)

| | |
|---|---|
|Description|The user profile name. Enter an alphanumeric string of 1 to 32 characters.|
|Type|string or null|
|Read Only|False|

**Users[{item}].UserEngineID**
Member of [HpeiLOSnmpService.v2_1_0.HpeiLOSnmpService](#hpeilosnmpservice-v2_1_0-hpeilosnmpservice)

| | |
|---|---|
|Description|The UserEngineID is combined with the SecurityName to create a SNMPv3 user for each manager. It is only used for creating remote accounts used with INFORM messages. If this property is not set then INFORM message will be sent with default or iLO configured engine ID. This value must be a hexadecimal string with an even number of 10 to 64 characters, excluding the first two characters, 0x (for example, 0x01020304abcdef).|
|Type|string or null|
|Read Only|False|

### Actions

**HpeiLOSnmpService.SendSNMPTestAlert**
Member of [HpeiLOSnmpService.v2_1_0.HpeiLOSnmpService](#hpeilosnmpservice-v2_1_0-hpeilosnmpservice)
There are no parameters for this action.
## HpeiLOSSO.v2_0_0.HpeiLOSSO
```@odata.type: "#HpeiLOSSO.v2_0_0.HpeiLOSSO"```

This is the schema definition for the HPE SSO Trusted Server.
### Resource Instances
|Uri|HTTP Allow|
|---|---|
|```/redfish/v1/managers/{item}/securityservice/sso/```|GET POST PATCH |

### ManagerTrustedCertificates (array)
Member of [HpeiLOSSO.v2_0_0.HpeiLOSSO](#hpeilosso-v2_0_0-hpeilosso)
```ManagerTrustedCertificates``` is an array containing elements of:

**ManagerTrustedCertificates[{item}].Certificate**
Member of [HpeiLOSSO.v2_0_0.HpeiLOSSO](#hpeilosso-v2_0_0-hpeilosso)

| | |
|---|---|
|Description|Contains PEM formatted X509 certificate (Base64 encoded).|
|Type|string or null|
|Read Only|True|

**ManagerTrustedCertificates[{item}].CertificateDetails**
**ManagerTrustedCertificates[{item}].CertificateDetails.Issuer**
Member of [HpeiLOSSO.v2_0_0.HpeiLOSSO](#hpeilosso-v2_0_0-hpeilosso)

| | |
|---|---|
|Description|The Certificate Authority that issued the certificate.|
|Type|string|
|Read Only|True|

**ManagerTrustedCertificates[{item}].CertificateDetails.Subject**
Member of [HpeiLOSSO.v2_0_0.HpeiLOSSO](#hpeilosso-v2_0_0-hpeilosso)

| | |
|---|---|
|Description|The entity to which the certificate was issued.|
|Type|string|
|Read Only|True|

**ManagerTrustedCertificates[{item}].CertificateDetails.ValidNotAfter**
Member of [HpeiLOSSO.v2_0_0.HpeiLOSSO](#hpeilosso-v2_0_0-hpeilosso)

| | |
|---|---|
|Description|The date on which the certificate validity period ends.|
|Type|string|
|Read Only|True|

**ManagerTrustedCertificates[{item}].CertificateDetails.ValidNotBefore**
Member of [HpeiLOSSO.v2_0_0.HpeiLOSSO](#hpeilosso-v2_0_0-hpeilosso)

| | |
|---|---|
|Description|The date on which the certificate validity period begins.|
|Type|string|
|Read Only|True|

**ManagerTrustedCertificates[{item}].RecordType**
Member of [HpeiLOSSO.v2_0_0.HpeiLOSSO](#hpeilosso-v2_0_0-hpeilosso)

| | |
|---|---|
|Description|Specifies the type of SSO record imported.|
|Type|string|
|Read Only|true|

The following are the supported values:

|Value|Description|
|---|---|
|```Certificate```|It is a PEM formatted X509 certificate (Base64 encoded).|
|```DNSName```|It is a DNS name or an IP address of the HPE SSO-compliant application.|

**ManagerTrustedCertificates[{item}].SerialNumber**
Member of [HpeiLOSSO.v2_0_0.HpeiLOSSO](#hpeilosso-v2_0_0-hpeilosso)

| | |
|---|---|
|Description|Contains the Serial number for the SSO records.|
|Type|integer|
|Read Only|True|

**ManagerTrustedCertificates[{item}].ServerName**
Member of [HpeiLOSSO.v2_0_0.HpeiLOSSO](#hpeilosso-v2_0_0-hpeilosso)

| | |
|---|---|
|Description|The Server name (or certificate subject).|
|Type|string or null|
|Read Only|True|

**ManagerTrustedCertificates[{item}].Status**
Member of [HpeiLOSSO.v2_0_0.HpeiLOSSO](#hpeilosso-v2_0_0-hpeilosso)
See the Redfish standard schema and specification for information on common Status object.

### SSOsettings
**SSOsettings.AdminPrivilege**
**SSOsettings.AdminPrivilege.HostBIOSConfigPriv**
Member of [HpeiLOSSO.v2_0_0.HpeiLOSSO](#hpeilosso-v2_0_0-hpeilosso)

| | |
|---|---|
|Description|Host BIOS Configuration Privileges.|
|Type|boolean|
|Read Only|False|

**SSOsettings.AdminPrivilege.HostNICConfigPriv**
Member of [HpeiLOSSO.v2_0_0.HpeiLOSSO](#hpeilosso-v2_0_0-hpeilosso)

| | |
|---|---|
|Description|Host NIC Configuration Privileges.|
|Type|boolean|
|Read Only|False|

**SSOsettings.AdminPrivilege.HostStorageConfigPriv**
Member of [HpeiLOSSO.v2_0_0.HpeiLOSSO](#hpeilosso-v2_0_0-hpeilosso)

| | |
|---|---|
|Description|Host Storage Configuration Privileges.|
|Type|boolean|
|Read Only|False|

**SSOsettings.AdminPrivilege.LoginPriv**
Member of [HpeiLOSSO.v2_0_0.HpeiLOSSO](#hpeilosso-v2_0_0-hpeilosso)

| | |
|---|---|
|Description|Login Privileges.|
|Type|boolean|
|Read Only|False|

**SSOsettings.AdminPrivilege.RemoteConsolePriv**
Member of [HpeiLOSSO.v2_0_0.HpeiLOSSO](#hpeilosso-v2_0_0-hpeilosso)

| | |
|---|---|
|Description|Remote Console Privileges.|
|Type|boolean|
|Read Only|False|

**SSOsettings.AdminPrivilege.SystemRecoveryConfigPriv**
Member of [HpeiLOSSO.v2_0_0.HpeiLOSSO](#hpeilosso-v2_0_0-hpeilosso)

| | |
|---|---|
|Description|System Recovery Configuration Privileges.|
|Type|boolean|
|Read Only|False|

**SSOsettings.AdminPrivilege.UserConfigPriv**
Member of [HpeiLOSSO.v2_0_0.HpeiLOSSO](#hpeilosso-v2_0_0-hpeilosso)

| | |
|---|---|
|Description|User Configuration Privileges.|
|Type|boolean|
|Read Only|False|

**SSOsettings.AdminPrivilege.VirtualMediaPriv**
Member of [HpeiLOSSO.v2_0_0.HpeiLOSSO](#hpeilosso-v2_0_0-hpeilosso)

| | |
|---|---|
|Description|Virtual Media Privileges.|
|Type|boolean|
|Read Only|False|

**SSOsettings.AdminPrivilege.VirtualPowerAndResetPriv**
Member of [HpeiLOSSO.v2_0_0.HpeiLOSSO](#hpeilosso-v2_0_0-hpeilosso)

| | |
|---|---|
|Description|Power and Reset Privileges.|
|Type|boolean|
|Read Only|False|

**SSOsettings.AdminPrivilege.iLOConfigPriv**
Member of [HpeiLOSSO.v2_0_0.HpeiLOSSO](#hpeilosso-v2_0_0-hpeilosso)

| | |
|---|---|
|Description|iLO Configuration Privileges.|
|Type|boolean|
|Read Only|False|

**SSOsettings.OperatorPrivilege**
**SSOsettings.OperatorPrivilege.HostBIOSConfigPriv**
Member of [HpeiLOSSO.v2_0_0.HpeiLOSSO](#hpeilosso-v2_0_0-hpeilosso)

| | |
|---|---|
|Description|Host BIOS Configuration Privileges.|
|Type|boolean|
|Read Only|False|

**SSOsettings.OperatorPrivilege.HostNICConfigPriv**
Member of [HpeiLOSSO.v2_0_0.HpeiLOSSO](#hpeilosso-v2_0_0-hpeilosso)

| | |
|---|---|
|Description|Host NIC Configuration Privileges.|
|Type|boolean|
|Read Only|False|

**SSOsettings.OperatorPrivilege.HostStorageConfigPriv**
Member of [HpeiLOSSO.v2_0_0.HpeiLOSSO](#hpeilosso-v2_0_0-hpeilosso)

| | |
|---|---|
|Description|Host Storage Configuration Privileges.|
|Type|boolean|
|Read Only|False|

**SSOsettings.OperatorPrivilege.LoginPriv**
Member of [HpeiLOSSO.v2_0_0.HpeiLOSSO](#hpeilosso-v2_0_0-hpeilosso)

| | |
|---|---|
|Description|Login Privileges.|
|Type|boolean|
|Read Only|False|

**SSOsettings.OperatorPrivilege.RemoteConsolePriv**
Member of [HpeiLOSSO.v2_0_0.HpeiLOSSO](#hpeilosso-v2_0_0-hpeilosso)

| | |
|---|---|
|Description|Remote Console Privileges.|
|Type|boolean|
|Read Only|False|

**SSOsettings.OperatorPrivilege.SystemRecoveryConfigPriv**
Member of [HpeiLOSSO.v2_0_0.HpeiLOSSO](#hpeilosso-v2_0_0-hpeilosso)

| | |
|---|---|
|Description|System Recovery Configuration Privileges.|
|Type|boolean|
|Read Only|False|

**SSOsettings.OperatorPrivilege.UserConfigPriv**
Member of [HpeiLOSSO.v2_0_0.HpeiLOSSO](#hpeilosso-v2_0_0-hpeilosso)

| | |
|---|---|
|Description|User Configuration Privileges.|
|Type|boolean|
|Read Only|False|

**SSOsettings.OperatorPrivilege.VirtualMediaPriv**
Member of [HpeiLOSSO.v2_0_0.HpeiLOSSO](#hpeilosso-v2_0_0-hpeilosso)

| | |
|---|---|
|Description|Virtual Media Privileges.|
|Type|boolean|
|Read Only|False|

**SSOsettings.OperatorPrivilege.VirtualPowerAndResetPriv**
Member of [HpeiLOSSO.v2_0_0.HpeiLOSSO](#hpeilosso-v2_0_0-hpeilosso)

| | |
|---|---|
|Description|Power and Reset Privileges.|
|Type|boolean|
|Read Only|False|

**SSOsettings.OperatorPrivilege.iLOConfigPriv**
Member of [HpeiLOSSO.v2_0_0.HpeiLOSSO](#hpeilosso-v2_0_0-hpeilosso)

| | |
|---|---|
|Description|iLO Configuration Privileges.|
|Type|boolean|
|Read Only|False|

**SSOsettings.SSOTrustMode**
Member of [HpeiLOSSO.v2_0_0.HpeiLOSSO](#hpeilosso-v2_0_0-hpeilosso)

| | |
|---|---|
|Description|Represents the SSO Trust Mode.|
|Type|string|
|Read Only|False|

The following are the supported values:

|Value|Description|
|---|---|
|```TrustNone```|Rejects all SSO connection request.|
|```TrustAll```|Accepts any SSO connection initiated from any HPE SSO compliant application.|
|```TrustbyName```|Enables SSO connections from an HPE SSO compliant application by matching a directly imported IP address or DNS name.|
|```TrustbyCert```|Enables SSO connections from an HPE SSO compliant application by matching a certificate previously imported to iLO.|

**SSOsettings.UserPrivilege**
**SSOsettings.UserPrivilege.HostBIOSConfigPriv**
Member of [HpeiLOSSO.v2_0_0.HpeiLOSSO](#hpeilosso-v2_0_0-hpeilosso)

| | |
|---|---|
|Description|Host BIOS Configuration Privileges.|
|Type|boolean|
|Read Only|False|

**SSOsettings.UserPrivilege.HostNICConfigPriv**
Member of [HpeiLOSSO.v2_0_0.HpeiLOSSO](#hpeilosso-v2_0_0-hpeilosso)

| | |
|---|---|
|Description|Host NIC Configuration Privileges.|
|Type|boolean|
|Read Only|False|

**SSOsettings.UserPrivilege.HostStorageConfigPriv**
Member of [HpeiLOSSO.v2_0_0.HpeiLOSSO](#hpeilosso-v2_0_0-hpeilosso)

| | |
|---|---|
|Description|Host Storage Configuration Privileges.|
|Type|boolean|
|Read Only|False|

**SSOsettings.UserPrivilege.LoginPriv**
Member of [HpeiLOSSO.v2_0_0.HpeiLOSSO](#hpeilosso-v2_0_0-hpeilosso)

| | |
|---|---|
|Description|Login Privileges.|
|Type|boolean|
|Read Only|False|

**SSOsettings.UserPrivilege.RemoteConsolePriv**
Member of [HpeiLOSSO.v2_0_0.HpeiLOSSO](#hpeilosso-v2_0_0-hpeilosso)

| | |
|---|---|
|Description|Remote Console Privileges.|
|Type|boolean|
|Read Only|False|

**SSOsettings.UserPrivilege.SystemRecoveryConfigPriv**
Member of [HpeiLOSSO.v2_0_0.HpeiLOSSO](#hpeilosso-v2_0_0-hpeilosso)

| | |
|---|---|
|Description|System Recovery Configuration Privileges.|
|Type|boolean|
|Read Only|False|

**SSOsettings.UserPrivilege.UserConfigPriv**
Member of [HpeiLOSSO.v2_0_0.HpeiLOSSO](#hpeilosso-v2_0_0-hpeilosso)

| | |
|---|---|
|Description|User Configuration Privileges.|
|Type|boolean|
|Read Only|False|

**SSOsettings.UserPrivilege.VirtualMediaPriv**
Member of [HpeiLOSSO.v2_0_0.HpeiLOSSO](#hpeilosso-v2_0_0-hpeilosso)

| | |
|---|---|
|Description|Virtual Media Privileges.|
|Type|boolean|
|Read Only|False|

**SSOsettings.UserPrivilege.VirtualPowerAndResetPriv**
Member of [HpeiLOSSO.v2_0_0.HpeiLOSSO](#hpeilosso-v2_0_0-hpeilosso)

| | |
|---|---|
|Description|Power and Reset Privileges.|
|Type|boolean|
|Read Only|False|

**SSOsettings.UserPrivilege.iLOConfigPriv**
Member of [HpeiLOSSO.v2_0_0.HpeiLOSSO](#hpeilosso-v2_0_0-hpeilosso)

| | |
|---|---|
|Description|iLO Configuration Privileges.|
|Type|boolean|
|Read Only|False|

### Actions

**HpeiLOSSO.ImportDNSName**
Member of [HpeiLOSSO.v2_0_0.HpeiLOSSO](#hpeilosso-v2_0_0-hpeilosso)
Add DNS Name to the record list.


**Parameters:**

**DNSName (string)**

DNS Name of the HPE SSO Trusted Server.

**HpeiLOSSO.ImportCertificate**
Member of [HpeiLOSSO.v2_0_0.HpeiLOSSO](#hpeilosso-v2_0_0-hpeilosso)
Import the HPE SSO Certificate.


**Parameters:**

**CertInput (string)**

PEM formatted X509 certificate (Base64 encoded)/DNS name or IP address to import the certificate.

**CertType (string)**

Specifies the type of certificate imported.

|Value|Description|
|---|---|
|ImportCertUri|iLO imports the certificate from the HPE SSO compliant application over the network.|
|DirectImportCert|iLO directly imports the Certificate.|

**HpeiLOSSO.DeleteSSORecordbyNumber**
Member of [HpeiLOSSO.v2_0_0.HpeiLOSSO](#hpeilosso-v2_0_0-hpeilosso)
Delete SSO record by record number.


**Parameters:**

**RecordNumber (integer)**

Index of the SSO record to be deleted.

**HpeiLOSSO.DeleteAllSSORecords**
Member of [HpeiLOSSO.v2_0_0.HpeiLOSSO](#hpeilosso-v2_0_0-hpeilosso)
Delete all the SSO records.

There are no parameters for this action.
## HpeiSCSISoftwareInitiator.v2_0_0.HpeiSCSISoftwareInitiator
```@odata.type: "#HpeiSCSISoftwareInitiator.v2_0_0.HpeiSCSISoftwareInitiator"```
### Resource Instances
|Uri|HTTP Allow|
|---|---|
|```/redfish/v1/systems/{item}/bios/iscsi/```|GET |
|```/redfish/v1/systems/{item}/bios/iscsi/settings/```|GET PATCH |

### Links to other Resources
|Link Name|Destination type
|---|---|
|```@Redfish.Settings/SettingsObject```|[HpeiSCSISoftwareInitiator](#hpeiscsisoftwareinitiator-v2_0_0-hpeiscsisoftwareinitiator)|
|```Oem/Hpe/Links/BaseConfigs```|[HpeBaseConfigs](#hpebaseconfigs-v2_0_0-hpebaseconfigs)|

### @Redfish.Settings
Member of [HpeiSCSISoftwareInitiator.v2_0_0.HpeiSCSISoftwareInitiator](#hpeiscsisoftwareinitiator-v2_0_0-hpeiscsisoftwareinitiator)
See the Redfish standard schema and specification for information on common @Redfish properties.

### iSCSIInitiatorName
Member of [HpeiSCSISoftwareInitiator.v2_0_0.HpeiSCSISoftwareInitiator](#hpeiscsisoftwareinitiator-v2_0_0-hpeiscsisoftwareinitiator)

| | |
|---|---|
|Description|The worldwide unique iSCSI Qualified Name (IQN) of this iSCSI Initiator. Only IQN format is accepted. EUI format is not supported (for example, 'iqn.1986-03.com.hp:init.sn-123456').|
|Type|string|
|Read Only|True|

### iSCSINicSources (array)
Member of [HpeiSCSISoftwareInitiator.v2_0_0.HpeiSCSISoftwareInitiator](#hpeiscsisoftwareinitiator-v2_0_0-hpeiscsisoftwareinitiator)
```iSCSINicSources``` is an array containing elements of:


| | |
|---|---|
|Description|The BIOS Attribute that describes a NIC instance that can be used as a target for iSCSI configuration.|
|Type|string|
|Read Only|True|

### iSCSISources (array)
Member of [HpeiSCSISoftwareInitiator.v2_0_0.HpeiSCSISoftwareInitiator](#hpeiscsisoftwareinitiator-v2_0_0-hpeiscsisoftwareinitiator)
```iSCSISources``` is an array containing elements of:

**iSCSISources[{item}].StructuredBootString**
Member of [HpeiSCSISoftwareInitiator.v2_0_0.HpeiSCSISoftwareInitiator](#hpeiscsisoftwareinitiator-v2_0_0-hpeiscsisoftwareinitiator)

| | |
|---|---|
|Description|Identifies this iSCSI option within the server.|
|Type|string or null|
|Read Only|True|

**iSCSISources[{item}].UEFIDevicePath**
Member of [HpeiSCSISoftwareInitiator.v2_0_0.HpeiSCSISoftwareInitiator](#hpeiscsisoftwareinitiator-v2_0_0-hpeiscsisoftwareinitiator)

| | |
|---|---|
|Description|Standardized text representation of the UEFI device path for this option, in UTF-8 format.|
|Type|string or null|
|Read Only|True|

**iSCSISources[{item}].iSCSIAttemptInstance**
Member of [HpeiSCSISoftwareInitiator.v2_0_0.HpeiSCSISoftwareInitiator](#hpeiscsisoftwareinitiator-v2_0_0-hpeiscsisoftwareinitiator)

| | |
|---|---|
|Description|Uniquely identifies this iSCSI attempt within iSCSISources array. If set to zero, all other properties in the boot option object are ignored (which will delete an existing boot attempt).|
|Type|integer|
|Read Only|True|

**iSCSISources[{item}].iSCSIAttemptName**
Member of [HpeiSCSISoftwareInitiator.v2_0_0.HpeiSCSISoftwareInitiator](#hpeiscsisoftwareinitiator-v2_0_0-hpeiscsisoftwareinitiator)

| | |
|---|---|
|Description|Human readable descriptive name for this iSCSI attempt configuration|
|Type|string or null|
|Read Only|True|

**iSCSISources[{item}].iSCSIAuthenticationMethod**
Member of [HpeiSCSISoftwareInitiator.v2_0_0.HpeiSCSISoftwareInitiator](#hpeiscsisoftwareinitiator-v2_0_0-hpeiscsisoftwareinitiator)

| | |
|---|---|
|Description|The iSCSI connection authentication method.|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```None```|No iSCSI connection security.|
|```CHAP```|iSCSI connection is secured using Challenge Handshake Authentication Protocol (CHAP).|

**iSCSISources[{item}].iSCSIChapSecret**
Member of [HpeiSCSISoftwareInitiator.v2_0_0.HpeiSCSISoftwareInitiator](#hpeiscsisoftwareinitiator-v2_0_0-hpeiscsisoftwareinitiator)

| | |
|---|---|
|Description|The password needed for CHAP authentication. This is applicable only when the Authentication Method is set to CHAP, and the CHAP Type is set to Mutual.|
|Type|string or null|
|Read Only|True|

**iSCSISources[{item}].iSCSIChapType**
Member of [HpeiSCSISoftwareInitiator.v2_0_0.HpeiSCSISoftwareInitiator](#hpeiscsisoftwareinitiator-v2_0_0-hpeiscsisoftwareinitiator)

| | |
|---|---|
|Description|The CHAP authentication type. This is applicable only when the Authentication Method is set to CHAP.|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```OneWay```|The target will authenticate the initiator. .|
|```Mutual```|both the initiator and target will authenticate each other.|

**iSCSISources[{item}].iSCSIChapUsername**
Member of [HpeiSCSISoftwareInitiator.v2_0_0.HpeiSCSISoftwareInitiator](#hpeiscsisoftwareinitiator-v2_0_0-hpeiscsisoftwareinitiator)

| | |
|---|---|
|Description|The password needed for CHAP authentication. This is applicable only when the Authentication Method is set to CHAP.|
|Type|string or null|
|Read Only|True|

**iSCSISources[{item}].iSCSIConnectRetry**
Member of [HpeiSCSISoftwareInitiator.v2_0_0.HpeiSCSISoftwareInitiator](#hpeiscsisoftwareinitiator-v2_0_0-hpeiscsisoftwareinitiator)

| | |
|---|---|
|Description|The number of times to retry the iSCSI connection. Zero means no retries.|
|Type|integer|
|Read Only|True|

**iSCSISources[{item}].iSCSIConnectTimeoutMS**
Member of [HpeiSCSISoftwareInitiator.v2_0_0.HpeiSCSISoftwareInitiator](#hpeiscsisoftwareinitiator-v2_0_0-hpeiscsisoftwareinitiator)

| | |
|---|---|
|Description|The iSCSI connection timeout value in milliseconds.|
|Type|integer|
|Read Only|True|

**iSCSISources[{item}].iSCSIConnection**
Member of [HpeiSCSISoftwareInitiator.v2_0_0.HpeiSCSISoftwareInitiator](#hpeiscsisoftwareinitiator-v2_0_0-hpeiscsisoftwareinitiator)

| | |
|---|---|
|Description|Enables or Disables iSCSI mode for a selected iSCSI attempt.|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```Disabled```|Connecting to this iSCSI attempt is disabled.|
|```Enabled```|Connecting to this iSCSI attempt is enabled.|
|```EnabledMpio```|Connecting to this iSCSI attempt is enabled with MPIO (Multi Path I/O).|

**iSCSISources[{item}].iSCSIInitiatorGateway**
Member of [HpeiSCSISoftwareInitiator.v2_0_0.HpeiSCSISoftwareInitiator](#hpeiscsisoftwareinitiator-v2_0_0-hpeiscsisoftwareinitiator)

| | |
|---|---|
|Description|The gateway address of the iSCSI Initiator, if not configured via DHCP. The address must be an IPv4 or IPv6 address, depending on the IP Address Type.|
|Type|string|
|Read Only|True|

**iSCSISources[{item}].iSCSIInitiatorInfoViaDHCP**
Member of [HpeiSCSISoftwareInitiator.v2_0_0.HpeiSCSISoftwareInitiator](#hpeiscsisoftwareinitiator-v2_0_0-hpeiscsisoftwareinitiator)

| | |
|---|---|
|Description|If enabled, the iSCSI Initiator information is configured from DHCP. Otherwise, the iSCSI initiator information must be statically configured. When providing static values for the Initiator, ensure Target settings are also configured with static values.|
|Type|boolean|
|Read Only|True|

**iSCSISources[{item}].iSCSIInitiatorIpAddress**
Member of [HpeiSCSISoftwareInitiator.v2_0_0.HpeiSCSISoftwareInitiator](#hpeiscsisoftwareinitiator-v2_0_0-hpeiscsisoftwareinitiator)

| | |
|---|---|
|Description|The IP Address of the iSCSI Initiator, if not configured via DHCP. The Initiator IP Address is always auto-assigned if IP address type is IPv6. The address must be an IPv4 or IPv6 address, depending on the IP Address Type.|
|Type|string|
|Read Only|True|

**iSCSISources[{item}].iSCSIInitiatorNetmask**
Member of [HpeiSCSISoftwareInitiator.v2_0_0.HpeiSCSISoftwareInitiator](#hpeiscsisoftwareinitiator-v2_0_0-hpeiscsisoftwareinitiator)

| | |
|---|---|
|Description|The subnet mask of the iSCSI Initiator, if not configured via DHCP. The address must be an IPv4.|
|Type|string|
|Read Only|True|

**iSCSISources[{item}].iSCSIIpAddressType**
Member of [HpeiSCSISoftwareInitiator.v2_0_0.HpeiSCSISoftwareInitiator](#hpeiscsisoftwareinitiator-v2_0_0-hpeiscsisoftwareinitiator)

| | |
|---|---|
|Description|The iSCSI IP Address type. If set to Auto, IPv4 will be attempted first, followed by IPv6.|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```IPv4```|The iSCSI IP address is configured in IPv4 format.|
|```IPv6```|The iSCSI IP address is configured in IPv6 format.|
|```Auto```|The iSCSI IP address is configured in IPv4. If an issue occurs with IPv4, then the IPv6 configuration is used.|

**iSCSISources[{item}].iSCSILUN**
Member of [HpeiSCSISoftwareInitiator.v2_0_0.HpeiSCSISoftwareInitiator](#hpeiscsisoftwareinitiator-v2_0_0-hpeiscsisoftwareinitiator)

| | |
|---|---|
|Description|The iSCSI target Logical Unit Number (LUN), if not obtained from DHCP. This value must follow the SAM-2 spec. E.g. 0001-1234-5678-9ABC. If the digit number is less then 5 characters, a dash character is not required. E.g. 0001. If the lun number is 12345, input 1234-5|
|Type|string|
|Read Only|True|

**iSCSISources[{item}].iSCSINicSource**
Member of [HpeiSCSISoftwareInitiator.v2_0_0.HpeiSCSISoftwareInitiator](#hpeiscsisoftwareinitiator-v2_0_0-hpeiscsisoftwareinitiator)

| | |
|---|---|
|Description|A BIOS Attribute that describes this selected NIC instance. This must match one of the possible values listed in the iSCSINicSources array.|
|Type|string or null|
|Read Only|True|

**iSCSISources[{item}].iSCSIReverseChapSecret**
Member of [HpeiSCSISoftwareInitiator.v2_0_0.HpeiSCSISoftwareInitiator](#hpeiscsisoftwareinitiator-v2_0_0-hpeiscsisoftwareinitiator)

| | |
|---|---|
|Description|The password needed for reverse CHAP authentication (from the target to the initiator). This is applicable only when the Authentication Method is set to CHAP, and the CHAP Type is set to Mutual.|
|Type|string or null|
|Read Only|True|

**iSCSISources[{item}].iSCSIReverseChapUsername**
Member of [HpeiSCSISoftwareInitiator.v2_0_0.HpeiSCSISoftwareInitiator](#hpeiscsisoftwareinitiator-v2_0_0-hpeiscsisoftwareinitiator)

| | |
|---|---|
|Description|User Name for reverse CHAP authentication (from the target to the initiator). This is applicable only when the Authentication Method is set to CHAP, and the CHAP Type is set to Mutual.|
|Type|string or null|
|Read Only|True|

**iSCSISources[{item}].iSCSITargetInfoViaDHCP**
Member of [HpeiSCSISoftwareInitiator.v2_0_0.HpeiSCSISoftwareInitiator](#hpeiscsisoftwareinitiator-v2_0_0-hpeiscsisoftwareinitiator)

| | |
|---|---|
|Description|If enabled, the iSCSI target information are configured from DHCP. Otherwise, the iSCSI target information must be statically configured.|
|Type|boolean|
|Read Only|True|

**iSCSISources[{item}].iSCSITargetIpAddress**
Member of [HpeiSCSISoftwareInitiator.v2_0_0.HpeiSCSISoftwareInitiator](#hpeiscsisoftwareinitiator-v2_0_0-hpeiscsisoftwareinitiator)

| | |
|---|---|
|Description|The IP Address of the iSCSI Target, if not obtained from DHCP. The address must be an IPv4 or IPv6 address, depending on the IP Address Type.|
|Type|string|
|Read Only|True|

**iSCSISources[{item}].iSCSITargetName**
Member of [HpeiSCSISoftwareInitiator.v2_0_0.HpeiSCSISoftwareInitiator](#hpeiscsisoftwareinitiator-v2_0_0-hpeiscsisoftwareinitiator)

| | |
|---|---|
|Description|The worldwide unique iSCSI Qualified Name (IQN) of this iSCSI target. Only the IQN format is accepted. EUI format is not supported (for example, 'iqn.1991-05.com.microsoft:iscsitarget-iscsidisk-target').|
|Type|string or null|
|Read Only|True|

**iSCSISources[{item}].iSCSITargetTcpPort**
Member of [HpeiSCSISoftwareInitiator.v2_0_0.HpeiSCSISoftwareInitiator](#hpeiscsisoftwareinitiator-v2_0_0-hpeiscsisoftwareinitiator)

| | |
|---|---|
|Description|The iSCSI Target TCP Port number, if not obtained from DHCP.|
|Type|integer|
|Read Only|True|

## HpeNetworkPortEVB.v1_0_0.HpeNetworkPortEVB
```@odata.type: "#HpeNetworkPortEVB.v1_0_0.HpeNetworkPortEVB"```

Hewlett Packard Enterprise property extensions for Network Ports Edge Virtual Bridging
### Resource Instances
|Uri|HTTP Allow|
|---|---|
|```/redfish/v1/chassis/{item}/networkadapters/{item}/networkports/{item}/hpeevb/```|GET |
|```/redfish/v1/systems/{item}/networkinterfaces/{item}/networkports/{item}/hpeevb/```|GET |

### Receiving
**Receiving.CdcpActive**
Member of [HpeNetworkPortEVB.v1_0_0.HpeNetworkPortEVB](#hpenetworkportevb-v1_0_0-hpenetworkportevb)

| | |
|---|---|
|Description|True if a currently active IEEE 802.1Qbg CDCP TLV has been received from the link partner.|
|Type|boolean|
|Read Only|True|

**Receiving.ChannelActive**
Member of [HpeNetworkPortEVB.v1_0_0.HpeNetworkPortEVB](#hpenetworkportevb-v1_0_0-hpenetworkportevb)

| | |
|---|---|
|Description|A currently unexpired HPE Channel Link Control or HPE Channel Description TLV has been received from the link partner.|
|Type|boolean|
|Read Only|True|

**Receiving.ChannelDescriptionLocalSequenceNumber**
Member of [HpeNetworkPortEVB.v1_0_0.HpeNetworkPortEVB](#hpenetworkportevb-v1_0_0-hpenetworkportevb)

| | |
|---|---|
|Description|The link partner's HPE Channel Description sequence number that was last successfully received and processed.|
|Type|integer|
|Read Only|True|

**Receiving.ChannelDescriptionRemoteSequenceNumber**
Member of [HpeNetworkPortEVB.v1_0_0.HpeNetworkPortEVB](#hpenetworkportevb-v1_0_0-hpenetworkportevb)

| | |
|---|---|
|Description|The last HPE Channel Decsription sequence number sent on this link that was successfully received and processed by the link partner.|
|Type|integer|
|Read Only|True|

**Receiving.ChannelDescriptionSubtype**
Member of [HpeNetworkPortEVB.v1_0_0.HpeNetworkPortEVB](#hpenetworkportevb-v1_0_0-hpenetworkportevb)

| | |
|---|---|
|Description|The header subtype field of the last received HPE Channel Description TLV.|
|Type|integer|
|Read Only|True|

**Receiving.ChannelLinkControlLocalSequenceNumber**
Member of [HpeNetworkPortEVB.v1_0_0.HpeNetworkPortEVB](#hpenetworkportevb-v1_0_0-hpenetworkportevb)

| | |
|---|---|
|Description|The link partner's HPE Channel Link Control sequence number that was last successfully received and processed.|
|Type|integer|
|Read Only|True|

**Receiving.ChannelLinkControlMCEnable**
Member of [HpeNetworkPortEVB.v1_0_0.HpeNetworkPortEVB](#hpenetworkportevb-v1_0_0-hpenetworkportevb)

| | |
|---|---|
|Description|The Feature Indicators field, Management Controller (MC) Channel (SCID 4094) enabled state in the HPE CLC TLV being received from the link partner on this port.|
|Type|boolean|
|Read Only|True|

**Receiving.ChannelLinkControlRemoteSequenceNumber**
Member of [HpeNetworkPortEVB.v1_0_0.HpeNetworkPortEVB](#hpenetworkportevb-v1_0_0-hpenetworkportevb)

| | |
|---|---|
|Description|The last HPE Channel Link control sequence number sent on this link that was successfully received and processed by the link partner.|
|Type|integer|
|Read Only|True|

**Receiving.ChannelLinkControlSubtype**
Member of [HpeNetworkPortEVB.v1_0_0.HpeNetworkPortEVB](#hpenetworkportevb-v1_0_0-hpenetworkportevb)

| | |
|---|---|
|Description|The header subtype field of the last received HPE Channel Link Control TLV.|
|Type|integer|
|Read Only|True|

**Receiving.Role**
Member of [HpeNetworkPortEVB.v1_0_0.HpeNetworkPortEVB](#hpenetworkportevb-v1_0_0-hpenetworkportevb)

| | |
|---|---|
|Description|The link partner's IEEE 802.1Qbg operating role.|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```bridge```|Indicates the link partner is operating as a Bridge.|
|```station```|Indicates the link partner is operating as a Station.|

**Receiving.SChannelAssignments (array)**
Member of [HpeNetworkPortEVB.v1_0_0.HpeNetworkPortEVB](#hpenetworkportevb-v1_0_0-hpenetworkportevb)
```SChannelAssignments``` is an array containing elements of:

**SChannelAssignments[{item}].Scid**
Member of [HpeNetworkPortEVB.v1_0_0.HpeNetworkPortEVB](#hpenetworkportevb-v1_0_0-hpenetworkportevb)

| | |
|---|---|
|Description|SCID value for this <SCID,SVID> S-Channel identifier pairreceived from the link partner on this port.|
|Type|integer|
|Read Only|True|

**SChannelAssignments[{item}].Svid**
Member of [HpeNetworkPortEVB.v1_0_0.HpeNetworkPortEVB](#hpenetworkportevb-v1_0_0-hpenetworkportevb)

| | |
|---|---|
|Description|SVID assignment value for this <SCID,SVID> S-Channel identifier pair received from the link partner on this port. When 0 it indicates an assignment request is in progress.|
|Type|integer|
|Read Only|True|

**Receiving.SChannelMaxCount**
Member of [HpeNetworkPortEVB.v1_0_0.HpeNetworkPortEVB](#hpenetworkportevb-v1_0_0-hpenetworkportevb)

| | |
|---|---|
|Description|Indicates the number of S-Channels the link partner can support on this physical link.|
|Type|integer|
|Read Only|True|

**Receiving.SChannelsSupported**
Member of [HpeNetworkPortEVB.v1_0_0.HpeNetworkPortEVB](#hpenetworkportevb-v1_0_0-hpenetworkportevb)

| | |
|---|---|
|Description|When true this link supports S-Channels.|
|Type|boolean|
|Read Only|True|

**Receiving.VirtualLinkStatusVector**
Member of [HpeNetworkPortEVB.v1_0_0.HpeNetworkPortEVB](#hpenetworkportevb-v1_0_0-hpenetworkportevb)

| | |
|---|---|
|Description|A bit vector indicating S-Channel status received from the link partner, 1=up, 0=down. S-Channel status bits are ordered by SCID from lowest numbered (first) to highest (last).|
|Type|string|
|Read Only|True|

### Transmitting
**Transmitting.ChannelDescriptionData (array)**
Member of [HpeNetworkPortEVB.v1_0_0.HpeNetworkPortEVB](#hpenetworkportevb-v1_0_0-hpenetworkportevb)
```ChannelDescriptionData``` is an array containing elements of:

**ChannelDescriptionData[{item}].Descriptor0BandwidthCirMbps**
Member of [HpeNetworkPortEVB.v1_0_0.HpeNetworkPortEVB](#hpenetworkportevb-v1_0_0-hpenetworkportevb)

| | |
|---|---|
|Description|The bandwidth Commited Information Rate (CIR) for this S-Channel, in Mbps.|
|Type|integer|
|Read Only|True|

**ChannelDescriptionData[{item}].Descriptor0BandwidthPirMbps**
Member of [HpeNetworkPortEVB.v1_0_0.HpeNetworkPortEVB](#hpenetworkportevb-v1_0_0-hpenetworkportevb)

| | |
|---|---|
|Description|The bandwidth Peak Information Rate (PIR) for this S-Channel, in Mbps.|
|Type|integer|
|Read Only|True|

**ChannelDescriptionData[{item}].Descriptor0ChannelTerminationType**
Member of [HpeNetworkPortEVB.v1_0_0.HpeNetworkPortEVB](#hpenetworkportevb-v1_0_0-hpenetworkportevb)

| | |
|---|---|
|Description|Indicates the termination provided for this S-Channel.|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```primary-physical```|This S-Channel is presented to the host OS as a primary PCI physical function.|
|```SR-IOV-virtual```|This S-Channel is presented to the host OS as a PCI SR-IOV virtual function.|
|```secondary-physical```|This S-Channel is presented to the host OS as a secondary PCI physical function, i.e. a PCI physical function behind a bridge on the device.|
|```vSwitch-port```|This S-Channel is mapped to a Virtual Switch port.|
|```NCSI-port```|This S-Channel is mapped to the NCSI internal port for management.|

**ChannelDescriptionData[{item}].Descriptor0EthernetSupport**
Member of [HpeNetworkPortEVB.v1_0_0.HpeNetworkPortEVB](#hpenetworkportevb-v1_0_0-hpenetworkportevb)

| | |
|---|---|
|Description|When true, this S-Channel supports Ethernet.|
|Type|boolean|
|Read Only|True|

**ChannelDescriptionData[{item}].Descriptor0FCoESupport**
Member of [HpeNetworkPortEVB.v1_0_0.HpeNetworkPortEVB](#hpenetworkportevb-v1_0_0-hpenetworkportevb)

| | |
|---|---|
|Description|When true, this S-Channel supports Fibre Channel over Ethernet (FCoE).|
|Type|boolean|
|Read Only|True|

**ChannelDescriptionData[{item}].Descriptor0PcpSupport**
Member of [HpeNetworkPortEVB.v1_0_0.HpeNetworkPortEVB](#hpenetworkportevb-v1_0_0-hpenetworkportevb)

| | |
|---|---|
|Description|Indicates which IEEE 802.1Q Ethernet Priority Code Point (PCP) classes are supported on this S-Channel. When no PCPs are supported, the S-Channel makes no attempt to filter or control traffic class. A string of 1/0 characters indicating 1=enabled, 0=disabled. PCP classes are ordered from highest numbered 7 (first) to lowest 0 (last).|
|Type|string|
|Read Only|True|

**ChannelDescriptionData[{item}].Descriptor0RoCEESupport**
Member of [HpeNetworkPortEVB.v1_0_0.HpeNetworkPortEVB](#hpenetworkportevb-v1_0_0-hpenetworkportevb)

| | |
|---|---|
|Description|When true, this S-Channel supports RDMA over Converged Enhanced Ethernet (RoCEE).|
|Type|boolean|
|Read Only|True|

**ChannelDescriptionData[{item}].Descriptor0Scid**
Member of [HpeNetworkPortEVB.v1_0_0.HpeNetworkPortEVB](#hpenetworkportevb-v1_0_0-hpenetworkportevb)

| | |
|---|---|
|Description|The S-Channel identifier for this Descriptor0 instance.|
|Type|integer|
|Read Only|True|

**ChannelDescriptionData[{item}].Descriptor0iSCSISupport**
Member of [HpeNetworkPortEVB.v1_0_0.HpeNetworkPortEVB](#hpenetworkportevb-v1_0_0-hpenetworkportevb)

| | |
|---|---|
|Description|When true, this S-Channel supports Internet SCSI (iSCSI).|
|Type|boolean|
|Read Only|True|

**ChannelDescriptionData[{item}].Descriptor1ConnectionID**
Member of [HpeNetworkPortEVB.v1_0_0.HpeNetworkPortEVB](#hpenetworkportevb-v1_0_0-hpenetworkportevb)

| | |
|---|---|
|Description|A unique S-Channel identifer in UUID format.|
|Type|string|
|Read Only|True|

**ChannelDescriptionData[{item}].Descriptor1Scid**
Member of [HpeNetworkPortEVB.v1_0_0.HpeNetworkPortEVB](#hpenetworkportevb-v1_0_0-hpenetworkportevb)

| | |
|---|---|
|Description|The S-Channel identifier for this Descriptor1 instance.|
|Type|integer|
|Read Only|True|

**Transmitting.ChannelDescriptionLocalSequenceNumber**
Member of [HpeNetworkPortEVB.v1_0_0.HpeNetworkPortEVB](#hpenetworkportevb-v1_0_0-hpenetworkportevb)

| | |
|---|---|
|Description|This station's channel discovery local sequence number which will be transmitted to the link partner on this port.|
|Type|integer|
|Read Only|True|

**Transmitting.ChannelDescriptionRemoteSequenceNumber**
Member of [HpeNetworkPortEVB.v1_0_0.HpeNetworkPortEVB](#hpenetworkportevb-v1_0_0-hpenetworkportevb)

| | |
|---|---|
|Description|The link partner's channel discovery local sequence number that was last successfully received and processed.|
|Type|integer|
|Read Only|True|

**Transmitting.ChannelDescriptorCount**
Member of [HpeNetworkPortEVB.v1_0_0.HpeNetworkPortEVB](#hpenetworkportevb-v1_0_0-hpenetworkportevb)

| | |
|---|---|
|Description|The number of channel descriptor pairs being transmitted to the link partner on this port.|
|Type|integer|
|Read Only|True|

**Transmitting.ChannelLinkControlLocalSequenceNumber**
Member of [HpeNetworkPortEVB.v1_0_0.HpeNetworkPortEVB](#hpenetworkportevb-v1_0_0-hpenetworkportevb)

| | |
|---|---|
|Description|This station's channel link control local sequence number which will be transmitted to the link partner on this port.|
|Type|integer|
|Read Only|True|

**Transmitting.ChannelLinkControlMCEnable**
Member of [HpeNetworkPortEVB.v1_0_0.HpeNetworkPortEVB](#hpenetworkportevb-v1_0_0-hpenetworkportevb)

| | |
|---|---|
|Description|The Feature Indicators field, Management Controller (MC) Channel (SCID 4094) enabled state in the HPE CLC TLV being transmitted to the link partner on this port.|
|Type|boolean|
|Read Only|True|

**Transmitting.ChannelLinkControlRemoteSequenceNumber**
Member of [HpeNetworkPortEVB.v1_0_0.HpeNetworkPortEVB](#hpenetworkportevb-v1_0_0-hpenetworkportevb)

| | |
|---|---|
|Description|The link partner's channel link control local sequence number that was last successfully received and processed.|
|Type|integer|
|Read Only|True|

**Transmitting.Role**
Member of [HpeNetworkPortEVB.v1_0_0.HpeNetworkPortEVB](#hpenetworkportevb-v1_0_0-hpenetworkportevb)

| | |
|---|---|
|Description|This port's IEEE 802.1Qbg role being advertised on the link.|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```bridge```|Indicates this link is operating locally as a Bridge.|
|```station```|Indicates this link is operating locally as a Station.|

**Transmitting.SChannelAssignments (array)**
Member of [HpeNetworkPortEVB.v1_0_0.HpeNetworkPortEVB](#hpenetworkportevb-v1_0_0-hpenetworkportevb)
```SChannelAssignments``` is an array containing elements of:

**SChannelAssignments[{item}].Scid**
Member of [HpeNetworkPortEVB.v1_0_0.HpeNetworkPortEVB](#hpenetworkportevb-v1_0_0-hpenetworkportevb)

| | |
|---|---|
|Description|SCID value for this <SCID,SVID> S-Channel identifier pair being transmitted to the link partner on this port.|
|Type|integer|
|Read Only|True|

**SChannelAssignments[{item}].Svid**
Member of [HpeNetworkPortEVB.v1_0_0.HpeNetworkPortEVB](#hpenetworkportevb-v1_0_0-hpenetworkportevb)

| | |
|---|---|
|Description|SVID assignment value for this <SCID,SVID> S-Channel identifier pair being transmitted to the link partner on this port. When 0 it indicates an SVID assignment request to the link partner is in progress.|
|Type|integer|
|Read Only|True|

**Transmitting.SChannelMaxCount**
Member of [HpeNetworkPortEVB.v1_0_0.HpeNetworkPortEVB](#hpenetworkportevb-v1_0_0-hpenetworkportevb)

| | |
|---|---|
|Description|The Channel Capacity value being advertised to the link partner. It indicates the number of S-Channels this station can support on this physical link.|
|Type|integer|
|Read Only|True|

**Transmitting.SChannelsSupported**
Member of [HpeNetworkPortEVB.v1_0_0.HpeNetworkPortEVB](#hpenetworkportevb-v1_0_0-hpenetworkportevb)

| | |
|---|---|
|Description|When true, indicates that this physical link has S-Channel capability.|
|Type|boolean|
|Read Only|True|

**Transmitting.VirtualLinkStatusVector**
Member of [HpeNetworkPortEVB.v1_0_0.HpeNetworkPortEVB](#hpenetworkportevb-v1_0_0-hpenetworkportevb)

| | |
|---|---|
|Description|A bit vector indicating S-Channel status being transmitted on this link, 1=up, 0=down. S-Channel status bits are ordered by SCID from lowest numbered (first) to highest (last).|
|Type|string|
|Read Only|True|

## HpeNetworkPortLLDP.v1_0_0.HpeNetworkPortLLDP
```@odata.type: "#HpeNetworkPortLLDP.v1_0_0.HpeNetworkPortLLDP"```

Hewlett Packard Enterprise property extensions for Network Ports Link Layer Discovery Protocol
### Resource Instances
|Uri|HTTP Allow|
|---|---|
|```/redfish/v1/chassis/{item}/networkadapters/{item}/networkports/{item}/hpelldp/```|GET |
|```/redfish/v1/systems/{item}/networkinterfaces/{item}/networkports/{item}/hpelldp/```|GET |

### Receiving
**Receiving.ChassisID**
Member of [HpeNetworkPortLLDP.v1_0_0.HpeNetworkPortLLDP](#hpenetworkportlldp-v1_0_0-hpenetworkportlldp)

| | |
|---|---|
|Description|The LLDP chassis ID received from the link partner.|
|Type|string|
|Read Only|True|

**Receiving.ChassisIDSubtype**
Member of [HpeNetworkPortLLDP.v1_0_0.HpeNetworkPortLLDP](#hpenetworkportlldp-v1_0_0-hpenetworkportlldp)

| | |
|---|---|
|Description|The IEEE 802.1AB-2009 chassis ID subtype received from the link partner.|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```chassisComp```|Chassis component, based in the value of entPhysicalAlias in IETF RFC 4133.|
|```ifAlias```|Interface alias, based on the ifAlias MIB object.|
|```portComp```|Port component, based in the value of entPhysicalAlias in IETF RFC 4133.|
|```mac-Addr```|MAC address, based on an agent detected unicast source address as defined in IEEE Std. 802.|
|```networkAddr```|Network address, based on an agent detected network address.|
|```ifName```|Interface name, based on the ifName MIB object.|
|```agent-ID```|Agent circuit ID, based on the agent-local identifier of the circuit as defined in RFC 3046.|
|```local-Assign```|Locally assigned, based on a alpha-numeric value locally assigned.|

**Receiving.Dcb**
**Receiving.Dcb.ApplicationPriorityReceived**
Member of [HpeNetworkPortLLDP.v1_0_0.HpeNetworkPortLLDP](#hpenetworkportlldp-v1_0_0-hpenetworkportlldp)

| | |
|---|---|
|Description|True when an unexpired Data Center Bridging (DCB) Application Priority Table TLV has been received.|
|Type|boolean|
|Read Only|True|

**Receiving.Dcb.ApplicationPriorityTable (array)**
Member of [HpeNetworkPortLLDP.v1_0_0.HpeNetworkPortLLDP](#hpenetworkportlldp-v1_0_0-hpenetworkportlldp)
```ApplicationPriorityTable``` is an array containing elements of:

**ApplicationPriorityTable[{item}].ApplicationPriority**
Member of [HpeNetworkPortLLDP.v1_0_0.HpeNetworkPortLLDP](#hpenetworkportlldp-v1_0_0-hpenetworkportlldp)

| | |
|---|---|
|Description|Indicates which priority level is assigned for this application protocol.|
|Type|integer|
|Read Only|True|

**ApplicationPriorityTable[{item}].ApplicationProtocol**
Member of [HpeNetworkPortLLDP.v1_0_0.HpeNetworkPortLLDP](#hpenetworkportlldp-v1_0_0-hpenetworkportlldp)

| | |
|---|---|
|Description|An integer value indicating application protocol identity, of the type described by DCBApplicationSelect.|
|Type|integer|
|Read Only|True|

**ApplicationPriorityTable[{item}].ApplicationSelect**
Member of [HpeNetworkPortLLDP.v1_0_0.HpeNetworkPortLLDP](#hpenetworkportlldp-v1_0_0-hpenetworkportlldp)

| | |
|---|---|
|Description|Indentifies the type of the DCBApplicationProtocol property.|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```reserved```|Reserved select value.|
|```default-Ethertype```|Default priority. Use when priority not otherwise specified.|
|```TCP-SCTP```|DCBApplicationProtocol value is a well known port over TCP or SCTP.|
|```UDP-DCCP```|DCBApplicationProtocol value is a well known port over UDP or DCCP.|
|```TCP-SCTP-UDP-DCCP```|DCBApplicationProtocol is a well known port over TCP, SCTP, SCTP, or DCCP.|

**Receiving.Dcb.Ets**
**Receiving.Dcb.Ets.BandwidthAssignmentTable (array)**
Member of [HpeNetworkPortLLDP.v1_0_0.HpeNetworkPortLLDP](#hpenetworkportlldp-v1_0_0-hpenetworkportlldp)
```BandwidthAssignmentTable``` is an array containing elements of:


| | |
|---|---|
|Description|One entry in the DCB ETS Traffic Class (TC) Bandwidth Assignment Table.|
|Type|integer|
|Read Only|True|

**Receiving.Dcb.Ets.CreditBasedShaper**
Member of [HpeNetworkPortLLDP.v1_0_0.HpeNetworkPortLLDP](#hpenetworkportlldp-v1_0_0-hpenetworkportlldp)

| | |
|---|---|
|Description|True if the link partner supports the Credit-based Shaper (CBS) transmmission selection algortithm.|
|Type|boolean|
|Read Only|True|

**Receiving.Dcb.Ets.MaximumTrafficClassCount**
Member of [HpeNetworkPortLLDP.v1_0_0.HpeNetworkPortLLDP](#hpenetworkportlldp-v1_0_0-hpenetworkportlldp)

| | |
|---|---|
|Description|The maximum number of traffic classes supported by the link partner.|
|Type|integer|
|Read Only|True|

**Receiving.Dcb.Ets.PriorityAssignmentTable (array)**
Member of [HpeNetworkPortLLDP.v1_0_0.HpeNetworkPortLLDP](#hpenetworkportlldp-v1_0_0-hpenetworkportlldp)
```PriorityAssignmentTable``` is an array containing elements of:


| | |
|---|---|
|Description|One entry in the DCB ETS Priority Assignment Table indicating this priority's Traffic Class assignment.|
|Type|integer|
|Read Only|True|

**Receiving.Dcb.Ets.TlvReceived**
Member of [HpeNetworkPortLLDP.v1_0_0.HpeNetworkPortLLDP](#hpenetworkportlldp-v1_0_0-hpenetworkportlldp)

| | |
|---|---|
|Description|True when an unexpired DCB Enhanced Transmission Selection (ETS) TLV has been received.|
|Type|boolean|
|Read Only|True|

**Receiving.Dcb.Ets.TrafficSelectionAlgorithmTable (array)**
Member of [HpeNetworkPortLLDP.v1_0_0.HpeNetworkPortLLDP](#hpenetworkportlldp-v1_0_0-hpenetworkportlldp)
```TrafficSelectionAlgorithmTable``` is an array containing elements of:


| | |
|---|---|
|Description|An assignment of a Traffic Selection Algorithm (TSA) to a traffic class.|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```strict```|Strict priority algorithm.|
|```CBS```|Credit-Based Shaper algorithm.|
|```ETS```|Enhanced Traffic Selection algorithm.|
|```vendor```|Vendor specific algorithm for use with DCB.|

**Receiving.Dcb.Ets.Willing**
Member of [HpeNetworkPortLLDP.v1_0_0.HpeNetworkPortLLDP](#hpenetworkportlldp-v1_0_0-hpenetworkportlldp)

| | |
|---|---|
|Description|True if the link partner is willing to accept ETS configurations.|
|Type|boolean|
|Read Only|True|

**Receiving.Dcb.LocalEqualRemote**
Member of [HpeNetworkPortLLDP.v1_0_0.HpeNetworkPortLLDP](#hpenetworkportlldp-v1_0_0-hpenetworkportlldp)

| | |
|---|---|
|Description|True when the transmitted and received contents match for both DCB ETS and PFC TLVs.|
|Type|boolean|
|Read Only|True|

**Receiving.Dcb.Pfc**
**Receiving.Dcb.Pfc.EnabledTrafficClasses**
Member of [HpeNetworkPortLLDP.v1_0_0.HpeNetworkPortLLDP](#hpenetworkportlldp-v1_0_0-hpenetworkportlldp)

| | |
|---|---|
|Description|A bit string indicating which priority levels have PFC enabled, 1=enabled. PFC levels are bit ordered from 7 (first) to 0 (last).|
|Type|string|
|Read Only|True|

**Receiving.Dcb.Pfc.MacSecurityBypassCapability**
Member of [HpeNetworkPortLLDP.v1_0_0.HpeNetworkPortLLDP](#hpenetworkportlldp-v1_0_0-hpenetworkportlldp)

| | |
|---|---|
|Description|True when the link partner has the ability to bypass MAC security in order to improve PFC responsiveness.|
|Type|boolean|
|Read Only|True|

**Receiving.Dcb.Pfc.MaximumTrafficClassCount**
Member of [HpeNetworkPortLLDP.v1_0_0.HpeNetworkPortLLDP](#hpenetworkportlldp-v1_0_0-hpenetworkportlldp)

| | |
|---|---|
|Description|Indicates the maximum number of traffic classes that the link partner can simultaneously support.|
|Type|integer|
|Read Only|True|

**Receiving.Dcb.Pfc.TlvReceived**
Member of [HpeNetworkPortLLDP.v1_0_0.HpeNetworkPortLLDP](#hpenetworkportlldp-v1_0_0-hpenetworkportlldp)

| | |
|---|---|
|Description|True when an unexpired DCB Priority Flow Control (PFC) TLV has been received.|
|Type|boolean|
|Read Only|True|

**Receiving.Dcb.Pfc.Willing**
Member of [HpeNetworkPortLLDP.v1_0_0.HpeNetworkPortLLDP](#hpenetworkportlldp-v1_0_0-hpenetworkportlldp)

| | |
|---|---|
|Description|True if the LLDP link partner is willing to accept PFC configurations.|
|Type|boolean|
|Read Only|True|

**Receiving.Dcb.Version**
Member of [HpeNetworkPortLLDP.v1_0_0.HpeNetworkPortLLDP](#hpenetworkportlldp-v1_0_0-hpenetworkportlldp)

| | |
|---|---|
|Description|The DCB version supported by the link partner.|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```unknown```|Unknown|
|```CEE```|Converged Enhanced Ethernet|
|```IEEE```|IEEE 802.1Q|

**Receiving.ManagementAddress**
Member of [HpeNetworkPortLLDP.v1_0_0.HpeNetworkPortLLDP](#hpenetworkportlldp-v1_0_0-hpenetworkportlldp)

| | |
|---|---|
|Description|The management address received from the link partner.|
|Type|string|
|Read Only|True|

**Receiving.ManagementAddressOID**
Member of [HpeNetworkPortLLDP.v1_0_0.HpeNetworkPortLLDP](#hpenetworkportlldp-v1_0_0-hpenetworkportlldp)

| | |
|---|---|
|Description|An object identifier for the hardware or protocol entity associated with the management address.|
|Type|string|
|Read Only|True|

**Receiving.ManagementAddressReceived**
Member of [HpeNetworkPortLLDP.v1_0_0.HpeNetworkPortLLDP](#hpenetworkportlldp-v1_0_0-hpenetworkportlldp)

| | |
|---|---|
|Description|True when a currently unexpired management address TLV has been received from the link partner.|
|Type|boolean|
|Read Only|True|

**Receiving.ManagementAddressType**
Member of [HpeNetworkPortLLDP.v1_0_0.HpeNetworkPortLLDP](#hpenetworkportlldp-v1_0_0-hpenetworkportlldp)

| | |
|---|---|
|Description|The type of management address received from the link partner.|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```IPv4```|Type 1 (IP version 4).|
|```IPv6```|Type 2 (IP version 6).|
|```all802```|Type 6 (All 802 media plus Ethernet 'canonical format').|

**Receiving.ManagementCvlanID**
Member of [HpeNetworkPortLLDP.v1_0_0.HpeNetworkPortLLDP](#hpenetworkportlldp-v1_0_0-hpenetworkportlldp)

| | |
|---|---|
|Description|The management CVLAN ID received from the link partner.|
|Type|integer|
|Read Only|True|

**Receiving.ManagementIFNumSubtype**
Member of [HpeNetworkPortLLDP.v1_0_0.HpeNetworkPortLLDP](#hpenetworkportlldp-v1_0_0-hpenetworkportlldp)

| | |
|---|---|
|Description|Management interface number subtype.|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```unknown```|Interface number is not known.|
|```ifIndex```|Interface number is based on the ifIndex MIB object.|
|```sysPortNum```|Interface number is based on the system port numbering convention.|

**Receiving.ManagementIFNumber**
Member of [HpeNetworkPortLLDP.v1_0_0.HpeNetworkPortLLDP](#hpenetworkportlldp-v1_0_0-hpenetworkportlldp)

| | |
|---|---|
|Description|Management interface number received from the link partner represented as a colon delimited string of hexadecimal octets.|
|Type|string|
|Read Only|True|

**Receiving.ManagementVlanReceived**
Member of [HpeNetworkPortLLDP.v1_0_0.HpeNetworkPortLLDP](#hpenetworkportlldp-v1_0_0-hpenetworkportlldp)

| | |
|---|---|
|Description|True when a currently unexpired management address VID TLV has been received from the link partner.|
|Type|boolean|
|Read Only|True|

**Receiving.NearestBridgeTtlExpired**
Member of [HpeNetworkPortLLDP.v1_0_0.HpeNetworkPortLLDP](#hpenetworkportlldp-v1_0_0-hpenetworkportlldp)

| | |
|---|---|
|Description|True when the LLDP PDU most recently received from the link partner has expired.|
|Type|boolean|
|Read Only|True|

**Receiving.PortDescription**
Member of [HpeNetworkPortLLDP.v1_0_0.HpeNetworkPortLLDP](#hpenetworkportlldp-v1_0_0-hpenetworkportlldp)

| | |
|---|---|
|Description|The remote link partner's port description.|
|Type|string|
|Read Only|True|

**Receiving.PortID**
Member of [HpeNetworkPortLLDP.v1_0_0.HpeNetworkPortLLDP](#hpenetworkportlldp-v1_0_0-hpenetworkportlldp)

| | |
|---|---|
|Description|A colon delimited string of hexadecimal octets received from the link partner identifying its port.|
|Type|string|
|Read Only|True|

**Receiving.PortIDSubtype**
Member of [HpeNetworkPortLLDP.v1_0_0.HpeNetworkPortLLDP](#hpenetworkportlldp-v1_0_0-hpenetworkportlldp)

| | |
|---|---|
|Description|The port ID subtype enumeration from IEEE 802.1AB-2009 Table 8-3, which indicates the format for the PortID property.|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```chassisComp```|Chassis component, based in the value of entPhysicalAlias in IETF RFC 4133.|
|```ifAlias```|Interface alias, based on the ifAlias MIB object.|
|```portComp```|Port component, based in the value of entPhysicalAlias in IETF RFC 4133.|
|```mac-Addr```|MAC address, based on an agent detected unicast source address as defined in IEEE Std. 802.|
|```networkAddr```|Network address, based on an agent detected network address.|
|```ifName```|Interface name, based on the ifName MIB object.|
|```agent-ID```|Agent circuit ID, based on the agent-local identifier of the circuit as defined in RFC 3046.|
|```local-Assign```|Locally assigned, based on a alpha-numeric value locally assigned.|

**Receiving.SystemDescription**
Member of [HpeNetworkPortLLDP.v1_0_0.HpeNetworkPortLLDP](#hpenetworkportlldp-v1_0_0-hpenetworkportlldp)

| | |
|---|---|
|Description|The system description received from the link partner.|
|Type|string|
|Read Only|True|

### Transmitting
**Transmitting.ChassisID**
Member of [HpeNetworkPortLLDP.v1_0_0.HpeNetworkPortLLDP](#hpenetworkportlldp-v1_0_0-hpenetworkportlldp)

| | |
|---|---|
|Description|The Link Layer Data Protocol (LLDP) chassis ID being transmitted on this link.|
|Type|string|
|Read Only|True|

**Transmitting.ChassisIDSubtype**
Member of [HpeNetworkPortLLDP.v1_0_0.HpeNetworkPortLLDP](#hpenetworkportlldp-v1_0_0-hpenetworkportlldp)

| | |
|---|---|
|Description|The IEEE 802.1AB-2009 chassis ID subtype being transmitted on this link.|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```chassisComp```|Chassis component, based in the value of entPhysicalAlias in IETF RFC 4133.|
|```ifAlias```|Interface alias, based on the ifAlias MIB object.|
|```portComp```|Port component, based in the value of entPhysicalAlias in IETF RFC 4133.|
|```mac-Addr```|MAC address, based on an agent detected unicast source address as defined in IEEE Std. 802.|
|```networkAddr```|Network address, based on an agent detected network address.|
|```ifName```|Interface name, based on the ifName MIB object.|
|```agent-ID```|Agent circuit ID, based on the agent-local identifier of the circuit as defined in RFC 3046.|
|```local-Assign```|Locally assigned, based on a alpha-numeric value locally assigned.|

**Transmitting.ManagementAddresses (array)**
Member of [HpeNetworkPortLLDP.v1_0_0.HpeNetworkPortLLDP](#hpenetworkportlldp-v1_0_0-hpenetworkportlldp)
```ManagementAddresses``` is an array containing elements of:

**ManagementAddresses[{item}].ManagementIPAddress**
Member of [HpeNetworkPortLLDP.v1_0_0.HpeNetworkPortLLDP](#hpenetworkportlldp-v1_0_0-hpenetworkportlldp)

| | |
|---|---|
|Description|A management address.|
|Type|string|
|Read Only|True|

**ManagementAddresses[{item}].ManagementIPAddressType**
Member of [HpeNetworkPortLLDP.v1_0_0.HpeNetworkPortLLDP](#hpenetworkportlldp-v1_0_0-hpenetworkportlldp)

| | |
|---|---|
|Description|The IANA type of this management address.|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```IPv4```|Type 1 (IP version 4).|
|```IPv6```|Type 2 (IP version 6).|
|```all802```|Type 6 (All 802 media plus Ethernet 'canonical format').|

**Transmitting.ManagementCvlanID**
Member of [HpeNetworkPortLLDP.v1_0_0.HpeNetworkPortLLDP](#hpenetworkportlldp-v1_0_0-hpenetworkportlldp)

| | |
|---|---|
|Description|The management CVLAN ID being transmitted on this link.|
|Type|integer|
|Read Only|True|

**Transmitting.ManagementCvlanIDTransmitted**
Member of [HpeNetworkPortLLDP.v1_0_0.HpeNetworkPortLLDP](#hpenetworkportlldp-v1_0_0-hpenetworkportlldp)

| | |
|---|---|
|Description|When true, indicates that a management CVLAN ID is being transmitted on this link.|
|Type|boolean|
|Read Only|True|

**Transmitting.PortDescription**
Member of [HpeNetworkPortLLDP.v1_0_0.HpeNetworkPortLLDP](#hpenetworkportlldp-v1_0_0-hpenetworkportlldp)

| | |
|---|---|
|Description|An alphanumeric string describing this link.|
|Type|string|
|Read Only|True|

**Transmitting.PortID**
Member of [HpeNetworkPortLLDP.v1_0_0.HpeNetworkPortLLDP](#hpenetworkportlldp-v1_0_0-hpenetworkportlldp)

| | |
|---|---|
|Description|A colon delimited string of hexadecimal octets identifying this port.|
|Type|string|
|Read Only|True|

**Transmitting.PortIDSubtype**
Member of [HpeNetworkPortLLDP.v1_0_0.HpeNetworkPortLLDP](#hpenetworkportlldp-v1_0_0-hpenetworkportlldp)

| | |
|---|---|
|Description|The port ID subtype from IEEE 802.1AB-2009 Table 8-3.|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```chassisComp```|Chassis component, based in the value of entPhysicalAlias in IETF RFC 4133.|
|```ifAlias```|Interface alias, based on the ifAlias MIB object.|
|```portComp```|Port component, based in the value of entPhysicalAlias in IETF RFC 4133.|
|```mac-Addr```|MAC address, based on an agent detected unicast source address as defined in IEEE Std. 802.|
|```networkAddr```|Network address, based on an agent detected network address.|
|```ifName```|Interface name, based on the ifName MIB object.|
|```agent-ID```|Agent circuit ID, based on the agent-local identifier of the circuit as defined in RFC 3046.|
|```local-Assign```|Locally assigned, based on a alpha-numeric value locally assigned.|

**Transmitting.SystemDescription**
Member of [HpeNetworkPortLLDP.v1_0_0.HpeNetworkPortLLDP](#hpenetworkportlldp-v1_0_0-hpenetworkportlldp)

| | |
|---|---|
|Description|A textual description of this system.|
|Type|string|
|Read Only|True|

## HpePowerMeter.v2_0_0.HpePowerMeter
```@odata.type: "#HpePowerMeter.v2_0_0.HpePowerMeter"```
### Resource Instances
|Uri|HTTP Allow|
|---|---|
|```/redfish/v1/chassis/{item}/power/fastpowermeter/```|GET |
|```/redfish/v1/chassis/{item}/power/powermeter/```|GET |

### Average
Member of [HpePowerMeter.v2_0_0.HpePowerMeter](#hpepowermeter-v2_0_0-hpepowermeter)

| | |
|---|---|
|Description|Average power across all samples, over the last 24 hours.|
|Type|integer|
|Read Only|True|

### Maximum
Member of [HpePowerMeter.v2_0_0.HpePowerMeter](#hpepowermeter-v2_0_0-hpepowermeter)

| | |
|---|---|
|Description|Maximum power across all samples, taken from the 24 hour history.|
|Type|integer|
|Read Only|True|

### Minimum
Member of [HpePowerMeter.v2_0_0.HpePowerMeter](#hpepowermeter-v2_0_0-hpepowermeter)

| | |
|---|---|
|Description|Minimum power across all samples, taken from the 24 hour history.|
|Type|integer|
|Read Only|True|

### PowerDetail (array)
Member of [HpePowerMeter.v2_0_0.HpePowerMeter](#hpepowermeter-v2_0_0-hpepowermeter)
```PowerDetail``` is an array containing elements of:

**PowerDetail[{item}].AmbTemp**
Member of [HpePowerMeter.v2_0_0.HpePowerMeter](#hpepowermeter-v2_0_0-hpepowermeter)

| | |
|---|---|
|Description|Ambient temperature, in degrees Celsius.|
|Type|integer|
|Read Only|True|

**PowerDetail[{item}].Average**
Member of [HpePowerMeter.v2_0_0.HpePowerMeter](#hpepowermeter-v2_0_0-hpepowermeter)

| | |
|---|---|
|Description|Average power over the sample time.|
|Type|integer|
|Read Only|True|

**PowerDetail[{item}].Cap**
Member of [HpePowerMeter.v2_0_0.HpePowerMeter](#hpepowermeter-v2_0_0-hpepowermeter)

| | |
|---|---|
|Description|Overall power cap for the power meter.|
|Type|integer|
|Read Only|True|

**PowerDetail[{item}].CpuAvgFreq**
Member of [HpePowerMeter.v2_0_0.HpePowerMeter](#hpepowermeter-v2_0_0-hpepowermeter)

| | |
|---|---|
|Description|CPU average frequency of the power supply.|
|Type|integer|
|Read Only|True|

**PowerDetail[{item}].CpuCapLim**
Member of [HpePowerMeter.v2_0_0.HpePowerMeter](#hpepowermeter-v2_0_0-hpepowermeter)

| | |
|---|---|
|Description|CPU cap limit for the power meter.|
|Type|integer|
|Read Only|True|

**PowerDetail[{item}].CpuMax**
Member of [HpePowerMeter.v2_0_0.HpePowerMeter](#hpepowermeter-v2_0_0-hpepowermeter)

| | |
|---|---|
|Description|CPU maximum power consumed by the power meter.|
|Type|integer|
|Read Only|True|

**PowerDetail[{item}].CpuPwrSavLim**
Member of [HpePowerMeter.v2_0_0.HpePowerMeter](#hpepowermeter-v2_0_0-hpepowermeter)

| | |
|---|---|
|Description|CPU power-saving limit for the power meter.|
|Type|integer|
|Read Only|True|

**PowerDetail[{item}].CpuUtil**
Member of [HpePowerMeter.v2_0_0.HpePowerMeter](#hpepowermeter-v2_0_0-hpepowermeter)

| | |
|---|---|
|Description|CPU power utilization.|
|Type|integer|
|Read Only|True|

**PowerDetail[{item}].Minimum**
Member of [HpePowerMeter.v2_0_0.HpePowerMeter](#hpepowermeter-v2_0_0-hpepowermeter)

| | |
|---|---|
|Description|Minimum power over the sample time.|
|Type|integer|
|Read Only|True|

**PowerDetail[{item}].Peak**
Member of [HpePowerMeter.v2_0_0.HpePowerMeter](#hpepowermeter-v2_0_0-hpepowermeter)

| | |
|---|---|
|Description|Peak power over the sample time.|
|Type|integer|
|Read Only|True|

**PowerDetail[{item}].PrMode**
Member of [HpePowerMeter.v2_0_0.HpePowerMeter](#hpepowermeter-v2_0_0-hpepowermeter)

| | |
|---|---|
|Description|Power regulator mode, which can be OS Control, Static High, Static Low or Dynamic.|
|Type|string or null|
|Read Only|True|

The following are the supported values:

|Value|
|---|
|```Null```|
|```dyn```|
|```min```|
|```max```|
|```osc```|

**PowerDetail[{item}].PunCap**
Member of [HpePowerMeter.v2_0_0.HpePowerMeter](#hpepowermeter-v2_0_0-hpepowermeter)

| | |
|---|---|
|Description|Punitive cap for the power meter.|
|Type|boolean|
|Read Only|True|

**PowerDetail[{item}].Time**
Member of [HpePowerMeter.v2_0_0.HpePowerMeter](#hpepowermeter-v2_0_0-hpepowermeter)

| | |
|---|---|
|Description|Time at which the power detail was captured.|
|Type|string|
|Read Only|True|

**PowerDetail[{item}].UnachCap**
Member of [HpePowerMeter.v2_0_0.HpePowerMeter](#hpepowermeter-v2_0_0-hpepowermeter)

| | |
|---|---|
|Description|Unachievable cap for the power meter.|
|Type|boolean|
|Read Only|True|

### Samples
Member of [HpePowerMeter.v2_0_0.HpePowerMeter](#hpepowermeter-v2_0_0-hpepowermeter)

| | |
|---|---|
|Description|Number of samples in the array.|
|Type|integer|
|Read Only|True|

## HpeRemoteSupport.v2_2_0.HpeRemoteSupport
```@odata.type: "#HpeRemoteSupport.v2_2_0.HpeRemoteSupport"```

This resource type was added in iLO 5 1.20

HpeRemoteSupport enables management of HPE Remote Support configuration on iLO 5.

### Resource Instances
|Uri|HTTP Allow|
|---|---|
|```/redfish/v1/managers/{item}/remotesupportservice/```|GET POST PATCH |

### Links to other Resources
|Link Name|Destination type
|---|---|
|```ServiceEventLogs```|Collection of [LogEntry](#logentry-v1_0_0-logentry)|

### ConnectModel
Member of [HpeRemoteSupport.v2_2_0.HpeRemoteSupport](#hperemotesupport-v2_2_0-hperemotesupport)

| | |
|---|---|
|Description|The Remote Support connect model type.|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|
|---|
|```DirectConnect```|
|```CentralConnect```|

### DataCollectionFrequencyInDays
Member of [HpeRemoteSupport.v2_2_0.HpeRemoteSupport](#hperemotesupport-v2_2_0-hperemotesupport)

| | |
|---|---|
|Description|The frequency of data collection in days. This is applicable only when the server is registered using Direct Connect.|
|Type|integer|
|Read Only|True|

### DestinationPort
Member of [HpeRemoteSupport.v2_2_0.HpeRemoteSupport](#hperemotesupport-v2_2_0-hperemotesupport)

| | |
|---|---|
|Description|The port number of the Insight Remote Support server. This is applicable for Central Connect only. |
|Type|integer|
|Read Only|True|

### DestinationURL
Member of [HpeRemoteSupport.v2_2_0.HpeRemoteSupport](#hperemotesupport-v2_2_0-hperemotesupport)

| | |
|---|---|
|Description|The host name or IP address of the Remote Support server. This is applicable for Central Connect only.|
|Type|string|
|Read Only|True|

### HpePassportPassword
Member of [HpeRemoteSupport.v2_2_0.HpeRemoteSupport](#hperemotesupport-v2_2_0-hperemotesupport)

| | |
|---|---|
|Description|HPE Passport Account Password.|
|Type|string or null|
|Read Only|True|

### HpePassportUserId
Member of [HpeRemoteSupport.v2_2_0.HpeRemoteSupport](#hperemotesupport-v2_2_0-hperemotesupport)

| | |
|---|---|
|Description|HPE Passport Account Id.|
|Type|string|
|Read Only|True|

### LastTransmissionDate
Member of [HpeRemoteSupport.v2_2_0.HpeRemoteSupport](#hperemotesupport-v2_2_0-hperemotesupport)

| | |
|---|---|
|Description|The last transmission date.|
|Type|string|
|Read Only|True|

### LastTransmissionError
Member of [HpeRemoteSupport.v2_2_0.HpeRemoteSupport](#hperemotesupport-v2_2_0-hperemotesupport)

| | |
|---|---|
|Description|The last transmission error.|
|Type|string|
|Read Only|True|

### LastTransmissionType
Member of [HpeRemoteSupport.v2_2_0.HpeRemoteSupport](#hperemotesupport-v2_2_0-hperemotesupport)

| | |
|---|---|
|Description|The last transmission type. |
|Type|string or null|
|Read Only|True|

The following are the supported values:

|Value|
|---|
|```ActiveHealthSystemData```|
|```L2DataCollection```|
|```Registration```|
|```Deregistration```|
|```ServiceEvent```|
|```NoTransmission```|
|```Null```|

### ProxySettings
**ProxySettings.Password**
Member of [HpeRemoteSupport.v2_2_0.HpeRemoteSupport](#hperemotesupport-v2_2_0-hperemotesupport)

| | |
|---|---|
|Description|Password for web proxy server authentication. |
|Type|string or null|
|Read Only|False|

**ProxySettings.Port**
Member of [HpeRemoteSupport.v2_2_0.HpeRemoteSupport](#hperemotesupport-v2_2_0-hperemotesupport)

| | |
|---|---|
|Description|Port number on which to communicate with the web proxy server. |
|Type|integer or null|
|Read Only|False|

**ProxySettings.Url**
Member of [HpeRemoteSupport.v2_2_0.HpeRemoteSupport](#hperemotesupport-v2_2_0-hperemotesupport)

| | |
|---|---|
|Description|Web proxy server host name or IP address.|
|Type|string|
|Read Only|False|

**ProxySettings.Username**
Member of [HpeRemoteSupport.v2_2_0.HpeRemoteSupport](#hperemotesupport-v2_2_0-hperemotesupport)

| | |
|---|---|
|Description|Username for web proxy server authentication. |
|Type|string or null|
|Read Only|False|

### RemoteSupportEnabled
Member of [HpeRemoteSupport.v2_2_0.HpeRemoteSupport](#hperemotesupport-v2_2_0-hperemotesupport)

| | |
|---|---|
|Description|This indicates if the Remote Support Service is available or not. |
|Type|boolean|
|Read Only|True|

### ServiceEventLogs
A reference to the collection of service event logs.
### Actions

**HpeRemoteSupport.RegisterDeviceToRemoteSupport**
Member of [HpeRemoteSupport.v2_2_0.HpeRemoteSupport](#hperemotesupport-v2_2_0-hperemotesupport)

**Parameters:**

**WebProxyUrl (string)**

Web proxy server host name or IP address when connecting using Direct Connect. 

**DestinationUrl (string)**

The host name or IP address of the Remote Support server. This is applicable for Central Connect only.
## HpeSecurityService.v2_2_0.HpeSecurityService
```@odata.type: "#HpeSecurityService.v2_2_0.HpeSecurityService"```
### Resource Instances
|Uri|HTTP Allow|
|---|---|
|```/redfish/v1/managers/{item}/securityservice/```|GET PATCH |

### Links to other Resources
|Link Name|Destination type
|---|---|
|```Links/CertAuth```|[HpeCertAuth](#hpecertauth-v1_1_0-hpecertauth)|
|```Links/SSO```|[HpeiLOSSO](#hpeilosso-v2_0_0-hpeilosso)|
|```Links/ESKM```|[HpeESKM](#hpeeskm-v2_0_0-hpeeskm)|
|```Links/HttpsCert```|[HpeHttpsCert](#hpehttpscert-v2_0_0-hpehttpscert)|

### CurrentCipher
Member of [HpeSecurityService.v2_2_0.HpeSecurityService](#hpesecurityservice-v2_2_0-hpesecurityservice)

| | |
|---|---|
|Description|Current cipher in use.|
|Type|string|
|Read Only|True|

### LoginSecurityBanner
**LoginSecurityBanner.IsEnabled**
Member of [HpeSecurityService.v2_2_0.HpeSecurityService](#hpesecurityservice-v2_2_0-hpesecurityservice)

| | |
|---|---|
|Description|Login security banner is enabled or not.|
|Type|boolean|
|Read Only|False|

**LoginSecurityBanner.SecurityMessage**
Member of [HpeSecurityService.v2_2_0.HpeSecurityService](#hpesecurityservice-v2_2_0-hpesecurityservice)

| | |
|---|---|
|Description|Text message to appear on the iLO login page when login security banner is enabled.|
|Type|string|
|Read Only|False|

### SecurityState
Member of [HpeSecurityService.v2_2_0.HpeSecurityService](#hpesecurityservice-v2_2_0-hpesecurityservice)

| | |
|---|---|
|Description|The operational security level of this Manager.|
|Type|string|
|Read Only|False|

The following are the supported values:

|Value|Description|
|---|---|
|```Wipe```|Manager is currently wiping security related content and returning to a lower security mode.  This state will transition automatically when finished.|
|```Production```|Manager is operating in a normal security mode.  Default state for new systems.|
|```HighSecurity```|Manager is operating in high security mode, requiring extra authentication on host interface(s), and stronger encryption on network interfaces.|
|```FIPS```|Similar to High Security. This mode is intended to meet the FIPS 140-2 level 1 and Common Criteria security requirements. A reset to defaults is required to exit this mode.|
|```CNSA```|Same as FIPS. Additionally meets the criteria for NSA Commercial National Security Algorithm suite.  Must be in FIPS mode to transition to CNSA.|
|```SuiteB```|Same as FIPS. Additionally meets the criteria for NSA SuiteB Top Secret installations.  Must be in FIPS mode to transition to SuiteB.|

### SecurityState@Redfish.AllowableValues (array)
Member of [HpeSecurityService.v2_2_0.HpeSecurityService](#hpesecurityservice-v2_2_0-hpesecurityservice)
```SecurityState@Redfish.AllowableValues``` is an array containing elements of:


| | |
|---|---|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|
|---|
|```Wipe```|
|```Production```|
|```HighSecurity```|
|```FIPS```|
|```CNSA```|
|```SuiteB```|

### SecurityState_A_Redfish.AllowableValues (array)
Member of [HpeSecurityService.v2_2_0.HpeSecurityService](#hpesecurityservice-v2_2_0-hpesecurityservice)
```SecurityState_A_Redfish.AllowableValues``` is an array containing elements of:


| | |
|---|---|
|Description|The operational security level of this Manager.|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```Wipe```|Manager is currently wiping security related content and returning to a lower security mode.  This state will transition automatically when finished.|
|```Production```|Manager is operating in a security mode.  Default state for customer systems.|
|```HighSecurity```|Manager is operating in high security mode, requiring extra authentication on host interface(s), and stronger encryption on network interfaces.|
|```FIPS```|Same as High Security. This mode is intended to meet the FIPS 140-2 level 1 and Common Criteria security requirements. A reset to defaults is required to exit this mode.|
|```CNSA```|Same as FIPS. Additionally meets the criteria for NSA Commercial National Security Algorithm suite.  Must be in FIPS mode to transition to CNSA.|
|```SuiteB```|Same as FIPS. Additionally meets the criteria for NSA SuiteB Top Secret installations.  Must be in FIPS mode to transition to SuiteB.|

## HpeServerAccHddService.v1_0_0.HpeServerAccHddService
```@odata.type: "#HpeServerAccHddService.v1_0_0.HpeServerAccHddService"```

This resource type was added in iLO 5 1.20 and is available on **HPE ProLiant Apollo XL** systems.

### Resource Instances
|Uri|HTTP Allow|
|---|---|
|```/redfish/v1/chassis/{item}/acchddservice/```|GET |

### BackplaneInfo
**BackplaneInfo.EndBay**
Member of [HpeServerAccHddService.v1_0_0.HpeServerAccHddService](#hpeserveracchddservice-v1_0_0-hpeserveracchddservice)

| | |
|---|---|
|Description|Represents a ending number of the bay.|
|Type|integer|
|Read Only|True|

**BackplaneInfo.FirmwareRevision**
Member of [HpeServerAccHddService.v1_0_0.HpeServerAccHddService](#hpeserveracchddservice-v1_0_0-hpeserveracchddservice)

| | |
|---|---|
|Description|Indicates the firmware revision in ASCII value.|
|Type|string|
|Read Only|True|

**BackplaneInfo.HostPortsInfo (array)**
Member of [HpeServerAccHddService.v1_0_0.HpeServerAccHddService](#hpeserveracchddservice-v1_0_0-hpeserveracchddservice)
```HostPortsInfo``` is an array containing elements of:

**HostPortsInfo[{item}].NodeNumber**
Member of [HpeServerAccHddService.v1_0_0.HpeServerAccHddService](#hpeserveracchddservice-v1_0_0-hpeserveracchddservice)

| | |
|---|---|
|Description|Represents the node number of compute node attached to host port x in SEP.|
|Type|integer|
|Read Only|True|

**HostPortsInfo[{item}].PortNumber**
Member of [HpeServerAccHddService.v1_0_0.HpeServerAccHddService](#hpeserveracchddservice-v1_0_0-hpeserveracchddservice)

| | |
|---|---|
|Description|Represents the number of physical host ports in SEP.|
|Type|integer|
|Read Only|True|

**HostPortsInfo[{item}].SlotNumber**
Member of [HpeServerAccHddService.v1_0_0.HpeServerAccHddService](#hpeserveracchddservice-v1_0_0-hpeserveracchddservice)

| | |
|---|---|
|Description|Represents the slot number of SAS attached to host port x in SEP.|
|Type|integer|
|Read Only|True|

**BackplaneInfo.SEPID**
Member of [HpeServerAccHddService.v1_0_0.HpeServerAccHddService](#hpeserveracchddservice-v1_0_0-hpeserveracchddservice)

| | |
|---|---|
|Description|Indicates the storage enclosure processor ID.|
|Type|integer|
|Read Only|True|

**BackplaneInfo.SEPNodeId**
Member of [HpeServerAccHddService.v1_0_0.HpeServerAccHddService](#hpeserveracchddservice-v1_0_0-hpeserveracchddservice)

| | |
|---|---|
|Description|The node ID represent the node ID where the storage enclosure processor is residing.|
|Type|integer|
|Read Only|True|

**BackplaneInfo.StartBay**
Member of [HpeServerAccHddService.v1_0_0.HpeServerAccHddService](#hpeserveracchddservice-v1_0_0-hpeserveracchddservice)

| | |
|---|---|
|Description|Represents a starting number of the bay.|
|Type|integer|
|Read Only|True|

**BackplaneInfo.TotalBays**
Member of [HpeServerAccHddService.v1_0_0.HpeServerAccHddService](#hpeserveracchddservice-v1_0_0-hpeserveracchddservice)

| | |
|---|---|
|Description|Total bay count represents the number of bays attached to the SEP.|
|Type|integer|
|Read Only|True|

**BackplaneInfo.TypeID**
Member of [HpeServerAccHddService.v1_0_0.HpeServerAccHddService](#hpeserveracchddservice-v1_0_0-hpeserveracchddservice)

| | |
|---|---|
|Description|Indicates the Backplane type ID for the identifier for backplane type.|
|Type|integer|
|Read Only|True|

**BackplaneInfo.WWID**
Member of [HpeServerAccHddService.v1_0_0.HpeServerAccHddService](#hpeserveracchddservice-v1_0_0-hpeserveracchddservice)

| | |
|---|---|
|Description|Represents a unique world wide ID defining a SEP.|
|Type|string|
|Read Only|True|

## HpeServerAccHddZone.v1_0_0.HpeServerAccHddZone
```@odata.type: "#HpeServerAccHddZone.v1_0_0.HpeServerAccHddZone"```

This resource type was added in iLO 5 1.20 and is available on **HPE ProLiant Apollo XL** systems.

### Resource Instances
|Uri|HTTP Allow|
|---|---|
|```/redfish/v1/chassis/{item}/acchddservice/zone/```|GET POST |

### CurrentZoneConfiguration
**CurrentZoneConfiguration.HostPort (array)**
Member of [HpeServerAccHddZone.v1_0_0.HpeServerAccHddZone](#hpeserveracchddzone-v1_0_0-hpeserveracchddzone)
```HostPort``` is an array containing elements of:

**HostPort[{item}].BayNumber (array)**
Member of [HpeServerAccHddZone.v1_0_0.HpeServerAccHddZone](#hpeserveracchddzone-v1_0_0-hpeserveracchddzone)
```BayNumber``` is an array containing elements of:


| | |
|---|---|
|Type|integer|
|Read Only|True|

**HostPort[{item}].PortNumber**
Member of [HpeServerAccHddZone.v1_0_0.HpeServerAccHddZone](#hpeserveracchddzone-v1_0_0-hpeserveracchddzone)

| | |
|---|---|
|Description|Represents the number of physical host ports in SEP, null represents unassigned bay group.|
|Type|integer or null|
|Read Only|True|

### PendingZoneConfiguration
**PendingZoneConfiguration.HostPort (array)**
Member of [HpeServerAccHddZone.v1_0_0.HpeServerAccHddZone](#hpeserveracchddzone-v1_0_0-hpeserveracchddzone)
```HostPort``` is an array containing elements of:

**HostPort[{item}].BayNumber (array)**
Member of [HpeServerAccHddZone.v1_0_0.HpeServerAccHddZone](#hpeserveracchddzone-v1_0_0-hpeserveracchddzone)
```BayNumber``` is an array containing elements of:


| | |
|---|---|
|Type|integer|
|Read Only|True|

**HostPort[{item}].PortNumber**
Member of [HpeServerAccHddZone.v1_0_0.HpeServerAccHddZone](#hpeserveracchddzone-v1_0_0-hpeserveracchddzone)

| | |
|---|---|
|Description|Represents the number of physical host ports in SEP, null represents unassigned bay group.|
|Type|integer or null|
|Read Only|True|

### SEPNodeId
Member of [HpeServerAccHddZone.v1_0_0.HpeServerAccHddZone](#hpeserveracchddzone-v1_0_0-hpeserveracchddzone)

| | |
|---|---|
|Description|The node ID represent the node ID where the storage enclosure processor is residing.|
|Type|integer|
|Read Only|True|

### TypeID
Member of [HpeServerAccHddZone.v1_0_0.HpeServerAccHddZone](#hpeserveracchddzone-v1_0_0-hpeserveracchddzone)

| | |
|---|---|
|Description|Indicates the Backplane type ID for the identifier for backplane type.|
|Type|integer|
|Read Only|True|

### Actions

**HpeServerAccHddZone.LoadDefault**
Member of [HpeServerAccHddZone.v1_0_0.HpeServerAccHddZone](#hpeserveracchddzone-v1_0_0-hpeserveracchddzone)
Load Apollo Chassis Controller default Hdd zone configuration.

There are no parameters for this action.

**HpeServerAccHddZone.ConfigureZone**
Member of [HpeServerAccHddZone.v1_0_0.HpeServerAccHddZone](#hpeserveracchddzone-v1_0_0-hpeserveracchddzone)
Execute Apollo Chassis Controller Hdd zone configuration.


**Parameters:**

**HostPort (array)**
## HpeServerAccPowerCalibration.v1_0_0.HpeServerAccPowerCalibration
```@odata.type: "#HpeServerAccPowerCalibration.v1_0_0.HpeServerAccPowerCalibration"```

This resource type was added in iLO 5 1.20 and is available on **HPE ProLiant Apollo XL** systems.

### Resource Instances
|Uri|HTTP Allow|
|---|---|
|```/redfish/v1/chassis/{item}/Power/accpowerservice/calibration/```|GET POST |

### CalibrationData
**CalibrationData.EndTime**
Member of [HpeServerAccPowerCalibration.v1_0_0.HpeServerAccPowerCalibration](#hpeserveraccpowercalibration-v1_0_0-hpeserveraccpowercalibration)

| | |
|---|---|
|Description|The calibration end time stamp.|
|Type|string|
|Read Only|True|

**CalibrationData.StartTime**
Member of [HpeServerAccPowerCalibration.v1_0_0.HpeServerAccPowerCalibration](#hpeserveraccpowercalibration-v1_0_0-hpeserveraccpowercalibration)

| | |
|---|---|
|Description|The calibration start time stamp.|
|Type|string|
|Read Only|True|

**CalibrationData.State**
Member of [HpeServerAccPowerCalibration.v1_0_0.HpeServerAccPowerCalibration](#hpeserveraccpowercalibration-v1_0_0-hpeserveraccpowercalibration)

| | |
|---|---|
|Description|Specifies whether the calibration is valid or not.|
|Type|boolean|
|Read Only|True|

**CalibrationData.ThrottlePeakPower**
**CalibrationData.ThrottlePeakPower.Percent_000**
Member of [HpeServerAccPowerCalibration.v1_0_0.HpeServerAccPowerCalibration](#hpeserveraccpowercalibration-v1_0_0-hpeserveraccpowercalibration)

| | |
|---|---|
|Description|The peak power of 0 Percent throttling.|
|Type|integer|
|Read Only|True|

**CalibrationData.ThrottlePeakPower.Percent_005**
Member of [HpeServerAccPowerCalibration.v1_0_0.HpeServerAccPowerCalibration](#hpeserveraccpowercalibration-v1_0_0-hpeserveraccpowercalibration)

| | |
|---|---|
|Description|The peak power of 5 Percent throttling.|
|Type|integer|
|Read Only|True|

**CalibrationData.ThrottlePeakPower.Percent_010**
Member of [HpeServerAccPowerCalibration.v1_0_0.HpeServerAccPowerCalibration](#hpeserveraccpowercalibration-v1_0_0-hpeserveraccpowercalibration)

| | |
|---|---|
|Description|The peak power of 10 Percent throttling.|
|Type|integer|
|Read Only|True|

**CalibrationData.ThrottlePeakPower.Percent_015**
Member of [HpeServerAccPowerCalibration.v1_0_0.HpeServerAccPowerCalibration](#hpeserveraccpowercalibration-v1_0_0-hpeserveraccpowercalibration)

| | |
|---|---|
|Description|The peak power of 15 Percent throttling.|
|Type|integer|
|Read Only|True|

**CalibrationData.ThrottlePeakPower.Percent_020**
Member of [HpeServerAccPowerCalibration.v1_0_0.HpeServerAccPowerCalibration](#hpeserveraccpowercalibration-v1_0_0-hpeserveraccpowercalibration)

| | |
|---|---|
|Description|The peak power of 20 Percent throttling.|
|Type|integer|
|Read Only|True|

**CalibrationData.ThrottlePeakPower.Percent_025**
Member of [HpeServerAccPowerCalibration.v1_0_0.HpeServerAccPowerCalibration](#hpeserveraccpowercalibration-v1_0_0-hpeserveraccpowercalibration)

| | |
|---|---|
|Description|The peak power of 25 Percent throttling.|
|Type|integer|
|Read Only|True|

**CalibrationData.ThrottlePeakPower.Percent_030**
Member of [HpeServerAccPowerCalibration.v1_0_0.HpeServerAccPowerCalibration](#hpeserveraccpowercalibration-v1_0_0-hpeserveraccpowercalibration)

| | |
|---|---|
|Description|The peak power of 30 Percent throttling.|
|Type|integer|
|Read Only|True|

**CalibrationData.ThrottlePeakPower.Percent_035**
Member of [HpeServerAccPowerCalibration.v1_0_0.HpeServerAccPowerCalibration](#hpeserveraccpowercalibration-v1_0_0-hpeserveraccpowercalibration)

| | |
|---|---|
|Description|The peak power of 35 Percent throttling.|
|Type|integer|
|Read Only|True|

**CalibrationData.ThrottlePeakPower.Percent_040**
Member of [HpeServerAccPowerCalibration.v1_0_0.HpeServerAccPowerCalibration](#hpeserveraccpowercalibration-v1_0_0-hpeserveraccpowercalibration)

| | |
|---|---|
|Description|The peak power of 40 Percent throttling.|
|Type|integer|
|Read Only|True|

**CalibrationData.ThrottlePeakPower.Percent_045**
Member of [HpeServerAccPowerCalibration.v1_0_0.HpeServerAccPowerCalibration](#hpeserveraccpowercalibration-v1_0_0-hpeserveraccpowercalibration)

| | |
|---|---|
|Description|The peak power of 45 Percent throttling.|
|Type|integer|
|Read Only|True|

**CalibrationData.ThrottlePeakPower.Percent_050**
Member of [HpeServerAccPowerCalibration.v1_0_0.HpeServerAccPowerCalibration](#hpeserveraccpowercalibration-v1_0_0-hpeserveraccpowercalibration)

| | |
|---|---|
|Description|The peak power of 50 Percent throttling.|
|Type|integer|
|Read Only|True|

**CalibrationData.ThrottlePeakPower.Percent_055**
Member of [HpeServerAccPowerCalibration.v1_0_0.HpeServerAccPowerCalibration](#hpeserveraccpowercalibration-v1_0_0-hpeserveraccpowercalibration)

| | |
|---|---|
|Description|The peak power of 55 Percent throttling.|
|Type|integer|
|Read Only|True|

**CalibrationData.ThrottlePeakPower.Percent_060**
Member of [HpeServerAccPowerCalibration.v1_0_0.HpeServerAccPowerCalibration](#hpeserveraccpowercalibration-v1_0_0-hpeserveraccpowercalibration)

| | |
|---|---|
|Description|The peak power of 60 Percent throttling.|
|Type|integer|
|Read Only|True|

**CalibrationData.ThrottlePeakPower.Percent_065**
Member of [HpeServerAccPowerCalibration.v1_0_0.HpeServerAccPowerCalibration](#hpeserveraccpowercalibration-v1_0_0-hpeserveraccpowercalibration)

| | |
|---|---|
|Description|The peak power of 65 Percent throttling.|
|Type|integer|
|Read Only|True|

**CalibrationData.ThrottlePeakPower.Percent_070**
Member of [HpeServerAccPowerCalibration.v1_0_0.HpeServerAccPowerCalibration](#hpeserveraccpowercalibration-v1_0_0-hpeserveraccpowercalibration)

| | |
|---|---|
|Description|The peak power of 70 Percent throttling.|
|Type|integer|
|Read Only|True|

**CalibrationData.ThrottlePeakPower.Percent_075**
Member of [HpeServerAccPowerCalibration.v1_0_0.HpeServerAccPowerCalibration](#hpeserveraccpowercalibration-v1_0_0-hpeserveraccpowercalibration)

| | |
|---|---|
|Description|The peak power of 75 Percent throttling.|
|Type|integer|
|Read Only|True|

**CalibrationData.ThrottlePeakPower.Percent_080**
Member of [HpeServerAccPowerCalibration.v1_0_0.HpeServerAccPowerCalibration](#hpeserveraccpowercalibration-v1_0_0-hpeserveraccpowercalibration)

| | |
|---|---|
|Description|The peak power of 80 Percent throttling.|
|Type|integer|
|Read Only|True|

**CalibrationData.ThrottlePeakPower.Percent_085**
Member of [HpeServerAccPowerCalibration.v1_0_0.HpeServerAccPowerCalibration](#hpeserveraccpowercalibration-v1_0_0-hpeserveraccpowercalibration)

| | |
|---|---|
|Description|The peak power of 85 Percent throttling.|
|Type|integer|
|Read Only|True|

**CalibrationData.ThrottlePeakPower.Percent_090**
Member of [HpeServerAccPowerCalibration.v1_0_0.HpeServerAccPowerCalibration](#hpeserveraccpowercalibration-v1_0_0-hpeserveraccpowercalibration)

| | |
|---|---|
|Description|The peak power of 90 Percent throttling.|
|Type|integer|
|Read Only|True|

**CalibrationData.ThrottlePeakPower.Percent_095**
Member of [HpeServerAccPowerCalibration.v1_0_0.HpeServerAccPowerCalibration](#hpeserveraccpowercalibration-v1_0_0-hpeserveraccpowercalibration)

| | |
|---|---|
|Description|The peak power of 95 Percent throttling.|
|Type|integer|
|Read Only|True|

**CalibrationData.ThrottlePeakPower.Percent_100**
Member of [HpeServerAccPowerCalibration.v1_0_0.HpeServerAccPowerCalibration](#hpeserveraccpowercalibration-v1_0_0-hpeserveraccpowercalibration)

| | |
|---|---|
|Description|The peak power of 100 Percent throttling.|
|Type|integer|
|Read Only|True|

**CalibrationData.ZoneNumber**
Member of [HpeServerAccPowerCalibration.v1_0_0.HpeServerAccPowerCalibration](#hpeserveraccpowercalibration-v1_0_0-hpeserveraccpowercalibration)

| | |
|---|---|
|Description|The zone number either on the entire chassis or specific zone. 0 for entire chassis, other number is for specific zone.|
|Type|integer|
|Read Only|True|

### CalibrationInProgress
Member of [HpeServerAccPowerCalibration.v1_0_0.HpeServerAccPowerCalibration](#hpeserveraccpowercalibration-v1_0_0-hpeserveraccpowercalibration)

| | |
|---|---|
|Description|The current state of the chassis power zone calibration task.|
|Type|boolean|
|Read Only|True|

### Actions

**HpeServerAccPowerCalibration.Calibrate**
Member of [HpeServerAccPowerCalibration.v1_0_0.HpeServerAccPowerCalibration](#hpeserveraccpowercalibration-v1_0_0-hpeserveraccpowercalibration)
Execute the Apollo Chassis Controller power calibration configuration.


**Parameters:**

**EEPROMSaveEnabled (boolean)**

**AllZone (boolean)**

**Seconds (integer)**

**ZoneNumber (integer)**

**ActionType (string)**

|Value|Description|
|---|---|
|Start|
|Stop|
## HpeServerAccPowerLimit.v1_0_0.HpeServerAccPowerLimit
```@odata.type: "#HpeServerAccPowerLimit.v1_0_0.HpeServerAccPowerLimit"```

This resource type was added in iLO 5 1.20 and is available on **HPE ProLiant Apollo XL** systems.

### Resource Instances
|Uri|HTTP Allow|
|---|---|
|```/redfish/v1/chassis/{item}/power/accpowerservice/powerlimit/```|GET POST |

### ActualPowerLimits (array)
Member of [HpeServerAccPowerLimit.v1_0_0.HpeServerAccPowerLimit](#hpeserveraccpowerlimit-v1_0_0-hpeserveraccpowerlimit)
```ActualPowerLimits``` is an array containing elements of:

**ActualPowerLimits[{item}].PowerLimitInWatts**
Member of [HpeServerAccPowerLimit.v1_0_0.HpeServerAccPowerLimit](#hpeserveraccpowerlimit-v1_0_0-hpeserveraccpowerlimit)

| | |
|---|---|
|Description|The actual power limit (in watts) for the zone, it will be set to null when power limit disabled.|
|Type|integer or null|
|Read Only|False|

**ActualPowerLimits[{item}].ZoneNumber**
Member of [HpeServerAccPowerLimit.v1_0_0.HpeServerAccPowerLimit](#hpeserveraccpowerlimit-v1_0_0-hpeserveraccpowerlimit)

| | |
|---|---|
|Description|The zone number either on the entire chassis or specific zone. 0 for entire chassis, other number is for specific zone.|
|Type|integer|
|Read Only|True|

### PowerLimitRanges (array)
Member of [HpeServerAccPowerLimit.v1_0_0.HpeServerAccPowerLimit](#hpeserveraccpowerlimit-v1_0_0-hpeserveraccpowerlimit)
```PowerLimitRanges``` is an array containing elements of:

**PowerLimitRanges[{item}].MaximumPowerLimit**
Member of [HpeServerAccPowerLimit.v1_0_0.HpeServerAccPowerLimit](#hpeserveraccpowerlimit-v1_0_0-hpeserveraccpowerlimit)

| | |
|---|---|
|Description|The Maximum power limit (in watts) for the zone.|
|Type|integer|
|Read Only|True|

**PowerLimitRanges[{item}].MinimumPowerLimit**
Member of [HpeServerAccPowerLimit.v1_0_0.HpeServerAccPowerLimit](#hpeserveraccpowerlimit-v1_0_0-hpeserveraccpowerlimit)

| | |
|---|---|
|Description|The Minimum power limit (in watts) for the zone.|
|Type|integer|
|Read Only|True|

**PowerLimitRanges[{item}].ZoneNumber**
Member of [HpeServerAccPowerLimit.v1_0_0.HpeServerAccPowerLimit](#hpeserveraccpowerlimit-v1_0_0-hpeserveraccpowerlimit)

| | |
|---|---|
|Description|The zone number either on the entire chassis or specific zone. 0 for entire chassis, other number is for specific zone.|
|Type|integer|
|Read Only|True|

### PowerLimits (array)
Member of [HpeServerAccPowerLimit.v1_0_0.HpeServerAccPowerLimit](#hpeserveraccpowerlimit-v1_0_0-hpeserveraccpowerlimit)
```PowerLimits``` is an array containing elements of:

**PowerLimits[{item}].PowerLimitInWatts**
Member of [HpeServerAccPowerLimit.v1_0_0.HpeServerAccPowerLimit](#hpeserveraccpowerlimit-v1_0_0-hpeserveraccpowerlimit)

| | |
|---|---|
|Description|The target power limit (in watts) for the zone, it will be set to null when power limit disabled.|
|Type|integer or null|
|Read Only|False|

**PowerLimits[{item}].ZoneNumber**
Member of [HpeServerAccPowerLimit.v1_0_0.HpeServerAccPowerLimit](#hpeserveraccpowerlimit-v1_0_0-hpeserveraccpowerlimit)

| | |
|---|---|
|Description|The zone number either on the entire chassis or specific zone. 0 for entire chassis, other number is for specific zone.|
|Type|integer|
|Read Only|True|

### Actions

**HpeServerAccPowerLimit.ConfigurePowerLimit**
Member of [HpeServerAccPowerLimit.v1_0_0.HpeServerAccPowerLimit](#hpeserveraccpowerlimit-v1_0_0-hpeserveraccpowerlimit)
Deploy the Apollo Chassis Controller power limit configuration.


**Parameters:**

**PowerLimits (array)**
## HpeServerAccPowerNodesInfo.v1_0_0.HpeServerAccPowerNodesInfo
```@odata.type: "#HpeServerAccPowerNodesInfo.v1_0_0.HpeServerAccPowerNodesInfo"```

This resource type was added in iLO 5 1.20 and is available on **HPE ProLiant Apollo XL** systems.

### Resource Instances
|Uri|HTTP Allow|
|---|---|
|```/redfish/v1/chassis/{item}/power/accpowerservice/nodesinfo/```|GET |

### MaxSupportedNodes
Member of [HpeServerAccPowerNodesInfo.v1_0_0.HpeServerAccPowerNodesInfo](#hpeserveraccpowernodesinfo-v1_0_0-hpeserveraccpowernodesinfo)

| | |
|---|---|
|Description|Total Nodes supported in Chassis.|
|Type|integer|
|Read Only|True|

### NodeInfoList (array)
Member of [HpeServerAccPowerNodesInfo.v1_0_0.HpeServerAccPowerNodesInfo](#hpeserveraccpowernodesinfo-v1_0_0-hpeserveraccpowernodesinfo)
```NodeInfoList``` is an array containing elements of:

**NodeInfoList[{item}].NodeNumber**
Member of [HpeServerAccPowerNodesInfo.v1_0_0.HpeServerAccPowerNodesInfo](#hpeserveraccpowernodesinfo-v1_0_0-hpeserveraccpowernodesinfo)

| | |
|---|---|
|Description|The physical node number in chassis.|
|Type|integer|
|Read Only|True|

**NodeInfoList[{item}].Throttle**
Member of [HpeServerAccPowerNodesInfo.v1_0_0.HpeServerAccPowerNodesInfo](#hpeserveraccpowernodesinfo-v1_0_0-hpeserveraccpowernodesinfo)

| | |
|---|---|
|Description|It indicates the current throttle on the node. (PWM %)|
|Type|integer|
|Read Only|True|

**NodeInfoList[{item}].WarningStatus**
Member of [HpeServerAccPowerNodesInfo.v1_0_0.HpeServerAccPowerNodesInfo](#hpeserveraccpowernodesinfo-v1_0_0-hpeserveraccpowernodesinfo)

| | |
|---|---|
|Description|Specifies whether the node is in warning status or not. WarningStatus indicates a node is over loading and chassis manager force it throttle at 50% for 5 mins|
|Type|boolean|
|Read Only|True|

## HpeServerAccPowerService.v1_0_0.HpeServerAccPowerService
```@odata.type: "#HpeServerAccPowerService.v1_0_0.HpeServerAccPowerService"```

This resource type was added in iLO 5 1.20 and is available on **HPE ProLiant Apollo XL** systems.

### Resource Instances
|Uri|HTTP Allow|
|---|---|
|```/redfish/v1/chassis/{item}/power/accpowerservice/```|GET PATCH |

### EEPROMSaveEnabled
Member of [HpeServerAccPowerService.v1_0_0.HpeServerAccPowerService](#hpeserveraccpowerservice-v1_0_0-hpeserveraccpowerservice)

| | |
|---|---|
|Description|Determines whether the EEPROM save is enabled or disabled.|
|Type|boolean|
|Read Only|False|

### PowerRegulationEnabled
Member of [HpeServerAccPowerService.v1_0_0.HpeServerAccPowerService](#hpeserveraccpowerservice-v1_0_0-hpeserveraccpowerservice)

| | |
|---|---|
|Description|Determines whether power regulation is enabled or disabled.|
|Type|boolean|
|Read Only|False|

### PowerRegulatorMode
Member of [HpeServerAccPowerService.v1_0_0.HpeServerAccPowerService](#hpeserveraccpowerservice-v1_0_0-hpeserveraccpowerservice)

| | |
|---|---|
|Type|string|
|Read Only|False|

The following are the supported values:

|Value|Description|
|---|---|
|```ACRedundancy```|AC Redundancy with Throttling Mode (Max Performance w/ Redundancy).|
|```FullACDCRedundancy```|Full AC/DC Redundancy Mode.|
|```UserConfig```|User Configurable Mode.|
|```APM```|APM Power Regulator Mode. Cannot configure by iLO.|
|```PowerFeedProtect```|Power Feed Protection Mode.|

## HpeServerAccPowerZone.v1_0_0.HpeServerAccPowerZone
```@odata.type: "#HpeServerAccPowerZone.v1_0_0.HpeServerAccPowerZone"```

This resource type was added in iLO 5 1.20 and is available on **HPE ProLiant Apollo XL** systems.

### Resource Instances
|Uri|HTTP Allow|
|---|---|
|```/redfish/v1/chassis/{item}/power/accpowerservice/zone/```|GET POST |

### ZoneConfiguration
**ZoneConfiguration.Zone (array)**
Member of [HpeServerAccPowerZone.v1_0_0.HpeServerAccPowerZone](#hpeserveraccpowerzone-v1_0_0-hpeserveraccpowerzone)
```Zone``` is an array containing elements of:

**Zone[{item}].Node (array)**
Member of [HpeServerAccPowerZone.v1_0_0.HpeServerAccPowerZone](#hpeserveraccpowerzone-v1_0_0-hpeserveraccpowerzone)
```Node``` is an array containing elements of:

**Node[{item}].NodeNumber**
Member of [HpeServerAccPowerZone.v1_0_0.HpeServerAccPowerZone](#hpeserveraccpowerzone-v1_0_0-hpeserveraccpowerzone)

| | |
|---|---|
|Description|The node number of zone configuration.|
|Type|integer|
|Read Only|True|

**Node[{item}].NodePriority**
Member of [HpeServerAccPowerZone.v1_0_0.HpeServerAccPowerZone](#hpeserveraccpowerzone-v1_0_0-hpeserveraccpowerzone)

| | |
|---|---|
|Description|The power regulation node priority, the range must between 1 - 5. 5 is default and lowest priority.|
|Type|integer|
|Read Only|True|

**Zone[{item}].ZoneNumber**
Member of [HpeServerAccPowerZone.v1_0_0.HpeServerAccPowerZone](#hpeserveraccpowerzone-v1_0_0-hpeserveraccpowerzone)

| | |
|---|---|
|Description|The zone number of zone configuration.|
|Type|integer|
|Read Only|True|

**Zone[{item}].ZonePriority**
Member of [HpeServerAccPowerZone.v1_0_0.HpeServerAccPowerZone](#hpeserveraccpowerzone-v1_0_0-hpeserveraccpowerzone)

| | |
|---|---|
|Description|The power regulation zone priority, the range must between 1 - 5. 5 is default and lowest priority.|
|Type|integer|
|Read Only|True|

### Actions

**HpeServerAccPowerZone.ConfigureZone**
Member of [HpeServerAccPowerZone.v1_0_0.HpeServerAccPowerZone](#hpeserveraccpowerzone-v1_0_0-hpeserveraccpowerzone)
Execute the Apollo Chassis Controller power regulation zone configuration.


**Parameters:**

**Zone (array)**
## HpeServerBootSettings.v2_0_0.HpeServerBootSettings
```@odata.type: "#HpeServerBootSettings.v2_0_0.HpeServerBootSettings"```

The schema definition of the server UEFI Boot Order resource.
### Resource Instances
|Uri|HTTP Allow|
|---|---|
|```/redfish/v1/systems/{item}/bios/boot/```|GET |
|```/redfish/v1/systems/{item}/bios/boot/settings/```|GET PATCH |

### Links to other Resources
|Link Name|Destination type
|---|---|
|```@Redfish.Settings/SettingsObject```|[HpeServerBootSettings](#hpeserverbootsettings-v2_0_0-hpeserverbootsettings)|
|```Oem/Hpe/Links/BaseConfigs```|[HpeBaseConfigs](#hpebaseconfigs-v2_0_0-hpebaseconfigs)|

### @Redfish.Settings
Member of [HpeServerBootSettings.v2_0_0.HpeServerBootSettings](#hpeserverbootsettings-v2_0_0-hpeserverbootsettings)
See the Redfish standard schema and specification for information on common @Redfish properties.

### BootSources (array)
Member of [HpeServerBootSettings.v2_0_0.HpeServerBootSettings](#hpeserverbootsettings-v2_0_0-hpeserverbootsettings)
```BootSources``` is an array containing elements of:

**BootSources[{item}].BootString**
Member of [HpeServerBootSettings.v2_0_0.HpeServerBootSettings](#hpeserverbootsettings-v2_0_0-hpeserverbootsettings)

| | |
|---|---|
|Description|User-readable string that describes the UEFI boot option.|
|Type|string|
|Read Only|True|

**BootSources[{item}].CorrelatableID**
Member of [HpeServerBootSettings.v2_0_0.HpeServerBootSettings](#hpeserverbootsettings-v2_0_0-hpeserverbootsettings)

| | |
|---|---|
|Description|Contains any CorrelatableIDs that represent this boot option. The correlatableID values can be JSON Pointers or UEFI identifiers.|
|Type|string|
|Read Only|True|

**BootSources[{item}].StructuredBootString**
Member of [HpeServerBootSettings.v2_0_0.HpeServerBootSettings](#hpeserverbootsettings-v2_0_0-hpeserverbootsettings)

| | |
|---|---|
|Description|Uniquely identifies this boot option within the server.|
|Type|string|
|Read Only|True|

**BootSources[{item}].UEFIDevicePath**
Member of [HpeServerBootSettings.v2_0_0.HpeServerBootSettings](#hpeserverbootsettings-v2_0_0-hpeserverbootsettings)

| | |
|---|---|
|Description|Standardized text representation of the UEFI device path for this boot option, in UTF-8 format.|
|Type|string|
|Read Only|True|

### DefaultBootOrder (array)
Member of [HpeServerBootSettings.v2_0_0.HpeServerBootSettings](#hpeserverbootsettings-v2_0_0-hpeserverbootsettings)
```DefaultBootOrder``` is an array containing elements of:


| | |
|---|---|
|Description|Default UEFI boot order device type. This is used to define the order in which UEFI boot order is reset to when a default configuration is requested.|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|
|---|
|```UefiShell```|
|```Floppy```|
|```Cd```|
|```Usb```|
|```EmbeddedStorage```|
|```PcieSlotStorage```|
|```EmbeddedFlexLOM```|
|```PcieSlotNic```|

### DesiredBootDevices (array)
Member of [HpeServerBootSettings.v2_0_0.HpeServerBootSettings](#hpeserverbootsettings-v2_0_0-hpeserverbootsettings)
```DesiredBootDevices``` is an array containing elements of:

**DesiredBootDevices[{item}].CorrelatableID**
Member of [HpeServerBootSettings.v2_0_0.HpeServerBootSettings](#hpeserverbootsettings-v2_0_0-hpeserverbootsettings)

| | |
|---|---|
|Description|Standardized text representation of the UEFI device path of the desired boot device, in UTF-8 format. For example 'PciRoot(0x0)/Pci(0x2,0x2)/Pci(0x0,0x0)'|
|Type|string|
|Read Only|False|

**DesiredBootDevices[{item}].Lun**
Member of [HpeServerBootSettings.v2_0_0.HpeServerBootSettings](#hpeserverbootsettings-v2_0_0-hpeserverbootsettings)

| | |
|---|---|
|Description|The Logical Unit Number (LUN) of the desired boot device. This value must be a hexadecimal string with an even number of 2 to 16 characters, excluding the first two characters, 0x (for example, '0x01').|
|Type|string|
|Read Only|False|

**DesiredBootDevices[{item}].Wwn**
Member of [HpeServerBootSettings.v2_0_0.HpeServerBootSettings](#hpeserverbootsettings-v2_0_0-hpeserverbootsettings)

| | |
|---|---|
|Description|The Fibre Channel World Wide Name (WWN) of the desired boot device. This value must be a hexadecimal string with an even number of 2 to 16 characters, excluding the first two characters, 0x (for example, '0x0001020304050607').|
|Type|string|
|Read Only|False|

**DesiredBootDevices[{item}].iScsiTargetName**
Member of [HpeServerBootSettings.v2_0_0.HpeServerBootSettings](#hpeserverbootsettings-v2_0_0-hpeserverbootsettings)

| | |
|---|---|
|Description|The iSCSI node target name of the desired boot device. The value must be a string based on IETF RFC 3270, and can be up to 223 characters in length (for example, 'iqn.1991-05.com.microsoft:iscsitarget-iscsidisk-target').|
|Type|string|
|Read Only|False|

### PersistentBootConfigOrder (array)
Member of [HpeServerBootSettings.v2_0_0.HpeServerBootSettings](#hpeserverbootsettings-v2_0_0-hpeserverbootsettings)
```PersistentBootConfigOrder``` is an array containing elements of:


| | |
|---|---|
|Description|The structured boot string that references a corresponding entry in the BootSources array.|
|Type|string|
|Read Only|True|

## HpeServerDevice.v2_0_0.HpeServerDevice
```@odata.type: "#HpeServerDevice.v2_0_0.HpeServerDevice"```

This resource type was added in iLO 5 1.20

HpeServerDevice represents physical server devices including part information.  This is especially useful for system inventory.

### Resource Instances
|Uri|HTTP Allow|
|---|---|
|```/redfish/v1/chassis/{item}/devices/{item}/```|GET PATCH |

### Links to other Resources
|Link Name|Destination type
|---|---|
|```DeviceInstances[]```|[HpeServerPciDevice](#hpeserverpcidevice-v2_0_0-hpeserverpcidevice)|

### DeviceInstances (array)
Member of [HpeServerDevice.v2_0_0.HpeServerDevice](#hpeserverdevice-v2_0_0-hpeserverdevice)
```DeviceInstances``` is an array containing elements of:

### DeviceType
Member of [HpeServerDevice.v2_0_0.HpeServerDevice](#hpeserverdevice-v2_0_0-hpeserverdevice)

| | |
|---|---|
|Description|Device type.|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```GPU```|GPU|
|```PLX Controller```|PLX Controller (Bridge)|
|```Expansion Riser```|Expansion Riser|
|```Smart Storage```|Smart Storage|
|```SAS/SATA Storage Controller```|SAS/SATA Storage Controller|
|```IDE Storage controller```||
|```USB Storage Controller```|USB Storage Controller|
|```Storage Controller```|Storage Controller|
|```LOM/NIC```|LOM/NIC|
|```Converged Network Adapter```|Converged Network Adapter|
|```Fibre Channel```|Fibre Channel|
|```Direct Attached NVMe Device```|Direct Attached NVMe Device|
|```Backplane PIC```|Backplane PIC|
|```Smart Storage Battery```|Smart Storage Battery|
|```USB```|Universal Serial Bus|
|```TPM```|Trusted Platform Module|
|```Communication Controller```|Communication Controller|
|```Unknown```|Unknown Device Type|

### FirmwareVersion
**FirmwareVersion.Current**
**FirmwareVersion.Current.VersionString**
Member of [HpeServerDevice.v2_0_0.HpeServerDevice](#hpeserverdevice-v2_0_0-hpeserverdevice)

| | |
|---|---|
|Description|This string represents the version of the firmware image.|
|Type|string or null|
|Read Only|True|

### Location
Member of [HpeServerDevice.v2_0_0.HpeServerDevice](#hpeserverdevice-v2_0_0-hpeserverdevice)

| | |
|---|---|
|Description|Location of the device.|
|Type|string or null|
|Read Only|True|

### MCTPProtocolDisabled
Member of [HpeServerDevice.v2_0_0.HpeServerDevice](#hpeserverdevice-v2_0_0-hpeserverdevice)

| | |
|---|---|
|Description|Set to true to disable MCTP on this slot. Once disabled, can be enabled only through MCTP factory reset.|
|Type|boolean|
|Read Only|False|

### Manufacturer
Member of [HpeServerDevice.v2_0_0.HpeServerDevice](#hpeserverdevice-v2_0_0-hpeserverdevice)

| | |
|---|---|
|Description|Device manufacturer.|
|Type|string or null|
|Read Only|True|

### PartNumber
Member of [HpeServerDevice.v2_0_0.HpeServerDevice](#hpeserverdevice-v2_0_0-hpeserverdevice)

| | |
|---|---|
|Description|Board part Number which is HPE PCA Assembly Number.|
|Type|string or null|
|Read Only|True|

### ProductPartNumber
Member of [HpeServerDevice.v2_0_0.HpeServerDevice](#hpeserverdevice-v2_0_0-hpeserverdevice)

| | |
|---|---|
|Description|Product Part Number.|
|Type|string or null|
|Read Only|True|

### ProductVersion
Member of [HpeServerDevice.v2_0_0.HpeServerDevice](#hpeserverdevice-v2_0_0-hpeserverdevice)

| | |
|---|---|
|Description|Product Version.|
|Type|string or null|
|Read Only|True|

### SerialNumber
Member of [HpeServerDevice.v2_0_0.HpeServerDevice](#hpeserverdevice-v2_0_0-hpeserverdevice)

| | |
|---|---|
|Description|Product Serial Number.|
|Type|string or null|
|Read Only|True|

### Status
Member of [HpeServerDevice.v2_0_0.HpeServerDevice](#hpeserverdevice-v2_0_0-hpeserverdevice)
See the Redfish standard schema and specification for information on common Status object.

## HpeServerPciDevice.v2_0_0.HpeServerPciDevice
```@odata.type: "#HpeServerPciDevice.v2_0_0.HpeServerPciDevice"```
### Resource Instances
|Uri|HTTP Allow|
|---|---|
|```/redfish/v1/systems/{item}/pcidevices/{item}/```|GET |

### BayNumber
Member of [HpeServerPciDevice.v2_0_0.HpeServerPciDevice](#hpeserverpcidevice-v2_0_0-hpeserverpcidevice)

| | |
|---|---|
|Description|Bay number value.|
|Type|integer|
|Read Only|True|

### BusNumber
Member of [HpeServerPciDevice.v2_0_0.HpeServerPciDevice](#hpeserverpcidevice-v2_0_0-hpeserverpcidevice)

| | |
|---|---|
|Description|PCI device bus number value.|
|Type|integer|
|Read Only|True|

### ClassCode
Member of [HpeServerPciDevice.v2_0_0.HpeServerPciDevice](#hpeserverpcidevice-v2_0_0-hpeserverpcidevice)

| | |
|---|---|
|Description|PCI class code of the endpoint.|
|Type|integer|
|Read Only|True|

### DeviceID
Member of [HpeServerPciDevice.v2_0_0.HpeServerPciDevice](#hpeserverpcidevice-v2_0_0-hpeserverpcidevice)

| | |
|---|---|
|Description|PCI device ID of the device.|
|Type|integer|
|Read Only|True|

### DeviceInstance
Member of [HpeServerPciDevice.v2_0_0.HpeServerPciDevice](#hpeserverpcidevice-v2_0_0-hpeserverpcidevice)

| | |
|---|---|
|Description|PCI device instance value.|
|Type|integer|
|Read Only|True|

### DeviceLocation
Member of [HpeServerPciDevice.v2_0_0.HpeServerPciDevice](#hpeserverpcidevice-v2_0_0-hpeserverpcidevice)

| | |
|---|---|
|Description|PCI device location.|
|Type|string|
|Read Only|True|

### DeviceNumber
Member of [HpeServerPciDevice.v2_0_0.HpeServerPciDevice](#hpeserverpcidevice-v2_0_0-hpeserverpcidevice)

| | |
|---|---|
|Description|PCI device number value.|
|Type|integer|
|Read Only|True|

### DeviceSubInstance
Member of [HpeServerPciDevice.v2_0_0.HpeServerPciDevice](#hpeserverpcidevice-v2_0_0-hpeserverpcidevice)

| | |
|---|---|
|Description|PCI device sub-instance value.|
|Type|integer|
|Read Only|True|

### DeviceType
Member of [HpeServerPciDevice.v2_0_0.HpeServerPciDevice](#hpeserverpcidevice-v2_0_0-hpeserverpcidevice)

| | |
|---|---|
|Description|Device type value.|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```Flexible LOM```|Flexible LAN-On-Motherboard|
|```Embedded LOM```|Embedded LAN-On-Motherboard|
|```NIC```|Network Interface Controller|
|```HDD Not attached to a SA Controller```|Hard Disk Drive|
|```HDD Attached to a SA Controller```|Hard Disk Drive attached to an array controller|
|```Other PCI Device```|Other PCI Device|
|```Unknown```|Unknown PCI Device|
|```Other```|Other PCI Device|
|```Video```|Video Controller|
|```SCSI Controller```|SCSI Controller|
|```Ethernet```|Ethernet Controller|
|```Token Ring```|Token Ring Controller|
|```Sound```|Sound Controller|
|```PATA Controller```|Parallel ATA Controller|
|```SATA Controller```|Serial ATA Controller|
|```SAS Controller```|Serial Attached SCSI Controller|
|```Storage Controller```|Storage Controller (not Smart Array)|
|```Storage Array Controller```|Smart Array Storage Controller|
|```USB Hard Disk Drive```|USB Hard Disk Drive|
|```Firmware Volume```|Firmware Volume|
|```UEFI Shell```|UEFI Shell|
|```Generic UEFI USB Boot Entry```|Generic UEFI USB Boot Entry|
|```Dynamic Storage Array Controller```|Dynamic Smart Array Controller|
|```File```|File|
|```NVMe Hard Drive```|NVMe Hard Drive|
|```NVDIMM```|NVDIMM|

### EnclosureNumber
Member of [HpeServerPciDevice.v2_0_0.HpeServerPciDevice](#hpeserverpcidevice-v2_0_0-hpeserverpcidevice)

| | |
|---|---|
|Description|Enclosure number value.|
|Type|integer|
|Read Only|True|

### FunctionNumber
Member of [HpeServerPciDevice.v2_0_0.HpeServerPciDevice](#hpeserverpcidevice-v2_0_0-hpeserverpcidevice)

| | |
|---|---|
|Description|PCI device function number value.|
|Type|integer|
|Read Only|True|

### LocationString
Member of [HpeServerPciDevice.v2_0_0.HpeServerPciDevice](#hpeserverpcidevice-v2_0_0-hpeserverpcidevice)

| | |
|---|---|
|Description|Text representation of the UEFI device location, in UTF-8 format|
|Type|string|
|Read Only|True|

### SegmentNumber
Member of [HpeServerPciDevice.v2_0_0.HpeServerPciDevice](#hpeserverpcidevice-v2_0_0-hpeserverpcidevice)

| | |
|---|---|
|Description|PCI segment group number value.|
|Type|integer|
|Read Only|True|

### StructuredName
Member of [HpeServerPciDevice.v2_0_0.HpeServerPciDevice](#hpeserverpcidevice-v2_0_0-hpeserverpcidevice)

| | |
|---|---|
|Description|PCI device structured name in UTF-8 format.|
|Type|string|
|Read Only|True|

### SubclassCode
Member of [HpeServerPciDevice.v2_0_0.HpeServerPciDevice](#hpeserverpcidevice-v2_0_0-hpeserverpcidevice)

| | |
|---|---|
|Description|PCI sub class code of the endpoint.|
|Type|integer|
|Read Only|True|

### SubsystemDeviceID
Member of [HpeServerPciDevice.v2_0_0.HpeServerPciDevice](#hpeserverpcidevice-v2_0_0-hpeserverpcidevice)

| | |
|---|---|
|Description|PCI subsystem device ID of the device.|
|Type|integer|
|Read Only|True|

### SubsystemVendorID
Member of [HpeServerPciDevice.v2_0_0.HpeServerPciDevice](#hpeserverpcidevice-v2_0_0-hpeserverpcidevice)

| | |
|---|---|
|Description|PCI subsystem vendor ID of the device.|
|Type|integer|
|Read Only|True|

### UEFIDevicePath
Member of [HpeServerPciDevice.v2_0_0.HpeServerPciDevice](#hpeserverpcidevice-v2_0_0-hpeserverpcidevice)

| | |
|---|---|
|Description|Standardized text representation of the UEFI device path, in UTF-8 format.|
|Type|string|
|Read Only|True|

### VendorID
Member of [HpeServerPciDevice.v2_0_0.HpeServerPciDevice](#hpeserverpcidevice-v2_0_0-hpeserverpcidevice)

| | |
|---|---|
|Description|PCI vendor ID of the device.|
|Type|integer|
|Read Only|True|

## HpeServerPCISlot.v2_1_0.HpeServerPCISlot
```@odata.type: "#HpeServerPCISlot.v2_1_0.HpeServerPCISlot"```
### Resource Instances
|Uri|HTTP Allow|
|---|---|
|```/redfish/v1/systems/{item}/pcislots/{item}/```|GET |

### BusNumber
Member of [HpeServerPCISlot.v2_1_0.HpeServerPCISlot](#hpeserverpcislot-v2_1_0-hpeserverpcislot)

| | |
|---|---|
|Description|PCI slot bus number.|
|Type|integer|
|Read Only|True|

### Characteristics
**Characteristics.Provides3_3Volts**
Member of [HpeServerPCISlot.v2_1_0.HpeServerPCISlot](#hpeserverpcislot-v2_1_0-hpeserverpcislot)

| | |
|---|---|
|Description|Provides 3.3 volts.|
|Type|boolean|
|Read Only|True|

**Characteristics.Provides5Volts**
Member of [HpeServerPCISlot.v2_1_0.HpeServerPCISlot](#hpeserverpcislot-v2_1_0-hpeserverpcislot)

| | |
|---|---|
|Description|Provides 5.0 volts.|
|Type|boolean|
|Read Only|True|

**Characteristics.SlotIsShared**
Member of [HpeServerPCISlot.v2_1_0.HpeServerPCISlot](#hpeserverpcislot-v2_1_0-hpeserverpcislot)

| | |
|---|---|
|Description|The slot shares its opening with another slot.|
|Type|boolean|
|Read Only|True|

**Characteristics.SupportsCardBus**
Member of [HpeServerPCISlot.v2_1_0.HpeServerPCISlot](#hpeserverpcislot-v2_1_0-hpeserverpcislot)

| | |
|---|---|
|Description|PC Card slot supports Card Bus.|
|Type|boolean|
|Read Only|True|

**Characteristics.SupportsHotPlugDevices**
Member of [HpeServerPCISlot.v2_1_0.HpeServerPCISlot](#hpeserverpcislot-v2_1_0-hpeserverpcislot)

| | |
|---|---|
|Description|Slot supports hot-plug devices.|
|Type|boolean|
|Read Only|True|

**Characteristics.SupportsModemRingResume**
Member of [HpeServerPCISlot.v2_1_0.HpeServerPCISlot](#hpeserverpcislot-v2_1_0-hpeserverpcislot)

| | |
|---|---|
|Description|PC Card slot supports Modem Ring Resume.|
|Type|boolean|
|Read Only|True|

**Characteristics.SupportsPCCard16**
Member of [HpeServerPCISlot.v2_1_0.HpeServerPCISlot](#hpeserverpcislot-v2_1_0-hpeserverpcislot)

| | |
|---|---|
|Description|PC Card slot supports PC Card-16.|
|Type|boolean|
|Read Only|True|

**Characteristics.SupportsPowerManagementEventSignal**
Member of [HpeServerPCISlot.v2_1_0.HpeServerPCISlot](#hpeserverpcislot-v2_1_0-hpeserverpcislot)

| | |
|---|---|
|Description|PCI slot supports Power Management Event signal.|
|Type|boolean|
|Read Only|True|

**Characteristics.SupportsSMBusSignal**
Member of [HpeServerPCISlot.v2_1_0.HpeServerPCISlot](#hpeserverpcislot-v2_1_0-hpeserverpcislot)

| | |
|---|---|
|Description|PCI slot supports SMBUS signal.|
|Type|boolean|
|Read Only|True|

**Characteristics.SupportsZoomVideo**
Member of [HpeServerPCISlot.v2_1_0.HpeServerPCISlot](#hpeserverpcislot-v2_1_0-hpeserverpcislot)

| | |
|---|---|
|Description|PC Card slot supports Zoom Video.|
|Type|boolean|
|Read Only|True|

### DeviceNumber
Member of [HpeServerPCISlot.v2_1_0.HpeServerPCISlot](#hpeserverpcislot-v2_1_0-hpeserverpcislot)

| | |
|---|---|
|Description|PCI slot device number.|
|Type|integer|
|Read Only|True|

### FunctionNumber
Member of [HpeServerPCISlot.v2_1_0.HpeServerPCISlot](#hpeserverpcislot-v2_1_0-hpeserverpcislot)

| | |
|---|---|
|Description|PCI slot function number.|
|Type|integer|
|Read Only|True|

### Length
Member of [HpeServerPCISlot.v2_1_0.HpeServerPCISlot](#hpeserverpcislot-v2_1_0-hpeserverpcislot)

| | |
|---|---|
|Description|PCI slot length|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|
|---|
|```Short```|
|```Long```|
|```Other```|

### LinkLanes
Member of [HpeServerPCISlot.v2_1_0.HpeServerPCISlot](#hpeserverpcislot-v2_1_0-hpeserverpcislot)

| | |
|---|---|
|Description|Bandwidth capacity of the slot, measured by the number of PCI Express Lanes present. Also known as the slot width.|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|
|---|
|```8 bit```|
|```16 bit```|
|```32 bit```|
|```64 bit```|
|```128 bit```|
|```x1```|
|```x2```|
|```x4```|
|```x8```|
|```x16```|
|```x32```|
|```Other```|

### Status
Member of [HpeServerPCISlot.v2_1_0.HpeServerPCISlot](#hpeserverpcislot-v2_1_0-hpeserverpcislot)
See the Redfish standard schema and specification for information on common Status object.

### SupportsHotPlug
Member of [HpeServerPCISlot.v2_1_0.HpeServerPCISlot](#hpeserverpcislot-v2_1_0-hpeserverpcislot)

| | |
|---|---|
|Description|Specifies whether the slot supports hot-plug devices.|
|Type|boolean|
|Read Only|True|

### Technology
Member of [HpeServerPCISlot.v2_1_0.HpeServerPCISlot](#hpeserverpcislot-v2_1_0-hpeserverpcislot)

| | |
|---|---|
|Description|PCI technology|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|
|---|
|```PCIExpressGen3```|
|```PCIExpressGen2```|
|```PCIExpress```|

### UEFIDevicePath
Member of [HpeServerPCISlot.v2_1_0.HpeServerPCISlot](#hpeserverpcislot-v2_1_0-hpeserverpcislot)

| | |
|---|---|
|Description|Standardized text representation of the UEFI device path, in UTF-8 format|
|Type|string|
|Read Only|True|

## HpeSmartStorage.v2_0_0.HpeSmartStorage
```@odata.type: "#HpeSmartStorage.v2_0_0.HpeSmartStorage"```

HpSmartStorage
### Resource Instances
|Uri|HTTP Allow|
|---|---|
|```/redfish/v1/systems/{item}/smartstorage/```|GET |

### Links to other Resources
|Link Name|Destination type
|---|---|
|```Links/HostBusAdapters```|Collection of [HpeSmartStorageHostBusAdapter](#hpesmartstoragehostbusadapter-v2_0_0-hpesmartstoragehostbusadapter)|
|```Links/ArrayControllers```|Collection of [HpeSmartStorageArrayController](#hpesmartstoragearraycontroller-v2_1_0-hpesmartstoragearraycontroller)|

### Status
Member of [HpeSmartStorage.v2_0_0.HpeSmartStorage](#hpesmartstorage-v2_0_0-hpesmartstorage)
See the Redfish standard schema and specification for information on common Status object.

## HpeSmartStorageArrayController.v2_1_0.HpeSmartStorageArrayController
```@odata.type: "#HpeSmartStorageArrayController.v2_1_0.HpeSmartStorageArrayController"```

HpSmartStorageArrayController
### Resource Instances
|Uri|HTTP Allow|
|---|---|
|```/redfish/v1/systems/{item}/smartstorage/arraycontrollers/{item}/```||

### Links to other Resources
|Link Name|Destination type
|---|---|
|```Links/PhysicalDrives```|Collection of [HpeSmartStorageDiskDrive](#hpesmartstoragediskdrive-v2_0_0-hpesmartstoragediskdrive)|
|```Links/LogicalDrives```|Collection of [HpeSmartStorageLogicalDrive](#hpesmartstoragelogicaldrive-v2_1_0-hpesmartstoragelogicaldrive)|
|```Links/StorageEnclosures```|Collection of [HpeSmartStorageStorageEnclosure](#hpesmartstoragestorageenclosure-v2_0_0-hpesmartstoragestorageenclosure)|
|```Links/UnconfiguredDrives```|Collection of [HpeSmartStorageDiskDrive](#hpesmartstoragediskdrive-v2_0_0-hpesmartstoragediskdrive)|

### AdapterType
Member of [HpeSmartStorageArrayController.v2_1_0.HpeSmartStorageArrayController](#hpesmartstoragearraycontroller-v2_1_0-hpesmartstoragearraycontroller)

| | |
|---|---|
|Description|Type of Smart controller|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```SmartArray```|A controller that supports all SmartArray features and configuration|
|```SmartHBA```|A controller that functions natively as an HBA, but has a ValueRAID mode for basic RAID configuration|
|```DynamicSmartArray```|A controller that allows software RAID configuration|

### ArrayCount
Member of [HpeSmartStorageArrayController.v2_1_0.HpeSmartStorageArrayController](#hpesmartstoragearraycontroller-v2_1_0-hpesmartstoragearraycontroller)

| | |
|---|---|
|Description|The number of arrays configured on this controller|
|Type|integer|
|Read Only|True|

### BackupPowerSourceStatus
Member of [HpeSmartStorageArrayController.v2_1_0.HpeSmartStorageArrayController](#hpesmartstoragearraycontroller-v2_1_0-hpesmartstoragearraycontroller)

| | |
|---|---|
|Description|The current status of the backup power source (battery, capacitor, megacell etc.)|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```Present```|The backup power source is present but charging information is unknown|
|```NotPresent```|The backup power source is not present|
|```PresentAndCharged```|The backup power source is present and fully charged|
|```PresentAndCharging```|The backup power source is present and is currently charging|

### BootVolumePrimary
Member of [HpeSmartStorageArrayController.v2_1_0.HpeSmartStorageArrayController](#hpesmartstoragearraycontroller-v2_1_0-hpesmartstoragearraycontroller)

| | |
|---|---|
|Description|The primary boot volume of this controller|
|Type|string|
|Read Only|True|

### BootVolumeSecondary
Member of [HpeSmartStorageArrayController.v2_1_0.HpeSmartStorageArrayController](#hpesmartstoragearraycontroller-v2_1_0-hpesmartstoragearraycontroller)

| | |
|---|---|
|Description|The secondary boot volume of this controller|
|Type|string|
|Read Only|True|

### CacheArrayCount
Member of [HpeSmartStorageArrayController.v2_1_0.HpeSmartStorageArrayController](#hpesmartstoragearraycontroller-v2_1_0-hpesmartstoragearraycontroller)

| | |
|---|---|
|Description|The number of cache arrays configured on this controller|
|Type|integer|
|Read Only|True|

### CacheLogicalDriveCount
Member of [HpeSmartStorageArrayController.v2_1_0.HpeSmartStorageArrayController](#hpesmartstoragearraycontroller-v2_1_0-hpesmartstoragearraycontroller)

| | |
|---|---|
|Description|The number of cache logical drives configured on this controller|
|Type|integer|
|Read Only|True|

### CacheMemorySizeMiB
Member of [HpeSmartStorageArrayController.v2_1_0.HpeSmartStorageArrayController](#hpesmartstoragearraycontroller-v2_1_0-hpesmartstoragearraycontroller)

| | |
|---|---|
|Description|The total cache memory size for the controller in MiB|
|Type|integer|
|Read Only|True|

### CacheModuleSerialNumber
Member of [HpeSmartStorageArrayController.v2_1_0.HpeSmartStorageArrayController](#hpesmartstoragearraycontroller-v2_1_0-hpesmartstoragearraycontroller)

| | |
|---|---|
|Description|The serial number of the Cache Module.|
|Type|string|
|Read Only|True|

### CachePhysicalDriveCount
Member of [HpeSmartStorageArrayController.v2_1_0.HpeSmartStorageArrayController](#hpesmartstoragearraycontroller-v2_1_0-hpesmartstoragearraycontroller)

| | |
|---|---|
|Description|The number of physical drives assigned as cache drives attached to this controller|
|Type|integer|
|Read Only|True|

### ControllerBoard
**ControllerBoard.Status**
Member of [HpeSmartStorageArrayController.v2_1_0.HpeSmartStorageArrayController](#hpesmartstoragearraycontroller-v2_1_0-hpesmartstoragearraycontroller)
See the Redfish standard schema and specification for information on common Status object.

### ControllerPartNumber
Member of [HpeSmartStorageArrayController.v2_1_0.HpeSmartStorageArrayController](#hpesmartstoragearraycontroller-v2_1_0-hpesmartstoragearraycontroller)

| | |
|---|---|
|Description|Smart Array Controller Part Number|
|Type|string|
|Read Only|True|

### CurrentOperatingMode
Member of [HpeSmartStorageArrayController.v2_1_0.HpeSmartStorageArrayController](#hpesmartstoragearraycontroller-v2_1_0-hpesmartstoragearraycontroller)

| | |
|---|---|
|Description|The current operating mode of the controller.|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```RAID```|The controller is currently functioning in RAID mode|
|```HBA```|The controller is currently functioning in HBA mode|
|```Mixed```|The controller is currently functioning in Mixed mode|

### CurrentParallelSurfaceScanCount
Member of [HpeSmartStorageArrayController.v2_1_0.HpeSmartStorageArrayController](#hpesmartstoragearraycontroller-v2_1_0-hpesmartstoragearraycontroller)

| | |
|---|---|
|Description|Number of disks the controller is scanning in parallel|
|Type|integer|
|Read Only|True|

### DataLogicalDriveCount
Member of [HpeSmartStorageArrayController.v2_1_0.HpeSmartStorageArrayController](#hpesmartstoragearraycontroller-v2_1_0-hpesmartstoragearraycontroller)

| | |
|---|---|
|Description|The number of data logical drives configured on this controller|
|Type|integer|
|Read Only|True|

### DataPhysicalDriveCount
Member of [HpeSmartStorageArrayController.v2_1_0.HpeSmartStorageArrayController](#hpesmartstoragearraycontroller-v2_1_0-hpesmartstoragearraycontroller)

| | |
|---|---|
|Description|The number of physical drives assigned as data drives attached to this controller|
|Type|integer|
|Read Only|True|

### DegradedPerformanceOptimization
Member of [HpeSmartStorageArrayController.v2_1_0.HpeSmartStorageArrayController](#hpesmartstoragearraycontroller-v2_1_0-hpesmartstoragearraycontroller)

| | |
|---|---|
|Description|Enables the controller to attempt to improve performance on RAID 5/50/6(ADG)/60 logical drives when one or more physical drives in the logical drive are failed|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```Enabled```|The controller will attempt to improve performance by buffering physical drive requests|
|```Disabled```|The controller will not buffer, which may result in reading from the same drive multiple times|

### DriveWriteCache
Member of [HpeSmartStorageArrayController.v2_1_0.HpeSmartStorageArrayController](#hpesmartstoragearraycontroller-v2_1_0-hpesmartstoragearraycontroller)

| | |
|---|---|
|Description|Enables or disables the write cache of the physical drives attached to the controller|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```Enabled```|The write cache of the physical drives attached to the controller are enabled|
|```Disabled```|The write cache of the physical drives attached to the controller are enabled|

### ElevatorSort
Member of [HpeSmartStorageArrayController.v2_1_0.HpeSmartStorageArrayController](#hpesmartstoragearraycontroller-v2_1_0-hpesmartstoragearraycontroller)

| | |
|---|---|
|Description|Enables the controller to sort requests to a physical drive|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```Enabled```|The controller will sort the requests to minimize the amount of seeking the drive must perform in order to reduce seek times|
|```Disabled```|The controller will perform the requests as they are recieved in order to improve request throughput|

### EncryptionBootPasswordSet
Member of [HpeSmartStorageArrayController.v2_1_0.HpeSmartStorageArrayController](#hpesmartstoragearraycontroller-v2_1_0-hpesmartstoragearraycontroller)

| | |
|---|---|
|Description|True if there is a boot password set, false otherwise|
|Type|boolean|
|Read Only|True|

### EncryptionCryptoOfficerPasswordSet
Member of [HpeSmartStorageArrayController.v2_1_0.HpeSmartStorageArrayController](#hpesmartstoragearraycontroller-v2_1_0-hpesmartstoragearraycontroller)

| | |
|---|---|
|Description|True if a password has been set for the Encryption Crypto Officer, false otherwise|
|Type|boolean|
|Read Only|True|

### EncryptionCspTestPassed
Member of [HpeSmartStorageArrayController.v2_1_0.HpeSmartStorageArrayController](#hpesmartstoragearraycontroller-v2_1_0-hpesmartstoragearraycontroller)

| | |
|---|---|
|Description|True if the encryption CSP test passed, false otherwise.|
|Type|boolean|
|Read Only|True|

### EncryptionEnabled
Member of [HpeSmartStorageArrayController.v2_1_0.HpeSmartStorageArrayController](#hpesmartstoragearraycontroller-v2_1_0-hpesmartstoragearraycontroller)

| | |
|---|---|
|Description|True if encryption is currently enabled for this controller, false otherwise|
|Type|boolean|
|Read Only|True|

### EncryptionFwLocked
Member of [HpeSmartStorageArrayController.v2_1_0.HpeSmartStorageArrayController](#hpesmartstoragearraycontroller-v2_1_0-hpesmartstoragearraycontroller)

| | |
|---|---|
|Description|True if the controller firmware has been locked, preventing firmware updates, false otherwise|
|Type|boolean|
|Read Only|True|

### EncryptionHasLockedVolumes
Member of [HpeSmartStorageArrayController.v2_1_0.HpeSmartStorageArrayController](#hpesmartstoragearraycontroller-v2_1_0-hpesmartstoragearraycontroller)

| | |
|---|---|
|Description|True if the controller has one or more volumes that are locked, false otherwise|
|Type|boolean|
|Read Only|True|

### EncryptionHasLockedVolumesMissingBootPassword
Member of [HpeSmartStorageArrayController.v2_1_0.HpeSmartStorageArrayController](#hpesmartstoragearraycontroller-v2_1_0-hpesmartstoragearraycontroller)

| | |
|---|---|
|Description|True if there are locked drives due to a missing boot password, false otherwise|
|Type|boolean|
|Read Only|True|

### EncryptionHasSuspendedVolumes
Member of [HpeSmartStorageArrayController.v2_1_0.HpeSmartStorageArrayController](#hpesmartstoragearraycontroller-v2_1_0-hpesmartstoragearraycontroller)

| | |
|---|---|
|Description|True if the controller password has been temporarily suspended, false otherwise|
|Type|boolean|
|Read Only|True|

### EncryptionKeySet
Member of [HpeSmartStorageArrayController.v2_1_0.HpeSmartStorageArrayController](#hpesmartstoragearraycontroller-v2_1_0-hpesmartstoragearraycontroller)

| | |
|---|---|
|Description|True if the Master Key has been set, false otherwise|
|Type|boolean|
|Read Only|True|

### EncryptionLocalKeyCacheEnabled
Member of [HpeSmartStorageArrayController.v2_1_0.HpeSmartStorageArrayController](#hpesmartstoragearraycontroller-v2_1_0-hpesmartstoragearraycontroller)

| | |
|---|---|
|Description|True if the controller caches encryption keys locally when a remote key manager is being used, false otherwise|
|Type|boolean|
|Read Only|True|

### EncryptionMixedVolumesEnabled
Member of [HpeSmartStorageArrayController.v2_1_0.HpeSmartStorageArrayController](#hpesmartstoragearraycontroller-v2_1_0-hpesmartstoragearraycontroller)

| | |
|---|---|
|Description|True if the controller will allow plaintext and encrypted volumes to exist simultaneously, false otherwise|
|Type|boolean|
|Read Only|True|

### EncryptionPhysicalDriveCount
Member of [HpeSmartStorageArrayController.v2_1_0.HpeSmartStorageArrayController](#hpesmartstoragearraycontroller-v2_1_0-hpesmartstoragearraycontroller)

| | |
|---|---|
|Description|The number of encrypted physical drives attached to the controller|
|Type|integer|
|Read Only|True|

### EncryptionRecoveryParamsSet
Member of [HpeSmartStorageArrayController.v2_1_0.HpeSmartStorageArrayController](#hpesmartstoragearraycontroller-v2_1_0-hpesmartstoragearraycontroller)

| | |
|---|---|
|Description|True if the encryption password recovery question and answer have been set, false otherwise|
|Type|boolean|
|Read Only|True|

### EncryptionSelfTestPassed
Member of [HpeSmartStorageArrayController.v2_1_0.HpeSmartStorageArrayController](#hpesmartstoragearraycontroller-v2_1_0-hpesmartstoragearraycontroller)

| | |
|---|---|
|Description|True if the encryption self test passed, false otherwise.|
|Type|boolean|
|Read Only|True|

### EncryptionStandaloneModeEnabled
Member of [HpeSmartStorageArrayController.v2_1_0.HpeSmartStorageArrayController](#hpesmartstoragearraycontroller-v2_1_0-hpesmartstoragearraycontroller)

| | |
|---|---|
|Description|True if the controller manages encryption keys locally, false if a remote key manager is being used|
|Type|boolean|
|Read Only|True|

### EncryptionUserPasswordSet
Member of [HpeSmartStorageArrayController.v2_1_0.HpeSmartStorageArrayController](#hpesmartstoragearraycontroller-v2_1_0-hpesmartstoragearraycontroller)

| | |
|---|---|
|Description|True if a password has been set for the Encryption User, false otherwise.|
|Type|boolean|
|Read Only|True|

### ExpandPriority
Member of [HpeSmartStorageArrayController.v2_1_0.HpeSmartStorageArrayController](#hpesmartstoragearraycontroller-v2_1_0-hpesmartstoragearraycontroller)

| | |
|---|---|
|Description|The level of priority that transformations have over handling current operating system requests|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```High```|Transformations will complete as fast as possible at the expense of normal I/O|
|```Medium```|Transformations will perform with some impact on normal I/O|
|```Low```|Transformations will perform only when normal I/O is not occurring and may take longer to complete|

### ExternalPortCount
Member of [HpeSmartStorageArrayController.v2_1_0.HpeSmartStorageArrayController](#hpesmartstoragearraycontroller-v2_1_0-hpesmartstoragearraycontroller)

| | |
|---|---|
|Description|The number of external ports|
|Type|integer|
|Read Only|True|

### FirmwareVersion
**FirmwareVersion.Current**
**FirmwareVersion.Current.VersionString**
Member of [HpeSmartStorageArrayController.v2_1_0.HpeSmartStorageArrayController](#hpesmartstoragearraycontroller-v2_1_0-hpesmartstoragearraycontroller)

| | |
|---|---|
|Description|This string represents the version of the firmware image.|
|Type|string or null|
|Read Only|True|

### FlexibleLatencySchedulerSetting
Member of [HpeSmartStorageArrayController.v2_1_0.HpeSmartStorageArrayController](#hpesmartstoragearraycontroller-v2_1_0-hpesmartstoragearraycontroller)

| | |
|---|---|
|Description|This allows the controller to process certain high-latency requests after a delay that may time out when elevator sorting|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```Default```|The controller will rely only on elevator sorting|
|```Low250```|The controller will apply a cutoff value of 250ms when suspending elevator sorting|
|```Middle100```|The controller will apply a cutoff value of 100ms when suspending elevator sorting|
|```Middle50```|The controller will apply a cutoff value of 50ms when suspending elevator sorting|
|```Aggressive30```|The controller will apply a cutoff value of 30ms when suspending elevator sorting|
|```Aggressive10```|The controller will apply a cutoff value of 10ms when suspending elevator sorting|

### HardwareRevision
Member of [HpeSmartStorageArrayController.v2_1_0.HpeSmartStorageArrayController](#hpesmartstoragearraycontroller-v2_1_0-hpesmartstoragearraycontroller)

| | |
|---|---|
|Description|The hardware revision of the controller|
|Type|string|
|Read Only|True|

### InconsistencyRepairPolicy
Member of [HpeSmartStorageArrayController.v2_1_0.HpeSmartStorageArrayController](#hpesmartstoragearraycontroller-v2_1_0-hpesmartstoragearraycontroller)

| | |
|---|---|
|Description|Enables the controller to update data on RAID 6(ADG) and 60 volumes based on parity information when an inconsistency is discovered during surface scan|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```Enabled```|The controller will update the data on the drives based on the parity information|
|```Disabled```|The controller will only update the parity information and leave the data untouched|

### InternalPortCount
Member of [HpeSmartStorageArrayController.v2_1_0.HpeSmartStorageArrayController](#hpesmartstoragearraycontroller-v2_1_0-hpesmartstoragearraycontroller)

| | |
|---|---|
|Description|The number of internal ports|
|Type|integer|
|Read Only|True|

### IsBootController
Member of [HpeSmartStorageArrayController.v2_1_0.HpeSmartStorageArrayController](#hpesmartstoragearraycontroller-v2_1_0-hpesmartstoragearraycontroller)

| | |
|---|---|
|Description|True if this controller is the OS boot controller, false otherwise|
|Type|boolean|
|Read Only|True|

### Location
Member of [HpeSmartStorageArrayController.v2_1_0.HpeSmartStorageArrayController](#hpesmartstoragearraycontroller-v2_1_0-hpesmartstoragearraycontroller)

| | |
|---|---|
|Description|Location identifier|
|Type|string|
|Read Only|True|

### LocationFormat
Member of [HpeSmartStorageArrayController.v2_1_0.HpeSmartStorageArrayController](#hpesmartstoragearraycontroller-v2_1_0-hpesmartstoragearraycontroller)

| | |
|---|---|
|Description|Format for Location Identifier|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```PCISlot```|The PCI slot the controller is located at. For embedded controllers, the slot is 0|

### LogicalDriveCount
Member of [HpeSmartStorageArrayController.v2_1_0.HpeSmartStorageArrayController](#hpesmartstoragearraycontroller-v2_1_0-hpesmartstoragearraycontroller)

| | |
|---|---|
|Description|The number of logical drives configured on this controller|
|Type|integer|
|Read Only|True|

### Manufacturer
Member of [HpeSmartStorageArrayController.v2_1_0.HpeSmartStorageArrayController](#hpesmartstoragearraycontroller-v2_1_0-hpesmartstoragearraycontroller)

| | |
|---|---|
|Description|The manufacturer of the controller|
|Type|string|
|Read Only|True|

### MaxParallelSurfaceScanCount
Member of [HpeSmartStorageArrayController.v2_1_0.HpeSmartStorageArrayController](#hpesmartstoragearraycontroller-v2_1_0-hpesmartstoragearraycontroller)

| | |
|---|---|
|Description|Maximum number of disks that the controller supports scanning in parallel|
|Type|integer|
|Read Only|True|

### Model
Member of [HpeSmartStorageArrayController.v2_1_0.HpeSmartStorageArrayController](#hpesmartstoragearraycontroller-v2_1_0-hpesmartstoragearraycontroller)

| | |
|---|---|
|Description|The model number for the controller|
|Type|string|
|Read Only|True|

### OperatingModeAfterReboot
Member of [HpeSmartStorageArrayController.v2_1_0.HpeSmartStorageArrayController](#hpesmartstoragearraycontroller-v2_1_0-hpesmartstoragearraycontroller)

| | |
|---|---|
|Description|The operating mode the controller will be functioning in (RAID versus HBA) after a reboot|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```RAID```|The controller will be functioning in RAID mode after rebooting|
|```HBA```|The controller will be functioning in HBA mode after rebooting|
|```Mixed```|The controller will be functioning in Mixed mode after rebooting|

### ParallelSurfaceScanSupported
Member of [HpeSmartStorageArrayController.v2_1_0.HpeSmartStorageArrayController](#hpesmartstoragearraycontroller-v2_1_0-hpesmartstoragearraycontroller)

| | |
|---|---|
|Description|True if the controller supports scanning multiple disk surfaces|
|Type|boolean|
|Read Only|True|

### PhysicalDriveCount
Member of [HpeSmartStorageArrayController.v2_1_0.HpeSmartStorageArrayController](#hpesmartstoragearraycontroller-v2_1_0-hpesmartstoragearraycontroller)

| | |
|---|---|
|Description|The number of physical drives attached to this controller|
|Type|integer|
|Read Only|True|

### PowerModeAfterReboot
Member of [HpeSmartStorageArrayController.v2_1_0.HpeSmartStorageArrayController](#hpesmartstoragearraycontroller-v2_1_0-hpesmartstoragearraycontroller)

| | |
|---|---|
|Description|The power mode of the controller after a reboot|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```Invalid```|The controller will be operating in an unknown power mode after a reboot|
|```Low```|The controller will be operating in minimum power mode after a reboot|
|```LowAutomated```|The controller will be operating in a balanced mode after a reboot|
|```Performant```|The controller will be operating in maximum performance power mode after a reboot|

### PowerModeConfigured
Member of [HpeSmartStorageArrayController.v2_1_0.HpeSmartStorageArrayController](#hpesmartstoragearraycontroller-v2_1_0-hpesmartstoragearraycontroller)

| | |
|---|---|
|Description|The current power mode of the controller|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```Invalid```|The power mode can not be determined|
|```Low```|The controller is currently operating in minimum power mode|
|```LowAutomated```|The controller is currently operating in a balanced power mode|
|```Performant```|The controller is currently operating in maximum performance power mode|

### PowerModeWarningChangedDrive
Member of [HpeSmartStorageArrayController.v2_1_0.HpeSmartStorageArrayController](#hpesmartstoragearraycontroller-v2_1_0-hpesmartstoragearraycontroller)

| | |
|---|---|
|Description|True if the controller's drive configuration has changed while using configuration based power settings, false otherwise|
|Type|boolean|
|Read Only|True|

### PowerModeWarningChangedMode
Member of [HpeSmartStorageArrayController.v2_1_0.HpeSmartStorageArrayController](#hpesmartstoragearraycontroller-v2_1_0-hpesmartstoragearraycontroller)

| | |
|---|---|
|Description|True if the controller has a new power mode configured, false otherwise|
|Type|boolean|
|Read Only|True|

### PowerModeWarningReboot
Member of [HpeSmartStorageArrayController.v2_1_0.HpeSmartStorageArrayController](#hpesmartstoragearraycontroller-v2_1_0-hpesmartstoragearraycontroller)

| | |
|---|---|
|Description|True if a reboot is required to change the active power mode on the controller, false otherwise|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```NotRequired```|No reboot is required|
|```RequiredNoReason```|A reboot is required for the configured power mode on the controller|
|```RequiredPowerSavings```|Rebooting will enable additional power savings on the controller|
|```RequiredPerformance```|Rebooting will enhance the performance of the controller|

### PowerModeWarningTemperature
Member of [HpeSmartStorageArrayController.v2_1_0.HpeSmartStorageArrayController](#hpesmartstoragearraycontroller-v2_1_0-hpesmartstoragearraycontroller)

| | |
|---|---|
|Description|True if the controller has crossed a critical temperature threshold and performance has been reduced to prevent damage to the controller, false otherwise|
|Type|boolean|
|Read Only|True|

### PredictiveSpareRebuild
Member of [HpeSmartStorageArrayController.v2_1_0.HpeSmartStorageArrayController](#hpesmartstoragearraycontroller-v2_1_0-hpesmartstoragearraycontroller)

| | |
|---|---|
|Description|Enables or disables predictive spare rebuild mode|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```Enabled```|Spare drives will replace physical drives that are predicted to fail preemptively|
|```Disabled```|Spare drives will replace physical drives only when they fail|

### QueueDepth
Member of [HpeSmartStorageArrayController.v2_1_0.HpeSmartStorageArrayController](#hpesmartstoragearraycontroller-v2_1_0-hpesmartstoragearraycontroller)

| | |
|---|---|
|Description|This sets the maximum number of requests the controller will submit to a drive at any given time|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```2```|2 requests|
|```4```|4 requests|
|```8```|8 requests|
|```16```|16 requests|
|```32```|32 requests|
|```Automatic```|Automatically determine the best queue depth for the controller|

### ReadCachePercent
Member of [HpeSmartStorageArrayController.v2_1_0.HpeSmartStorageArrayController](#hpesmartstoragearraycontroller-v2_1_0-hpesmartstoragearraycontroller)

| | |
|---|---|
|Description|This indicates the percentage of cache used for read cache on the controller, with the rest of the cache being used for write cache|
|Type|integer or null|
|Read Only|False|

### RebuildPriority
Member of [HpeSmartStorageArrayController.v2_1_0.HpeSmartStorageArrayController](#hpesmartstoragearraycontroller-v2_1_0-hpesmartstoragearraycontroller)

| | |
|---|---|
|Description|The level of priority that rebuilds have over handling current operating system requests|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```High```|Rebuilds will complete as fast as possible at the expense of normal I/O|
|```Medium```|Rebuilds will perform with some impact on normal I/O|
|```Low```|Rebuilds will perform only when normal I/O is not occurring and may take longer to complete|
|```RapidHigh```|Rebuilds will complete as fast as possible at the expense of normal I/O|
|```RapidMediumHigh```|Rebuilds will perform with an impact on normal I/O|
|```RapidMedium```|Rebuilds will perform with some impact on normal I/O|
|```RapidLow```|Rebuilds will perform only when normal I/O is not occurring and may take longer to complete|

### SerialNumber
Member of [HpeSmartStorageArrayController.v2_1_0.HpeSmartStorageArrayController](#hpesmartstoragearraycontroller-v2_1_0-hpesmartstoragearraycontroller)

| | |
|---|---|
|Description|The serial number for this controller|
|Type|string|
|Read Only|True|

### SoftwareRaidHbaFirmwareRev
Member of [HpeSmartStorageArrayController.v2_1_0.HpeSmartStorageArrayController](#hpesmartstoragearraycontroller-v2_1_0-hpesmartstoragearraycontroller)

| | |
|---|---|
|Description|The firmware version of the underlying HBA that is being used by the software RAID stack|
|Type|string|
|Read Only|True|

### SoftwareRaidHbaModeOptionRomRev
Member of [HpeSmartStorageArrayController.v2_1_0.HpeSmartStorageArrayController](#hpesmartstoragearraycontroller-v2_1_0-hpesmartstoragearraycontroller)

| | |
|---|---|
|Description|The option ROM firmware version used to bootstrap the software RAID stack|
|Type|string|
|Read Only|True|

### SparePhysicalDriveCount
Member of [HpeSmartStorageArrayController.v2_1_0.HpeSmartStorageArrayController](#hpesmartstoragearraycontroller-v2_1_0-hpesmartstoragearraycontroller)

| | |
|---|---|
|Description|he number of physical drives assigned as spare drives attached to this controller|
|Type|integer|
|Read Only|True|

### Status
Member of [HpeSmartStorageArrayController.v2_1_0.HpeSmartStorageArrayController](#hpesmartstoragearraycontroller-v2_1_0-hpesmartstoragearraycontroller)
See the Redfish standard schema and specification for information on common Status object.

### SupportedOperatingModes (array)
Member of [HpeSmartStorageArrayController.v2_1_0.HpeSmartStorageArrayController](#hpesmartstoragearraycontroller-v2_1_0-hpesmartstoragearraycontroller)
```SupportedOperatingModes``` is an array containing elements of:


| | |
|---|---|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```RAID```|The controller supports functioning in RAID mode|
|```HBA```|The controller supports functioning in HBA mode|
|```Mixed```|The controller supports functioning in Mixed mode|

### SupportedPowerModes (array)
Member of [HpeSmartStorageArrayController.v2_1_0.HpeSmartStorageArrayController](#hpesmartstoragearraycontroller-v2_1_0-hpesmartstoragearraycontroller)
```SupportedPowerModes``` is an array containing elements of:


| | |
|---|---|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```Low```|The controller is currently operating in minimum power mode|
|```LowAutomated```|The controller is currently operating in a balanced power mode|
|```Performant```|The controller is currently operating in maximum performance power mode|

### SupportedRaidLevels (array)
Member of [HpeSmartStorageArrayController.v2_1_0.HpeSmartStorageArrayController](#hpesmartstoragearraycontroller-v2_1_0-hpesmartstoragearraycontroller)
```SupportedRaidLevels``` is an array containing elements of:


| | |
|---|---|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```0```|There is no fault tolerance used on the logical drive|
|```1```|Two sets of duplicate data is being stored on a pair of drives|
|```1ADM```|Three sets of duplicate data is being stored on a trio of drives|
|```10```|Data is duplicated and striped across pairs of disk drives|
|```10ADM```|Data is duplicated and striped across trios of disk drives|
|```5```|Fault tolerance is achieved by storing parity data across 3 or more disk drives|
|```50```|Fault tolerance is achieved by storing parity data and striping the data across 6 or more disk drives|
|```6```|Fault tolerance is achieved by storing multiple sets parity data across 4 or more disk drives|
|```60```|Fault tolerance is achieved by storing multiple sets parity data and striping the data across 8 or more disk drives|

### SurfaceScanAnalysisPriority
Member of [HpeSmartStorageArrayController.v2_1_0.HpeSmartStorageArrayController](#hpesmartstoragearraycontroller-v2_1_0-hpesmartstoragearraycontroller)

| | |
|---|---|
|Description|Priority that the controller takes to find and correct disk surface errors|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```Disabled```|Surface scan is disabled and may lead to data loss|
|```High```|Surface scan commands will be sent with the host I/O, resulting in faster scanning, but may inpact host I/O performance|
|```Medium```|Surface scan commands have a medium priority, and will have some impact on host I/O performance|
|```Low```|Surface scan commands have a low priority, and will have little impact on host I/O performance|
|```Idle```|Surface scan commands will ony be issued when no host I/O is present after a delay|

### UnassignedPhysicalDriveCount
Member of [HpeSmartStorageArrayController.v2_1_0.HpeSmartStorageArrayController](#hpesmartstoragearraycontroller-v2_1_0-hpesmartstoragearraycontroller)

| | |
|---|---|
|Description|The number of unassigned physical drives attached to this controller|
|Type|integer|
|Read Only|True|

### WriteCacheBypassThresholdKB
Member of [HpeSmartStorageArrayController.v2_1_0.HpeSmartStorageArrayController](#hpesmartstoragearraycontroller-v2_1_0-hpesmartstoragearraycontroller)

| | |
|---|---|
|Description|This value sets the write cache bypass threshold, ranging from 16 KB to 1040 KB in multiples of 16 KB, where all writes larger than the specified value in KB units will bypass the write cache and be written directly to the disk for non-parity RAID volumes.|
|Type|integer or null|
|Read Only|True|

### WriteCacheWithoutBackupPowerEnabled
Member of [HpeSmartStorageArrayController.v2_1_0.HpeSmartStorageArrayController](#hpesmartstoragearraycontroller-v2_1_0-hpesmartstoragearraycontroller)

| | |
|---|---|
|Description|True if the controller will continue to use write cache even if the backup power source is not available. False, otherwise.|
|Type|boolean|
|Read Only|True|

## HpeSmartStorageDiskDrive.v2_0_0.HpeSmartStorageDiskDrive
```@odata.type: "#HpeSmartStorageDiskDrive.v2_0_0.HpeSmartStorageDiskDrive"```

HpSmartStorageDiskDrive
### Resource Instances
|Uri|HTTP Allow|
|---|---|
|```/redfish/v1/systems/{item}/smartstorage/arraycontrollers/{item}/diskdrives/{item}/```||
|```/redfish/v1/systems/{item}/smartstorage/arraycontrollers/{item}/unconfigureddrives/{item}/```||
|```/redfish/v1/systems/{item}/smartstorage/hostbusadapters/{item}/diskdrives/{item}/```||

### BlockSizeBytes
Member of [HpeSmartStorageDiskDrive.v2_0_0.HpeSmartStorageDiskDrive](#hpesmartstoragediskdrive-v2_0_0-hpesmartstoragediskdrive)

| | |
|---|---|
|Description|Block size of the drive in bytes. This is the block size presented by the drive to clients such as the array controller or operating system.|
|Type|integer|
|Read Only|True|

### CapacityGB
Member of [HpeSmartStorageDiskDrive.v2_0_0.HpeSmartStorageDiskDrive](#hpesmartstoragediskdrive-v2_0_0-hpesmartstoragediskdrive)

| | |
|---|---|
|Description|Total capacity of the drive in GB. This denotes the marketing capacity (base 10)|
|Type|integer|
|Read Only|True|

### CapacityLogicalBlocks
Member of [HpeSmartStorageDiskDrive.v2_0_0.HpeSmartStorageDiskDrive](#hpesmartstoragediskdrive-v2_0_0-hpesmartstoragediskdrive)

| | |
|---|---|
|Description|Total number of logical blocks in the drive|
|Type|integer|
|Read Only|True|

### CapacityMiB
Member of [HpeSmartStorageDiskDrive.v2_0_0.HpeSmartStorageDiskDrive](#hpesmartstoragediskdrive-v2_0_0-hpesmartstoragediskdrive)

| | |
|---|---|
|Description|Total capacity of the drive in MiB|
|Type|integer|
|Read Only|True|

### CarrierApplicationVersion
Member of [HpeSmartStorageDiskDrive.v2_0_0.HpeSmartStorageDiskDrive](#hpesmartstoragediskdrive-v2_0_0-hpesmartstoragediskdrive)

| | |
|---|---|
|Description|Carrier PIC firmware version currently running|
|Type|string|
|Read Only|True|

### CarrierAuthenticationStatus
Member of [HpeSmartStorageDiskDrive.v2_0_0.HpeSmartStorageDiskDrive](#hpesmartstoragediskdrive-v2_0_0-hpesmartstoragediskdrive)

| | |
|---|---|
|Description|Authentication status of the drive carrier|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```OK```|Carrier authenticated as genuine HPE product|
|```Fail```|Carrier authentication failed|
|```NoCommunication```|Communication could not be established with the carrier|
|```NotApplicable```|Carrier does not support authentication|

### CurrentTemperatureCelsius
Member of [HpeSmartStorageDiskDrive.v2_0_0.HpeSmartStorageDiskDrive](#hpesmartstoragediskdrive-v2_0_0-hpesmartstoragediskdrive)

| | |
|---|---|
|Description|The current temperature of the drive|
|Type|integer|
|Read Only|True|

### DiskDriveStatusReasons (array)
Member of [HpeSmartStorageDiskDrive.v2_0_0.HpeSmartStorageDiskDrive](#hpesmartstoragediskdrive-v2_0_0-hpesmartstoragediskdrive)
```DiskDriveStatusReasons``` is an array containing elements of:


| | |
|---|---|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```None```|No status reason available|
|```Unknown```|Reason is unknown|
|```CommunicationFailure```|Cannot communicate with drive|
|```Zoned```|Drive is currently zoned, only basic information can be displayed|
|```EraseInProgress```|Drive is currently in process of an erase operation|
|```QueuedForErase```|Drive is currently queued for an erase operation|
|```EraseCompleted```|Drive has completed the erase operation|
|```EraseFailed```|The erase operation has failed for the drive|
|```EraseAborted```|The erase operation was aborted|
|```Failed```|The drive has failed|
|```NonAuthenticDrive```|The drive is not an authentic drive|
|```CarrierCommunicationFailure```|The drive carrier has a communication fault|
|```PredictiveFail```|Drive failure is imminent|
|```NotSupported```|The drive is not supported by the controller|
|```SizeNotValid```|The drive size is invalid. Typically occurs if a drive part of a raid volume is replaced with a smaller sized drive|
|```FailedDueToPredictiveSpareActivation```|The drive was failed due to a predictive spare activation|
|```Rebuilding```|The drive is currently rebuilding|
|```TransientDataDrive```|The drive is part of a volume that is currently undergoing a transformation. After the transformation is complete the drive's state will change|
|```Unrecoverable```|The drive is in an unrecoverable condition|

### DiskDriveUse
Member of [HpeSmartStorageDiskDrive.v2_0_0.HpeSmartStorageDiskDrive](#hpesmartstoragediskdrive-v2_0_0-hpesmartstoragediskdrive)

| | |
|---|---|
|Description|The current use of the physical drive.|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```Data```|It is a Data drive which is a part of an array.|
|```Spare```|It is a spare drive which is a part of an array.|
|```Raw```|Indicates the drive is available to the OS via HBA mode on the controller.|
|```Unconfigured```|Indicates the drive is not available to the OS as controller is in RAID mode.|
|```Unknown```|The current use of the disk drive is not known.|

### EncryptedDrive
Member of [HpeSmartStorageDiskDrive.v2_0_0.HpeSmartStorageDiskDrive](#hpesmartstoragediskdrive-v2_0_0-hpesmartstoragediskdrive)

| | |
|---|---|
|Description|True if encryption is currently enabled on this disk drive, false otherwise|
|Type|boolean|
|Read Only|True|

### EraseCompletionPercentage
Member of [HpeSmartStorageDiskDrive.v2_0_0.HpeSmartStorageDiskDrive](#hpesmartstoragediskdrive-v2_0_0-hpesmartstoragediskdrive)

| | |
|---|---|
|Description|The percent complete for an erase operation currently occurring on the disk drive or null if not currently erasing a drive.|
|Type|integer or null|
|Read Only|True|

### ErasePattern
Member of [HpeSmartStorageDiskDrive.v2_0_0.HpeSmartStorageDiskDrive](#hpesmartstoragediskdrive-v2_0_0-hpesmartstoragediskdrive)

| | |
|---|---|
|Description|The pattern used for erasing the disk drive|
|Type|string|
|Read Only|True|

### FirmwareVersion
**FirmwareVersion.Current**
**FirmwareVersion.Current.VersionString**
Member of [HpeSmartStorageDiskDrive.v2_0_0.HpeSmartStorageDiskDrive](#hpesmartstoragediskdrive-v2_0_0-hpesmartstoragediskdrive)

| | |
|---|---|
|Description|This string represents the version of the firmware image.|
|Type|string or null|
|Read Only|True|

### IndicatorLED
Member of [HpeSmartStorageDiskDrive.v2_0_0.HpeSmartStorageDiskDrive](#hpesmartstoragediskdrive-v2_0_0-hpesmartstoragediskdrive)

| | |
|---|---|
|Description|The state of the indicator LED.|
|Type|string or null|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```Null```|A value is temporarily unavailable|
|```Unknown```|The state of the Indicator LED cannot be determined.|
|```Lit```|The Indicator LED is lit.|
|```Blinking```|The Indicator LED is blinking.|
|```Off```|The Indicator LED is off.|

### InterfaceSpeedMbps
Member of [HpeSmartStorageDiskDrive.v2_0_0.HpeSmartStorageDiskDrive](#hpesmartstoragediskdrive-v2_0_0-hpesmartstoragediskdrive)

| | |
|---|---|
|Description|Native interface speed for the device|
|Type|integer|
|Read Only|True|

### InterfaceType
Member of [HpeSmartStorageDiskDrive.v2_0_0.HpeSmartStorageDiskDrive](#hpesmartstoragediskdrive-v2_0_0-hpesmartstoragediskdrive)

| | |
|---|---|
|Description|The connection interface of the drive. The value NVME has been deprecated.|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```SAS```|SAS|
|```SATA```|SATA|
|```NVME```|Non-volatile memory (deprecated)|
|```PCIe```|PCIe interface|
|```Unknown```|Information is unavailable|

### LegacyBootPriority
Member of [HpeSmartStorageDiskDrive.v2_0_0.HpeSmartStorageDiskDrive](#hpesmartstoragediskdrive-v2_0_0-hpesmartstoragediskdrive)

| | |
|---|---|
|Description|This indicates that the array controller should provide legacy boot support.|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```Primary```|This indicates that the array controller should provide legacy boot support (Interrupt 13h BIOS support) for this physical drive. The physical drive will be listed as first in the LUN list returned via SCSI commands|
|```Secondary```|This indicates that the array controller should provide legacy boot support (Interrupt 13h BIOS support) for this physical drive. The physical drive will be listed as second in the LUN list returned via SCSI commands|
|```None```|Legacy boot not supported on this physical drive|

### Location
Member of [HpeSmartStorageDiskDrive.v2_0_0.HpeSmartStorageDiskDrive](#hpesmartstoragediskdrive-v2_0_0-hpesmartstoragediskdrive)

| | |
|---|---|
|Description|The location of the drive|
|Type|string|
|Read Only|True|

### LocationFormat
Member of [HpeSmartStorageDiskDrive.v2_0_0.HpeSmartStorageDiskDrive](#hpesmartstoragediskdrive-v2_0_0-hpesmartstoragediskdrive)

| | |
|---|---|
|Description|Format for the location property|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```ControllerPort:Box:Bay```|This format typically used in controller context where the drive would be identified using the controller port, JBOD box number and drive bay|
|```SwitchPort:Box:Bay```|This format typically used in a SAS switch context where the drive would be identified using the switch port, JBOD box number and drive bay|
|```SwitchPort:SwitchBay:Bay```|This format typically used in a SAS switch context where the drive would be identified using the switch port, ICM bay number for the switch and drive bay|

### Manufacturer
Member of [HpeSmartStorageDiskDrive.v2_0_0.HpeSmartStorageDiskDrive](#hpesmartstoragediskdrive-v2_0_0-hpesmartstoragediskdrive)

| | |
|---|---|
|Description|Manufacturer of the disk drive|
|Type|string|
|Read Only|True|

### MaximumTemperatureCelsius
Member of [HpeSmartStorageDiskDrive.v2_0_0.HpeSmartStorageDiskDrive](#hpesmartstoragediskdrive-v2_0_0-hpesmartstoragediskdrive)

| | |
|---|---|
|Description|The maximum recommended temperature for the drive|
|Type|integer|
|Read Only|True|

### MediaType
Member of [HpeSmartStorageDiskDrive.v2_0_0.HpeSmartStorageDiskDrive](#hpesmartstoragediskdrive-v2_0_0-hpesmartstoragediskdrive)

| | |
|---|---|
|Description|Type of disk|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```HDD```|The drive media type is traditional magnetic platters|
|```SSD```|The drive media type is solid state or flash memory|
|```SMR```|The drive media type is shingled magnetic recording|

### MinimumGoodFirmwareVersion
Member of [HpeSmartStorageDiskDrive.v2_0_0.HpeSmartStorageDiskDrive](#hpesmartstoragediskdrive-v2_0_0-hpesmartstoragediskdrive)

| | |
|---|---|
|Description|The minimum recommended firmware revision for the drive|
|Type|string|
|Read Only|True|

### Model
Member of [HpeSmartStorageDiskDrive.v2_0_0.HpeSmartStorageDiskDrive](#hpesmartstoragediskdrive-v2_0_0-hpesmartstoragediskdrive)

| | |
|---|---|
|Description|Drive model number|
|Type|string|
|Read Only|True|

### NativeBlockSizeBytes
Member of [HpeSmartStorageDiskDrive.v2_0_0.HpeSmartStorageDiskDrive](#hpesmartstoragediskdrive-v2_0_0-hpesmartstoragediskdrive)

| | |
|---|---|
|Description|Native block size of the drive in bytes. This is the underlying sector size used by the physical drive to store data. For example, an advanced format drive that uses 4K sector sizes to store data will return 4K as the NativeBlockSizeBytes but may return 512 for the BlockSizeBytes when running in 512e (emulation) mode for backward compatibility|
|Type|integer|
|Read Only|True|

### PhyCount
Member of [HpeSmartStorageDiskDrive.v2_0_0.HpeSmartStorageDiskDrive](#hpesmartstoragediskdrive-v2_0_0-hpesmartstoragediskdrive)

| | |
|---|---|
|Description|The number of phys the drive has|
|Type|integer|
|Read Only|True|

### PortCount
Member of [HpeSmartStorageDiskDrive.v2_0_0.HpeSmartStorageDiskDrive](#hpesmartstoragediskdrive-v2_0_0-hpesmartstoragediskdrive)

| | |
|---|---|
|Description|The number of ports on the drive. Typically 1 (single-domain) or 2 (dual-domain)|
|Type|integer|
|Read Only|True|

### PowerOnHours
Member of [HpeSmartStorageDiskDrive.v2_0_0.HpeSmartStorageDiskDrive](#hpesmartstoragediskdrive-v2_0_0-hpesmartstoragediskdrive)

| | |
|---|---|
|Description|The number of lifetime hours that the drive has been powered on. The value is null if the disk power on hours cannot be determined or is not supported.|
|Type|integer or null|
|Read Only|True|

### RotationalSpeedRpm
Member of [HpeSmartStorageDiskDrive.v2_0_0.HpeSmartStorageDiskDrive](#hpesmartstoragediskdrive-v2_0_0-hpesmartstoragediskdrive)

| | |
|---|---|
|Description|The rotational speed of the drive, only applicable on HDDs|
|Type|integer|
|Read Only|True|

### SSDEnduranceUtilizationPercentage
Member of [HpeSmartStorageDiskDrive.v2_0_0.HpeSmartStorageDiskDrive](#hpesmartstoragediskdrive-v2_0_0-hpesmartstoragediskdrive)

| | |
|---|---|
|Description|This is the percentage of the drive that has been worn out and can no longer be used. When this values reaches 100%, the drive has 0% usage remaining and is completely worn out. The value is null if percent endurance used cannot be determined or is not supported.|
|Type|integer or null|
|Read Only|True|

### SerialNumber
Member of [HpeSmartStorageDiskDrive.v2_0_0.HpeSmartStorageDiskDrive](#hpesmartstoragediskdrive-v2_0_0-hpesmartstoragediskdrive)

| | |
|---|---|
|Description|The serial number of the drive|
|Type|string|
|Read Only|True|

### SpareRebuildMode
Member of [HpeSmartStorageDiskDrive.v2_0_0.HpeSmartStorageDiskDrive](#hpesmartstoragediskdrive-v2_0_0-hpesmartstoragediskdrive)

| | |
|---|---|
|Description|Method to used activate this drive when another drive fails, this is only applicable if the drive is configured as a spare drive|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```Dedicated```|This drive will take over a failed drive temporarily. When the failed drive is replaced, this will return to being a spare. This drive be shared between arrays.|
|```Roaming```|This drive will permanently replace a failed drive. The failed drive will become a spare. This spare drive cannot be shared between arrays.|

### Status
Member of [HpeSmartStorageDiskDrive.v2_0_0.HpeSmartStorageDiskDrive](#hpesmartstoragediskdrive-v2_0_0-hpesmartstoragediskdrive)
See the Redfish standard schema and specification for information on common Status object.

### TransferSpeedMbps
Member of [HpeSmartStorageDiskDrive.v2_0_0.HpeSmartStorageDiskDrive](#hpesmartstoragediskdrive-v2_0_0-hpesmartstoragediskdrive)

| | |
|---|---|
|Description|Effective transfer speed to the device taking into account hardware acceleration such as edge-buffering|
|Type|integer|
|Read Only|True|

### WWID
Member of [HpeSmartStorageDiskDrive.v2_0_0.HpeSmartStorageDiskDrive](#hpesmartstoragediskdrive-v2_0_0-hpesmartstoragediskdrive)

| | |
|---|---|
|Description|Unique identifier for the device|
|Type|string|
|Read Only|True|

## HpeSmartStorageHostBusAdapter.v2_0_0.HpeSmartStorageHostBusAdapter
```@odata.type: "#HpeSmartStorageHostBusAdapter.v2_0_0.HpeSmartStorageHostBusAdapter"```

HpSmartStorageHostBusAdapter
### Resource Instances
|Uri|HTTP Allow|
|---|---|
|```/redfish/v1/systems/{item}/smartstorage/hostbusadapters/{item}/```|GET |

### Links to other Resources
|Link Name|Destination type
|---|---|
|```Links/Drives```|Collection of [HpeSmartStorageDiskDrive](#hpesmartstoragediskdrive-v2_0_0-hpesmartstoragediskdrive)|

### FirmwareVersion
**FirmwareVersion.Current**
**FirmwareVersion.Current.VersionString**
Member of [HpeSmartStorageHostBusAdapter.v2_0_0.HpeSmartStorageHostBusAdapter](#hpesmartstoragehostbusadapter-v2_0_0-hpesmartstoragehostbusadapter)

| | |
|---|---|
|Description|This string represents the version of the firmware image.|
|Type|string or null|
|Read Only|True|

### HardwareRevision
Member of [HpeSmartStorageHostBusAdapter.v2_0_0.HpeSmartStorageHostBusAdapter](#hpesmartstoragehostbusadapter-v2_0_0-hpesmartstoragehostbusadapter)

| | |
|---|---|
|Description|The hardware revision of the controller|
|Type|string|
|Read Only|True|

### Location
Member of [HpeSmartStorageHostBusAdapter.v2_0_0.HpeSmartStorageHostBusAdapter](#hpesmartstoragehostbusadapter-v2_0_0-hpesmartstoragehostbusadapter)

| | |
|---|---|
|Description|Location identifier|
|Type|string|
|Read Only|True|

### LocationFormat
Member of [HpeSmartStorageHostBusAdapter.v2_0_0.HpeSmartStorageHostBusAdapter](#hpesmartstoragehostbusadapter-v2_0_0-hpesmartstoragehostbusadapter)

| | |
|---|---|
|Description|Format for Location Identifier|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```PCISlot```|The PCI slot the controller is located at. For embedded controllers, the slot is 0|

### Manufacturer
Member of [HpeSmartStorageHostBusAdapter.v2_0_0.HpeSmartStorageHostBusAdapter](#hpesmartstoragehostbusadapter-v2_0_0-hpesmartstoragehostbusadapter)

| | |
|---|---|
|Description|The manufacturer of the controller|
|Type|string|
|Read Only|True|

### Model
Member of [HpeSmartStorageHostBusAdapter.v2_0_0.HpeSmartStorageHostBusAdapter](#hpesmartstoragehostbusadapter-v2_0_0-hpesmartstoragehostbusadapter)

| | |
|---|---|
|Description|The model number for the controller|
|Type|string|
|Read Only|True|

### SerialNumber
Member of [HpeSmartStorageHostBusAdapter.v2_0_0.HpeSmartStorageHostBusAdapter](#hpesmartstoragehostbusadapter-v2_0_0-hpesmartstoragehostbusadapter)

| | |
|---|---|
|Description|The serial number for this controller|
|Type|string|
|Read Only|True|

### Status
Member of [HpeSmartStorageHostBusAdapter.v2_0_0.HpeSmartStorageHostBusAdapter](#hpesmartstoragehostbusadapter-v2_0_0-hpesmartstoragehostbusadapter)
See the Redfish standard schema and specification for information on common Status object.

## HpeSmartStorageLogicalDrive.v2_1_0.HpeSmartStorageLogicalDrive
```@odata.type: "#HpeSmartStorageLogicalDrive.v2_1_0.HpeSmartStorageLogicalDrive"```

HpSmartStorageLogicalDrive
### Resource Instances
|Uri|HTTP Allow|
|---|---|
|```/redfish/v1/systems/{item}/smartstorage/arraycontrollers/{item}/logicaldrives/{item}/```||

### Links to other Resources
|Link Name|Destination type
|---|---|
|```Links/DataDrives```|Collection of [HpeSmartStorageDiskDrive](#hpesmartstoragediskdrive-v2_0_0-hpesmartstoragediskdrive)|

### AccelerationMethod
Member of [HpeSmartStorageLogicalDrive.v2_1_0.HpeSmartStorageLogicalDrive](#hpesmartstoragelogicaldrive-v2_1_0-hpesmartstoragelogicaldrive)

| | |
|---|---|
|Description|The acceleration method of the logical drive|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```None```|Logical drive acceleration is disabled|
|```ControllerCache```|Reads and writes to the logical drive are being cached by the controller.|
|```IOBypass```|For logical drives on SSDs, read and write information directly from the drive.|

### BlockSizeBytes
Member of [HpeSmartStorageLogicalDrive.v2_1_0.HpeSmartStorageLogicalDrive](#hpesmartstoragelogicaldrive-v2_1_0-hpesmartstoragelogicaldrive)

| | |
|---|---|
|Description|The block size of the disk drive in bytes|
|Type|integer|
|Read Only|True|

### CapacityMiB
Member of [HpeSmartStorageLogicalDrive.v2_1_0.HpeSmartStorageLogicalDrive](#hpesmartstoragelogicaldrive-v2_1_0-hpesmartstoragelogicaldrive)

| | |
|---|---|
|Description|Total usable capacity available on this logical drive in MiB units|
|Type|integer|
|Read Only|True|

### DriveAccessName
Member of [HpeSmartStorageLogicalDrive.v2_1_0.HpeSmartStorageLogicalDrive](#hpesmartstoragelogicaldrive-v2_1_0-hpesmartstoragelogicaldrive)

| | |
|---|---|
|Description|The access ID of the logical drive given by the OS|
|Type|string|
|Read Only|True|

### DriveGeometryCylinders
Member of [HpeSmartStorageLogicalDrive.v2_1_0.HpeSmartStorageLogicalDrive](#hpesmartstoragelogicaldrive-v2_1_0-hpesmartstoragelogicaldrive)

| | |
|---|---|
|Description|The number of cylinders on the drive|
|Type|string|
|Read Only|True|

### DriveGeometryHeads
Member of [HpeSmartStorageLogicalDrive.v2_1_0.HpeSmartStorageLogicalDrive](#hpesmartstoragelogicaldrive-v2_1_0-hpesmartstoragelogicaldrive)

| | |
|---|---|
|Description|The number of heads on the drive|
|Type|string|
|Read Only|True|

### DriveGeometrySectors
Member of [HpeSmartStorageLogicalDrive.v2_1_0.HpeSmartStorageLogicalDrive](#hpesmartstoragelogicaldrive-v2_1_0-hpesmartstoragelogicaldrive)

| | |
|---|---|
|Description|The number of sectors on the drive|
|Type|string|
|Read Only|True|

### InterfaceType
Member of [HpeSmartStorageLogicalDrive.v2_1_0.HpeSmartStorageLogicalDrive](#hpesmartstoragelogicaldrive-v2_1_0-hpesmartstoragelogicaldrive)

| | |
|---|---|
|Description|The connection interface of the logical drive.|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```SAS```|SAS|
|```SATA```|SATA|
|```Mixed```|Contains both SAS and SATA.|
|```Unknown```|Information is unavailable|

### LegacyBootPriority
Member of [HpeSmartStorageLogicalDrive.v2_1_0.HpeSmartStorageLogicalDrive](#hpesmartstoragelogicaldrive-v2_1_0-hpesmartstoragelogicaldrive)

| | |
|---|---|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```Primary```|This indicates that the array controller should provide legacy boot support (Interrupt 13h BIOS support) for this logical drive. The logical drive will be listed as first in the LUN list returned via SCSI commands|
|```Secondary```|This indicates that the array controller should provide legacy boot support (Interrupt 13h BIOS support) for this logical drive. The logical drive will be listed as second in the LUN list returned via SCSI commands|
|```None```|Legacy boot not supported on this logical drive|

### LogicalDriveEncryption
Member of [HpeSmartStorageLogicalDrive.v2_1_0.HpeSmartStorageLogicalDrive](#hpesmartstoragelogicaldrive-v2_1_0-hpesmartstoragelogicaldrive)

| | |
|---|---|
|Description|True if encryption is currently enabled on this logical drive, false otherwise|
|Type|boolean|
|Read Only|True|

### LogicalDriveEncryptionDataKeysVolatile
Member of [HpeSmartStorageLogicalDrive.v2_1_0.HpeSmartStorageLogicalDrive](#hpesmartstoragelogicaldrive-v2_1_0-hpesmartstoragelogicaldrive)

| | |
|---|---|
|Description|True if volatile keys are enabled for encryption, false otherwise|
|Type|boolean|
|Read Only|True|

### LogicalDriveEncryptionDataKeysVolatileBackup
Member of [HpeSmartStorageLogicalDrive.v2_1_0.HpeSmartStorageLogicalDrive](#hpesmartstoragelogicaldrive-v2_1_0-hpesmartstoragelogicaldrive)

| | |
|---|---|
|Description|True if volatile keys are backed up to a remote key manager, false if volatile keys are not backed up|
|Type|boolean|
|Read Only|True|

### LogicalDriveEncryptionDataKeysVolatileStatus
Member of [HpeSmartStorageLogicalDrive.v2_1_0.HpeSmartStorageLogicalDrive](#hpesmartstoragelogicaldrive-v2_1_0-hpesmartstoragelogicaldrive)

| | |
|---|---|
|Description|The status of the encryption volatile keys|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```NoOp```|No operations are pending for the volatile keys|
|```BackupInProgress```|The volatile keys are being backed up to a remote key manager|
|```BackupAndSetInProgress```|The volatile keys are being set and being backed up to a remote key manager|
|```RestoreInProgress```|The volatile keys are being restored from a remote key manager|
|```DeleteInProgress```|The volatile keys are being removed|

### LogicalDriveName
Member of [HpeSmartStorageLogicalDrive.v2_1_0.HpeSmartStorageLogicalDrive](#hpesmartstoragelogicaldrive-v2_1_0-hpesmartstoragelogicaldrive)

| | |
|---|---|
|Description|Label given to the logical drive|
|Type|string|
|Read Only|True|

### LogicalDriveNumber
Member of [HpeSmartStorageLogicalDrive.v2_1_0.HpeSmartStorageLogicalDrive](#hpesmartstoragelogicaldrive-v2_1_0-hpesmartstoragelogicaldrive)

| | |
|---|---|
|Description|logical drive number|
|Type|integer|
|Read Only|True|

### LogicalDriveType
Member of [HpeSmartStorageLogicalDrive.v2_1_0.HpeSmartStorageLogicalDrive](#hpesmartstoragelogicaldrive-v2_1_0-hpesmartstoragelogicaldrive)

| | |
|---|---|
|Description|How the logical drive is being used|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```Data```|The drive is being used as a storage drive|
|```Cache```|The drive is being used as a cache drive for a different storage drive|
|```SplitMirrorSetPrimary```|This drive is being used as the primary storage drive of a split mirror set after a Split Mirror Array has been performed|
|```SplitMirrorSetBackup```|This drive is being used as the backup storage drive of a split mirror set after a Split Mirror Array has been performed|
|```SplitMirrorSetBackupOrphan```|This drive was being used as the backup storage drive of a split mirror set that no longer exists|

### MediaType
Member of [HpeSmartStorageLogicalDrive.v2_1_0.HpeSmartStorageLogicalDrive](#hpesmartstoragelogicaldrive-v2_1_0-hpesmartstoragelogicaldrive)

| | |
|---|---|
|Description|Type of the disk this logical drive is associated with.|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```HDD```|Spinning disk hard drive.|
|```SSD```|Solid state disk.|
|```SMR```|Shingled Magnetic Recording.|
|```Mixed```|Contains both HDD and SSD.|
|```Unknown```|Information is unavailable|

### ParityInitializationCompletionPercentage
Member of [HpeSmartStorageLogicalDrive.v2_1_0.HpeSmartStorageLogicalDrive](#hpesmartstoragelogicaldrive-v2_1_0-hpesmartstoragelogicaldrive)

| | |
|---|---|
|Description|Parity initialization complete percentage for a parity based logical drive (e.g. RAID 5)|
|Type|integer|
|Read Only|True|

### ParityInitializationType
Member of [HpeSmartStorageLogicalDrive.v2_1_0.HpeSmartStorageLogicalDrive](#hpesmartstoragelogicaldrive-v2_1_0-hpesmartstoragelogicaldrive)

| | |
|---|---|
|Description|When creating a logical drive with a RAID level that requires parity, parity blocks can be initialized with two different methods|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```Default```|Parity blocks are initialized in the background and the logical drive is available during this time|
|```Rapid```|Both data and parity blocks are initialized in the foreground and the logical drive will not be available to the operating system until initialization completes|

### PartitionInformation
Member of [HpeSmartStorageLogicalDrive.v2_1_0.HpeSmartStorageLogicalDrive](#hpesmartstoragelogicaldrive-v2_1_0-hpesmartstoragelogicaldrive)

| | |
|---|---|
|Description|OS partition information for the drive|
|Type|string|
|Read Only|True|

### Raid
Member of [HpeSmartStorageLogicalDrive.v2_1_0.HpeSmartStorageLogicalDrive](#hpesmartstoragelogicaldrive-v2_1_0-hpesmartstoragelogicaldrive)

| | |
|---|---|
|Description|The current RAID level configured on the logical drive|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```0```|There is no fault tolerance used on this logical drive|
|```1```|Two sets of duplicate data is being stored on a pair of drives|
|```1ADM```|Three sets of duplicate data is being stored on a trio of drives|
|```10```|Data is duplicated and striped across pairs of disk drives|
|```10ADM```|Data is duplicated and striped across trios of disk drives|
|```5```|Fault tolerance is achieved by storing parity data across 3 or more disk drives|
|```50```|Fault tolerance is achieved by storing parity data and striping the data across 6 or more disk drives|
|```6```|Fault tolerance is achieved by storing multiple sets parity data across 4 or more disk drives|
|```60```|Fault tolerance is achieved by storing multiple sets parity data and striping the data across 8 or more disk drives|

### RebuildCompletionPercentage
Member of [HpeSmartStorageLogicalDrive.v2_1_0.HpeSmartStorageLogicalDrive](#hpesmartstoragelogicaldrive-v2_1_0-hpesmartstoragelogicaldrive)

| | |
|---|---|
|Description|The percent complete for a rebuild operation currently occurring on the logical drive|
|Type|integer|
|Read Only|True|

### SmartCacheState
Member of [HpeSmartStorageLogicalDrive.v2_1_0.HpeSmartStorageLogicalDrive](#hpesmartstoragelogicaldrive-v2_1_0-hpesmartstoragelogicaldrive)

| | |
|---|---|
|Description|The state of the SmartCache cache. This is valid if this drive either is a cache drive, or has a cache drive attached to it|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```Good```|The cache is functioning properly|
|```Limited```|The cache is functioning in a degraded mode, and may not be functioning at maximum performance|
|```DDRUnsafe```|The DDR is unsafe for the cache drive|
|```CacheLUNOffline```|The cache drive is offline|
|```PrimaryLUNOffline```|The primary logical drive that is being cached is offline|
|```Destroyed```|The cache is destroyed and not functional|
|```Flushing```|The cache drive is flushing|
|```Configuring```|The caching pair is being configured|
|```PairFailAtPowerup```|The primary and cache drive were unable to be paired at powerup|
|```Unknown```|The state of the cache is unknown|

### Status
Member of [HpeSmartStorageLogicalDrive.v2_1_0.HpeSmartStorageLogicalDrive](#hpesmartstoragelogicaldrive-v2_1_0-hpesmartstoragelogicaldrive)
See the Redfish standard schema and specification for information on common Status object.

### StripSizeBytes
Member of [HpeSmartStorageLogicalDrive.v2_1_0.HpeSmartStorageLogicalDrive](#hpesmartstoragelogicaldrive-v2_1_0-hpesmartstoragelogicaldrive)

| | |
|---|---|
|Description|The strip size of the logical drive in bytes|
|Type|integer|
|Read Only|True|

### StripeSizeBytes
Member of [HpeSmartStorageLogicalDrive.v2_1_0.HpeSmartStorageLogicalDrive](#hpesmartstoragelogicaldrive-v2_1_0-hpesmartstoragelogicaldrive)

| | |
|---|---|
|Description|The stripe size of the logical drive in bytes|
|Type|integer|
|Read Only|True|

### TransformationCompletionPercentage
Member of [HpeSmartStorageLogicalDrive.v2_1_0.HpeSmartStorageLogicalDrive](#hpesmartstoragelogicaldrive-v2_1_0-hpesmartstoragelogicaldrive)

| | |
|---|---|
|Description|The percent complete for any transformations the logical drive may be undergoing such as RAID migration, stripesize migration, capacity expansion etc.|
|Type|integer|
|Read Only|True|

### VolumeUniqueIdentifier
Member of [HpeSmartStorageLogicalDrive.v2_1_0.HpeSmartStorageLogicalDrive](#hpesmartstoragelogicaldrive-v2_1_0-hpesmartstoragelogicaldrive)

| | |
|---|---|
|Description|An identifier (typically SCSI Inquiry based such as Inquiry VPD Page 0x83 NAA 64 identifier) used to uniquely identify this volume.|
|Type|string|
|Read Only|True|

## HpeSmartStorageStorageEnclosure.v2_0_0.HpeSmartStorageStorageEnclosure
```@odata.type: "#HpeSmartStorageStorageEnclosure.v2_0_0.HpeSmartStorageStorageEnclosure"```

HpSmartStorageStorageEnclosure
### Resource Instances
|Uri|HTTP Allow|
|---|---|
|```/redfish/v1/systems/{item}/smartstorage/arraycontrollers/{item}/storageenclosures/{item}/```||

### DoorLockLED
Member of [HpeSmartStorageStorageEnclosure.v2_0_0.HpeSmartStorageStorageEnclosure](#hpesmartstoragestorageenclosure-v2_0_0-hpesmartstoragestorageenclosure)

| | |
|---|---|
|Description|The state of the Door Lock LED. When Lit, this indicates that the Enclosure should not be removed since the drives are currently in use.|
|Type|string or null|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```Null```|A value is temporarily unavailable|
|```Unknown```|The state of the Door Lock LED cannot be determined.|
|```Lit```|The Door Lock LED is lit.|
|```Off```|The Door Lock LED is off.|

### DriveBayCount
Member of [HpeSmartStorageStorageEnclosure.v2_0_0.HpeSmartStorageStorageEnclosure](#hpesmartstoragestorageenclosure-v2_0_0-hpesmartstoragestorageenclosure)

| | |
|---|---|
|Description|Number of drive bays supported within the storage enclosure|
|Type|integer|
|Read Only|True|

### EnclosureLogicalID
Member of [HpeSmartStorageStorageEnclosure.v2_0_0.HpeSmartStorageStorageEnclosure](#hpesmartstoragestorageenclosure-v2_0_0-hpesmartstoragestorageenclosure)

| | |
|---|---|
|Description|Unique ID for the storage enclosure|
|Type|string|
|Read Only|True|

### FaultLED
Member of [HpeSmartStorageStorageEnclosure.v2_0_0.HpeSmartStorageStorageEnclosure](#hpesmartstoragestorageenclosure-v2_0_0-hpesmartstoragestorageenclosure)

| | |
|---|---|
|Description|The state of the Fault LED.|
|Type|string or null|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```Null```|A value is temporarily unavailable|
|```Unknown```|The state of the Fault LED cannot be determined.|
|```Lit```|The Fault LED is lit.|
|```Off```|The Fault LED is off.|

### FirmwareVersion
**FirmwareVersion.Current**
**FirmwareVersion.Current.VersionString**
Member of [HpeSmartStorageStorageEnclosure.v2_0_0.HpeSmartStorageStorageEnclosure](#hpesmartstoragestorageenclosure-v2_0_0-hpesmartstoragestorageenclosure)

| | |
|---|---|
|Description|This string represents the version of the firmware image.|
|Type|string or null|
|Read Only|True|

### IndicatorLED
Member of [HpeSmartStorageStorageEnclosure.v2_0_0.HpeSmartStorageStorageEnclosure](#hpesmartstoragestorageenclosure-v2_0_0-hpesmartstoragestorageenclosure)

| | |
|---|---|
|Description|The state of the indicator LED.|
|Type|string or null|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```Null```|A value is temporarily unavailable|
|```Unknown```|The state of the Indicator LED cannot be determined.|
|```Lit```|The Indicator LED is lit.|
|```Blinking```|The Indicator LED is blinking.|
|```Off```|The Indicator LED is off.|

### Location
Member of [HpeSmartStorageStorageEnclosure.v2_0_0.HpeSmartStorageStorageEnclosure](#hpesmartstoragestorageenclosure-v2_0_0-hpesmartstoragestorageenclosure)

| | |
|---|---|
|Description|Location identifier|
|Type|string|
|Read Only|True|

### LocationFormat
Member of [HpeSmartStorageStorageEnclosure.v2_0_0.HpeSmartStorageStorageEnclosure](#hpesmartstoragestorageenclosure-v2_0_0-hpesmartstoragestorageenclosure)

| | |
|---|---|
|Description|Format for Location Identifier|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```Controller:Box```|This format typically used in controller context where the drive would be identified using the controller port and JBOD box number|
|```SwitchPort:Box```|This format typically used in a SAS switch context where the drive would be identified using the switch port and JBOD box number|
|```SwitchPort:SwitchBay```|This format typically used in a SAS switch context where the drive would be identified using the switch port and ICM bay number for the switch|

### Manufacturer
Member of [HpeSmartStorageStorageEnclosure.v2_0_0.HpeSmartStorageStorageEnclosure](#hpesmartstoragestorageenclosure-v2_0_0-hpesmartstoragestorageenclosure)

| | |
|---|---|
|Description|The manufacturer of the storage enclosure|
|Type|string|
|Read Only|True|

### Model
Member of [HpeSmartStorageStorageEnclosure.v2_0_0.HpeSmartStorageStorageEnclosure](#hpesmartstoragestorageenclosure-v2_0_0-hpesmartstoragestorageenclosure)

| | |
|---|---|
|Description|The model string for the storage enclosure|
|Type|string|
|Read Only|True|

### PartNumber
Member of [HpeSmartStorageStorageEnclosure.v2_0_0.HpeSmartStorageStorageEnclosure](#hpesmartstoragestorageenclosure-v2_0_0-hpesmartstoragestorageenclosure)

| | |
|---|---|
|Description|Part number of this storage enclosure|
|Type|string|
|Read Only|True|

### SKU
Member of [HpeSmartStorageStorageEnclosure.v2_0_0.HpeSmartStorageStorageEnclosure](#hpesmartstoragestorageenclosure-v2_0_0-hpesmartstoragestorageenclosure)

| | |
|---|---|
|Description|SKU for the storage enclosure|
|Type|string|
|Read Only|True|

### SerialNumber
Member of [HpeSmartStorageStorageEnclosure.v2_0_0.HpeSmartStorageStorageEnclosure](#hpesmartstoragestorageenclosure-v2_0_0-hpesmartstoragestorageenclosure)

| | |
|---|---|
|Description|The serial number for this storage enclosure|
|Type|string|
|Read Only|True|

### Status
Member of [HpeSmartStorageStorageEnclosure.v2_0_0.HpeSmartStorageStorageEnclosure](#hpesmartstoragestorageenclosure-v2_0_0-hpesmartstoragestorageenclosure)
See the Redfish standard schema and specification for information on common Status object.

### SubEnclosureLocation
Member of [HpeSmartStorageStorageEnclosure.v2_0_0.HpeSmartStorageStorageEnclosure](#hpesmartstoragestorageenclosure-v2_0_0-hpesmartstoragestorageenclosure)

| | |
|---|---|
|Description|Location within the chassis if this storage enclosure is part of a larger chassis hosting multiple storage enclosures|
|Type|string|
|Read Only|True|

## HpeSNMPAlertDestination.v2_0_0.HpeSNMPAlertDestination
```@odata.type: "#HpeSNMPAlertDestination.v2_0_0.HpeSNMPAlertDestination"```

The alert destination configuration up to 8 remote management systems that receive SNMP alerts from the management processor.

This resource type was added in iLO 5 1.20

### Resource Instances
|Uri|HTTP Allow|
|---|---|
|```/redfish/v1/managers/{item}/snmpservice/snmpalertdestinations/{item}/```|GET PATCH DELETE |

### AlertDestination
Member of [HpeSNMPAlertDestination.v2_0_0.HpeSNMPAlertDestination](#hpesnmpalertdestination-v2_0_0-hpesnmpalertdestination)

| | |
|---|---|
|Description|The IP address or FQDN of remote management system that receive SNMP alerts.|
|Type|string|
|Read Only|False|

### SNMPAlertProtocol
Member of [HpeSNMPAlertDestination.v2_0_0.HpeSNMPAlertDestination](#hpesnmpalertdestination-v2_0_0-hpesnmpalertdestination)

| | |
|---|---|
|Description|Indicate the SNMP protocol associated with the AlertDestination.|
|Type|string or null|
|Read Only|False|

The following are the supported values:

|Value|Description|
|---|---|
|```SNMPv1Trap```|Indicate SNMPv1 trap is enabled for the destination.|
|```SNMPv3Trap```|Indicate SNMPv3 trap is enabled for the destination. Needs to fill the SecurityName as well.|
|```SNMPv3Inform```|Indicate SNMPv3 Inform is enabled for the destination. Needs to fill the SecurityName as well.|
|```Null```|A value is temporarily unavailable|

### SNMPv3User
SNMPv3 User associated with the destination when SNMP alert protocol is SNMPv3trap.
### SecurityName
Member of [HpeSNMPAlertDestination.v2_0_0.HpeSNMPAlertDestination](#hpesnmpalertdestination-v2_0_0-hpesnmpalertdestination)

| | |
|---|---|
|Description|Provides the SNMPv3 security name associated with SNMPv3trap or SNMPv3Inform set on SNMPAlertProtocol.|
|Type|string or null|
|Read Only|False|

### TrapCommunity
Member of [HpeSNMPAlertDestination.v2_0_0.HpeSNMPAlertDestination](#hpesnmpalertdestination-v2_0_0-hpesnmpalertdestination)

| | |
|---|---|
|Description|The configured SNMPv1 trap community string.|
|Type|string|
|Read Only|False|

## HpeSNMPUser.v2_0_0.HpeSNMPUser
```@odata.type: "#HpeSNMPUser.v2_0_0.HpeSNMPUser"```

SNMPv3 supports the User-based Security Model (USM). With this model, security parameters are configured at both the agent level and the manager level. Messages exchanged between the agent and the manager are subject to a data integrity check and data origin authentication. Up to 8 user profiles are supported for setting SNMPv3 USM parameters.

This resource type was added in iLO 5 1.20

### Resource Instances
|Uri|HTTP Allow|
|---|---|
|```/redfish/v1/managers/{item}/snmpservice/snmpusers/{item}/```|GET PATCH DELETE |

### AuthPassphrase
Member of [HpeSNMPUser.v2_0_0.HpeSNMPUser](#hpesnmpuser-v2_0_0-hpesnmpuser)

| | |
|---|---|
|Description|Sets the passphrase to use for sign operations. Enter a value of 8 to 49 characters.|
|Type|string or null|
|Read Only|False|

### AuthProtocol
Member of [HpeSNMPUser.v2_0_0.HpeSNMPUser](#hpesnmpuser-v2_0_0-hpesnmpuser)

| | |
|---|---|
|Description|Sets the message digest algorithm to use for encoding the authorization passphrase. The message digest is calculated over an appropriate portion of an SNMP message, and is included as part of the message sent to the recipient.|
|Type|string|
|Read Only|False|

The following are the supported values:

|Value|Description|
|---|---|
|```MD5```|Indicate Message Digest Algorithm.|
|```SHA```|Indicate Secure Hash Algorithm.|

### PrivacyPassphrase
Member of [HpeSNMPUser.v2_0_0.HpeSNMPUser](#hpesnmpuser-v2_0_0-hpesnmpuser)

| | |
|---|---|
|Description|Sets the passphrase to use for encrypt operations. Enter a value of 8 to 49 characters.|
|Type|string or null|
|Read Only|False|

### PrivacyProtocol
Member of [HpeSNMPUser.v2_0_0.HpeSNMPUser](#hpesnmpuser-v2_0_0-hpesnmpuser)

| | |
|---|---|
|Description|Sets the encryption algorithm to use for encoding the privacy passphrase. A portion of an SNMP message is encrypted before transmission.|
|Type|string|
|Read Only|False|

The following are the supported values:

|Value|Description|
|---|---|
|```DES```|Indicate Data Encryption Standard Algorithm.|
|```AES```|Indicate Advanced Encryption Standard Algorithm.|

### SecurityName
Member of [HpeSNMPUser.v2_0_0.HpeSNMPUser](#hpesnmpuser-v2_0_0-hpesnmpuser)

| | |
|---|---|
|Description|The user profile name. Enter an alphanumeric string of 1 to 32 characters.|
|Type|string or null|
|Read Only|False|

### UserEngineID
Member of [HpeSNMPUser.v2_0_0.HpeSNMPUser](#hpesnmpuser-v2_0_0-hpesnmpuser)

| | |
|---|---|
|Description|The UserEngineID is combined with the SecurityName to create a SNMPv3 user for each manager. It is only used for creating remote accounts used with INFORM messages. If this property is not set then INFORM message will be sent with default or iLO configured engine ID. This value must be a hexadecimal string with an even number of 10 to 64 characters, excluding the first two characters, 0x (for example, 0x01020304abcdef).|
|Type|string or null|
|Read Only|False|

## HpeTlsConfig.v1_0_0.HpeTlsConfig
```@odata.type: "#HpeTlsConfig.v1_0_0.HpeTlsConfig"```

The schema definition for TLS configuration.
### Resource Instances
|Uri|HTTP Allow|
|---|---|
|```/redfish/v1/systems/{item}/bios/tlsconfig/```|GET |
|```/redfish/v1/systems/{item}/bios/tlsconfig/settings/```|GET PATCH |

### Links to other Resources
|Link Name|Destination type
|---|---|
|```@Redfish.Settings/SettingsObject```|[HpeTlsConfig](#hpetlsconfig-v1_0_0-hpetlsconfig)|
|```Oem/Hpe/Links/BaseConfigs```|[HpeBaseConfigs](#hpebaseconfigs-v2_0_0-hpebaseconfigs)|

### @Redfish.Settings
Member of [HpeTlsConfig.v1_0_0.HpeTlsConfig](#hpetlsconfig-v1_0_0-hpetlsconfig)
See the Redfish standard schema and specification for information on common @Redfish properties.

### Certificates (array)
Member of [HpeTlsConfig.v1_0_0.HpeTlsConfig](#hpetlsconfig-v1_0_0-hpetlsconfig)
```Certificates``` is an array containing elements of:

**Certificates[{item}].FingerPrint**
Member of [HpeTlsConfig.v1_0_0.HpeTlsConfig](#hpetlsconfig-v1_0_0-hpetlsconfig)

| | |
|---|---|
|Description|The fingerprint of the certificate. It is the sha256 (SHA2) of the Der format of the certificate|
|Type|string|
|Read Only|True|

**Certificates[{item}].Issuer**
Member of [HpeTlsConfig.v1_0_0.HpeTlsConfig](#hpetlsconfig-v1_0_0-hpetlsconfig)

| | |
|---|---|
|Description|The Issuer of the certificate|
|Type|string|
|Read Only|True|

**Certificates[{item}].SerialNumber**
Member of [HpeTlsConfig.v1_0_0.HpeTlsConfig](#hpetlsconfig-v1_0_0-hpetlsconfig)

| | |
|---|---|
|Description|The Serial Number of the certificate.|
|Type|string|
|Read Only|True|

**Certificates[{item}].Subject**
Member of [HpeTlsConfig.v1_0_0.HpeTlsConfig](#hpetlsconfig-v1_0_0-hpetlsconfig)

| | |
|---|---|
|Description|The Subject of the certificate.|
|Type|string|
|Read Only|True|

**Certificates[{item}].ValidNotAfter**
Member of [HpeTlsConfig.v1_0_0.HpeTlsConfig](#hpetlsconfig-v1_0_0-hpetlsconfig)

| | |
|---|---|
|Description|The expiration date of the certificate.|
|Type|string|
|Read Only|True|

**Certificates[{item}].ValidNotBefore**
Member of [HpeTlsConfig.v1_0_0.HpeTlsConfig](#hpetlsconfig-v1_0_0-hpetlsconfig)

| | |
|---|---|
|Description|The date when the certificate becomes valid.|
|Type|string|
|Read Only|True|

### Ciphers
Member of [HpeTlsConfig.v1_0_0.HpeTlsConfig](#hpetlsconfig-v1_0_0-hpetlsconfig)

| | |
|---|---|
|Description|The encryption used. It can have more than one type of encryption, example: "AES128-SHA:AES256-SHA:AES128-SHA256:AES256-SHA256"|
|Type|string|
|Read Only|False|

### DeleteCertificates (array)
Member of [HpeTlsConfig.v1_0_0.HpeTlsConfig](#hpetlsconfig-v1_0_0-hpetlsconfig)
```DeleteCertificates``` is an array containing elements of:

**DeleteCertificates[{item}].FingerPrint**
Member of [HpeTlsConfig.v1_0_0.HpeTlsConfig](#hpetlsconfig-v1_0_0-hpetlsconfig)

| | |
|---|---|
|Description|To delete a certificate, the user should place its fingerprint here. The fingerprint would be found as a property under the single certificate object in the "Certificates" array |
|Type|string|
|Read Only|False|

### HostnameCheck
Member of [HpeTlsConfig.v1_0_0.HpeTlsConfig](#hpetlsconfig-v1_0_0-hpetlsconfig)

| | |
|---|---|
|Description|Use this option to enable or disable verification of the connected server's hostname with the hostname in the certificate supplied by the server|
|Type|string|
|Read Only|False|

The following are the supported values:

|Value|Description|
|---|---|
|```Disabled```|Disable verification of the connected server's hostname.|
|```Enabled```|enable verification of the connected server's hostname.|

### NewCertificates (array)
Member of [HpeTlsConfig.v1_0_0.HpeTlsConfig](#hpetlsconfig-v1_0_0-hpetlsconfig)
```NewCertificates``` is an array containing elements of:

**NewCertificates[{item}].X509Certificate**
Member of [HpeTlsConfig.v1_0_0.HpeTlsConfig](#hpetlsconfig-v1_0_0-hpetlsconfig)

| | |
|---|---|
|Description|the body (PEM format) of the Certificate to be added|
|Type|string|
|Read Only|False|

### ProtocolVersion
Member of [HpeTlsConfig.v1_0_0.HpeTlsConfig](#hpetlsconfig-v1_0_0-hpetlsconfig)

| | |
|---|---|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|
|---|
|```AUTO```|
|```1.0```|
|```1.1```|
|```1.2```|

### TlsCaCertificateCount
Member of [HpeTlsConfig.v1_0_0.HpeTlsConfig](#hpetlsconfig-v1_0_0-hpetlsconfig)

| | |
|---|---|
|Description|The certificates count.|
|Type|integer|
|Read Only|False|

### VerifyMode
Member of [HpeTlsConfig.v1_0_0.HpeTlsConfig](#hpetlsconfig-v1_0_0-hpetlsconfig)

| | |
|---|---|
|Description|It determines if/how the certificates are validated.|
|Type|string|
|Read Only|False|

The following are the supported values:

|Value|
|---|
|```NONE```|
|```PEER```|

## HpeUSBDevice.v2_0_0.HpeUSBDevice
```@odata.type: "#HpeUSBDevice.v2_0_0.HpeUSBDevice"```
### Resource Instances
|Uri|HTTP Allow|
|---|---|
|```/redfish/v1/systems/{item}/usbdevices/{item}/```|GET |

### DeviceCapacityMB
Member of [HpeUSBDevice.v2_0_0.HpeUSBDevice](#hpeusbdevice-v2_0_0-hpeusbdevice)

| | |
|---|---|
|Description|USB device usable capacity (if applicable) in Mbytes|
|Type|integer|
|Read Only|True|

### DeviceClass
Member of [HpeUSBDevice.v2_0_0.HpeUSBDevice](#hpeusbdevice-v2_0_0-hpeusbdevice)

| | |
|---|---|
|Description|USB device Class code as defined by the USB HID device specification.|
|Type|integer|
|Read Only|True|

### DeviceName
Member of [HpeUSBDevice.v2_0_0.HpeUSBDevice](#hpeusbdevice-v2_0_0-hpeusbdevice)

| | |
|---|---|
|Description|USB device name in UTF-8 format.|
|Type|string or null|
|Read Only|True|

### DeviceProtocol
Member of [HpeUSBDevice.v2_0_0.HpeUSBDevice](#hpeusbdevice-v2_0_0-hpeusbdevice)

| | |
|---|---|
|Description|Protocol code as defined by the USB HID specification.|
|Type|integer|
|Read Only|True|

### DeviceSubClass
Member of [HpeUSBDevice.v2_0_0.HpeUSBDevice](#hpeusbdevice-v2_0_0-hpeusbdevice)

| | |
|---|---|
|Description|USB device SubClass code as defined by the USB HID device specification.|
|Type|integer|
|Read Only|True|

### Location
Member of [HpeUSBDevice.v2_0_0.HpeUSBDevice](#hpeusbdevice-v2_0_0-hpeusbdevice)

| | |
|---|---|
|Description|Location of the USB device on the server|
|Type|string or null|
|Read Only|True|

### ProductID
Member of [HpeUSBDevice.v2_0_0.HpeUSBDevice](#hpeusbdevice-v2_0_0-hpeusbdevice)

| | |
|---|---|
|Description|USB product ID as defined by manufacturer.|
|Type|integer|
|Read Only|True|

### StructuredName
Member of [HpeUSBDevice.v2_0_0.HpeUSBDevice](#hpeusbdevice-v2_0_0-hpeusbdevice)

| | |
|---|---|
|Description|USB device structured name in UTF-8 format.|
|Type|string or null|
|Read Only|True|

### UEFIDevicePath
Member of [HpeUSBDevice.v2_0_0.HpeUSBDevice](#hpeusbdevice-v2_0_0-hpeusbdevice)

| | |
|---|---|
|Description|UEFI device path of USB device. Standardized text representation of the UEFI device path, in UTF-8 format|
|Type|string or null|
|Read Only|True|

### VendorID
Member of [HpeUSBDevice.v2_0_0.HpeUSBDevice](#hpeusbdevice-v2_0_0-hpeusbdevice)

| | |
|---|---|
|Description|Vendor ID of detected USB device.|
|Type|integer|
|Read Only|True|

## HpeUSBPort.v2_0_0.HpeUSBPort
```@odata.type: "#HpeUSBPort.v2_0_0.HpeUSBPort"```
### Resource Instances
|Uri|HTTP Allow|
|---|---|
|```/redfish/v1/systems/{item}/usbports/{item}/```|GET |

### InstanceNumber
Member of [HpeUSBPort.v2_0_0.HpeUSBPort](#hpeusbport-v2_0_0-hpeusbport)

| | |
|---|---|
|Description|Instance number of the USB Port|
|Type|integer|
|Read Only|True|

### Location
Member of [HpeUSBPort.v2_0_0.HpeUSBPort](#hpeusbport-v2_0_0-hpeusbport)

| | |
|---|---|
|Description|Location of the USB Device on the server|
|Type|string or null|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```Null```|A value is temporarily unavailable|
|```Back```|Located on the rear panel of the server.|
|```Front```|Located on the front bezel of the server.|
|```Internal```|Located internally within the server chassis.|
|```InternalManagement```|Internal management media.|
|```InternalSDCard```|The internal SD-Card slot.|
|```iLOManagement```|iLO virtual USB devices.|

### PCIBusNumber
Member of [HpeUSBPort.v2_0_0.HpeUSBPort](#hpeusbport-v2_0_0-hpeusbport)

| | |
|---|---|
|Description|PCI Bus number of the USB controller that controls this USB port |
|Type|integer|
|Read Only|True|

### PCIDeviceNumber
Member of [HpeUSBPort.v2_0_0.HpeUSBPort](#hpeusbport-v2_0_0-hpeusbport)

| | |
|---|---|
|Description|PCI Device Number of the USB Controller that controls this USB Port.|
|Type|integer|
|Read Only|True|

### PCIFunctionNumber
Member of [HpeUSBPort.v2_0_0.HpeUSBPort](#hpeusbport-v2_0_0-hpeusbport)

| | |
|---|---|
|Description|PCI Function Number of the USB Controller that controls this USB Port.|
|Type|integer|
|Read Only|True|

### ParentHubInstance
Member of [HpeUSBPort.v2_0_0.HpeUSBPort](#hpeusbport-v2_0_0-hpeusbport)

| | |
|---|---|
|Description|Parent Hub Instance that provides an instance number of the internal hub this USB Port is connected to.|
|Type|integer|
|Read Only|True|

### SharedCapability
Member of [HpeUSBPort.v2_0_0.HpeUSBPort](#hpeusbport-v2_0_0-hpeusbport)

| | |
|---|---|
|Description|Shared Capability of the USB Port|
|Type|string or null|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```Null```|A value is temporarily unavailable|
|```UnsharedManagement```|Not shared as a Management Port.|
|```SharedManagementPhysicalSwitch```|Shared management port w/ physical switch to control whether muxed to iLO or host.|
|```SharedManagementPortAutomaticControl```||

### SpeedCapability
Member of [HpeUSBPort.v2_0_0.HpeUSBPort](#hpeusbport-v2_0_0-hpeusbport)

| | |
|---|---|
|Description|USB speed capability of the USB port as configured by the BIOS during POST.|
|Type|string or null|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```Null```|A value is temporarily unavailable|
|```USB1FullSpeed```|USB 1.0 Full Speed|
|```USB2HighSpeed```|USB 2.0 High Speed|
|```USB3SuperSpeed```|USB 3.x SuperSpeed|

### UEFIDevicePath
Member of [HpeUSBPort.v2_0_0.HpeUSBPort](#hpeusbport-v2_0_0-hpeusbport)

| | |
|---|---|
|Description|UEFI Device Path of USB Endpoint. Standardized text representation of the UEFI device path, in UTF-8 format|
|Type|string|
|Read Only|True|

## LogEntry.v1_0_0.LogEntry
```@odata.type: "#LogEntry.v1_0_0.LogEntry"```
### Resource Instances
|Uri|HTTP Allow|
|---|---|
|```/redfish/v1/managers/{item}/logservices/iel/entries/{item}/```|GET |
|```/redfish/v1/managers/{item}/remotesupportservice/serviceeventlogs/{item}/```|GET |
|```/redfish/v1/systems/{item}/logservices/iml/entries/{item}/```|GET PATCH |

### Created
Member of [LogEntry.v1_0_0.LogEntry](#logentry-v1_0_0-logentry)

| | |
|---|---|
|Description|The date and time when the log entry was created, for example, 2014-04-15T00:38:00Z.|
|Type|string|
|Read Only|True|

### EntryType
Member of [LogEntry.v1_0_0.LogEntry](#logentry-v1_0_0-logentry)

| | |
|---|---|
|Description|The log entry type.|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|
|---|
|```Oem```|

### Message
Member of [LogEntry.v1_0_0.LogEntry](#logentry-v1_0_0-logentry)

| | |
|---|---|
|Description|The log entry details.|
|Type|string|
|Read Only|True|

### Oem.Hpe.Categories (array)
Member of [LogEntry.v1_0_0.LogEntry](#logentry-v1_0_0-logentry)
```Categories``` is an array containing elements of:


| | |
|---|---|
|Type|string or null|
|Read Only|True|

### Oem.Hpe.Class
Member of [LogEntry.v1_0_0.LogEntry](#logentry-v1_0_0-logentry)

| | |
|---|---|
|Description|The log entry event class.|
|Type|integer|
|Read Only|True|

### Oem.Hpe.Code
Member of [LogEntry.v1_0_0.LogEntry](#logentry-v1_0_0-logentry)

| | |
|---|---|
|Description|The log entry event code.|
|Type|integer|
|Read Only|True|

### Oem.Hpe.Count
Member of [LogEntry.v1_0_0.LogEntry](#logentry-v1_0_0-logentry)

| | |
|---|---|
|Description|The occurrence count of the log entry.|
|Type|integer|
|Read Only|True|

### Oem.Hpe.Destination
Member of [LogEntry.v1_0_0.LogEntry](#logentry-v1_0_0-logentry)

| | |
|---|---|
|Description|The destination host name or IP address of the remote server that recevied the service event.|
|Type|string|
|Read Only|True|

### Oem.Hpe.EventNumber
Member of [LogEntry.v1_0_0.LogEntry](#logentry-v1_0_0-logentry)

| | |
|---|---|
|Description|The event log identification number. Events are numbered in the order in which they are generated.|
|Type|integer|
|Read Only|True|

### Oem.Hpe.Identifier
Member of [LogEntry.v1_0_0.LogEntry](#logentry-v1_0_0-logentry)

| | |
|---|---|
|Description|The unique identifier of the service event.|
|Type|string|
|Read Only|True|

### Oem.Hpe.LearnMoreLink
Member of [LogEntry.v1_0_0.LogEntry](#logentry-v1_0_0-logentry)

| | |
|---|---|
|Description|The link to troubleshooting information.|
|Type|string|
|Read Only|True|

### Oem.Hpe.RecommendedAction
Member of [LogEntry.v1_0_0.LogEntry](#logentry-v1_0_0-logentry)

| | |
|---|---|
|Description|The recommended action for the event.|
|Type|string|
|Read Only|True|

### Oem.Hpe.Repaired
Member of [LogEntry.v1_0_0.LogEntry](#logentry-v1_0_0-logentry)

| | |
|---|---|
|Description|The repaired status of the IML event.|
|Type|boolean|
|Read Only|False|

### Oem.Hpe.SubmitStatus
Member of [LogEntry.v1_0_0.LogEntry](#logentry-v1_0_0-logentry)

| | |
|---|---|
|Description|The service event log submission status .|
|Type|string|
|Read Only|True|

### Oem.Hpe.Updated
Member of [LogEntry.v1_0_0.LogEntry](#logentry-v1_0_0-logentry)

| | |
|---|---|
|Description|The date and time of the latest log entry update, for example, 2014-04-15T00:38:00Z.|
|Type|string|
|Read Only|True|

### OemRecordFormat
Member of [LogEntry.v1_0_0.LogEntry](#logentry-v1_0_0-logentry)

| | |
|---|---|
|Description|The format of an OEM record.|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|
|---|
|```Hpe-IML```|
|```Hpe-iLOEventLog```|

### Severity
Member of [LogEntry.v1_0_0.LogEntry](#logentry-v1_0_0-logentry)

| | |
|---|---|
|Description|The log entry severity.|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|
|---|
|```OK```|
|```Warning```|
|```Critical```|

## LogService.v1_0_0.LogService
```@odata.type: "#LogService.v1_0_0.LogService"```
### Resource Instances
|Uri|HTTP Allow|
|---|---|
|```/redfish/v1/managers/{item}/logservices/iel/```|GET POST |
|```/redfish/v1/systems/{item}/logservices/iml/```|GET POST |

### Links to other Resources
|Link Name|Destination type
|---|---|
|```Entries```|Collection of [LogEntry](#logentry-v1_0_0-logentry)|

### Entries
The URI to this log entries collection resource.
### MaxNumberOfRecords
Member of [LogService.v1_0_0.LogService](#logservice-v1_0_0-logservice)

| | |
|---|---|
|Description|The maximum number of log entries.|
|Type|integer|
|Read Only|True|

### OverWritePolicy
Member of [LogService.v1_0_0.LogService](#logservice-v1_0_0-logservice)

| | |
|---|---|
|Description|When the log is full, the overwrite policy is enforced.|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```Unknown```|The overwrite policy is not known or is undefined.|
|```WrapsWhenFull```|When the log is full, new entries will overwrite previous entries.|
|```NeverOverwrites```|When the log is full, new entries are discarded.|

### Actions

**LogService.ClearLog**
Member of [LogService.v1_0_0.LogService](#logservice-v1_0_0-logservice)
There are no parameters for this action.
## Manager.v1_1_0.Manager
```@odata.type: "#Manager.v1_1_0.Manager"```

This is the schema definition for a manager.  Examples of managers are BMCs, Enclosure Managers, Management Controllers and other subsystems assigned manageability functions.
### Resource Instances
|Uri|HTTP Allow|
|---|---|
|```/redfish/v1/managers/{item}/```|GET POST PATCH |

### Links to other Resources
|Link Name|Destination type
|---|---|
|```Oem/Hpe/Links/DateTimeService```|[HpeiLODateTime](#hpeilodatetime-v2_0_0-hpeilodatetime)|
|```Oem/Hpe/Links/RemoteSupport```|[HpeRemoteSupport](#hperemotesupport-v2_2_0-hperemotesupport)|
|```Links/ManagerForChassis[]```|[Chassis](#chassis-v1_2_0-chassis)|
|```VirtualMedia```|Collection of [VirtualMedia](#virtualmedia-v1_0_0-virtualmedia)|
|```NetworkProtocol```|[ManagerNetworkProtocol](#managernetworkprotocol-v1_0_0-managernetworkprotocol)|
|```Links/ManagerInChassis```|[Chassis](#chassis-v1_2_0-chassis)|
|```EthernetInterfaces```|Collection of [EthernetInterface](#ethernetinterface-v1_0_3-ethernetinterface)|
|```Links/ManagerForServers[]```|[ComputerSystem](#computersystem-v1_4_0-computersystem)|
|```Oem/Hpe/Links/ActiveHealthSystem```|[HpeiLOActiveHealthSystem](#hpeiloactivehealthsystem-v2_2_0-hpeiloactivehealthsystem)|
|```Oem/Hpe/Links/SecurityService```|[HpeSecurityService](#hpesecurityservice-v2_2_0-hpesecurityservice)|
|```Oem/Hpe/Links/LicenseService```|Collection of [HpeiLOLicense](#hpeilolicense-v2_1_0-hpeilolicense)|
|```LogServices```|Collection of [LogService](#logservice-v1_0_0-logservice)|
|```Oem/Hpe/Links/FederationPeers```|Collection of [HpeiLOFederationPeers](#hpeilofederationpeers-v2_0_0-hpeilofederationpeers)|
|```Oem/Hpe/Links/EmbeddedMediaService```|[HpeiLOEmbeddedMedia](#hpeiloembeddedmedia-v2_0_0-hpeiloembeddedmedia)|
|```Oem/Hpe/Links/FederationGroups```|Collection of [HpeiLOFederationGroup](#hpeilofederationgroup-v2_0_0-hpeilofederationgroup)|
|```Oem/Hpe/Links/BackupRestoreService```|[HpeiLOBackupRestoreService](#hpeilobackuprestoreservice-v2_1_0-hpeilobackuprestoreservice)|

### CommandShell
**CommandShell.ConnectTypesSupported (array)**
Member of [Manager.v1_1_0.Manager](#manager-v1_1_0-manager)
```ConnectTypesSupported``` is an array containing elements of:


| | |
|---|---|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```SSH```|The controller supports a Command Shell connection using the SSH protocol|
|```Telnet```|The controller supports a Command Shell connection using the Telnet protocol|
|```IPMI```|The controller supports a Command Shell connection using the IPMI Serial-over-LAN (SOL) protocol|
|```Oem```|The controller supports a Command Shell connectino using an OEM-specific protocol|

**CommandShell.MaxConcurrentSessions**
Member of [Manager.v1_1_0.Manager](#manager-v1_1_0-manager)

| | |
|---|---|
|Description|This is the maximum number of Command Shell sessions, regardless of protocol, that this manager supports.|
|Type|integer|
|Read Only|True|

**CommandShell.ServiceEnabled**
Member of [Manager.v1_1_0.Manager](#manager-v1_1_0-manager)

| | |
|---|---|
|Description|Indicates if the Command Shell service is enabled for this manager.|
|Type|boolean|
|Read Only|False|

### EthernetInterfaces
This is a reference to a collection of NICs that this manager uses for network communication.  It is here that clients will find NIC configuration options and settings.
### FirmwareVersion
Member of [Manager.v1_1_0.Manager](#manager-v1_1_0-manager)

| | |
|---|---|
|Description|The firmware version of this Manager|
|Type|string or null|
|Read Only|True|

### GraphicalConsole
**GraphicalConsole.ConnectTypesSupported (array)**
Member of [Manager.v1_1_0.Manager](#manager-v1_1_0-manager)
```ConnectTypesSupported``` is an array containing elements of:


| | |
|---|---|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```KVMIP```|The controller supports a Graphical Console connection using a KVM-IP (redirection of Keyboard, Video, Mouse over IP) protocol|
|```Oem```|The controller supports a Graphical Console connection using an OEM-specific protocol|

**GraphicalConsole.MaxConcurrentSessions**
Member of [Manager.v1_1_0.Manager](#manager-v1_1_0-manager)

| | |
|---|---|
|Description|Indicates the maximum number of Graphical Console sessions, regardless of protocol, this manager supports.|
|Type|integer|
|Read Only|True|

**GraphicalConsole.ServiceEnabled**
Member of [Manager.v1_1_0.Manager](#manager-v1_1_0-manager)

| | |
|---|---|
|Description|Indicates if the Command Shell service is enabled for this manager.|
|Type|boolean|
|Read Only|False|

### LogServices
Reference to a resource of type Collection with a MemberType of Logs.
### ManagerType
Member of [Manager.v1_1_0.Manager](#manager-v1_1_0-manager)

| | |
|---|---|
|Description|This property is the manager type for this resource.|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```ManagementController```|A controller used primarily to monitor or manage the operation of a device or system|
|```EnclosureManager```|A controller which provides management functions for a chassis or group of devices or systems|
|```BMC```|A controller which provides management functions for a single computer system|

### Model
Member of [Manager.v1_1_0.Manager](#manager-v1_1_0-manager)

| | |
|---|---|
|Description|Model name of the manager.|
|Type|string or null|
|Read Only|True|

### NetworkProtocol
 This is a reference to the network services and their settings that the manager controls.  It is here that clients will find network configuration options as well as network services.
### Oem.Hpe.ClearRestApiStatus
Member of [Manager.v1_1_0.Manager](#manager-v1_1_0-manager)

| | |
|---|---|
|Description|Status of external provider data in NVRAM.|
|Type|string or null|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```Null```|A value is temporarily unavailable|
|```DataPresent```|External Provider data is present in NVRAM.|
|```DataCleared```|External Provider data is not present in NVRAM.|

### Oem.Hpe.ConfigurationSettings
Member of [Manager.v1_1_0.Manager](#manager-v1_1_0-manager)

| | |
|---|---|
|Description|State of the currently displayed configuration settings.|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|
|---|
|```Current```|
|```SomePendingReset```|

### Oem.Hpe.FederationConfig
**Oem.Hpe.FederationConfig.IPv6MulticastScope**
Member of [Manager.v1_1_0.Manager](#manager-v1_1_0-manager)

| | |
|---|---|
|Description|The IPv6 network scope of multicast announcements.|
|Type|string|
|Read Only|False|

The following are the supported values:

|Value|
|---|
|```Link```|
|```Site```|
|```Organization```|

**Oem.Hpe.FederationConfig.MulticastAnnouncementInterval**
Member of [Manager.v1_1_0.Manager](#manager-v1_1_0-manager)

| | |
|---|---|
|Description|The frequency in Seconds at which the iLO system announces itself on the network. A value of 0 disables multicast announcments.|
|Type|integer|
|Read Only|False|

The following are the supported values:

|Value|
|---|
|```Null```|
|```30```|
|```60```|
|```120```|
|```300```|
|```600```|
|```900```|
|```1800```|

**Oem.Hpe.FederationConfig.MulticastDiscovery**
Member of [Manager.v1_1_0.Manager](#manager-v1_1_0-manager)

| | |
|---|---|
|Description|Enables or Disables Multicast Discovery for the local iLO system.|
|Type|string|
|Read Only|False|

The following are the supported values:

|Value|
|---|
|```Enabled```|
|```Disabled```|

**Oem.Hpe.FederationConfig.MulticastTimeToLive**
Member of [Manager.v1_1_0.Manager](#manager-v1_1_0-manager)

| | |
|---|---|
|Description|The maximum number of switches a multicast announcement will traverse before being discarded.|
|Type|integer|
|Read Only|False|

**Oem.Hpe.FederationConfig.iLOFederationManagement**
Member of [Manager.v1_1_0.Manager](#manager-v1_1_0-manager)

| | |
|---|---|
|Description|Enables or Disables iLO Federation features for the local iLO system.|
|Type|string|
|Read Only|False|

The following are the supported values:

|Value|
|---|
|```Enabled```|
|```Disabled```|

### Oem.Hpe.Firmware
**Oem.Hpe.Firmware.Backup**
**Oem.Hpe.Firmware.Backup.BuildNumber**
Member of [Manager.v1_1_0.Manager](#manager-v1_1_0-manager)

| | |
|---|---|
|Description|The build number of the firmware.|
|Type|integer|
|Read Only|True|

**Oem.Hpe.Firmware.Backup.BuildNumberString**
Member of [Manager.v1_1_0.Manager](#manager-v1_1_0-manager)

| | |
|---|---|
|Description|The string version of the build number of the firmware.|
|Type|string|
|Read Only|True|

**Oem.Hpe.Firmware.Backup.Date**
Member of [Manager.v1_1_0.Manager](#manager-v1_1_0-manager)

| | |
|---|---|
|Description|The build date of the firmware.|
|Type|string|
|Read Only|True|

**Oem.Hpe.Firmware.Backup.DebugBuild**
Member of [Manager.v1_1_0.Manager](#manager-v1_1_0-manager)

| | |
|---|---|
|Description|True if the firmware is a debug build; False if it is not.|
|Type|boolean|
|Read Only|True|

**Oem.Hpe.Firmware.Backup.Family**
Member of [Manager.v1_1_0.Manager](#manager-v1_1_0-manager)

| | |
|---|---|
|Description|The family of the firmware.|
|Type|string|
|Read Only|True|

**Oem.Hpe.Firmware.Backup.MajorVersion**
Member of [Manager.v1_1_0.Manager](#manager-v1_1_0-manager)

| | |
|---|---|
|Description|The major version of the firmware.|
|Type|integer|
|Read Only|True|

**Oem.Hpe.Firmware.Backup.MinorVersion**
Member of [Manager.v1_1_0.Manager](#manager-v1_1_0-manager)

| | |
|---|---|
|Description|The minor version of the firmware.|
|Type|integer|
|Read Only|True|

**Oem.Hpe.Firmware.Backup.Time**
Member of [Manager.v1_1_0.Manager](#manager-v1_1_0-manager)

| | |
|---|---|
|Description|The build time of the firmware.|
|Type|string|
|Read Only|True|

**Oem.Hpe.Firmware.Backup.VersionString**
Member of [Manager.v1_1_0.Manager](#manager-v1_1_0-manager)

| | |
|---|---|
|Description|The version string of the firmware. This value might be null if VersionString is unavailable.|
|Type|string or null|
|Read Only|True|

**Oem.Hpe.Firmware.Bootblock**
**Oem.Hpe.Firmware.Bootblock.BuildNumber**
Member of [Manager.v1_1_0.Manager](#manager-v1_1_0-manager)

| | |
|---|---|
|Description|The build number of the firmware.|
|Type|integer|
|Read Only|True|

**Oem.Hpe.Firmware.Bootblock.BuildNumberString**
Member of [Manager.v1_1_0.Manager](#manager-v1_1_0-manager)

| | |
|---|---|
|Description|The string version of the build number of the firmware.|
|Type|string|
|Read Only|True|

**Oem.Hpe.Firmware.Bootblock.Date**
Member of [Manager.v1_1_0.Manager](#manager-v1_1_0-manager)

| | |
|---|---|
|Description|The build date of the firmware.|
|Type|string|
|Read Only|True|

**Oem.Hpe.Firmware.Bootblock.DebugBuild**
Member of [Manager.v1_1_0.Manager](#manager-v1_1_0-manager)

| | |
|---|---|
|Description|True if the firmware is a debug build; False if it is not.|
|Type|boolean|
|Read Only|True|

**Oem.Hpe.Firmware.Bootblock.Family**
Member of [Manager.v1_1_0.Manager](#manager-v1_1_0-manager)

| | |
|---|---|
|Description|The family of the firmware.|
|Type|string|
|Read Only|True|

**Oem.Hpe.Firmware.Bootblock.MajorVersion**
Member of [Manager.v1_1_0.Manager](#manager-v1_1_0-manager)

| | |
|---|---|
|Description|The major version of the firmware.|
|Type|integer|
|Read Only|True|

**Oem.Hpe.Firmware.Bootblock.MinorVersion**
Member of [Manager.v1_1_0.Manager](#manager-v1_1_0-manager)

| | |
|---|---|
|Description|The minor version of the firmware.|
|Type|integer|
|Read Only|True|

**Oem.Hpe.Firmware.Bootblock.Time**
Member of [Manager.v1_1_0.Manager](#manager-v1_1_0-manager)

| | |
|---|---|
|Description|The build time of the firmware.|
|Type|string|
|Read Only|True|

**Oem.Hpe.Firmware.Bootblock.VersionString**
Member of [Manager.v1_1_0.Manager](#manager-v1_1_0-manager)

| | |
|---|---|
|Description|The version string of the firmware. This value might be null if VersionString is unavailable.|
|Type|string or null|
|Read Only|True|

**Oem.Hpe.Firmware.Current**
**Oem.Hpe.Firmware.Current.BuildNumber**
Member of [Manager.v1_1_0.Manager](#manager-v1_1_0-manager)

| | |
|---|---|
|Description|The build number of the firmware.|
|Type|integer|
|Read Only|True|

**Oem.Hpe.Firmware.Current.BuildNumberString**
Member of [Manager.v1_1_0.Manager](#manager-v1_1_0-manager)

| | |
|---|---|
|Description|The string version of the build number of the firmware.|
|Type|string|
|Read Only|True|

**Oem.Hpe.Firmware.Current.Date**
Member of [Manager.v1_1_0.Manager](#manager-v1_1_0-manager)

| | |
|---|---|
|Description|The build date of the firmware.|
|Type|string|
|Read Only|True|

**Oem.Hpe.Firmware.Current.DebugBuild**
Member of [Manager.v1_1_0.Manager](#manager-v1_1_0-manager)

| | |
|---|---|
|Description|True if the firmware is a debug build; False if it is not.|
|Type|boolean|
|Read Only|True|

**Oem.Hpe.Firmware.Current.Family**
Member of [Manager.v1_1_0.Manager](#manager-v1_1_0-manager)

| | |
|---|---|
|Description|The family of the firmware.|
|Type|string|
|Read Only|True|

**Oem.Hpe.Firmware.Current.MajorVersion**
Member of [Manager.v1_1_0.Manager](#manager-v1_1_0-manager)

| | |
|---|---|
|Description|The major version of the firmware.|
|Type|integer|
|Read Only|True|

**Oem.Hpe.Firmware.Current.MinorVersion**
Member of [Manager.v1_1_0.Manager](#manager-v1_1_0-manager)

| | |
|---|---|
|Description|The minor version of the firmware.|
|Type|integer|
|Read Only|True|

**Oem.Hpe.Firmware.Current.Time**
Member of [Manager.v1_1_0.Manager](#manager-v1_1_0-manager)

| | |
|---|---|
|Description|The build time of the firmware.|
|Type|string|
|Read Only|True|

**Oem.Hpe.Firmware.Current.VersionString**
Member of [Manager.v1_1_0.Manager](#manager-v1_1_0-manager)

| | |
|---|---|
|Description|The version string of the firmware. This value might be null if VersionString is unavailable.|
|Type|string or null|
|Read Only|True|

**Oem.Hpe.Firmware.Pending**
**Oem.Hpe.Firmware.Pending.BuildNumber**
Member of [Manager.v1_1_0.Manager](#manager-v1_1_0-manager)

| | |
|---|---|
|Description|The build number of the firmware.|
|Type|integer|
|Read Only|True|

**Oem.Hpe.Firmware.Pending.BuildNumberString**
Member of [Manager.v1_1_0.Manager](#manager-v1_1_0-manager)

| | |
|---|---|
|Description|The string version of the build number of the firmware.|
|Type|string|
|Read Only|True|

**Oem.Hpe.Firmware.Pending.Date**
Member of [Manager.v1_1_0.Manager](#manager-v1_1_0-manager)

| | |
|---|---|
|Description|The build date of the firmware.|
|Type|string|
|Read Only|True|

**Oem.Hpe.Firmware.Pending.DebugBuild**
Member of [Manager.v1_1_0.Manager](#manager-v1_1_0-manager)

| | |
|---|---|
|Description|True if the firmware is a debug build; False if it is not.|
|Type|boolean|
|Read Only|True|

**Oem.Hpe.Firmware.Pending.Family**
Member of [Manager.v1_1_0.Manager](#manager-v1_1_0-manager)

| | |
|---|---|
|Description|The family of the firmware.|
|Type|string|
|Read Only|True|

**Oem.Hpe.Firmware.Pending.MajorVersion**
Member of [Manager.v1_1_0.Manager](#manager-v1_1_0-manager)

| | |
|---|---|
|Description|The major version of the firmware.|
|Type|integer|
|Read Only|True|

**Oem.Hpe.Firmware.Pending.MinorVersion**
Member of [Manager.v1_1_0.Manager](#manager-v1_1_0-manager)

| | |
|---|---|
|Description|The minor version of the firmware.|
|Type|integer|
|Read Only|True|

**Oem.Hpe.Firmware.Pending.Time**
Member of [Manager.v1_1_0.Manager](#manager-v1_1_0-manager)

| | |
|---|---|
|Description|The build time of the firmware.|
|Type|string|
|Read Only|True|

**Oem.Hpe.Firmware.Pending.VersionString**
Member of [Manager.v1_1_0.Manager](#manager-v1_1_0-manager)

| | |
|---|---|
|Description|The version string of the firmware. This value might be null if VersionString is unavailable.|
|Type|string or null|
|Read Only|True|

### Oem.Hpe.FrontPanelUSB
**Oem.Hpe.FrontPanelUSB.State**
Member of [Manager.v1_1_0.Manager](#manager-v1_1_0-manager)

| | |
|---|---|
|Description|The state of the front USB port device.|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```Null```|A value is temporarily unavailable|
|```Ready```|iLO has not detected a front panel device.|
|```Busy```|iLO has detected a front panel device and is initializing or executing operations on the device.|
|```Complete```|iLO has successfully finished initializing or executing operations on the device.|
|```Error```|iLO failed to initialize or execute operations on the device.|
|```Disabled```|The front panel device is disabled by user configuration.|

### Oem.Hpe.IdleConnectionTimeoutMinutes
Member of [Manager.v1_1_0.Manager](#manager-v1_1_0-manager)

| | |
|---|---|
|Description|This setting specifies how long a user can be inactive before an iLO web interface ends automatically.|
|Type|integer|
|Read Only|False|

The following are the supported values:

|Value|
|---|
|```Null```|
|```15```|
|```30```|
|```60```|
|```120```|

### Oem.Hpe.IntegratedRemoteConsole
**Oem.Hpe.IntegratedRemoteConsole.HotKeys (array)**
Member of [Manager.v1_1_0.Manager](#manager-v1_1_0-manager)
```HotKeys``` is an array containing elements of:

**HotKeys[{item}].KeySequence (array)**
Member of [Manager.v1_1_0.Manager](#manager-v1_1_0-manager)
```KeySequence``` is an array containing elements of:


| | |
|---|---|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```NONE```|No key|
|```ESC```|Escape key|
|```L_ALT```|Left Alt key|
|```R_ALT```|Right Alt key|
|```L_SHIFT```|Left Shift key|
|```R_SHIFT```|Right Shift key|
|```L_CTRL```|Left Control key|
|```R_CTRL```|Right Control key|
|```L_GUI```|Left Windows key|
|```R_GUI```|Right Windows key|
|```INS```|Insert key|
|```DEL```|Delete key|
|```HOME```|Home key|
|```END```|End key|
|```PG_UP```|Page Up key|
|```PG_DN```|Page Down key|
|```ENTER```|Enter key|
|```TAB```|Tab key|
|```BREAK```|Break key|
|```BACKSPACE```|Backspace key|
|```NUM_PLUS```|Num Plus key|
|```NUM_MINUS```|Num Minus key|
|```SCRL_LCK```|Scroll Lock key|
|```SYS_RQ```|Sys Rq key|
|```PRINT_SCREEN```|Print Screen key|
|```F1```|F1 key|
|```F2```|F2 key|
|```F3```|F3 key|
|```F4```|F4 key|
|```F5```|F5 key|
|```F6```|F6 key|
|```F7```|F7 key|
|```F8```|F8 key|
|```F9```|F9 key|
|```F10```|F10 key|
|```F11```|F11 key|
|```F12```|F12 key|
|```SPACE```|Space key|
|```'```|Apostrophe key|
|```,```|Comma key|
|```-```|Hyphen key|
|```.```|Period key|
|```/```|Slash key|
|```;```|Semicolon key|
|```=```|Equals key|
|```[```|Left square bracket key|
|```\```|Backslash key|
|```]```|Right square bracket key|
|```````|Backtick key|
|```0```|0 key|
|```1```|1 key|
|```2```|2 key|
|```3```|3 key|
|```4```|4 key|
|```5```|5 key|
|```6```|6 key|
|```7```|7 key|
|```8```|8 key|
|```9```|9 key|
|```a```|a key|
|```b```|b key|
|```c```|c key|
|```d```|d key|
|```e```|e key|
|```f```|f key|
|```g```|g key|
|```h```|h key|
|```i```|i key|
|```j```|j key|
|```k```|k key|
|```l```|l key|
|```m```|m key|
|```n```|n key|
|```o```|o key|
|```p```|p key|
|```q```|q key|
|```r```|r key|
|```s```|s key|
|```t```|t key|
|```u```|u key|
|```v```|v key|
|```w```|w key|
|```x```|x key|
|```y```|y key|
|```z```|z key|

**Oem.Hpe.IntegratedRemoteConsole.LockKey**
**Oem.Hpe.IntegratedRemoteConsole.LockKey.CustomKeySequence (array)**
Member of [Manager.v1_1_0.Manager](#manager-v1_1_0-manager)
```CustomKeySequence``` is an array containing elements of:


| | |
|---|---|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```NONE```|No key|
|```ESC```|Escape key|
|```L_ALT```|Left Alt key|
|```R_ALT```|Right Alt key|
|```L_SHIFT```|Left Shift key|
|```R_SHIFT```|Right Shift key|
|```L_CTRL```|Left Control key|
|```R_CTRL```|Right Control key|
|```L_GUI```|Left Windows key|
|```R_GUI```|Right Windows key|
|```INS```|Insert key|
|```DEL```|Delete key|
|```HOME```|Home key|
|```END```|End key|
|```PG_UP```|Page Up key|
|```PG_DN```|Page Down key|
|```ENTER```|Enter key|
|```TAB```|Tab key|
|```BREAK```|Break key|
|```BACKSPACE```|Backspace key|
|```NUM_PLUS```|Num Plus key|
|```NUM_MINUS```|Num Minus key|
|```SCRL_LCK```|Scroll Lock key|
|```SYS_RQ```|Sys Rq key|
|```PRINT_SCREEN```|Print Screen key|
|```F1```|F1 key|
|```F2```|F2 key|
|```F3```|F3 key|
|```F4```|F4 key|
|```F5```|F5 key|
|```F6```|F6 key|
|```F7```|F7 key|
|```F8```|F8 key|
|```F9```|F9 key|
|```F10```|F10 key|
|```F11```|F11 key|
|```F12```|F12 key|
|```SPACE```|Space key|
|```'```|Apostrophe key|
|```,```|Comma key|
|```-```|Hyphen key|
|```.```|Period key|
|```/```|Slash key|
|```;```|Semicolon key|
|```=```|Equals key|
|```[```|Left square bracket key|
|```\```|Backslash key|
|```]```|Right square bracket key|
|```````|Backtick key|
|```0```|0 key|
|```1```|1 key|
|```2```|2 key|
|```3```|3 key|
|```4```|4 key|
|```5```|5 key|
|```6```|6 key|
|```7```|7 key|
|```8```|8 key|
|```9```|9 key|
|```a```|a key|
|```b```|b key|
|```c```|c key|
|```d```|d key|
|```e```|e key|
|```f```|f key|
|```g```|g key|
|```h```|h key|
|```i```|i key|
|```j```|j key|
|```k```|k key|
|```l```|l key|
|```m```|m key|
|```n```|n key|
|```o```|o key|
|```p```|p key|
|```q```|q key|
|```r```|r key|
|```s```|s key|
|```t```|t key|
|```u```|u key|
|```v```|v key|
|```w```|w key|
|```x```|x key|
|```y```|y key|
|```z```|z key|

**Oem.Hpe.IntegratedRemoteConsole.LockKey.LockOption**
Member of [Manager.v1_1_0.Manager](#manager-v1_1_0-manager)

| | |
|---|---|
|Description|Lock option setting.|
|Type|string|
|Read Only|False|

The following are the supported values:

|Value|Description|
|---|---|
|```Windows```|This option configures iLO to lock a managed server running a Windows operating system.|
|```Custom```|This option configures iLO to use a custom key sequence to lock a managed server or log out a user on that server.|
|```Disabled```|This option disables the Remote Console Computer Lock feature.|

**Oem.Hpe.IntegratedRemoteConsole.TrustedCertificateRequired**
Member of [Manager.v1_1_0.Manager](#manager-v1_1_0-manager)

| | |
|---|---|
|Description|When this setting is enabled and a trusted SSL certificate has been imported into iLO, the .NET IRC is launched by using an HTTPS connection. When this setting is disabled, the .NET IRC is launched by using a non-SSL connection.|
|Type|boolean|
|Read Only|False|

### Oem.Hpe.License
**Oem.Hpe.License.LicenseKey**
Member of [Manager.v1_1_0.Manager](#manager-v1_1_0-manager)

| | |
|---|---|
|Description|The installed license key.|
|Type|string|
|Read Only|True|

**Oem.Hpe.License.LicenseString**
Member of [Manager.v1_1_0.Manager](#manager-v1_1_0-manager)

| | |
|---|---|
|Description|Describes the type of license installed on management processor.|
|Type|string|
|Read Only|True|

**Oem.Hpe.License.LicenseType**
Member of [Manager.v1_1_0.Manager](#manager-v1_1_0-manager)

| | |
|---|---|
|Description|Indicates whether the license is Perpetual or Evaluation.|
|Type|string|
|Read Only|True|

### Oem.Hpe.PersistentMouseKeyboardEnabled
Member of [Manager.v1_1_0.Manager](#manager-v1_1_0-manager)

| | |
|---|---|
|Description|Persistent mouse and keyboard feature is enabled or not. When this feature is enabled, the iLO virtual mouse and keyboard are always connected to the iLO UHCI USB controller. When this feature is disabled, the iLO virtual mouse and keyboard are connected dynamically to the iLO UHCI controller only when a Remote Console application is open and connected to iLO.|
|Type|boolean|
|Read Only|False|

### Oem.Hpe.RIBCLEnabled
Member of [Manager.v1_1_0.Manager](#manager-v1_1_0-manager)

| | |
|---|---|
|Description|This property enables or disables RIBCL for the management processor. The management processor will require reset when this field is modified.|
|Type|boolean|
|Read Only|False|

### Oem.Hpe.RequiredLoginForiLORBSU
Member of [Manager.v1_1_0.Manager](#manager-v1_1_0-manager)

| | |
|---|---|
|Description|Determines whether a user-credential prompt is displayed when a user accesses the iLO RBSU or the iLO Configuration Utility. The following settings are valid: Enabled-A login dialog box opens when a user accesses the iLO RBSU or the iLO Configuration Utility. Disabled (default)-No login is required when a user accesses the iLO RBSU or the iLO Configuration Utility.|
|Type|boolean|
|Read Only|False|

### Oem.Hpe.SerialCLISpeed
Member of [Manager.v1_1_0.Manager](#manager-v1_1_0-manager)

| | |
|---|---|
|Description|Serial command line interface speed in bits/second.|
|Type|integer|
|Read Only|False|

The following are the supported values:

|Value|
|---|
|```9600```|
|```19200```|
|```38400```|
|```57600```|
|```115200```|

### Oem.Hpe.SerialCLIStatus
Member of [Manager.v1_1_0.Manager](#manager-v1_1_0-manager)

| | |
|---|---|
|Description|Status of serial command line interface.|
|Type|string or null|
|Read Only|False|

The following are the supported values:

|Value|Description|
|---|---|
|```Null```|A value is temporarily unavailable|
|```Disabled```|Serial command line interface is disabled.|
|```EnabledNoAuth```|Serial command line interface is enabled with no authentication required.|
|```EnabledAuthReq```|Serial command line interface is enabled with authentication required.|

### Oem.Hpe.VSPDlLoggingEnabled
Member of [Manager.v1_1_0.Manager](#manager-v1_1_0-manager)

| | |
|---|---|
|Description|This property enables or disables logging to the downloadable Virtual Serial Port (VSP) log.|
|Type|boolean|
|Read Only|False|

### Oem.Hpe.VSPLogDownloadEnabled
Member of [Manager.v1_1_0.Manager](#manager-v1_1_0-manager)

| | |
|---|---|
|Description|This property enables or disables download of the downloadable Virtual Serial Port (VSP) log.|
|Type|boolean|
|Read Only|False|

### Oem.Hpe.WebGuiEnabled
Member of [Manager.v1_1_0.Manager](#manager-v1_1_0-manager)

| | |
|---|---|
|Description|This property enables or disables WEB GUI access for the management processor. The management processor will require reset when this field is modified.|
|Type|boolean|
|Read Only|False|

### Oem.Hpe.iLOFunctionalityRequired
Member of [Manager.v1_1_0.Manager](#manager-v1_1_0-manager)

| | |
|---|---|
|Description|iLO functionality is required and can't be disabled on this platform (usually blades).|
|Type|boolean|
|Read Only|True|

### Oem.Hpe.iLOIPduringPOSTEnabled
Member of [Manager.v1_1_0.Manager](#manager-v1_1_0-manager)

| | |
|---|---|
|Description|Specifies whether displaying the iLO network IP address during host server POST is enabled(default) or not.|
|Type|boolean|
|Read Only|False|

### Oem.Hpe.iLORBSUEnabled
Member of [Manager.v1_1_0.Manager](#manager-v1_1_0-manager)

| | |
|---|---|
|Description|Enables or disables the iLO Configuration Utility. The following settings are valid: Enabled (default)-On servers that support the iLO Configuration Utility,  the iLO Configuration Utility is available when you access the UEFI System Utilities by pressing F9 during POST. Disabled-On servers that support the iLO Configuration Utility, the iLO Configuration Utility is not available when you access the UEFI System Utilities by pressing F9 during POST.|
|Type|boolean|
|Read Only|False|

### Oem.Hpe.iLOSelfTestResults (array)
Member of [Manager.v1_1_0.Manager](#manager-v1_1_0-manager)
```iLOSelfTestResults``` is an array containing elements of:

**iLOSelfTestResults[{item}].Notes**
Member of [Manager.v1_1_0.Manager](#manager-v1_1_0-manager)

| | |
|---|---|
|Description|Additional Information (if any) about the Self Test.|
|Type|string|
|Read Only|True|

**iLOSelfTestResults[{item}].SelfTestName**
Member of [Manager.v1_1_0.Manager](#manager-v1_1_0-manager)

| | |
|---|---|
|Description|iLO Self Test Name.|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```UnknownSelfTest```|UnknownSelfTest self test result.|
|```CryptographicHardware```|CryptographicHardware self test result.|
|```Memory```|Memory self test result.|
|```WebServerCryptography```|WebServerCryptography self test result.|
|```MiscCryptography```|MiscCryptography self test result.|
|```UART```|UART self test result.|
|```HoodSense```|Hood Sense self test result.|
|```NVRAMInterface```|NVRAMInterface self test result.|
|```NVRAMData```|NVRAMData self test result.|
|```NVRAMSpace```|NVRAM space self test result.|
|```NIC```|NIC self test result.|
|```EmbeddedFlash```|EmbeddedFlash or SD Card self test result.|
|```StaticRAM```|StaticRAM self test result.|
|```EEPROM```|EEPROM self test result.|
|```I2C```|I2C self test result.|
|```BootBlock```|BootBlock self test result.|
|```ThreadInit```|ThreadInit self test result.|
|```Infrastructure```|Infrastructure self test result.|
|```HostRom```||
|```SupportedHost```|Supported Host self test result.|
|```EEPROMContent```|EEPROMContent self test result.|
|```PowerManagementController```|Power Management Controller self test result.|
|```CPLDPAL0```|CPLD PAL0 self test result.|
|```CPLDPAL1```|CPLD PAL1 self test result.|
|```CPLDPAL2```|CPLD PAL2 self test result.|
|```CPLDPAL3```|CPLD PAL3 self test result.|
|```CPLDPAL4```|CPLD PAL4 self test result.|
|```CPLDPAL5```|CPLD PAL5 self test result.|
|```ASICFuses```|ASIC Fuses self test result.|

**iLOSelfTestResults[{item}].Status**
Member of [Manager.v1_1_0.Manager](#manager-v1_1_0-manager)
See the Redfish standard schema and specification for information on common Status object.

### Oem.Hpe.iLOServicePort
**Oem.Hpe.iLOServicePort.MassStorageAuthenticationRequired**
Member of [Manager.v1_1_0.Manager](#manager-v1_1_0-manager)

| | |
|---|---|
|Description|Indicates whether mass storage authentication is required or not.|
|Type|boolean|
|Read Only|False|

**Oem.Hpe.iLOServicePort.USBEthernetAdaptersEnabled**
Member of [Manager.v1_1_0.Manager](#manager-v1_1_0-manager)

| | |
|---|---|
|Description|Indicates whether the USB Ethernet Adapters are enabled or not.|
|Type|boolean|
|Read Only|False|

**Oem.Hpe.iLOServicePort.USBFlashDriveEnabled**
Member of [Manager.v1_1_0.Manager](#manager-v1_1_0-manager)

| | |
|---|---|
|Description|Indicates whether the USB Flash Drive is enabled or not.|
|Type|boolean|
|Read Only|False|

**Oem.Hpe.iLOServicePort.iLOServicePortEnabled**
Member of [Manager.v1_1_0.Manager](#manager-v1_1_0-manager)

| | |
|---|---|
|Description|Indicates whether the iLO Service Port is enabled or not.|
|Type|boolean|
|Read Only|False|

### Redundancy
Member of [Manager.v1_1_0.Manager](#manager-v1_1_0-manager)
See the Redfish standard schema and specification for information on common Redundancy object.

### SerialConsole
**SerialConsole.ConnectTypesSupported (array)**
Member of [Manager.v1_1_0.Manager](#manager-v1_1_0-manager)
```ConnectTypesSupported``` is an array containing elements of:


| | |
|---|---|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```SSH```|The controller supports a Serial Console connection using the SSH protocol|
|```Telnet```|The controller supports a Serial Console connection using the Telnet protocol|
|```IPMI```|The controller supports a Serial Console connection using the IPMI Serial-over-LAN (SOL) protocol|
|```Oem```||

**SerialConsole.MaxConcurrentSessions**
Member of [Manager.v1_1_0.Manager](#manager-v1_1_0-manager)

| | |
|---|---|
|Description|This is the maximum number of Serial Console sessions, regardless of protocol, that this manager supports.|
|Type|integer|
|Read Only|True|

**SerialConsole.ServiceEnabled**
Member of [Manager.v1_1_0.Manager](#manager-v1_1_0-manager)

| | |
|---|---|
|Description|Indicates if the Command Shell service is enabled for this manager.|
|Type|boolean|
|Read Only|False|

### Status
Member of [Manager.v1_1_0.Manager](#manager-v1_1_0-manager)
See the Redfish standard schema and specification for information on common Status object.

### UUID
Member of [Manager.v1_1_0.Manager](#manager-v1_1_0-manager)

| | |
|---|---|
|Description|This is a universally unique identifier that supervisory software uses to uniquely identify this manager. The UUID is assigned when the system is manufactured.|
|Type|string or null|
|Read Only|True|

### VirtualMedia
This is a reference to the virtual media services for this manager.
### Actions

**Manager.Reset**
Member of [Manager.v1_1_0.Manager](#manager-v1_1_0-manager)
There are no parameters for this action.

**HpeiLO.ClearRestApiState**
Member of [Manager.v1_1_0.Manager](#manager-v1_1_0-manager)
Clears the persistent state of the REST API.  Some portions of the API may not be available until after the server reboots.

There are no parameters for this action.

**HpeiLO.ResetToFactoryDefaults**
Member of [Manager.v1_1_0.Manager](#manager-v1_1_0-manager)
Resets the iLO to Factory Defaults.


**Parameters:**

**ResetType (string)**

|Value|Description|
|---|---|
|Default|Reset iLO to defaults, clear logs and reboot iLO.|

**HpeiLO.RequestFirmwareAndOsRecovery**
Member of [Manager.v1_1_0.Manager](#manager-v1_1_0-manager)
Requests that the Recovery Install set be invoked, and when complete causes a OS reinstallation.

There are no parameters for this action.

**HpeiLO.DisableiLOFunctionality**
Member of [Manager.v1_1_0.Manager](#manager-v1_1_0-manager)
This action will disable the iLO network and will terminate communications with operating system drivers.  To re-enable iLO functionality, use the iLO Configuration Utility (in the UEFI System Utilities) to set iLO Functionality to Enabled. For more information see the HPE UEFI System Utilities User Guide.  The action resets/reboots the manager.  iLO functionality cannot be disabled on server blades.

There are no parameters for this action.
## ManagerAccount.v1_0_0.ManagerAccount
```@odata.type: "#ManagerAccount.v1_0_0.ManagerAccount"```
### Resource Instances
|Uri|HTTP Allow|
|---|---|
|```/redfish/v1/accountservice/accounts/{item}/```|GET PATCH DELETE |

### Oem.Hpe.LoginName
Member of [ManagerAccount.v1_0_0.ManagerAccount](#manageraccount-v1_0_0-manageraccount)

| | |
|---|---|
|Description|Descriptive login name that helps to easily identify the owner of each user name. The login name does not have to be the same as the user name and must use printable characters. The maximum length for a user name is 39 characters.|
|Type|string|
|Read Only|False|

### Oem.Hpe.Privileges
**Oem.Hpe.Privileges.HostBIOSConfigPriv**
Member of [ManagerAccount.v1_0_0.ManagerAccount](#manageraccount-v1_0_0-manageraccount)

| | |
|---|---|
|Description|This privilege enables a user to configure Host Bios Settings.|
|Type|boolean|
|Read Only|False|

**Oem.Hpe.Privileges.HostNICConfigPriv**
Member of [ManagerAccount.v1_0_0.ManagerAccount](#manageraccount-v1_0_0-manageraccount)

| | |
|---|---|
|Description|This privilege enables a user to configure Host NIC Settings.|
|Type|boolean|
|Read Only|False|

**Oem.Hpe.Privileges.HostStorageConfigPriv**
Member of [ManagerAccount.v1_0_0.ManagerAccount](#manageraccount-v1_0_0-manageraccount)

| | |
|---|---|
|Description|This privilege enables a user to configure Host Storage Settings.|
|Type|boolean|
|Read Only|False|

**Oem.Hpe.Privileges.LoginPriv**
Member of [ManagerAccount.v1_0_0.ManagerAccount](#manageraccount-v1_0_0-manageraccount)

| | |
|---|---|
|Description|This privilege enables a user to log in to management processor. All local accounts have the login privilege. This privilege is added automatically if it is not specified.|
|Type|boolean|
|Read Only|False|

**Oem.Hpe.Privileges.RemoteConsolePriv**
Member of [ManagerAccount.v1_0_0.ManagerAccount](#manageraccount-v1_0_0-manageraccount)

| | |
|---|---|
|Description|This privilege enables a user to remotely access the host system Remote Console, including video, keyboard, and mouse control.|
|Type|boolean|
|Read Only|False|

**Oem.Hpe.Privileges.SystemRecoveryConfigPriv**
Member of [ManagerAccount.v1_0_0.ManagerAccount](#manageraccount-v1_0_0-manageraccount)

| | |
|---|---|
|Description|This privilege enables a user to manage the critical recovery firmware images on the iLO Repository.|
|Type|boolean|
|Read Only|False|

**Oem.Hpe.Privileges.UserConfigPriv**
Member of [ManagerAccount.v1_0_0.ManagerAccount](#manageraccount-v1_0_0-manageraccount)

| | |
|---|---|
|Description|This privilege enables a user to add, edit, and delete local management processor user accounts. A user with this privilege can change privileges for all users.|
|Type|boolean|
|Read Only|False|

**Oem.Hpe.Privileges.VirtualMediaPriv**
Member of [ManagerAccount.v1_0_0.ManagerAccount](#manageraccount-v1_0_0-manageraccount)

| | |
|---|---|
|Description|This privilege enables a user to use the Virtual Media feature on the host system.|
|Type|boolean|
|Read Only|False|

**Oem.Hpe.Privileges.VirtualPowerAndResetPriv**
Member of [ManagerAccount.v1_0_0.ManagerAccount](#manageraccount-v1_0_0-manageraccount)

| | |
|---|---|
|Description|This privilege enables a user to power-cycle or reset the host system. These activities interrupt system availability. A user with this privilege can diagnose the system by using the Generate NMI to System button.|
|Type|boolean|
|Read Only|False|

**Oem.Hpe.Privileges.iLOConfigPriv**
Member of [ManagerAccount.v1_0_0.ManagerAccount](#manageraccount-v1_0_0-manageraccount)

| | |
|---|---|
|Description|This privilege enables a user to configure most management processor settings, including security settings, and to remotely update the management processor firmware. This privilege does not enable local user account administration.|
|Type|boolean|
|Read Only|False|

### Oem.Hpe.ServiceAccount
Member of [ManagerAccount.v1_0_0.ManagerAccount](#manageraccount-v1_0_0-manageraccount)

| | |
|---|---|
|Description|Indicate that the account type is service account|
|Type|boolean|
|Read Only|True|

### Password
Member of [ManagerAccount.v1_0_0.ManagerAccount](#manageraccount-v1_0_0-manageraccount)

| | |
|---|---|
|Description|The password used to log in to the management processor. The maximum length for a password is 39 characters. The minimum length for a password is specified in the MinPasswordLength property of the AccountService schema.|
|Type|string or null|
|Read Only|False|

### UserName
Member of [ManagerAccount.v1_0_0.ManagerAccount](#manageraccount-v1_0_0-manageraccount)

| | |
|---|---|
|Description|The name used to log in to the management processor. The user name does not have to be the same as the login name. The maximum length for the user name is 39 characters. The user name must use printable characters.|
|Type|string|
|Read Only|False|

## ManagerNetworkProtocol.v1_0_0.ManagerNetworkProtocol
```@odata.type: "#ManagerNetworkProtocol.v1_0_0.ManagerNetworkProtocol"```

This resource is used to obtain or modify the network services managed by this manager.
### Resource Instances
|Uri|HTTP Allow|
|---|---|
|```/redfish/v1/managers/{item}/networkservice/```|GET POST PATCH |

### Links to other Resources
|Link Name|Destination type
|---|---|
|```Oem/Hpe/Links/SNMPService```|[HpeiLOSnmpService](#hpeilosnmpservice-v2_1_0-hpeilosnmpservice)|
|```Oem/Hpe/Links/EthernetInterfaces```|Collection of [EthernetInterface](#ethernetinterface-v1_0_3-ethernetinterface)|

### FQDN
Member of [ManagerNetworkProtocol.v1_0_0.ManagerNetworkProtocol](#managernetworkprotocol-v1_0_0-managernetworkprotocol)

| | |
|---|---|
|Description|The fully-qualified domain name of the manager that is obtained by DNS and includes the host name and top-level domain name.|
|Type|string or null|
|Read Only|True|

### HTTP
**HTTP.Port**
Member of [ManagerNetworkProtocol.v1_0_0.ManagerNetworkProtocol](#managernetworkprotocol-v1_0_0-managernetworkprotocol)

| | |
|---|---|
|Description|The HTTP port number.|
|Type|integer or null|
|Read Only|False|

**HTTP.ProtocolEnabled**
Member of [ManagerNetworkProtocol.v1_0_0.ManagerNetworkProtocol](#managernetworkprotocol-v1_0_0-managernetworkprotocol)

| | |
|---|---|
|Description|Indicates whether HTTP is enabled or disabled.|
|Type|boolean or null|
|Read Only|False|

### HTTPS
**HTTPS.Port**
Member of [ManagerNetworkProtocol.v1_0_0.ManagerNetworkProtocol](#managernetworkprotocol-v1_0_0-managernetworkprotocol)

| | |
|---|---|
|Description|The HTTPS/SSL port number.|
|Type|integer or null|
|Read Only|False|

**HTTPS.ProtocolEnabled**
Member of [ManagerNetworkProtocol.v1_0_0.ManagerNetworkProtocol](#managernetworkprotocol-v1_0_0-managernetworkprotocol)

| | |
|---|---|
|Description|Indicates whether HTTPS/SSL is enabled or disabled.|
|Type|boolean or null|
|Read Only|False|

### HostName
Member of [ManagerNetworkProtocol.v1_0_0.ManagerNetworkProtocol](#managernetworkprotocol-v1_0_0-managernetworkprotocol)

| | |
|---|---|
|Description|The host name of the manager that is obtained by DNS and does not include any domain information.|
|Type|string or null|
|Read Only|False|

### IPMI
**IPMI.Port**
Member of [ManagerNetworkProtocol.v1_0_0.ManagerNetworkProtocol](#managernetworkprotocol-v1_0_0-managernetworkprotocol)

| | |
|---|---|
|Description|The IPMI over LAN port number.|
|Type|integer or null|
|Read Only|False|

**IPMI.ProtocolEnabled**
Member of [ManagerNetworkProtocol.v1_0_0.ManagerNetworkProtocol](#managernetworkprotocol-v1_0_0-managernetworkprotocol)

| | |
|---|---|
|Description|Indicates whether IPMI over LAN is enabled for the manager.|
|Type|boolean or null|
|Read Only|False|

### KVMIP
**KVMIP.Port**
Member of [ManagerNetworkProtocol.v1_0_0.ManagerNetworkProtocol](#managernetworkprotocol-v1_0_0-managernetworkprotocol)

| | |
|---|---|
|Description|The KVM-IP port number.|
|Type|integer or null|
|Read Only|False|

**KVMIP.ProtocolEnabled**
Member of [ManagerNetworkProtocol.v1_0_0.ManagerNetworkProtocol](#managernetworkprotocol-v1_0_0-managernetworkprotocol)

| | |
|---|---|
|Description|Indicates whether KVM-IP is enabled for the manager.|
|Type|boolean or null|
|Read Only|False|

### Oem.Hpe.AlertMailEmail
Member of [ManagerNetworkProtocol.v1_0_0.ManagerNetworkProtocol](#managernetworkprotocol-v1_0_0-managernetworkprotocol)

| | |
|---|---|
|Description|The destination email address for email alerts.|
|Type|string|
|Read Only|False|

### Oem.Hpe.AlertMailEnabled
Member of [ManagerNetworkProtocol.v1_0_0.ManagerNetworkProtocol](#managernetworkprotocol-v1_0_0-managernetworkprotocol)

| | |
|---|---|
|Description|Indicates whether AlertMail is enabled. This can be enabled only when the properties AlertMailEmail, AlertMailSenderDomain and AlertMailSMTPServer are set or not empty.|
|Type|boolean|
|Read Only|False|

### Oem.Hpe.AlertMailSMTPPort
Member of [ManagerNetworkProtocol.v1_0_0.ManagerNetworkProtocol](#managernetworkprotocol-v1_0_0-managernetworkprotocol)

| | |
|---|---|
|Description|The SMTP server port number.|
|Type|integer|
|Read Only|False|

### Oem.Hpe.AlertMailSMTPServer
Member of [ManagerNetworkProtocol.v1_0_0.ManagerNetworkProtocol](#managernetworkprotocol-v1_0_0-managernetworkprotocol)

| | |
|---|---|
|Description|The IP address or DNS name of the SMTP server or the Mail Submission Agent (MSA).|
|Type|string|
|Read Only|False|

### Oem.Hpe.AlertMailSenderDomain
Member of [ManagerNetworkProtocol.v1_0_0.ManagerNetworkProtocol](#managernetworkprotocol-v1_0_0-managernetworkprotocol)

| | |
|---|---|
|Description|The domain name for the sender email address.|
|Type|string|
|Read Only|False|

### Oem.Hpe.ConfigurationSettings
Member of [ManagerNetworkProtocol.v1_0_0.ManagerNetworkProtocol](#managernetworkprotocol-v1_0_0-managernetworkprotocol)

| | |
|---|---|
|Description|State of the currently displayed configuration settings.|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|
|---|
|```Current```|
|```SomePendingReset```|

### Oem.Hpe.FederationEnabled
Member of [ManagerNetworkProtocol.v1_0_0.ManagerNetworkProtocol](#managernetworkprotocol-v1_0_0-managernetworkprotocol)

| | |
|---|---|
|Description|Indicates whether management processor federation management is enabled or disabled.|
|Type|boolean|
|Read Only|False|

### Oem.Hpe.FederationSupported
Member of [ManagerNetworkProtocol.v1_0_0.ManagerNetworkProtocol](#managernetworkprotocol-v1_0_0-managernetworkprotocol)

| | |
|---|---|
|Description|Indicates whether management processor federation is supported.|
|Type|boolean|
|Read Only|True|

### Oem.Hpe.RemoteSyslogEnabled
Member of [ManagerNetworkProtocol.v1_0_0.ManagerNetworkProtocol](#managernetworkprotocol-v1_0_0-managernetworkprotocol)

| | |
|---|---|
|Description|Indicates whether Remote Syslog is enabled. When enabled, management processor sends notification messages to the specified Syslog server. This can be enabled only when the property RemoteSyslogServer is set or not empty.|
|Type|boolean|
|Read Only|False|

### Oem.Hpe.RemoteSyslogPort
Member of [ManagerNetworkProtocol.v1_0_0.ManagerNetworkProtocol](#managernetworkprotocol-v1_0_0-managernetworkprotocol)

| | |
|---|---|
|Description|The port number through which the Syslog servers are listening.|
|Type|integer|
|Read Only|False|

### Oem.Hpe.RemoteSyslogServer
Member of [ManagerNetworkProtocol.v1_0_0.ManagerNetworkProtocol](#managernetworkprotocol-v1_0_0-managernetworkprotocol)

| | |
|---|---|
|Description|The IP address, FQDN, IPv6 name, or short name of the servers running the Syslog service.|
|Type|string|
|Read Only|False|

### Oem.Hpe.SNMPTrapPort
Member of [ManagerNetworkProtocol.v1_0_0.ManagerNetworkProtocol](#managernetworkprotocol-v1_0_0-managernetworkprotocol)

| | |
|---|---|
|Description|The SNMP trap port number.|
|Type|integer|
|Read Only|False|

### Oem.Hpe.SerialOverLanLogging
Member of [ManagerNetworkProtocol.v1_0_0.ManagerNetworkProtocol](#managernetworkprotocol-v1_0_0-managernetworkprotocol)

| | |
|---|---|
|Description|Indicates whether Serial Over LAN (SOL) or Virtual Serial Port (VSP) logging is enabled.|
|Type|boolean|
|Read Only|False|

### Oem.Hpe.XMLResponseEnabled
Member of [ManagerNetworkProtocol.v1_0_0.ManagerNetworkProtocol](#managernetworkprotocol-v1_0_0-managernetworkprotocol)

| | |
|---|---|
|Description|Determines whether management processor responds to anonymous XML discovery requests.|
|Type|boolean|
|Read Only|False|

### SNMP
**SNMP.Port**
Member of [ManagerNetworkProtocol.v1_0_0.ManagerNetworkProtocol](#managernetworkprotocol-v1_0_0-managernetworkprotocol)

| | |
|---|---|
|Description|The SNMP port number.|
|Type|integer or null|
|Read Only|False|

**SNMP.ProtocolEnabled**
Member of [ManagerNetworkProtocol.v1_0_0.ManagerNetworkProtocol](#managernetworkprotocol-v1_0_0-managernetworkprotocol)

| | |
|---|---|
|Description|Indicates whether SNMP is enabled for the manager.|
|Type|boolean or null|
|Read Only|False|

### SSDP
**SSDP.NotifyIPv6Scope**
Member of [ManagerNetworkProtocol.v1_0_0.ManagerNetworkProtocol](#managernetworkprotocol-v1_0_0-managernetworkprotocol)

| | |
|---|---|
|Description|The scope for IPv6 Notify messages for SSDP.|
|Type|string or null|
|Read Only|False|

The following are the supported values:

|Value|Description|
|---|---|
|```Null```|A value is temporarily unavailable|
|```Link```|SSDP Notify messages are sent to addresses in the IPv6 Local Link scope|
|```Site```|SSDP Notify messages are sent to addresses in the IPv6 Local Site scope.|
|```Organization```|SSDP Notify messages are sent to addresses in the IPv6 Local Organization scope.|

**SSDP.NotifyMulticastIntervalSeconds**
Member of [ManagerNetworkProtocol.v1_0_0.ManagerNetworkProtocol](#managernetworkprotocol-v1_0_0-managernetworkprotocol)

| | |
|---|---|
|Description|Indicates how often multicast is performed for SSDP. Allowed values are 0, 30, 60, 120, 300, 600, 900 or 1800.|
|Type|integer or null|
|Read Only|False|

**SSDP.NotifyTTL**
Member of [ManagerNetworkProtocol.v1_0_0.ManagerNetworkProtocol](#managernetworkprotocol-v1_0_0-managernetworkprotocol)

| | |
|---|---|
|Description|The Time to Live (TTL) hop count for SSDP Notify messages.|
|Type|integer or null|
|Read Only|False|

**SSDP.Port**
Member of [ManagerNetworkProtocol.v1_0_0.ManagerNetworkProtocol](#managernetworkprotocol-v1_0_0-managernetworkprotocol)

| | |
|---|---|
|Description|The SSDP port number.|
|Type|integer or null|
|Read Only|True|

**SSDP.ProtocolEnabled**
Member of [ManagerNetworkProtocol.v1_0_0.ManagerNetworkProtocol](#managernetworkprotocol-v1_0_0-managernetworkprotocol)

| | |
|---|---|
|Description|Indicates whether SSDP is enabled for the manager.|
|Type|boolean or null|
|Read Only|False|

### SSH
**SSH.Port**
Member of [ManagerNetworkProtocol.v1_0_0.ManagerNetworkProtocol](#managernetworkprotocol-v1_0_0-managernetworkprotocol)

| | |
|---|---|
|Description|The SSH port number.  NOTE: When this field is modified, the Manager will reset automatically.|
|Type|integer or null|
|Read Only|False|

**SSH.ProtocolEnabled**
Member of [ManagerNetworkProtocol.v1_0_0.ManagerNetworkProtocol](#managernetworkprotocol-v1_0_0-managernetworkprotocol)

| | |
|---|---|
|Description|Indicates whether SSH is enabled for the manager.  NOTE: When this field is modified, the Manager will reset automatically.|
|Type|boolean or null|
|Read Only|False|

### Status
Member of [ManagerNetworkProtocol.v1_0_0.ManagerNetworkProtocol](#managernetworkprotocol-v1_0_0-managernetworkprotocol)
See the Redfish standard schema and specification for information on common Status object.

### VirtualMedia
**VirtualMedia.Port**
Member of [ManagerNetworkProtocol.v1_0_0.ManagerNetworkProtocol](#managernetworkprotocol-v1_0_0-managernetworkprotocol)

| | |
|---|---|
|Description|The Virtual Media port number.|
|Type|integer or null|
|Read Only|False|

**VirtualMedia.ProtocolEnabled**
Member of [ManagerNetworkProtocol.v1_0_0.ManagerNetworkProtocol](#managernetworkprotocol-v1_0_0-managernetworkprotocol)

| | |
|---|---|
|Description|Indicates whether Virtual Media is enabled for the manager.|
|Type|boolean or null|
|Read Only|False|

### Actions

**HpeiLOManagerNetworkService.SendTestAlertMail**
Member of [ManagerNetworkProtocol.v1_0_0.ManagerNetworkProtocol](#managernetworkprotocol-v1_0_0-managernetworkprotocol)
There are no parameters for this action.

**HpeiLOManagerNetworkService.SendTestSyslog**
Member of [ManagerNetworkProtocol.v1_0_0.ManagerNetworkProtocol](#managernetworkprotocol-v1_0_0-managernetworkprotocol)
There are no parameters for this action.
## Memory.v1_1_0.Memory
```@odata.type: "#Memory.v1_1_0.Memory"```
### Resource Instances
|Uri|HTTP Allow|
|---|---|
|```/redfish/v1/systems/{item}/memory/{item}/```|GET |

### BaseModuleType
Member of [Memory.v1_1_0.Memory](#memory-v1_1_0-memory)

| | |
|---|---|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```RDIMM```|Registered DIMM|
|```UDIMM```|UDIMM|
|```SO_DIMM```|SO_DIMM|
|```LRDIMM```|Load Reduced|
|```Mini_RDIMM```|Mini_RDIMM|
|```Mini_UDIMM```|Mini_UDIMM|
|```SO_RDIMM_72b```|SO_RDIMM_72b|
|```SO_UDIMM_72b```|SO_UDIMM_72b|
|```SO_DIMM_16b```|SO_DIMM_16b|
|```SO_DIMM_32b```|SO_DIMM_32b|

### BusWidthBits
Member of [Memory.v1_1_0.Memory](#memory-v1_1_0-memory)

| | |
|---|---|
|Description|Bus Width in bits.|
|Type|number or null|
|Read Only|True|

### CapacityMiB
Member of [Memory.v1_1_0.Memory](#memory-v1_1_0-memory)

| | |
|---|---|
|Description|Memory Capacity in MiB.|
|Type|number or null|
|Read Only|True|

### DataWidthBits
Member of [Memory.v1_1_0.Memory](#memory-v1_1_0-memory)

| | |
|---|---|
|Description|Data Width in bits.|
|Type|number or null|
|Read Only|True|

### DeviceID
Member of [Memory.v1_1_0.Memory](#memory-v1_1_0-memory)

| | |
|---|---|
|Description|Device ID|
|Type|string or null|
|Read Only|True|

### DeviceLocator
Member of [Memory.v1_1_0.Memory](#memory-v1_1_0-memory)

| | |
|---|---|
|Description|Location of the Memory in the platform|
|Type|string or null|
|Read Only|True|

### ErrorCorrection
Member of [Memory.v1_1_0.Memory](#memory-v1_1_0-memory)

| | |
|---|---|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```NoECC```|No ECC available|
|```SingleBitECC```|Single bit Data error can be corrected by ECC|
|```MultiBitECC```|Multi-bit Data errors can be corrected by ECC|
|```AddressParity```|Address Parity errors can be corrected|

### FirmwareRevision
Member of [Memory.v1_1_0.Memory](#memory-v1_1_0-memory)

| | |
|---|---|
|Description|The firmware revision of this device|
|Type|string or null|
|Read Only|True|

### Manufacturer
Member of [Memory.v1_1_0.Memory](#memory-v1_1_0-memory)

| | |
|---|---|
|Description|The Memory manufacturer|
|Type|string or null|
|Read Only|True|

### MemoryDeviceType
Member of [Memory.v1_1_0.Memory](#memory-v1_1_0-memory)

| | |
|---|---|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```DDR```|DDR|
|```DDR2```|DDR2|
|```DDR3```|DDR3|
|```DDR4```|DDR4|
|```DDR4_SDRAM```|DDR4 SDRAM|
|```DDR4E_SDRAM```|DDR4E SDRAM|
|```LPDDR4_SDRAM```|LPDDR4 SDRAM|
|```DDR3_SDRAM```|DDR3 SDRAM|
|```LPDDR3_SDRAM```|LPDDR3 SDRAM|
|```DDR2_SDRAM```|DDR2 SDRAM|
|```DDR2_SDRAM_FB_DIMM```|DDR2 SDRAM FB_DIMM|
|```DDR2_SDRAM_FB_DIMM_PROBE```|DDR2 SDRAM FB_DIMM PROBE|
|```DDR_SGRAM```|DDR SGRAM|
|```DDR_SDRAM```|DDR SDRAM|
|```ROM```|ROM|
|```SDRAM```|SDRAM|
|```EDO```|EDO|
|```FastPageMode```|Fast Page Mode|
|```PipelinedNibble```|Pipelined Nibble|

### MemoryLocation
**MemoryLocation.Channel**
Member of [Memory.v1_1_0.Memory](#memory-v1_1_0-memory)

| | |
|---|---|
|Description|Channel number in which Memory is connected|
|Type|number or null|
|Read Only|True|

**MemoryLocation.MemoryController**
Member of [Memory.v1_1_0.Memory](#memory-v1_1_0-memory)

| | |
|---|---|
|Description|Memory controller number in which Memory is connected|
|Type|number or null|
|Read Only|True|

**MemoryLocation.Slot**
Member of [Memory.v1_1_0.Memory](#memory-v1_1_0-memory)

| | |
|---|---|
|Description|Slot number in which Memory is connected|
|Type|number or null|
|Read Only|True|

**MemoryLocation.Socket**
Member of [Memory.v1_1_0.Memory](#memory-v1_1_0-memory)

| | |
|---|---|
|Description|Socket number in which Memory is connected|
|Type|number or null|
|Read Only|True|

### MemoryMedia (array)
Member of [Memory.v1_1_0.Memory](#memory-v1_1_0-memory)
```MemoryMedia``` is an array containing elements of:


| | |
|---|---|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```DRAM```|DRAM media|
|```NAND```|NAND media|
|```Proprietary```|Proprietary media|

### MemoryType
Member of [Memory.v1_1_0.Memory](#memory-v1_1_0-memory)

| | |
|---|---|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```DRAM```|DRAM|
|```NVDIMM_N```|NVDIMM_N as defined by JEDEC.|
|```NVDIMM_F```|NVDIMM_F as defined by JEDEC.|
|```NVDIMM_P```|NVDIMM_P as defined by JEDEC.|

### Oem.Hpe.Armed
Member of [Memory.v1_1_0.Memory](#memory-v1_1_0-memory)

| | |
|---|---|
|Description|Specifies the current backup-ready status of the NVDIMM_N if available.|
|Type|boolean or null|
|Read Only|True|

### Oem.Hpe.Attributes (array)
Member of [Memory.v1_1_0.Memory](#memory-v1_1_0-memory)
```Attributes``` is an array containing elements of:


| | |
|---|---|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```HpeSmartMemory```|This DIMM is HPE Smart Memory|
|```HpeStandardMemory```|This DIMM is HPE Standard Memory|
|```HpeLogicalNVDIMM```|This DIMM is HPE Logical Memory.|

### Oem.Hpe.DIMMStatus
Member of [Memory.v1_1_0.Memory](#memory-v1_1_0-memory)

| | |
|---|---|
|Description|Specifies memory module status and whether the module in use.|
|Type|string or null|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```Null```|A value is temporarily unavailable|
|```Unknown```|The status of the DIMM is unknown.|
|```Other```|DIMM status that does not fit any of these definitions.|
|```NotPresent```|DIMM is not present.|
|```PresentUnused```|DIMM is present but unused.|
|```GoodInUse```|DIMM is functioning properly and currently in use.|
|```AddedButUnused```|DIMM is added but currently unused.|
|```UpgradedButUnused```|DIMM is upgraded but currently unused.|
|```ExpectedButMissing```|DIMM is expected but missing.|
|```DoesNotMatch```|DIMM type does not match.|
|```NotSupported```|DIMM is not supported.|
|```ConfigurationError```|Configuration error in DIMM.|
|```Degraded```|DIMM state is degraded.|
|```PresentSpare```|DIMM is present but used as spare.|
|```GoodPartiallyInUse```|DIMM is functioning properly but partially in use.|

### Oem.Hpe.MinimumVoltageVoltsX10
Member of [Memory.v1_1_0.Memory](#memory-v1_1_0-memory)

| | |
|---|---|
|Description|The minimum DIMM voltage multiplied by 10, for example, 1.2v = 12.|
|Type|integer or null|
|Read Only|True|

### Oem.Hpe.PredictedMediaLifeLeftPercent
Member of [Memory.v1_1_0.Memory](#memory-v1_1_0-memory)

| | |
|---|---|
|Description|The percentage of media life left.|
|Type|integer or null|
|Read Only|True|

### Oem.Hpe.ProductName
Member of [Memory.v1_1_0.Memory](#memory-v1_1_0-memory)

| | |
|---|---|
|Description|friendly product name from SMBIOS 202 record|
|Type|string|
|Read Only|True|

### Oem.Hpe.RelatedBackupStores (array)
Member of [Memory.v1_1_0.Memory](#memory-v1_1_0-memory)
```RelatedBackupStores``` is an array containing elements of:

### Oem.Hpe.RelatedPhysicalDIMMs (array)
Member of [Memory.v1_1_0.Memory](#memory-v1_1_0-memory)
```RelatedPhysicalDIMMs``` is an array containing elements of:

### Oem.Hpe.RelatedPowerBackupUnitBays (array)
Member of [Memory.v1_1_0.Memory](#memory-v1_1_0-memory)
```RelatedPowerBackupUnitBays``` is an array containing elements of:


| | |
|---|---|
|Description|Battery backup unit bay number.|
|Type|integer|
|Read Only|True|

### Oem.Hpe.SPDBytes (array)
Member of [Memory.v1_1_0.Memory](#memory-v1_1_0-memory)
```SPDBytes``` is an array containing elements of:


| | |
|---|---|
|Description|The SPD Bytes in the DIMM|
|Type|integer|
|Read Only|True|

### OperatingMemoryModes (array)
Member of [Memory.v1_1_0.Memory](#memory-v1_1_0-memory)
```OperatingMemoryModes``` is an array containing elements of:


| | |
|---|---|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```Volatile```|Volatile memory|
|```PMEM```|Persistent memory, byte accesible through system address space|
|```Block```|Block accessible system memory|

### OperatingSpeedMhz
Member of [Memory.v1_1_0.Memory](#memory-v1_1_0-memory)

| | |
|---|---|
|Description|Operating speed of Memory in MHz|
|Type|number or null|
|Read Only|True|

### PartNumber
Member of [Memory.v1_1_0.Memory](#memory-v1_1_0-memory)

| | |
|---|---|
|Description|The product part number of this device|
|Type|string or null|
|Read Only|True|

### PersistentRegionSizeLimitMiB
Member of [Memory.v1_1_0.Memory](#memory-v1_1_0-memory)

| | |
|---|---|
|Description|Total size of persistent regions in MiB|
|Type|number or null|
|Read Only|True|

### RankCount
Member of [Memory.v1_1_0.Memory](#memory-v1_1_0-memory)

| | |
|---|---|
|Description|Number of ranks available in the Memory|
|Type|number or null|
|Read Only|True|

### SerialNumber
Member of [Memory.v1_1_0.Memory](#memory-v1_1_0-memory)

| | |
|---|---|
|Description|The serial number of this device|
|Type|string or null|
|Read Only|True|

### Status
Member of [Memory.v1_1_0.Memory](#memory-v1_1_0-memory)
See the Redfish standard schema and specification for information on common Status object.

### SubsystemDeviceID
Member of [Memory.v1_1_0.Memory](#memory-v1_1_0-memory)

| | |
|---|---|
|Description|Subsystem Device ID|
|Type|string or null|
|Read Only|True|

### SubsystemVendorID
Member of [Memory.v1_1_0.Memory](#memory-v1_1_0-memory)

| | |
|---|---|
|Description|SubSystem Vendor ID|
|Type|string or null|
|Read Only|True|

### VendorID
Member of [Memory.v1_1_0.Memory](#memory-v1_1_0-memory)

| | |
|---|---|
|Description|Vendor ID|
|Type|string or null|
|Read Only|True|

### VolatileRegionSizeLimitMiB
Member of [Memory.v1_1_0.Memory](#memory-v1_1_0-memory)

| | |
|---|---|
|Description|Total size of volatile regions in MiB|
|Type|number or null|
|Read Only|True|

## NetworkAdapter.v1_0_1.NetworkAdapter
```@odata.type: "#NetworkAdapter.v1_0_1.NetworkAdapter"```

A NetworkAdapter represents the physical network adapter capable of connecting to a computer network.  Examples include but are not limited to Ethernet, Fibre Channel, and converged network adapters.
### Resource Instances
|Uri|HTTP Allow|
|---|---|
|```/redfish/v1/chassis/{item}/networkadapters/{item}/```|GET |
|```/redfish/v1/chassis/{item}/networkadapters/{item}/Settings/```|GET POST PATCH |

### Controllers (array)
Member of [NetworkAdapter.v1_0_1.NetworkAdapter](#networkadapter-v1_0_1-networkadapter)
```Controllers``` is an array containing elements of:

**Controllers[{item}].ControllerCapabilities**
**Controllers[{item}].ControllerCapabilities.DataCenterBridging**
**Controllers[{item}].ControllerCapabilities.DataCenterBridging.Capable**
Member of [NetworkAdapter.v1_0_1.NetworkAdapter](#networkadapter-v1_0_1-networkadapter)

| | |
|---|---|
|Description|The value of this property shall be a boolean indicating whether this controller is capable of Data Center Bridging (DCB).|
|Type|boolean or null|
|Read Only|True|

**Controllers[{item}].ControllerCapabilities.NPIV**
**Controllers[{item}].ControllerCapabilities.NPIV.MaxDeviceLogins**
Member of [NetworkAdapter.v1_0_1.NetworkAdapter](#networkadapter-v1_0_1-networkadapter)

| | |
|---|---|
|Description|The maximum number of N_Port ID Virtualization (NPIV) logins allowed simultaneously from all ports on this controller.|
|Type|number or null|
|Read Only|True|

**Controllers[{item}].ControllerCapabilities.NPIV.MaxPortLogins**
Member of [NetworkAdapter.v1_0_1.NetworkAdapter](#networkadapter-v1_0_1-networkadapter)

| | |
|---|---|
|Description|The maximum number of N_Port ID Virtualization (NPIV) logins allowed per physical port on this controller.|
|Type|number or null|
|Read Only|True|

**Controllers[{item}].ControllerCapabilities.NetworkDeviceFunctionCount**
Member of [NetworkAdapter.v1_0_1.NetworkAdapter](#networkadapter-v1_0_1-networkadapter)

| | |
|---|---|
|Description|The maximum number of physical functions available on this controller.|
|Type|number or null|
|Read Only|True|

**Controllers[{item}].ControllerCapabilities.NetworkPortCount**
Member of [NetworkAdapter.v1_0_1.NetworkAdapter](#networkadapter-v1_0_1-networkadapter)

| | |
|---|---|
|Description|The number of physical ports on this controller.|
|Type|number or null|
|Read Only|True|

**Controllers[{item}].ControllerCapabilities.VirtualizationOffload**
**Controllers[{item}].ControllerCapabilities.VirtualizationOffload.SRIOV**
**Controllers[{item}].ControllerCapabilities.VirtualizationOffload.SRIOV.SRIOVVEPACapable**
Member of [NetworkAdapter.v1_0_1.NetworkAdapter](#networkadapter-v1_0_1-networkadapter)

| | |
|---|---|
|Description|The value of this property shall be a boolean indicating whether this controller supports Single Root Input/Output Virtualization (SR-IOV) in Virtual Ethernet Port Aggregator (VEPA) mode.|
|Type|boolean or null|
|Read Only|True|

**Controllers[{item}].ControllerCapabilities.VirtualizationOffload.VirtualFunction**
**Controllers[{item}].ControllerCapabilities.VirtualizationOffload.VirtualFunction.DeviceMaxCount**
Member of [NetworkAdapter.v1_0_1.NetworkAdapter](#networkadapter-v1_0_1-networkadapter)

| | |
|---|---|
|Description|The maximum number of Virtual Functions (VFs) supported by this controller.|
|Type|number or null|
|Read Only|True|

**Controllers[{item}].ControllerCapabilities.VirtualizationOffload.VirtualFunction.MinAssignmentGroupSize**
Member of [NetworkAdapter.v1_0_1.NetworkAdapter](#networkadapter-v1_0_1-networkadapter)

| | |
|---|---|
|Description|The minimum number of Virtual Functions (VFs) that can be allocated or moved between physical functions for this controller.|
|Type|number or null|
|Read Only|True|

**Controllers[{item}].ControllerCapabilities.VirtualizationOffload.VirtualFunction.NetworkPortMaxCount**
Member of [NetworkAdapter.v1_0_1.NetworkAdapter](#networkadapter-v1_0_1-networkadapter)

| | |
|---|---|
|Description|The maximum number of Virtual Functions (VFs) supported per network port for this controller.|
|Type|number or null|
|Read Only|True|

**Controllers[{item}].FirmwarePackageVersion**
Member of [NetworkAdapter.v1_0_1.NetworkAdapter](#networkadapter-v1_0_1-networkadapter)

| | |
|---|---|
|Description|The version number of the user-facing firmware package.|
|Type|string or null|
|Read Only|True|

### Manufacturer
Member of [NetworkAdapter.v1_0_1.NetworkAdapter](#networkadapter-v1_0_1-networkadapter)

| | |
|---|---|
|Description|The manufacturer or OEM of this network adapter.|
|Type|string or null|
|Read Only|True|

### Model
Member of [NetworkAdapter.v1_0_1.NetworkAdapter](#networkadapter-v1_0_1-networkadapter)

| | |
|---|---|
|Description|The model string used by the manufacturer to reference this network adapter.|
|Type|string or null|
|Read Only|True|

### NetworkDeviceFunctions (array)
Member of [NetworkAdapter.v1_0_1.NetworkAdapter](#networkadapter-v1_0_1-networkadapter)
```NetworkDeviceFunctions``` is an array containing elements of:

### NetworkPorts (array)
Member of [NetworkAdapter.v1_0_1.NetworkAdapter](#networkadapter-v1_0_1-networkadapter)
```NetworkPorts``` is an array containing elements of:

### Oem.Hpe.CLPVersion
Member of [NetworkAdapter.v1_0_1.NetworkAdapter](#networkadapter-v1_0_1-networkadapter)

| | |
|---|---|
|Description|Option ROM Systems Management Architecture for Server Hardware (SMASH) Command Line Protocol (CLP) support version.|
|Type|string|
|Read Only|True|

### Oem.Hpe.Controllers (array)
Member of [NetworkAdapter.v1_0_1.NetworkAdapter](#networkadapter-v1_0_1-networkadapter)
```Controllers``` is an array containing elements of:

**Controllers[{item}].ConfigurationStatus**
**Controllers[{item}].ConfigurationStatus.Detail (array)**
Member of [NetworkAdapter.v1_0_1.NetworkAdapter](#networkadapter-v1_0_1-networkadapter)
```Detail``` is an array containing elements of:

**Detail[{item}].Group**
Member of [NetworkAdapter.v1_0_1.NetworkAdapter](#networkadapter-v1_0_1-networkadapter)

| | |
|---|---|
|Description|Configuration group identifier.|
|Type|integer|
|Read Only|True|

**Detail[{item}].SubGroup**
Member of [NetworkAdapter.v1_0_1.NetworkAdapter](#networkadapter-v1_0_1-networkadapter)

| | |
|---|---|
|Description|Configuration sub-group identifier.|
|Type|integer|
|Read Only|True|

**Detail[{item}].Summary**
Member of [NetworkAdapter.v1_0_1.NetworkAdapter](#networkadapter-v1_0_1-networkadapter)

| | |
|---|---|
|Description|A digest value representing the current state of configuration for this group/sub-group.|
|Type|integer|
|Read Only|True|

**Controllers[{item}].ConfigurationStatus.Summary**
Member of [NetworkAdapter.v1_0_1.NetworkAdapter](#networkadapter-v1_0_1-networkadapter)

| | |
|---|---|
|Description|A digest value representing the current configuration state of this network adapter controller.|
|Type|integer|
|Read Only|True|

**Controllers[{item}].DeviceLimitationsBitmap**
Member of [NetworkAdapter.v1_0_1.NetworkAdapter](#networkadapter-v1_0_1-networkadapter)

| | |
|---|---|
|Description|Indicates any unique device limitations. A value of 0 indicates no limitations are present. When set, bit 0 indicates that the device cannot validate data received when in standby power. All other bit mappings are reserved.|
|Type|integer|
|Read Only|True|

**Controllers[{item}].EdgeVirtualBridging**
**Controllers[{item}].EdgeVirtualBridging.ChannelDescriptionTLVCapable**
Member of [NetworkAdapter.v1_0_1.NetworkAdapter](#networkadapter-v1_0_1-networkadapter)

| | |
|---|---|
|Description|When true, this controller supports HPE Flex10Qbg Channel Description TLVs.|
|Type|boolean|
|Read Only|True|

**Controllers[{item}].EdgeVirtualBridging.ChannelLinkControlTLVCapable**
Member of [NetworkAdapter.v1_0_1.NetworkAdapter](#networkadapter-v1_0_1-networkadapter)

| | |
|---|---|
|Description|When true, this controller supports HPE Flex10Qbg Channel Link Control TLVs.|
|Type|boolean|
|Read Only|True|

**Controllers[{item}].FactoryDefaultsCurrentlyActive**
Member of [NetworkAdapter.v1_0_1.NetworkAdapter](#networkadapter-v1_0_1-networkadapter)

| | |
|---|---|
|Description|When true, this controller's configuration matches factory default settings.|
|Type|boolean|
|Read Only|True|

**Controllers[{item}].FunctionTypeLimits (array)**
Member of [NetworkAdapter.v1_0_1.NetworkAdapter](#networkadapter-v1_0_1-networkadapter)
```FunctionTypeLimits``` is an array containing elements of:

**FunctionTypeLimits[{item}].ConstraintDescription**
Member of [NetworkAdapter.v1_0_1.NetworkAdapter](#networkadapter-v1_0_1-networkadapter)

| | |
|---|---|
|Type|string|
|Read Only|True|

**FunctionTypeLimits[{item}].EthernetResourcesConsumed**
Member of [NetworkAdapter.v1_0_1.NetworkAdapter](#networkadapter-v1_0_1-networkadapter)

| | |
|---|---|
|Type|integer|
|Read Only|True|

**FunctionTypeLimits[{item}].FCoEResourcesConsumed**
Member of [NetworkAdapter.v1_0_1.NetworkAdapter](#networkadapter-v1_0_1-networkadapter)

| | |
|---|---|
|Type|integer|
|Read Only|True|

**FunctionTypeLimits[{item}].RDMAResourcesConsumed**
Member of [NetworkAdapter.v1_0_1.NetworkAdapter](#networkadapter-v1_0_1-networkadapter)

| | |
|---|---|
|Type|integer|
|Read Only|True|

**FunctionTypeLimits[{item}].TotalSharedResourcesAvailable**
Member of [NetworkAdapter.v1_0_1.NetworkAdapter](#networkadapter-v1_0_1-networkadapter)

| | |
|---|---|
|Type|integer|
|Read Only|True|

**FunctionTypeLimits[{item}].iSCSIResourcesConsumed**
Member of [NetworkAdapter.v1_0_1.NetworkAdapter](#networkadapter-v1_0_1-networkadapter)

| | |
|---|---|
|Type|integer|
|Read Only|True|

**Controllers[{item}].MostRecentConfigurationChangeSource**
Member of [NetworkAdapter.v1_0_1.NetworkAdapter](#networkadapter-v1_0_1-networkadapter)

| | |
|---|---|
|Description|Type of the last client to have changed configuration on this device.|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```None```|No change detected.|
|```OS```|Operating System Driver|
|```VendorControl```|Vendor Control Software|
|```VirtualConnect```|Virtual Connect|
|```CNU```|Converged Network Utility|
|```Other```|Other configuration or diagnostic software.|
|```Redfish```|Redfish Client|
|```UEFI-HII```|UEFI Human Interface Infrastructure|

### Oem.Hpe.FactoryDefaultsActuationBehavior
Member of [NetworkAdapter.v1_0_1.NetworkAdapter](#networkadapter-v1_0_1-networkadapter)

| | |
|---|---|
|Description|Indicates the implementation timing of a reset to factory default settings request, when made with the server in the standby power state.|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```Immediate```|Defaults take effect within 2 seconds of being applied.|
|```AtFullPower```|Defaults take effect within 5 seconds of power being applied.|
|```AtNextReboot```|Defaults take effect on next reboot to full power.|

### Oem.Hpe.PCAVersion
Member of [NetworkAdapter.v1_0_1.NetworkAdapter](#networkadapter-v1_0_1-networkadapter)

| | |
|---|---|
|Description|Printed Circuit Assembly number for the circuit board comprising this device.|
|Type|string|
|Read Only|True|

### Oem.Hpe.RedfishConfiguration
Member of [NetworkAdapter.v1_0_1.NetworkAdapter](#networkadapter-v1_0_1-networkadapter)

| | |
|---|---|
|Description|Controls Redfish configuration write access to network adapters.  When present and disabled, network adapter information is read-only.  Note that some HPE advanced network adapters will present a reduced level of capability when disabled.|
|Type|string|
|Read Only|False|

The following are the supported values:

|Value|Description|
|---|---|
|```Enabled```|The Redfish management interface is enabled to make changes on this network adapter.  To return to the Disabled state, a network adapter reset to factory default operation is required.|
|```Disabled```|The network adapter is operating in read-only mode relative to the Redfish management interface. To transition to this state, a network adapter reset to factory default operation is required.|

### PartNumber
Member of [NetworkAdapter.v1_0_1.NetworkAdapter](#networkadapter-v1_0_1-networkadapter)

| | |
|---|---|
|Description|Manufacturer's Part number for this network adapter.|
|Type|string or null|
|Read Only|True|

### SKU
Member of [NetworkAdapter.v1_0_1.NetworkAdapter](#networkadapter-v1_0_1-networkadapter)

| | |
|---|---|
|Description|The value of this property shall contain the Stock Keeping Unit (SKU) for the network adapter.|
|Type|string or null|
|Read Only|True|

### SerialNumber
Member of [NetworkAdapter.v1_0_1.NetworkAdapter](#networkadapter-v1_0_1-networkadapter)

| | |
|---|---|
|Description|The serial number for this network adapter.|
|Type|string or null|
|Read Only|True|

### Settings
**Settings.href**
Member of [NetworkAdapter.v1_0_1.NetworkAdapter](#networkadapter-v1_0_1-networkadapter)

| | |
|---|---|
|Description|Reference to the resource the client may PUT/PATCH to in order to change this resource.|
|Type|string|
|Read Only|True|

### Status
Member of [NetworkAdapter.v1_0_1.NetworkAdapter](#networkadapter-v1_0_1-networkadapter)
See the Redfish standard schema and specification for information on common Status object.

### Actions

**NetworkAdapter.ResetSettingsToDefault**
Member of [NetworkAdapter.v1_0_1.NetworkAdapter](#networkadapter-v1_0_1-networkadapter)
There are no parameters for this action.

**NetworkAdapter.FlushConfigurationToNVM**
Member of [NetworkAdapter.v1_0_1.NetworkAdapter](#networkadapter-v1_0_1-networkadapter)
There are no parameters for this action.
## NetworkDeviceFunction.v1_1_0.NetworkDeviceFunction
```@odata.type: "#NetworkDeviceFunction.v1_1_0.NetworkDeviceFunction"```

A Network Device Function represents a logical interface exposed by the network adapter.
### Resource Instances
|Uri|HTTP Allow|
|---|---|
|```/redfish/v1/chassis/{item}/networkadapters/{item}/networkdevicefunctions/{item}/```|GET |
|```/redfish/v1/chassis/{item}/networkadapters/{item}/networkdevicefunctions/{item}/settings/```|GET POST PATCH |

### Links to other Resources
|Link Name|Destination type
|---|---|
|```@Redfish.Settings/SettingsObject```|[NetworkDeviceFunction](#networkdevicefunction-v1_1_0-networkdevicefunction)|

### AssignablePhysicalPorts (array)
Member of [NetworkDeviceFunction.v1_1_0.NetworkDeviceFunction](#networkdevicefunction-v1_1_0-networkdevicefunction)
```AssignablePhysicalPorts``` is an array containing elements of:


| | |
|---|---|
|Type|string|
|Read Only|True|

### AssignablePhysicalPorts@odata.count
Member of [NetworkDeviceFunction.v1_1_0.NetworkDeviceFunction](#networkdevicefunction-v1_1_0-networkdevicefunction)

| | |
|---|---|
|Description|The total number of assignable physical ports.|
|Type|integer|
|Read Only|True|

### BootMode
Member of [NetworkDeviceFunction.v1_1_0.NetworkDeviceFunction](#networkdevicefunction-v1_1_0-networkdevicefunction)

| | |
|---|---|
|Description|Network device boot mode configuration values.|
|Type|string|
|Read Only|False|

The following are the supported values:

|Value|Description|
|---|---|
|```Disabled```|Do not indicate to UEFI/BIOS that this device is bootable.|
|```PXE```|Boot this device using the embedded PXE support.  Only applicable if the NetworkDeviceFunctionType is set to Ethernet. Not supported by HPE.|
|```iSCSI```|Boot this device using the embedded iSCSI boot support and configuration.  Only applicable if the NetworkDeviceFunctionType is set to iSCSI.|
|```FibreChannel```|Boot this device using the embedded Fibre Channel support and configuration.  Only applicable if the NetworkDeviceFunctionType is set to FibreChannel.|
|```FibreChannelOverEthernet```|Boot this device using the embedded Fibre Channel over Ethernet (FCoE) boot support and configuration.  Only applicable if the NetworkDeviceFunctionType is set to FibreChannelOverEthernet.|

### DeviceEnabled
Member of [NetworkDeviceFunction.v1_1_0.NetworkDeviceFunction](#networkdevicefunction-v1_1_0-networkdevicefunction)

| | |
|---|---|
|Description|A boolean indicating whether the network device function is enabled. Disabled network device functions shall not be enumerated or seen by the operating system.|
|Type|boolean or null|
|Read Only|False|

### Ethernet
**Ethernet.MACAddress**
Member of [NetworkDeviceFunction.v1_1_0.NetworkDeviceFunction](#networkdevicefunction-v1_1_0-networkdevicefunction)

| | |
|---|---|
|Description|The effective current MAC Address of this network device function. If an assignable MAC address is not supported, this is a read only alias of the PermanentMACAddress.|
|Type|string or null|
|Read Only|False|

**Ethernet.MTUSize**
Member of [NetworkDeviceFunction.v1_1_0.NetworkDeviceFunction](#networkdevicefunction-v1_1_0-networkdevicefunction)

| | |
|---|---|
|Description|The Maximum Transmission Unit (MTU) configured for this Network Device Function.  This value serves as a default for the OS driver when booting.  The value only takes-effect on boot.|
|Type|number or null|
|Read Only|False|

**Ethernet.PermanentMACAddress**
Member of [NetworkDeviceFunction.v1_1_0.NetworkDeviceFunction](#networkdevicefunction-v1_1_0-networkdevicefunction)

| | |
|---|---|
|Description|The Permanent MAC Address of this network device function (physical function). This value is typically programmed during the manufacturing time. This address is not assignable.|
|Type|string or null|
|Read Only|True|

### FibreChannel
**FibreChannel.AllowFIPVLANDiscovery**
Member of [NetworkDeviceFunction.v1_1_0.NetworkDeviceFunction](#networkdevicefunction-v1_1_0-networkdevicefunction)

| | |
|---|---|
|Description|For FCoE connections, a boolean indicating whether the FIP VLAN Discovery Protocol is used to determine the FCoE VLAN ID selected by the network device function for the FCoE connection.  If true, and the FIP VLAN Discovery succeeds, the FCoEActiveVLANId property shall reflect the FCoE VLAN ID to be used for all FCoE traffic.  If false, or if the FIP VLAN Discovery protocol fails, the FCoELocalVLANId shall be used for all FCoE traffic and the FCoEActiveVLANId shall reflect the FCoELocalVLANId.|
|Type|boolean or null|
|Read Only|False|

**FibreChannel.BootTargets (array)**
Member of [NetworkDeviceFunction.v1_1_0.NetworkDeviceFunction](#networkdevicefunction-v1_1_0-networkdevicefunction)
```BootTargets``` is an array containing elements of:

**BootTargets[{item}].BootPriority**
Member of [NetworkDeviceFunction.v1_1_0.NetworkDeviceFunction](#networkdevicefunction-v1_1_0-networkdevicefunction)

| | |
|---|---|
|Description|The relative priority for this entry in the boot targets array.  Lower numbers shall represent higher priority, with zero being the highest priority.  The BootPriority shall be unique for all entries of the BootTargets array.|
|Type|number or null|
|Read Only|False|

**BootTargets[{item}].LUNID**
Member of [NetworkDeviceFunction.v1_1_0.NetworkDeviceFunction](#networkdevicefunction-v1_1_0-networkdevicefunction)

| | |
|---|---|
|Description|The Logical Unit Number (LUN) ID to boot from on the device referred to by the corresponding WWPN.|
|Type|string or null|
|Read Only|False|

**BootTargets[{item}].WWPN**
Member of [NetworkDeviceFunction.v1_1_0.NetworkDeviceFunction](#networkdevicefunction-v1_1_0-networkdevicefunction)

| | |
|---|---|
|Description|The value of this property shall be World-Wide Port Name (WWPN) to boot from.|
|Type|string or null|
|Read Only|False|

**FibreChannel.FCoEActiveVLANId**
Member of [NetworkDeviceFunction.v1_1_0.NetworkDeviceFunction](#networkdevicefunction-v1_1_0-networkdevicefunction)

| | |
|---|---|
|Description|For FCoE connections, the value of this property shall be null or a VLAN ID currently being used for FCoE traffic.  When the FCoE link is down this value shall be null.  When the FCoE link is up this value shall be either the FCoELocalVLANId property or a VLAN discovered via the FIP protocol.|
|Type|number or null|
|Read Only|True|

**FibreChannel.FCoELocalVLANId**
Member of [NetworkDeviceFunction.v1_1_0.NetworkDeviceFunction](#networkdevicefunction-v1_1_0-networkdevicefunction)

| | |
|---|---|
|Description|For FCoE connections, the locally configured VLAN ID.  This value shall be used for FCoE traffic to this network device function during boot unless AllowFIPVLANDiscovery is true and a valid FCoE VLAN ID is found via the FIP VLAN Discovery Protocol.|
|Type|number or null|
|Read Only|False|

**FibreChannel.PermanentWWNN**
Member of [NetworkDeviceFunction.v1_1_0.NetworkDeviceFunction](#networkdevicefunction-v1_1_0-networkdevicefunction)

| | |
|---|---|
|Description|The permanent World-Wide Node Name (WWNN) of this network device function (physical function). This value is typically programmed during the manufacturing time. This address is not assignable.|
|Type|string or null|
|Read Only|True|

**FibreChannel.PermanentWWPN**
Member of [NetworkDeviceFunction.v1_1_0.NetworkDeviceFunction](#networkdevicefunction-v1_1_0-networkdevicefunction)

| | |
|---|---|
|Type|string or null|
|Read Only|True|

**FibreChannel.WWNN**
Member of [NetworkDeviceFunction.v1_1_0.NetworkDeviceFunction](#networkdevicefunction-v1_1_0-networkdevicefunction)

| | |
|---|---|
|Description|The value of this property shall be the effective current World-Wide Node Name (WWNN) of this network device function (physical function). If an assignable WWNN is not supported, this is a read only alias of the PermanentWWNN.|
|Type|string or null|
|Read Only|False|

**FibreChannel.WWNSource**
Member of [NetworkDeviceFunction.v1_1_0.NetworkDeviceFunction](#networkdevicefunction-v1_1_0-networkdevicefunction)

| | |
|---|---|
|Description|The configuration source of the WWNs for this connection (WWPN and WWNN).|
|Type|string|
|Read Only|False|

The following are the supported values:

|Value|Description|
|---|---|
|```ConfiguredLocally```|The set of FC/FCoE boot targets was applied locally through API or UI.|
|```ProvidedByFabric```|The set of FC/FCoE boot targets was applied by the Fibre Channel fabric.|

**FibreChannel.WWPN**
Member of [NetworkDeviceFunction.v1_1_0.NetworkDeviceFunction](#networkdevicefunction-v1_1_0-networkdevicefunction)

| | |
|---|---|
|Description|The effective current World-Wide Port Name (WWPN) of this network device function (physical function). If an assignable WWPN is not supported, this is a read only alias of the PermanentWWPN.|
|Type|string or null|
|Read Only|False|

### MaxVirtualFunctions
Member of [NetworkDeviceFunction.v1_1_0.NetworkDeviceFunction](#networkdevicefunction-v1_1_0-networkdevicefunction)

| | |
|---|---|
|Description|The number of virtual functions (VFs) availbale for this network device function.|
|Type|number or null|
|Read Only|True|

### NetDevFuncCapabilities (array)
Member of [NetworkDeviceFunction.v1_1_0.NetworkDeviceFunction](#networkdevicefunction-v1_1_0-networkdevicefunction)
```NetDevFuncCapabilities``` is an array containing elements of:


| | |
|---|---|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```Disabled```|Neither enumerated nor visible to the operating system.|
|```Ethernet```|Appears to the operating system as an Ethernet device.|
|```FibreChannel```|Appears to the operating system as a Fibre Channel device.|
|```iSCSI```|Appears to the operating system as an iSCSI device.|
|```FibreChannelOverEthernet```|Appears to the operating system as an FCoE device.|

### NetDevFuncType
Member of [NetworkDeviceFunction.v1_1_0.NetworkDeviceFunction](#networkdevicefunction-v1_1_0-networkdevicefunction)

| | |
|---|---|
|Description|The configured capability of this network device function.|
|Type|string|
|Read Only|False|

The following are the supported values:

|Value|Description|
|---|---|
|```Disabled```|Neither enumerated nor visible to the operating system.|
|```Ethernet```|Appears to the operating system as an Ethernet device.|
|```FibreChannel```|Appears to the operating system as a Fibre Channel device.|
|```iSCSI```|Appears to the operating system as an iSCSI device.|
|```FibreChannelOverEthernet```|Appears to the operating system as an FCoE device.|

### Oem.Hpe.ConnectionID
Member of [NetworkDeviceFunction.v1_1_0.NetworkDeviceFunction](#networkdevicefunction-v1_1_0-networkdevicefunction)

| | |
|---|---|
|Description|The Connection ID to be used with EVB, in IETF RFC-4122 UUID format.|
|Type|string|
|Read Only|False|

### Oem.Hpe.NetDevFuncCapabilities (array)
Member of [NetworkDeviceFunction.v1_1_0.NetworkDeviceFunction](#networkdevicefunction-v1_1_0-networkdevicefunction)
```NetDevFuncCapabilities``` is an array containing elements of:


| | |
|---|---|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```Disabled```|Neither enumerated nor visible to the operating system.|
|```Ethernet```|Appears to the operating system as an Ethernet device.|
|```FibreChannel```|Appears to the operating system as a Fibre Channel device.|
|```iSCSI```|Appears to the operating system as an iSCSI device.|
|```FCoE```|Appears to the operating system as an FCoE device.|
|```InfiniBand```|Appears to the operating system as an InfiniBand device.|
|```RoCE```|Appears to the operating system as an RDMA over converged Ethernet device.|
|```iWarp```|Appears to the operating system as an iWarp RDMA device.|
|```GenZ```|Appears to the operating systems as a Gen-Z device.|

### Oem.Hpe.NetDevFuncType
Member of [NetworkDeviceFunction.v1_1_0.NetworkDeviceFunction](#networkdevicefunction-v1_1_0-networkdevicefunction)

| | |
|---|---|
|Description|The presently configured interconnection capability of this network device function.|
|Type|string|
|Read Only|False|

The following are the supported values:

|Value|Description|
|---|---|
|```Disabled```|This function is disabled, and is neither enumerated nor visible to the operating system.|
|```Ethernet```|This function is configured to operate as an Ethernet device.|
|```FibreChannel```|This function is configured to operate as a Fibre Channel device.|
|```iSCSI```|This function is configured to operate as an iSCSI device.|
|```FCoE```|This function is configured to oeprate as an FCoE device.|
|```InfiniBand```||
|```RCoE```||
|```iWarp```|This function is configured to operate as an iWarp RDMA device.|
|```Gen-Z```|Appears to the operating systems as a Gen-Z device.|

### Oem.Hpe.SupportedFCBootTargetCount
Member of [NetworkDeviceFunction.v1_1_0.NetworkDeviceFunction](#networkdevicefunction-v1_1_0-networkdevicefunction)

| | |
|---|---|
|Description|The number of Fibre Channel boot targets supported by this network device function.|
|Type|integer|
|Read Only|True|

### Oem.Hpe.VirtualLinkStatus
Member of [NetworkDeviceFunction.v1_1_0.NetworkDeviceFunction](#networkdevicefunction-v1_1_0-networkdevicefunction)

| | |
|---|---|
|Description|Current status of the EVB Virtual Link (S-Channel) supporting this function.|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```NoChannel```|Port link is down, or the connected switch has not assigned an SVID.|
|```SwitchChannelDown```|SVID is assigned but Virtual Link status is down.|
|```HostDriverDown```|SVID is assigned and Virtual Link status is up, but the host OS driver is inactive.|
|```VirtualLinkUp```|SVID is assigned, Virual Link status is up, and the host OS driver is active.|

### Oem.Hpe.WakeOnLANEnabled
Member of [NetworkDeviceFunction.v1_1_0.NetworkDeviceFunction](#networkdevicefunction-v1_1_0-networkdevicefunction)

| | |
|---|---|
|Description|Enables Ethernet Wake On LAN (WoL) capability for this function when true.|
|Type|boolean|
|Read Only|False|

### PhysicalPortAssignment
A reference to the physical port currently assigned to this network device function.
### Settings
**Settings.href**
Member of [NetworkDeviceFunction.v1_1_0.NetworkDeviceFunction](#networkdevicefunction-v1_1_0-networkdevicefunction)

| | |
|---|---|
|Description|Reference to the resource the client may PUT/PATCH to in order to change this resource.|
|Type|string|
|Read Only|True|

### Status
Member of [NetworkDeviceFunction.v1_1_0.NetworkDeviceFunction](#networkdevicefunction-v1_1_0-networkdevicefunction)
See the Redfish standard schema and specification for information on common Status object.

### VirtualFunctionsEnabled
Member of [NetworkDeviceFunction.v1_1_0.NetworkDeviceFunction](#networkdevicefunction-v1_1_0-networkdevicefunction)

| | |
|---|---|
|Description|Indicates whether Single Root I/O Virtualization (SR-IOV) Virual Functions (VFs) are enabled for this network device function.|
|Type|boolean or null|
|Read Only|True|

### iSCSIBoot
**iSCSIBoot.AuthenticationMethod**
Member of [NetworkDeviceFunction.v1_1_0.NetworkDeviceFunction](#networkdevicefunction-v1_1_0-networkdevicefunction)

| | |
|---|---|
|Description|iSCSI Boot authentication method configuration values.|
|Type|string|
|Read Only|False|

The following are the supported values:

|Value|Description|
|---|---|
|```None```|No iSCSI authentication is used.|
|```CHAP```|iSCSI Challenge Handshake Authentication Protocol (CHAP) authentication is used.|
|```MutualCHAP```|iSCSI Mutual Challenge Handshake Authentication Protocol (CHAP) authentication is used.|

**iSCSIBoot.CHAPSecret**
Member of [NetworkDeviceFunction.v1_1_0.NetworkDeviceFunction](#networkdevicefunction-v1_1_0-networkdevicefunction)

| | |
|---|---|
|Description|The shared secret for CHAP authentication. Must be 0, 12, or 16 characters in length.|
|Type|string or null|
|Read Only|False|

**iSCSIBoot.CHAPUsername**
Member of [NetworkDeviceFunction.v1_1_0.NetworkDeviceFunction](#networkdevicefunction-v1_1_0-networkdevicefunction)

| | |
|---|---|
|Description|The username for CHAP authentication.|
|Type|string or null|
|Read Only|False|

**iSCSIBoot.IPAddressType**
Member of [NetworkDeviceFunction.v1_1_0.NetworkDeviceFunction](#networkdevicefunction-v1_1_0-networkdevicefunction)

| | |
|---|---|
|Description|The type of IP address (IPv6 or IPv4) being populated in the iSCSIBoot IP address fields.  Mixing of IPv6 and IPv4 addresses on the same network device function is not allowed.|
|Type|string|
|Read Only|False|

The following are the supported values:

|Value|Description|
|---|---|
|```IPv4```|IPv4 addressing is used for all IP-fields in this object.|
|```IPv6```|IPv6 addressing is used for all IP-fields in this object.|

**iSCSIBoot.IPMaskDNSViaDHCP**
Member of [NetworkDeviceFunction.v1_1_0.NetworkDeviceFunction](#networkdevicefunction-v1_1_0-networkdevicefunction)

| | |
|---|---|
|Description|When true, the iSCSI boot initiator will use DHCP to obtain the iniator name, IP address, and netmask.|
|Type|boolean or null|
|Read Only|False|

**iSCSIBoot.InitiatorDefaultGateway**
Member of [NetworkDeviceFunction.v1_1_0.NetworkDeviceFunction](#networkdevicefunction-v1_1_0-networkdevicefunction)

| | |
|---|---|
|Description|The IPv6 or IPv4 iSCSI boot default gateway.|
|Type|string or null|
|Read Only|False|

**iSCSIBoot.InitiatorIPAddress**
Member of [NetworkDeviceFunction.v1_1_0.NetworkDeviceFunction](#networkdevicefunction-v1_1_0-networkdevicefunction)

| | |
|---|---|
|Description|The IPv6 or IPv4 address of the iSCSI boot initiator.|
|Type|string or null|
|Read Only|False|

**iSCSIBoot.InitiatorName**
Member of [NetworkDeviceFunction.v1_1_0.NetworkDeviceFunction](#networkdevicefunction-v1_1_0-networkdevicefunction)

| | |
|---|---|
|Description|The iSCSI initiator name.|
|Type|string or null|
|Read Only|False|

**iSCSIBoot.InitiatorNetmask**
Member of [NetworkDeviceFunction.v1_1_0.NetworkDeviceFunction](#networkdevicefunction-v1_1_0-networkdevicefunction)

| | |
|---|---|
|Description|The IPv6 or IPv4 netmask of the iSCSI boot initiator.|
|Type|string or null|
|Read Only|False|

**iSCSIBoot.MutualCHAPSecret**
Member of [NetworkDeviceFunction.v1_1_0.NetworkDeviceFunction](#networkdevicefunction-v1_1_0-networkdevicefunction)

| | |
|---|---|
|Description|The CHAP secret for 2-way CHAP authentication. Must be 0, 12, or 16 characters in length.|
|Type|string or null|
|Read Only|False|

**iSCSIBoot.MutualCHAPUsername**
Member of [NetworkDeviceFunction.v1_1_0.NetworkDeviceFunction](#networkdevicefunction-v1_1_0-networkdevicefunction)

| | |
|---|---|
|Description|The CHAP username for 2-way CHAP authentication.|
|Type|string or null|
|Read Only|False|

**iSCSIBoot.PrimaryDNS**
Member of [NetworkDeviceFunction.v1_1_0.NetworkDeviceFunction](#networkdevicefunction-v1_1_0-networkdevicefunction)

| | |
|---|---|
|Description|The IPv6 or IPv4 address of the primary DNS server for the iSCSI boot initiator.|
|Type|string or null|
|Read Only|False|

**iSCSIBoot.PrimaryLUN**
Member of [NetworkDeviceFunction.v1_1_0.NetworkDeviceFunction](#networkdevicefunction-v1_1_0-networkdevicefunction)

| | |
|---|---|
|Description|The logical unit number (LUN) for the primary iSCSI boot target.|
|Type|number or null|
|Read Only|False|

**iSCSIBoot.PrimaryTargetIPAddress**
Member of [NetworkDeviceFunction.v1_1_0.NetworkDeviceFunction](#networkdevicefunction-v1_1_0-networkdevicefunction)

| | |
|---|---|
|Description|The IP address (IPv6 or IPv4) for the primary iSCSI boot target.|
|Type|string or null|
|Read Only|False|

**iSCSIBoot.PrimaryTargetName**
Member of [NetworkDeviceFunction.v1_1_0.NetworkDeviceFunction](#networkdevicefunction-v1_1_0-networkdevicefunction)

| | |
|---|---|
|Description|The name of the primary iSCSI boot target, iSCSI Qualified Name (IQN).|
|Type|string or null|
|Read Only|False|

**iSCSIBoot.PrimaryTargetTCPPort**
Member of [NetworkDeviceFunction.v1_1_0.NetworkDeviceFunction](#networkdevicefunction-v1_1_0-networkdevicefunction)

| | |
|---|---|
|Description|The TCP port for the primary iSCSI boot target.|
|Type|number or null|
|Read Only|False|

**iSCSIBoot.PrimaryVLANEnable**
Member of [NetworkDeviceFunction.v1_1_0.NetworkDeviceFunction](#networkdevicefunction-v1_1_0-networkdevicefunction)

| | |
|---|---|
|Description|This indicates if the primary VLAN is enabled.  Not supported by HPE.|
|Type|boolean or null|
|Read Only|False|

**iSCSIBoot.PrimaryVLANId**
Member of [NetworkDeviceFunction.v1_1_0.NetworkDeviceFunction](#networkdevicefunction-v1_1_0-networkdevicefunction)

| | |
|---|---|
|Description|The 802.1q VLAN ID to use for iSCSI boot for both the primary and secondary targets.  Assign null value to disable.|
|Type|number or null|
|Read Only|False|

**iSCSIBoot.RouterAdvertisementEnabled**
Member of [NetworkDeviceFunction.v1_1_0.NetworkDeviceFunction](#networkdevicefunction-v1_1_0-networkdevicefunction)

| | |
|---|---|
|Description|A boolean indicating whether IPv6 router advertisement is enabled for the iSCSI boot target.  This setting shall only apply to IPv6 configurations.|
|Type|boolean or null|
|Read Only|False|

**iSCSIBoot.SecondaryDNS**
Member of [NetworkDeviceFunction.v1_1_0.NetworkDeviceFunction](#networkdevicefunction-v1_1_0-networkdevicefunction)

| | |
|---|---|
|Description|The value of this property shall be the IPv6 or IPv4 address of the secondary DNS server for the iSCSI boot initiator.|
|Type|string or null|
|Read Only|False|

**iSCSIBoot.SecondaryLUN**
Member of [NetworkDeviceFunction.v1_1_0.NetworkDeviceFunction](#networkdevicefunction-v1_1_0-networkdevicefunction)

| | |
|---|---|
|Description|The logical unit number (LUN) for the secondary iSCSI boot target.  Not supported by HPE.|
|Type|number or null|
|Read Only|False|

**iSCSIBoot.SecondaryTargetIPAddress**
Member of [NetworkDeviceFunction.v1_1_0.NetworkDeviceFunction](#networkdevicefunction-v1_1_0-networkdevicefunction)

| | |
|---|---|
|Description|The IP address (IPv6 or IPv4) for the secondary iSCSI boot target.|
|Type|string or null|
|Read Only|False|

**iSCSIBoot.SecondaryTargetName**
Member of [NetworkDeviceFunction.v1_1_0.NetworkDeviceFunction](#networkdevicefunction-v1_1_0-networkdevicefunction)

| | |
|---|---|
|Description|The name of the iSCSI secondary boot target, iSCSI Qualified Name (IQN).  Not supported by HPE. The value from PrimaryTargetName will be used for the secondary iSCSI boot target if configured.|
|Type|string or null|
|Read Only|False|

**iSCSIBoot.SecondaryTargetTCPPort**
Member of [NetworkDeviceFunction.v1_1_0.NetworkDeviceFunction](#networkdevicefunction-v1_1_0-networkdevicefunction)

| | |
|---|---|
|Description|The TCP port for the secondary iSCSI boot target.|
|Type|number or null|
|Read Only|False|

**iSCSIBoot.SecondaryVLANEnable**
Member of [NetworkDeviceFunction.v1_1_0.NetworkDeviceFunction](#networkdevicefunction-v1_1_0-networkdevicefunction)

| | |
|---|---|
|Description|This indicates if the secondary VLAN is enabled.  Not supported by HPE.|
|Type|boolean or null|
|Read Only|False|

**iSCSIBoot.SecondaryVLANId**
Member of [NetworkDeviceFunction.v1_1_0.NetworkDeviceFunction](#networkdevicefunction-v1_1_0-networkdevicefunction)

| | |
|---|---|
|Description|The 802.1q VLAN ID to use for iSCSI boot from the secondary target.  Not supported by HPE.|
|Type|number or null|
|Read Only|False|

**iSCSIBoot.TargetInfoViaDHCP**
Member of [NetworkDeviceFunction.v1_1_0.NetworkDeviceFunction](#networkdevicefunction-v1_1_0-networkdevicefunction)

| | |
|---|---|
|Description|When true indicates the iSCSI boot target name, LUN, IP address, and netmask should be obtained from DHCP.|
|Type|boolean or null|
|Read Only|False|

## NetworkInterface.v1_1_0.NetworkInterface
```@odata.type: "#NetworkInterface.v1_1_0.NetworkInterface"```

A NetworkInterface contains references linking NetworkAdapter, NetworkPort, and NetworkDeviceFunction resources and represents the functionality available to the containing system.
### Resource Instances
|Uri|HTTP Allow|
|---|---|
|```/redfish/v1/systems/{item}/networkinterfaces/{item}/```|GET |

### NetworkDeviceFunctions
link to collection of membertype NetworkDeviceFunction. The collection of device functions avaliable on this network interface.
### NetworkPorts
Link to a collection of membertype NetworkPort. The collection of ports avaliable on this network interface.
### Status
Member of [NetworkInterface.v1_1_0.NetworkInterface](#networkinterface-v1_1_0-networkinterface)
See the Redfish standard schema and specification for information on common Status object.

## NetworkPort.v1_1_0.NetworkPort
```@odata.type: "#NetworkPort.v1_1_0.NetworkPort"```

A Network Port represents a discrete physical port capable of connecting to a network.
### Resource Instances
|Uri|HTTP Allow|
|---|---|
|```/redfish/v1/chassis/{item}/networkadapters/{item}/networkports/{item}/```|GET |
|```/redfish/v1/chassis/{item}/networkadapters/{item}/networkports/{item}/settings/```|GET POST PATCH |
|```/redfish/v1/systems/{item}/networkinterfaces/{item}/networkports/{item}/```|GET |
|```/redfish/v1/systems/{item}/networkinterfaces/{item}/networkports/{item}/settings/```|GET POST PATCH |

### Links to other Resources
|Link Name|Destination type
|---|---|
|```@Redfish.Settings/SettingsObject```|[NetworkPort](#networkport-v1_1_0-networkport)|

### ActiveLinkTechnology
Member of [NetworkPort.v1_1_0.NetworkPort](#networkport-v1_1_0-networkport)

| | |
|---|---|
|Description|Physical link technology values.|
|Type|string|
|Read Only|False|

The following are the supported values:

|Value|Description|
|---|---|
|```Ethernet```|The port is capable of connecting to an Ethernet network.|
|```InfiniBand```|The port is capable of connecting to an InfiniBand network.|
|```FibreChannel```|The port is capable of connecting to a Fibre Channel network.|

### AssociatedNetworkAddresses (array)
Member of [NetworkPort.v1_1_0.NetworkPort](#networkport-v1_1_0-networkport)
```AssociatedNetworkAddresses``` is an array containing elements of:


| | |
|---|---|
|Type|string or null|
|Read Only|True|

### EEEEnabled
Member of [NetworkPort.v1_1_0.NetworkPort](#networkport-v1_1_0-networkport)

| | |
|---|---|
|Description|Indicates whether IEEE 802.3az Energy Efficient Ethernet (EEE) is enabled for this network port.|
|Type|boolean or null|
|Read Only|False|

### FlowControlConfiguration
Member of [NetworkPort.v1_1_0.NetworkPort](#networkport-v1_1_0-networkport)

| | |
|---|---|
|Description|Ethernet flow control configuration values.|
|Type|string|
|Read Only|False|

The following are the supported values:

|Value|Description|
|---|---|
|```None```|No IEEE 802.3x flow control is enabled on this port.|
|```TX```|IEEE 802.3x flow control may be initiated by this station.|
|```RX```|IEEE 802.3x flow control may be initiated by the link partner.|
|```TX_RX```|IEEE 802.3x flow control may be initiated by this station or the link partner.|

### FlowControlStatus
Member of [NetworkPort.v1_1_0.NetworkPort](#networkport-v1_1_0-networkport)

| | |
|---|---|
|Description|Ethernet flow control configuration values.|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```None```|No IEEE 802.3x flow control is enabled on this port.|
|```TX```|IEEE 802.3x flow control may be initiated by this station.|
|```RX```|IEEE 802.3x flow control may be initiated by the link partner.|
|```TX_RX```|IEEE 802.3x flow control may be initiated by this station or the link partner.|

### LinkStatus
Member of [NetworkPort.v1_1_0.NetworkPort](#networkport-v1_1_0-networkport)

| | |
|---|---|
|Description|Physical link status values.|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```Down```|The port is enabled but link is down.|
|```Up```|The port is enabled and link is good (up).|

### NetDevFuncMaxBWAlloc (array)
Member of [NetworkPort.v1_1_0.NetworkPort](#networkport-v1_1_0-networkport)
```NetDevFuncMaxBWAlloc``` is an array containing elements of:

**NetDevFuncMaxBWAlloc[{item}].MaxBWAllocPercent**
Member of [NetworkPort.v1_1_0.NetworkPort](#networkport-v1_1_0-networkport)

| | |
|---|---|
|Description|The maximum bandwidth allocation percentage allocated to the associated network device function.|
|Type|number or null|
|Read Only|False|

**NetDevFuncMaxBWAlloc[{item}].NetworkDeviceFunction**
A reference to the associated network device function that this maximum bandwidth percentage allocation applies to.
### NetDevFuncMinBWAlloc (array)
Member of [NetworkPort.v1_1_0.NetworkPort](#networkport-v1_1_0-networkport)
```NetDevFuncMinBWAlloc``` is an array containing elements of:

**NetDevFuncMinBWAlloc[{item}].MinBWAllocPercent**
Member of [NetworkPort.v1_1_0.NetworkPort](#networkport-v1_1_0-networkport)

| | |
|---|---|
|Description|The minimum bandwidth allocation percentage allocated to the associated network device function instance. The sum total of all minimum percentages shall not exceed 100.|
|Type|number or null|
|Read Only|False|

**NetDevFuncMinBWAlloc[{item}].NetworkDeviceFunction**
A reference to the associated network device function that this minimum bandwidth percentage allocation applies to.
### Oem.Hpe.AutoNegotiationCapable
Member of [NetworkPort.v1_1_0.NetworkPort](#networkport-v1_1_0-networkport)

| | |
|---|---|
|Description|Indicates the ability of this network port to autonegotiate link speed.|
|Type|boolean|
|Read Only|True|

### Oem.Hpe.Evb
Edge Virtual Bridging (EVB) information for this port.
### Oem.Hpe.Lldp
Link-Layer Discovery Protocol (LLDP) information for this port.
### Oem.Hpe.PortDiagnosticEnableLocalLoopback
Member of [NetworkPort.v1_1_0.NetworkPort](#networkport-v1_1_0-networkport)

| | |
|---|---|
|Description|When true, local loopback is active on this port.  PortDiagnosticsEnabled must first be true in order to set this property to true.|
|Type|boolean|
|Read Only|False|

### Oem.Hpe.PortDiagnosticEnableRemoteLoopback
Member of [NetworkPort.v1_1_0.NetworkPort](#networkport-v1_1_0-networkport)

| | |
|---|---|
|Description|When true, remote loopback is active on this port. PortDiagnosticsEnabled must first be true in order to set this property to true.|
|Type|boolean|
|Read Only|False|

### Oem.Hpe.PortDiagnosticLocalLoopbackCapable
Member of [NetworkPort.v1_1_0.NetworkPort](#networkport-v1_1_0-networkport)

| | |
|---|---|
|Description|When true, the port has local loopback capability.|
|Type|boolean|
|Read Only|True|

### Oem.Hpe.PortDiagnosticRemoteLoopbackCapable
Member of [NetworkPort.v1_1_0.NetworkPort](#networkport-v1_1_0-networkport)

| | |
|---|---|
|Description|When true, the port has remote loopback capability.|
|Type|boolean|
|Read Only|True|

### Oem.Hpe.PortDiagnosticsEnabled
Member of [NetworkPort.v1_1_0.NetworkPort](#networkport-v1_1_0-networkport)

| | |
|---|---|
|Description|When true, diagnostic features are enabled on this port.|
|Type|boolean|
|Read Only|False|

### Oem.Hpe.VirtualFunctionAllocations (array)
Member of [NetworkPort.v1_1_0.NetworkPort](#networkport-v1_1_0-networkport)
```VirtualFunctionAllocations``` is an array containing elements of:

**VirtualFunctionAllocations[{item}].NetworkDeviceFunction**
The logical network device function to which this virtual function allocation applies.
**VirtualFunctionAllocations[{item}].VirtualFunctionsAllocated**
Member of [NetworkPort.v1_1_0.NetworkPort](#networkport-v1_1_0-networkport)

| | |
|---|---|
|Description|The number of virtual functions allocated to this logical network device function instance.|
|Type|number or null|
|Read Only|False|

### PhysicalPortNumber
Member of [NetworkPort.v1_1_0.NetworkPort](#networkport-v1_1_0-networkport)

| | |
|---|---|
|Description|The physical port number on the network adapter hardware that this Network Port corresponds to.  This value should match a value visible on the hardware.  When HostPortEnabled and ManagementPortEnabled are both "false", the port shall not establish physical link.|
|Type|string or null|
|Read Only|True|

### PortMaximumMTU
Member of [NetworkPort.v1_1_0.NetworkPort](#networkport-v1_1_0-networkport)

| | |
|---|---|
|Description|The largest maximum transmission unit (MTU) that can be configured for this network port.|
|Type|number or null|
|Read Only|True|

### Settings
**Settings.href**
Member of [NetworkPort.v1_1_0.NetworkPort](#networkport-v1_1_0-networkport)

| | |
|---|---|
|Description|Reference to the resource the client may PUT/PATCH to in order to change this resource.|
|Type|string|
|Read Only|True|

### SignalDetected
Member of [NetworkPort.v1_1_0.NetworkPort](#networkport-v1_1_0-networkport)

| | |
|---|---|
|Type|boolean or null|
|Read Only|True|

### Status
Member of [NetworkPort.v1_1_0.NetworkPort](#networkport-v1_1_0-networkport)
See the Redfish standard schema and specification for information on common Status object.

### SupportedEthernetCapabilities (array)
Member of [NetworkPort.v1_1_0.NetworkPort](#networkport-v1_1_0-networkport)
```SupportedEthernetCapabilities``` is an array containing elements of:


| | |
|---|---|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```WakeOnLAN```|Wake on LAN (WoL) is supported on this port.|
|```EEE```|IEEE 802.3az Energy Efficient Ethernet (EEE) is supported on this port.|

### SupportedLinkCapabilities (array)
Member of [NetworkPort.v1_1_0.NetworkPort](#networkport-v1_1_0-networkport)
```SupportedLinkCapabilities``` is an array containing elements of:

**SupportedLinkCapabilities[{item}].LinkNetworkTechnology**
Member of [NetworkPort.v1_1_0.NetworkPort](#networkport-v1_1_0-networkport)

| | |
|---|---|
|Description|Physical link technology values.|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```Ethernet```|The port is capable of connecting to an Ethernet network.|
|```InfiniBand```|The port is capable of connecting to an InfiniBand network.|
|```FibreChannel```|The port is capable of connecting to a Fibre Channel network.|

**SupportedLinkCapabilities[{item}].LinkSpeedMbps**
Member of [NetworkPort.v1_1_0.NetworkPort](#networkport-v1_1_0-networkport)

| | |
|---|---|
|Description|The speed of the link in Mbps when this link network technology is active.|
|Type|number or null|
|Read Only|True|

### WakeOnLANEnabled
Member of [NetworkPort.v1_1_0.NetworkPort](#networkport-v1_1_0-networkport)

| | |
|---|---|
|Description|Indicates whether Wake on LAN (WoL) is enabled for this network port.|
|Type|boolean or null|
|Read Only|False|

### Actions

**NetworkPort.DiagnosticsReset**
Member of [NetworkPort.v1_1_0.NetworkPort](#networkport-v1_1_0-networkport)
There are no parameters for this action.
## Power.v1_2_1.Power
```@odata.type: "#Power.v1_2_1.Power"```

This is the schema definition for the Power Metrics.  It represents the properties for Power Consumption and Power Limiting.
### Resource Instances
|Uri|HTTP Allow|
|---|---|
|```/redfish/v1/chassis/{item}/power/```|GET PATCH |

### Links to other Resources
|Link Name|Destination type
|---|---|
|```Oem/Hpe/Links/FederatedGroupCapping```|[HpeiLOFederatedGroupCapping](#hpeilofederatedgroupcapping-v2_0_0-hpeilofederatedgroupcapping)|
|```Oem/Hpe/Links/PowerMeter```|[HpePowerMeter](#hpepowermeter-v2_0_0-hpepowermeter)|
|```Redundancy[]/RedundancySet[]```|[Power](#power-v1_2_1-power)|
|```Oem/Hpe/Links/FastPowerMeter```|[HpePowerMeter](#hpepowermeter-v2_0_0-hpepowermeter)|

### Oem.Hpe.BatteryBackedUnits (array)
Member of [Power.v1_2_1.Power](#power-v1_2_1-power)
```BatteryBackedUnits``` is an array containing elements of:

**BatteryBackedUnits[{item}].BBUStatus**
**BatteryBackedUnits[{item}].BBUStatus.Health**
Member of [Power.v1_2_1.Power](#power-v1_2_1-power)

| | |
|---|---|
|Description|This represents the health state of this resource in the absence of its dependent resources.|
|Type|string or null|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```Null```|A value is temporarily unavailable|
|```OK```|Normal|
|```Warning```|A condition exists that requires attention|
|```Critical```|A critical condition exists that requires immediate attention|

**BatteryBackedUnits[{item}].BBUStatus.HealthRollup**
Member of [Power.v1_2_1.Power](#power-v1_2_1-power)

| | |
|---|---|
|Description|This represents the overall health state from the view of this resource.|
|Type|string or null|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```Null```|A value is temporarily unavailable|
|```OK```|Normal|
|```Warning```|A condition exists that requires attention|
|```Critical```|A critical condition exists that requires immediate attention|

**BatteryBackedUnits[{item}].BBUStatus.State**
Member of [Power.v1_2_1.Power](#power-v1_2_1-power)

| | |
|---|---|
|Description|This indicates the known state of the resource, such as if it is enabled.|
|Type|string or null|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```Null```|A value is temporarily unavailable|
|```Enabled```|This function or resource has been enabled|
|```Disabled```|This function or resource has been disabled|
|```Offline```|This function or resource is enabled, but currently unavailable|
|```InTest```|This function or resource is underdoing testing|
|```Starting```|This function or resource is starting|
|```Absent```|This function or resource is not installed|

**BatteryBackedUnits[{item}].BayNumber**
Member of [Power.v1_2_1.Power](#power-v1_2_1-power)

| | |
|---|---|
|Description|Bay number of the battery backed unit.|
|Type|integer|
|Read Only|True|

**BatteryBackedUnits[{item}].CapacityWatts**
Member of [Power.v1_2_1.Power](#power-v1_2_1-power)

| | |
|---|---|
|Description|Total capacity (in Watts) of the battery backed unit.|
|Type|integer|
|Read Only|True|

**BatteryBackedUnits[{item}].CutOffSetPointmAh**
Member of [Power.v1_2_1.Power](#power-v1_2_1-power)

| | |
|---|---|
|Description|Cut off threshold (mAh) where battery backed unit stops supplying power to the server.|
|Type|integer|
|Read Only|True|

**BatteryBackedUnits[{item}].FirmwareVersion**
Member of [Power.v1_2_1.Power](#power-v1_2_1-power)

| | |
|---|---|
|Description|Firmware version of the battery backed unit.|
|Type|string|
|Read Only|True|

**BatteryBackedUnits[{item}].PercentCharge**
Member of [Power.v1_2_1.Power](#power-v1_2_1-power)

| | |
|---|---|
|Description|Percentage charge remaining for the battery backed unit.|
|Type|integer|
|Read Only|True|

**BatteryBackedUnits[{item}].RemainingCapacitymAh**
Member of [Power.v1_2_1.Power](#power-v1_2_1-power)

| | |
|---|---|
|Description|Remaining capacity (mAh) of the battery backed unit.|
|Type|integer|
|Read Only|True|

**BatteryBackedUnits[{item}].SerialNumber**
Member of [Power.v1_2_1.Power](#power-v1_2_1-power)

| | |
|---|---|
|Description|Serial number of the battery backed unit.|
|Type|string|
|Read Only|True|

**BatteryBackedUnits[{item}].TimeToCutOffSeconds**
Member of [Power.v1_2_1.Power](#power-v1_2_1-power)

| | |
|---|---|
|Description|Run time (in seconds) available with the battery backed unit until cut off. This is detected only when battery is charging or discharging, otherwise set to 0.|
|Type|integer|
|Read Only|True|

**BatteryBackedUnits[{item}].TimeToFullChargeMinutes**
Member of [Power.v1_2_1.Power](#power-v1_2_1-power)

| | |
|---|---|
|Description|Time required (in minutes) to fully charge the battery backed unit. This is detected only when battery is charging or discharging, otherwise set to 0.|
|Type|integer|
|Read Only|True|

**BatteryBackedUnits[{item}].UsableCapacitymAh**
Member of [Power.v1_2_1.Power](#power-v1_2_1-power)

| | |
|---|---|
|Description| Usable capacity (mAh) of the battery backed unit.|
|Type|integer|
|Read Only|True|

### Oem.Hpe.BbuPowerSupply
Member of [Power.v1_2_1.Power](#power-v1_2_1-power)

| | |
|---|---|
|Description|Battery Backup Unit Power Supply action determines what will occur when a server is running on battery power.|
|Type|string|
|Read Only|False|

The following are the supported values:

|Value|Description|
|---|---|
|```DoNothing```|No action will be taken when a server switches to battery power.|
|```MomentaryPowerButtonPress```|Momentary virtual power button press which should shutdown host operating system when pressed.|
|```HostShutdown```|Shutdown message sent to host operating system with installed management software to initiate a shutdown.|

### Oem.Hpe.BrownoutRecoveryEnabled
Member of [Power.v1_2_1.Power](#power-v1_2_1-power)

| | |
|---|---|
|Description|When a brownout condition occurs in the server, this setting will determine if the server should recover from it.|
|Type|boolean or null|
|Read Only|False|

### Oem.Hpe.HasPowerMetering
Member of [Power.v1_2_1.Power](#power-v1_2_1-power)

| | |
|---|---|
|Description|Indicates if the system has power metering.|
|Type|boolean|
|Read Only|True|

### Oem.Hpe.HighEfficiencyMode
Member of [Power.v1_2_1.Power](#power-v1_2_1-power)

| | |
|---|---|
|Description|The redundant power supply mode that will be used when redundant power supplies are configured.|
|Type|string or null|
|Read Only|True|

The following are the supported values:

|Value|
|---|
|```Null```|
|```Auto```|
|```Balanced```|
|```Even```|
|```Odd```|

### Oem.Hpe.MinimumSafelyAchievableCap
Member of [Power.v1_2_1.Power](#power-v1_2_1-power)

| | |
|---|---|
|Description|Minimum Safely Achievable Cap is the lowest cap value that is safe for a group power manager to apply to a particular server. It can either be identical to or slightly greater than the 0 percent cap value calculated during ROM power burn.|
|Type|integer or null|
|Read Only|True|

### Oem.Hpe.MinimumSafelyAchievableCapValid
Member of [Power.v1_2_1.Power](#power-v1_2_1-power)

| | |
|---|---|
|Description|Indicates if the msac is valid.  msac is valid only if this is true.|
|Type|boolean|
|Read Only|True|

### Oem.Hpe.SNMPPowerThresholdAlert
**Oem.Hpe.SNMPPowerThresholdAlert.DurationInMin**
Member of [Power.v1_2_1.Power](#power-v1_2_1-power)

| | |
|---|---|
|Description|Sets the length of time, in minutes, that power consumption must remain above the warning threshold before an SNMP alert is triggered. The maximum duration is 240 minutes, and the duration must be a multiple of 5.|
|Type|integer|
|Read Only|False|

**Oem.Hpe.SNMPPowerThresholdAlert.ThresholdWatts**
Member of [Power.v1_2_1.Power](#power-v1_2_1-power)

| | |
|---|---|
|Description|Sets the power consumption threshold (watts). If power consumption exceeds this value for the specified time duration, an SNMP alert is triggered.|
|Type|integer|
|Read Only|False|

**Oem.Hpe.SNMPPowerThresholdAlert.Trigger**
Member of [Power.v1_2_1.Power](#power-v1_2_1-power)

| | |
|---|---|
|Description|Trigger determines whether alerts are based on peak power consumption, average power consumption, or if they are disabled. Trigger property can only be enabled if the ThresholdWatts and DurationInMin values are specified/configured.|
|Type|string|
|Read Only|False|

The following are the supported values:

|Value|
|---|
|```Disabled```|
|```AveragePowerConsumption```|
|```PeakPowerConsumption```|

### PowerControl (array)
Member of [Power.v1_2_1.Power](#power-v1_2_1-power)
```PowerControl``` is an array containing elements of:

**PowerControl[{item}].MemberId**
Member of [Power.v1_2_1.Power](#power-v1_2_1-power)

| | |
|---|---|
|Description|This is the identifier for the member within the collection.|
|Type|string|
|Read Only|True|

**PowerControl[{item}].PowerAllocatedWatts**
Member of [Power.v1_2_1.Power](#power-v1_2_1-power)

| | |
|---|---|
|Description|The total amount of power that has been allocated (or budegeted)to  chassis resources.|
|Type|number or null|
|Read Only|True|

**PowerControl[{item}].PowerAvailableWatts**
Member of [Power.v1_2_1.Power](#power-v1_2_1-power)

| | |
|---|---|
|Description|The amount of power not already budgeted and therefore available for additional allocation. (powerCapacity - powerAllocated).  This indicates how much reserve power capacity is left.|
|Type|number or null|
|Read Only|True|

**PowerControl[{item}].PowerCapacityWatts**
Member of [Power.v1_2_1.Power](#power-v1_2_1-power)

| | |
|---|---|
|Description|The total amount of power available to the chassis for allocation. This may the power supply capacity, or power budget assigned to the chassis from an up-stream chassis.|
|Type|number or null|
|Read Only|True|

**PowerControl[{item}].PowerConsumedWatts**
Member of [Power.v1_2_1.Power](#power-v1_2_1-power)

| | |
|---|---|
|Description|The actual power being consumed by the chassis.|
|Type|number or null|
|Read Only|True|

**PowerControl[{item}].PowerLimit**
**PowerControl[{item}].PowerLimit.CorrectionInMs**
Member of [Power.v1_2_1.Power](#power-v1_2_1-power)

| | |
|---|---|
|Description|The time required for the limiting process to reduce power consumption to below the limit.|
|Type|integer or null|
|Read Only|True|

**PowerControl[{item}].PowerLimit.LimitException**
Member of [Power.v1_2_1.Power](#power-v1_2_1-power)

| | |
|---|---|
|Description|The action that is taken if the power cannot be maintained below the LimitInWatts.|
|Type|string|
|Read Only|False|

The following are the supported values:

|Value|Description|
|---|---|
|```NoAction```|Take no action when the limit is exceeded.|
|```HardPowerOff```|Turn the power off immediately when the limit is exceeded.|
|```LogEventOnly```|Log an event when the limit is exceeded, but take no further action.|
|```Oem```|Take an OEM-defined action.|

**PowerControl[{item}].PowerLimit.LimitInWatts**
Member of [Power.v1_2_1.Power](#power-v1_2_1-power)

| | |
|---|---|
|Description|The Power limit in watts. Set to null to disable power capping.|
|Type|number or null|
|Read Only|False|

**PowerControl[{item}].PowerMetrics**
**PowerControl[{item}].PowerMetrics.AverageConsumedWatts**
Member of [Power.v1_2_1.Power](#power-v1_2_1-power)

| | |
|---|---|
|Description|The average power level over the measurement window (the last IntervalInMin minutes).|
|Type|number or null|
|Read Only|True|

**PowerControl[{item}].PowerMetrics.IntervalInMin**
Member of [Power.v1_2_1.Power](#power-v1_2_1-power)

| | |
|---|---|
|Description|The time interval (or window) in which the PowerMetrics are measured over.|
|Type|integer or null|
|Read Only|True|

**PowerControl[{item}].PowerMetrics.MaxConsumedWatts**
Member of [Power.v1_2_1.Power](#power-v1_2_1-power)

| | |
|---|---|
|Description|The highest power consumption level that has occured over the measurement window (the last IntervalInMin minutes).|
|Type|number or null|
|Read Only|True|

**PowerControl[{item}].PowerMetrics.MinConsumedWatts**
Member of [Power.v1_2_1.Power](#power-v1_2_1-power)

| | |
|---|---|
|Description|The lowest power consumption level over the measurement window (the last IntervalInMin minutes).|
|Type|number or null|
|Read Only|True|

**PowerControl[{item}].PowerRequestedWatts**
Member of [Power.v1_2_1.Power](#power-v1_2_1-power)

| | |
|---|---|
|Description|The potential power that the chassis resources are requesting which may be higher than the current level being consumed since requested power includes budget that the chassis resource wants for future use.|
|Type|number or null|
|Read Only|True|

**PowerControl[{item}].RelatedItem (array)**
Member of [Power.v1_2_1.Power](#power-v1_2_1-power)
```RelatedItem``` is an array containing elements of:

**PowerControl[{item}].Status**
Member of [Power.v1_2_1.Power](#power-v1_2_1-power)
See the Redfish standard schema and specification for information on common Status object.

### PowerSupplies (array)
Member of [Power.v1_2_1.Power](#power-v1_2_1-power)
```PowerSupplies``` is an array containing elements of:

**PowerSupplies[{item}].FirmwareVersion**
Member of [Power.v1_2_1.Power](#power-v1_2_1-power)

| | |
|---|---|
|Description|The firmware version for this Power Supply|
|Type|string or null|
|Read Only|True|

**PowerSupplies[{item}].LastPowerOutputWatts**
Member of [Power.v1_2_1.Power](#power-v1_2_1-power)

| | |
|---|---|
|Description|The average power output of this Power Supply|
|Type|number or null|
|Read Only|True|

**PowerSupplies[{item}].LineInputVoltage**
Member of [Power.v1_2_1.Power](#power-v1_2_1-power)

| | |
|---|---|
|Description|The line input voltage at which the Power Supply is operating|
|Type|number or null|
|Read Only|True|

**PowerSupplies[{item}].LineInputVoltageType**
Member of [Power.v1_2_1.Power](#power-v1_2_1-power)

| | |
|---|---|
|Description|The line voltage type supported as an input to this Power Supply|
|Type|string or null|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```Null```|A value is temporarily unavailable|
|```Unknown```|The power supply line input voltage type cannot be determined.|
|```ACLowLine```|100-127V AC input.|
|```ACMidLine```|200-240V AC input.|
|```ACHighLine```|277V AC input.|
|```DCNeg48V```|-48V DC input.|
|```HighVoltageDC```|High Voltage DC input (380V).|

**PowerSupplies[{item}].MemberId**
Member of [Power.v1_2_1.Power](#power-v1_2_1-power)

| | |
|---|---|
|Description|This is the identifier for the member within the collection.|
|Type|string|
|Read Only|True|

**PowerSupplies[{item}].Model**
Member of [Power.v1_2_1.Power](#power-v1_2_1-power)

| | |
|---|---|
|Description|The model number for this Power Supply|
|Type|string or null|
|Read Only|True|

**PowerSupplies[{item}].Oem.Hpe.AveragePowerOutputWatts**
Member of [Power.v1_2_1.Power](#power-v1_2_1-power)

| | |
|---|---|
|Description|The latest observed average power being drawn by the power supply (Watts). This is usually updated every 10 seconds but the period can vary in some circumstances.|
|Type|integer|
|Read Only|True|

**PowerSupplies[{item}].Oem.Hpe.BayNumber**
Member of [Power.v1_2_1.Power](#power-v1_2_1-power)

| | |
|---|---|
|Description|The power supply bay number.|
|Type|integer|
|Read Only|True|

**PowerSupplies[{item}].Oem.Hpe.HotplugCapable**
Member of [Power.v1_2_1.Power](#power-v1_2_1-power)

| | |
|---|---|
|Description|If true, this power supply (and power supply bay) is capable of being hot-plugged.|
|Type|boolean|
|Read Only|True|

**PowerSupplies[{item}].Oem.Hpe.MaxPowerOutputWatts**
Member of [Power.v1_2_1.Power](#power-v1_2_1-power)

| | |
|---|---|
|Description|The latest observed maximum output power being drawn by the power supply (Watts). This is usually updated every 10 seconds but the period can vary in some circumstances.|
|Type|integer|
|Read Only|True|

**PowerSupplies[{item}].Oem.Hpe.Mismatched**
Member of [Power.v1_2_1.Power](#power-v1_2_1-power)

| | |
|---|---|
|Description|If true, this power supply is mismatched with others in the system.|
|Type|boolean|
|Read Only|True|

**PowerSupplies[{item}].Oem.Hpe.PowerSupplyStatus**
**PowerSupplies[{item}].Oem.Hpe.PowerSupplyStatus.State**
Member of [Power.v1_2_1.Power](#power-v1_2_1-power)

| | |
|---|---|
|Description|Indicates the known state of the resource.|
|Type|string or null|
|Read Only|True|

The following are the supported values:

|Value|
|---|
|```Unknown```|
|```Ok```|
|```Degraded```|
|```Failed```|
|```OverVoltage```|
|```OverCurrent```|
|```OverTemperature```|
|```ACPowerLost```|
|```FanFailure```|
|```WarningHighInputVoltage```|
|```WarningLowInputVoltage```|
|```WarningHighOutputVoltage```|
|```WarningLowOutputVoltage```|
|```WarningInletTemperature```|
|```WarningInternalTemperature```|
|```WarningHighAuxiliaryVoltage```|
|```WarningLowAuxiliaryVoltage```|
|```PowerSupplyMismatch```|
|```GoodInStandby```|

**PowerSupplies[{item}].Oem.Hpe.iPDU**
**PowerSupplies[{item}].Oem.Hpe.iPDU.IPAddress**
Member of [Power.v1_2_1.Power](#power-v1_2_1-power)

| | |
|---|---|
|Description|The IP address of the iPDU connected to this power supply.|
|Type|string or null|
|Read Only|True|

**PowerSupplies[{item}].Oem.Hpe.iPDU.MacAddress**
Member of [Power.v1_2_1.Power](#power-v1_2_1-power)

| | |
|---|---|
|Description|The Ethernet MAC address of the iPDU connected to this power supply.|
|Type|string or null|
|Read Only|True|

**PowerSupplies[{item}].Oem.Hpe.iPDU.Model**
Member of [Power.v1_2_1.Power](#power-v1_2_1-power)

| | |
|---|---|
|Description|The model number of the iPDU connected to this power supply.|
|Type|string|
|Read Only|True|

**PowerSupplies[{item}].Oem.Hpe.iPDU.SerialNumber**
Member of [Power.v1_2_1.Power](#power-v1_2_1-power)

| | |
|---|---|
|Description|The serial number of the iPDU connected to this power supply.|
|Type|string|
|Read Only|True|

**PowerSupplies[{item}].Oem.Hpe.iPDU.iPDUStatus**
**PowerSupplies[{item}].Oem.Hpe.iPDU.iPDUStatus.State**
Member of [Power.v1_2_1.Power](#power-v1_2_1-power)

| | |
|---|---|
|Description|Indicates the known state of the resource.|
|Type|string or null|
|Read Only|True|

The following are the supported values:

|Value|
|---|
|```Unknown```|
|```Ok```|
|```Degraded```|
|```Failed```|
|```OverVoltage```|
|```OverCurrent```|
|```OverTemperature```|
|```ACPowerLost```|
|```FanFailure```|
|```WarningHighInputVoltage```|
|```WarningLowInputVoltage```|
|```WarningHighOutputVoltage```|
|```WarningLowOutputVoltage```|
|```WarningInletTemperature```|
|```WarningInternalTemperature```|
|```WarningHighAuxiliaryVoltage```|
|```WarningLowAuxiliaryVoltage```|
|```PowerSupplyMismatch```|
|```GoodInStandby```|

**PowerSupplies[{item}].Oem.Hpe.iPDUCapable**
Member of [Power.v1_2_1.Power](#power-v1_2_1-power)

| | |
|---|---|
|Description|If true, this power supply is capable of being connected to an iPDUs.|
|Type|boolean|
|Read Only|True|

**PowerSupplies[{item}].PartNumber**
Member of [Power.v1_2_1.Power](#power-v1_2_1-power)

| | |
|---|---|
|Description|The part number for this Power Supply|
|Type|string or null|
|Read Only|True|

**PowerSupplies[{item}].PowerCapacityWatts**
Member of [Power.v1_2_1.Power](#power-v1_2_1-power)

| | |
|---|---|
|Description|The maximum capacity of this Power Supply|
|Type|number or null|
|Read Only|True|

**PowerSupplies[{item}].PowerSupplyType**
Member of [Power.v1_2_1.Power](#power-v1_2_1-power)

| | |
|---|---|
|Description|The Power Supply type (AC or DC)|
|Type|string or null|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```Null```|A value is temporarily unavailable|
|```Unknown```|The power supply type cannot be determined|
|```AC```|Alternating Current (AC) power supply|
|```DC```|Direct Current (DC) power supply|

**PowerSupplies[{item}].Redundancy**
Member of [Power.v1_2_1.Power](#power-v1_2_1-power)
See the Redfish standard schema and specification for information on common Redundancy object.

**PowerSupplies[{item}].RelatedItem (array)**
Member of [Power.v1_2_1.Power](#power-v1_2_1-power)
```RelatedItem``` is an array containing elements of:

**PowerSupplies[{item}].SerialNumber**
Member of [Power.v1_2_1.Power](#power-v1_2_1-power)

| | |
|---|---|
|Description|The serial number for this Power Supply|
|Type|string or null|
|Read Only|True|

**PowerSupplies[{item}].SparePartNumber**
Member of [Power.v1_2_1.Power](#power-v1_2_1-power)

| | |
|---|---|
|Description|The spare part number for this Power Supply|
|Type|string or null|
|Read Only|True|

**PowerSupplies[{item}].Status**
Member of [Power.v1_2_1.Power](#power-v1_2_1-power)
See the Redfish standard schema and specification for information on common Status object.

### Redundancy
Member of [Power.v1_2_1.Power](#power-v1_2_1-power)
See the Redfish standard schema and specification for information on common Redundancy object.

### Status
Member of [Power.v1_2_1.Power](#power-v1_2_1-power)
See the Redfish standard schema and specification for information on common Status object.

## Processor.v1_0_0.Processor
```@odata.type: "#Processor.v1_0_0.Processor"```

This is the schema definition for the Processor resource.  It represents the properties of a processor attached to a System.
### Resource Instances
|Uri|HTTP Allow|
|---|---|
|```/redfish/v1/systems/{item}/processors/{item}/```|GET |

### InstructionSet
Member of [Processor.v1_0_0.Processor](#processor-v1_0_0-processor)

| | |
|---|---|
|Description|The instruction set of the processor|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```x86```|x86 32-bit|
|```x86-64```|x86 64-bit|
|```IA-64```|Intel IA-64|
|```ARM-A32```|ARM 32-bit|
|```ARM-A64```|ARM 64-bit|
|```MIPS32```|MIPS 32-bit|
|```MIPS64```|MIPS 64-bit|
|```OEM```|OEM-defined|

### Manufacturer
Member of [Processor.v1_0_0.Processor](#processor-v1_0_0-processor)

| | |
|---|---|
|Description|The processor manufacturer|
|Type|string or null|
|Read Only|True|

### MaxSpeedMHz
Member of [Processor.v1_0_0.Processor](#processor-v1_0_0-processor)

| | |
|---|---|
|Description|The maximum clock speed of the processor|
|Type|integer or null|
|Read Only|True|

### Model
Member of [Processor.v1_0_0.Processor](#processor-v1_0_0-processor)

| | |
|---|---|
|Description|The product model number of this device|
|Type|string or null|
|Read Only|True|

### Oem.Hpe.AssetTag
Member of [Processor.v1_0_0.Processor](#processor-v1_0_0-processor)

| | |
|---|---|
|Description|The processor asset tag.|
|Type|string or null|
|Read Only|True|

### Oem.Hpe.Cache (array)
Member of [Processor.v1_0_0.Processor](#processor-v1_0_0-processor)
```Cache``` is an array containing elements of:

**Cache[{item}].Associativity**
Member of [Processor.v1_0_0.Processor](#processor-v1_0_0-processor)

| | |
|---|---|
|Description|The associativity of the cache.|
|Type|string or null|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```DirectMapped```|Direct Mapped|
|```2waySetAssociative```|2-way Set-Associative|
|```4waySetAssociative```|4-way Set-Associative|
|```FullyAssociative```|Fully Associative|
|```8waySetAssociative```|8-way Set-Associative|
|```16waySetAssociative```|16-way Set-Associative|
|```12waySetAssociative```|12-way Set-Associative|
|```24waySetAssociative```|24-way Set-Associative|
|```32waySetAssociative```|32-way Set-Associative|
|```48waySetAssociative```|48-way Set-Associative|
|```64waySetAssociative```|64-way Set-Associative|
|```20waySetAssociative```|20-way Set-Associative|

**Cache[{item}].CacheSpeedns**
Member of [Processor.v1_0_0.Processor](#processor-v1_0_0-processor)

| | |
|---|---|
|Description|The cache speed (ns).|
|Type|integer or null|
|Read Only|True|

**Cache[{item}].CurrentSRAMType (array)**
Member of [Processor.v1_0_0.Processor](#processor-v1_0_0-processor)
```CurrentSRAMType``` is an array containing elements of:


| | |
|---|---|
|Description|The array of supported SRAM attributes currently used by the cache.|
|Type|string or null|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```NonBurst```|Non-Burst|
|```Burst```|Burst|
|```PipelineBurst```|Pipeline Burst|
|```Synchronous```|Synchronous|
|```Asynchronous```|Asynchronous|

**Cache[{item}].EccType**
Member of [Processor.v1_0_0.Processor](#processor-v1_0_0-processor)

| | |
|---|---|
|Description|The cache memory ECC type.|
|Type|string or null|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```None```|None|
|```Parity```|Parity|
|```SingleBitECC```|Single-bit ECC|
|```MultiBitECC```|Multi-bit ECC|

**Cache[{item}].InstalledSizeKB**
Member of [Processor.v1_0_0.Processor](#processor-v1_0_0-processor)

| | |
|---|---|
|Description|The installed cache size (KB).|
|Type|integer or null|
|Read Only|True|

**Cache[{item}].Location**
Member of [Processor.v1_0_0.Processor](#processor-v1_0_0-processor)

| | |
|---|---|
|Description|The cache location (internal or external).|
|Type|string or null|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```Internal```|Internal|
|```External```|External|

**Cache[{item}].MaximumSizeKB**
Member of [Processor.v1_0_0.Processor](#processor-v1_0_0-processor)

| | |
|---|---|
|Description|The maximum cache size (KB).|
|Type|integer or null|
|Read Only|True|

**Cache[{item}].Policy**
Member of [Processor.v1_0_0.Processor](#processor-v1_0_0-processor)

| | |
|---|---|
|Description|The caching policy.|
|Type|string or null|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```WriteThrough```|Write through|
|```WriteBack```|Write back|
|```Varies```|Varies with memory address|

**Cache[{item}].Socketed**
Member of [Processor.v1_0_0.Processor](#processor-v1_0_0-processor)

| | |
|---|---|
|Description|If true, the cache is a socketed component.|
|Type|boolean or null|
|Read Only|True|

**Cache[{item}].Status**
Member of [Processor.v1_0_0.Processor](#processor-v1_0_0-processor)
See the Redfish standard schema and specification for information on common Status object.

**Cache[{item}].SupportedSRAMType (array)**
Member of [Processor.v1_0_0.Processor](#processor-v1_0_0-processor)
```SupportedSRAMType``` is an array containing elements of:


| | |
|---|---|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```NonBurst```|Non-Burst|
|```Burst```|Burst|
|```PipelineBurst```|Pipeline Burst|
|```Synchronous```|Synchronous|
|```Asynchronous```|Asynchronous|

**Cache[{item}].SystemCacheType**
Member of [Processor.v1_0_0.Processor](#processor-v1_0_0-processor)

| | |
|---|---|
|Description|The cache type (unified, instructions, or data).|
|Type|string or null|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```Instruction```|Instruction|
|```Data```|Data|
|```Unified```|Unified|

### Oem.Hpe.Characteristics (array)
Member of [Processor.v1_0_0.Processor](#processor-v1_0_0-processor)
```Characteristics``` is an array containing elements of:


| | |
|---|---|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```64Bit```|64-bit Capable|
|```MultiCore```|Multi-Core|
|```HwThread```|Hardware Thread|
|```ExecuteProtection```|Execute Protection|
|```EnhancedVirtualization```|Enhanced Virtualization|
|```PowerPerfControl```|Power/Performance Control|

### Oem.Hpe.ConfigStatus
**Oem.Hpe.ConfigStatus.Populated**
Member of [Processor.v1_0_0.Processor](#processor-v1_0_0-processor)

| | |
|---|---|
|Description|True if the processor socket is populated with a CPU.|
|Type|boolean or null|
|Read Only|True|

**Oem.Hpe.ConfigStatus.State**
Member of [Processor.v1_0_0.Processor](#processor-v1_0_0-processor)

| | |
|---|---|
|Description|The current state of the processor.|
|Type|string or null|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```Enabled```|CPU Enabled|
|```DisabledByUser```|CPU Disabled by User through BIOS Setup|
|```DisabledByBios```|CPU Disabled By BIOS (POST Error)|
|```Idle```|CPU is Idle, waiting to be enabled.|

### Oem.Hpe.CoresEnabled
Member of [Processor.v1_0_0.Processor](#processor-v1_0_0-processor)

| | |
|---|---|
|Description|The number of enabled cores in the processor.|
|Type|integer or null|
|Read Only|True|

### Oem.Hpe.ExternalClockMHz
Member of [Processor.v1_0_0.Processor](#processor-v1_0_0-processor)

| | |
|---|---|
|Description|The processor external clock frequency (MHZ), for example, 1000 = 1 GHZ.|
|Type|integer or null|
|Read Only|True|

### Oem.Hpe.MicrocodePatches (array)
Member of [Processor.v1_0_0.Processor](#processor-v1_0_0-processor)
```MicrocodePatches``` is an array containing elements of:

**MicrocodePatches[{item}].CpuId**
Member of [Processor.v1_0_0.Processor](#processor-v1_0_0-processor)

| | |
|---|---|
|Description|The microcode patch CPUID.|
|Type|string|
|Read Only|True|

**MicrocodePatches[{item}].Date**
Member of [Processor.v1_0_0.Processor](#processor-v1_0_0-processor)

| | |
|---|---|
|Description|The microcode patch date.|
|Type|string|
|Read Only|True|

**MicrocodePatches[{item}].PatchId**
Member of [Processor.v1_0_0.Processor](#processor-v1_0_0-processor)

| | |
|---|---|
|Description|The microcode patch ID.|
|Type|string|
|Read Only|True|

### Oem.Hpe.PartNumber
Member of [Processor.v1_0_0.Processor](#processor-v1_0_0-processor)

| | |
|---|---|
|Description|The processor part number.|
|Type|string or null|
|Read Only|True|

### Oem.Hpe.RatedSpeedMHz
Member of [Processor.v1_0_0.Processor](#processor-v1_0_0-processor)

| | |
|---|---|
|Description|The speed of the processor (in MHz) as of the last system boot, for example, 1000 = 1GHz.|
|Type|integer or null|
|Read Only|True|

### Oem.Hpe.SerialNumber
Member of [Processor.v1_0_0.Processor](#processor-v1_0_0-processor)

| | |
|---|---|
|Description|The processor serial number.|
|Type|string or null|
|Read Only|True|

### Oem.Hpe.VoltageVoltsX10
Member of [Processor.v1_0_0.Processor](#processor-v1_0_0-processor)

| | |
|---|---|
|Description|The processor voltage multiplied by 10, for example, 3.3v = 33.|
|Type|integer or null|
|Read Only|True|

### ProcessorArchitecture
Member of [Processor.v1_0_0.Processor](#processor-v1_0_0-processor)

| | |
|---|---|
|Description|The architecture of the processor|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```x86```|x86 or x86-64|
|```IA-64```|Intel Itanium|
|```ARM```|ARM|
|```MIPS```|MIPS|
|```OEM```|OEM-defined|

### ProcessorId
**ProcessorId.EffectiveFamily**
Member of [Processor.v1_0_0.Processor](#processor-v1_0_0-processor)

| | |
|---|---|
|Description|The effective Family for this processor|
|Type|string or null|
|Read Only|True|

**ProcessorId.EffectiveModel**
Member of [Processor.v1_0_0.Processor](#processor-v1_0_0-processor)

| | |
|---|---|
|Description|The effective Model for this processor|
|Type|string or null|
|Read Only|True|

**ProcessorId.IdentificationRegisters**
Member of [Processor.v1_0_0.Processor](#processor-v1_0_0-processor)

| | |
|---|---|
|Description|The contents of the Identification Registers (CPUID) for this processor|
|Type|string or null|
|Read Only|True|

**ProcessorId.MicrocodeInfo**
Member of [Processor.v1_0_0.Processor](#processor-v1_0_0-processor)

| | |
|---|---|
|Description|The Microcode Information for this processor|
|Type|string or null|
|Read Only|True|

**ProcessorId.Step**
Member of [Processor.v1_0_0.Processor](#processor-v1_0_0-processor)

| | |
|---|---|
|Description|The Step value for this processor|
|Type|string or null|
|Read Only|True|

**ProcessorId.VendorId**
Member of [Processor.v1_0_0.Processor](#processor-v1_0_0-processor)

| | |
|---|---|
|Description|The Vendor Identification for this processor|
|Type|string or null|
|Read Only|True|

### ProcessorType
Member of [Processor.v1_0_0.Processor](#processor-v1_0_0-processor)

| | |
|---|---|
|Description|The type of processor|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```CPU```|A Central Processing Unit|
|```GPU```|A Graphics Processing Unit|
|```FPGA```|A Field Programmable Gate Array|
|```DSP```|A Digital Signal Processor|
|```Accelerator```|An Accelerator|
|```OEM```|An OEM-defined Processing Unit|

### Socket
Member of [Processor.v1_0_0.Processor](#processor-v1_0_0-processor)

| | |
|---|---|
|Description|The socket or location of the processor|
|Type|string or null|
|Read Only|True|

### Status
Member of [Processor.v1_0_0.Processor](#processor-v1_0_0-processor)
See the Redfish standard schema and specification for information on common Status object.

### TotalCores
Member of [Processor.v1_0_0.Processor](#processor-v1_0_0-processor)

| | |
|---|---|
|Description|The total number of cores contained in this processor|
|Type|integer or null|
|Read Only|True|

### TotalThreads
Member of [Processor.v1_0_0.Processor](#processor-v1_0_0-processor)

| | |
|---|---|
|Description|The total number of execution threads supported by this processor|
|Type|integer or null|
|Read Only|True|

## SecureBoot.v1_0_0.SecureBoot
```@odata.type: "#SecureBoot.v1_0_0.SecureBoot"```
### Resource Instances
|Uri|HTTP Allow|
|---|---|
|```/redfish/v1/systems/{item}/secureboot/```|GET POST PATCH |

### SecureBootCurrentBoot
Member of [SecureBoot.v1_0_0.SecureBoot](#secureboot-v1_0_0-secureboot)

| | |
|---|---|
|Description|Secure Boot state during the current boot cycle.|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```Enabled```|Secure Boot is currently enabled.|
|```Disabled```|Secure Boot is currently disabled.|

### SecureBootEnable
Member of [SecureBoot.v1_0_0.SecureBoot](#secureboot-v1_0_0-secureboot)

| | |
|---|---|
|Description|Enable or disable UEFI Secure Boot (takes effect on next boot).|
|Type|boolean or null|
|Read Only|False|

### SecureBootMode
Member of [SecureBoot.v1_0_0.SecureBoot](#secureboot-v1_0_0-secureboot)

| | |
|---|---|
|Description|Current Secure Boot Mode.|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```SetupMode```|Secure Boot is currently in Setup Mode.|
|```UserMode```|Secure Boot is currently in User Mode.|
|```AuditMode```|Secure Boot is currently in Audit Mode.|
|```DeployedMode```|Secure Boot is currently in Deployed Mode.|

### Actions

**SecureBoot.ResetKeys**
Member of [SecureBoot.v1_0_0.SecureBoot](#secureboot-v1_0_0-secureboot)
Action to perform reset of the Secure Boot Keys.


**Parameters:**

**ResetKeysType (string)**

This parameter specifies what type of reset action to perform.

|Value|Description|
|---|---|
|ResetAllKeysToDefault|Reset to default Secure Boot keys on next boot.|
|DeletePK|Delete Secure Boot platform keys on next boot.|
|DeleteAllKeys|Delete all Secure Boot keys on next boot.|
## ServiceRoot.v1_1_0.ServiceRoot
```@odata.type: "#ServiceRoot.v1_1_0.ServiceRoot"```

This object represents the HPE RESTful API root service.
### Resource Instances
|Uri|HTTP Allow|
|---|---|
|```/redfish/v1/```|GET |

### Links to other Resources
|Link Name|Destination type
|---|---|
|```Registries```|Collection of [MessageRegistryFile](#messageregistryfile-v1_0_4-messageregistryfile)|
|```Managers```|Collection of [Manager](#manager-v1_1_0-manager)|
|```AccountService```|[AccountService](#accountservice-v1_0_2-accountservice)|
|```JsonSchemas```|Collection of [JsonSchemaFile](#jsonschemafile-v1_0_4-jsonschemafile)|
|```UpdateService```|[UpdateService](#updateservice-v1_1_0-updateservice)|
|```Oem/Hpe/Links/ResourceDirectory```|[HpeiLOResourceDirectory](#hpeiloresourcedirectory-v2_0_0-hpeiloresourcedirectory)|
|```SessionService```|[SessionService](#sessionservice-v1_0_0-sessionservice)|
|```EventService```|[EventService](#eventservice-v1_0_1-eventservice)|
|```Chassis```|Collection of [Chassis](#chassis-v1_2_0-chassis)|
|```Systems```|Collection of [ComputerSystem](#computersystem-v1_4_0-computersystem)|
|```Links/Sessions```|Collection of [Session](#session-v1_0_0-session)|

### AccountService
The URI to this account service resource.
### Chassis
The URI to this chassis resource.
### EventService
The URI to the event service resource.
### JsonSchemas
The URI to this registries resource.
### Managers
The URI to this managers resource.
### Oem.Hpe.DevSystem
Member of [ServiceRoot.v1_1_0.ServiceRoot](#serviceroot-v1_1_0-serviceroot)

| | |
|---|---|
|Description|Specifies whether the test key is enabled.|
|Type|boolean|
|Read Only|True|

### Oem.Hpe.Manager (array)
Member of [ServiceRoot.v1_1_0.ServiceRoot](#serviceroot-v1_1_0-serviceroot)
```Manager``` is an array containing elements of:

**Manager[{item}].Blade**
**Manager[{item}].Blade.BayNumber**
Member of [ServiceRoot.v1_1_0.ServiceRoot](#serviceroot-v1_1_0-serviceroot)

| | |
|---|---|
|Description|Specifies the location of the blade in the enclosure.|
|Type|string|
|Read Only|True|

**Manager[{item}].Blade.EnclosureName**
Member of [ServiceRoot.v1_1_0.ServiceRoot](#serviceroot-v1_1_0-serviceroot)

| | |
|---|---|
|Description|Specifies the name of the enclosure in which the blade is present.|
|Type|string|
|Read Only|True|

**Manager[{item}].Blade.RackName**
Member of [ServiceRoot.v1_1_0.ServiceRoot](#serviceroot-v1_1_0-serviceroot)

| | |
|---|---|
|Description|Specifies the name of the rack in which the enclosure is present.|
|Type|string|
|Read Only|True|

**Manager[{item}].DefaultLanguage**
Member of [ServiceRoot.v1_1_0.ServiceRoot](#serviceroot-v1_1_0-serviceroot)

| | |
|---|---|
|Description|Default language used for the Web interface.|
|Type|string|
|Read Only|True|

**Manager[{item}].FQDN**
Member of [ServiceRoot.v1_1_0.ServiceRoot](#serviceroot-v1_1_0-serviceroot)

| | |
|---|---|
|Description|Fully qualified domain name of the management processor.|
|Type|string|
|Read Only|True|

**Manager[{item}].HostName**
Member of [ServiceRoot.v1_1_0.ServiceRoot](#serviceroot-v1_1_0-serviceroot)

| | |
|---|---|
|Description|The name of management processor.|
|Type|string|
|Read Only|True|

**Manager[{item}].IPManager**
**Manager[{item}].Languages (array)**
Member of [ServiceRoot.v1_1_0.ServiceRoot](#serviceroot-v1_1_0-serviceroot)
```Languages``` is an array containing elements of:

**Languages[{item}].Language**
Member of [ServiceRoot.v1_1_0.ServiceRoot](#serviceroot-v1_1_0-serviceroot)

| | |
|---|---|
|Description|Specifies one of the languages supported by the management processor.|
|Type|string|
|Read Only|True|

**Languages[{item}].TranslationName**
Member of [ServiceRoot.v1_1_0.ServiceRoot](#serviceroot-v1_1_0-serviceroot)

| | |
|---|---|
|Description|Specifies one of the languages supported by the management processor.|
|Type|string|
|Read Only|True|

**Languages[{item}].Version**
Member of [ServiceRoot.v1_1_0.ServiceRoot](#serviceroot-v1_1_0-serviceroot)

| | |
|---|---|
|Description|Specifies the version of the management processor in the respective language.|
|Type|string|
|Read Only|True|

**Manager[{item}].ManagerFirmwareVersion**
Member of [ServiceRoot.v1_1_0.ServiceRoot](#serviceroot-v1_1_0-serviceroot)

| | |
|---|---|
|Description|The major and minor management processor version numbers.|
|Type|string|
|Read Only|True|

**Manager[{item}].ManagerFirmwareVersionPass**
Member of [ServiceRoot.v1_1_0.ServiceRoot](#serviceroot-v1_1_0-serviceroot)

| | |
|---|---|
|Description|The build or pass number of the management processor version.|
|Type|string|
|Read Only|True|

**Manager[{item}].ManagerType**
Member of [ServiceRoot.v1_1_0.ServiceRoot](#serviceroot-v1_1_0-serviceroot)

| | |
|---|---|
|Description|The type of the service manager.|
|Type|string|
|Read Only|True|

### Oem.Hpe.Moniker
**Oem.Hpe.Moniker.ADVLIC**
Member of [ServiceRoot.v1_1_0.ServiceRoot](#serviceroot-v1_1_0-serviceroot)

| | |
|---|---|
|Description|Optional Licensed functionality tier name.|
|Type|string|
|Read Only|True|

**Oem.Hpe.Moniker.BMC**
Member of [ServiceRoot.v1_1_0.ServiceRoot](#serviceroot-v1_1_0-serviceroot)

| | |
|---|---|
|Description|Generic abbreviation for the management processor.|
|Type|string|
|Read Only|True|

**Oem.Hpe.Moniker.BSYS**
Member of [ServiceRoot.v1_1_0.ServiceRoot](#serviceroot-v1_1_0-serviceroot)

| | |
|---|---|
|Description|Product category name.|
|Type|string|
|Read Only|True|

**Oem.Hpe.Moniker.CLASS**
Member of [ServiceRoot.v1_1_0.ServiceRoot](#serviceroot-v1_1_0-serviceroot)

| | |
|---|---|
|Description|Management processor product category.|
|Type|string|
|Read Only|True|

**Oem.Hpe.Moniker.FEDGRP**
Member of [ServiceRoot.v1_1_0.ServiceRoot](#serviceroot-v1_1_0-serviceroot)

| | |
|---|---|
|Description|Default federation group name.|
|Type|string|
|Read Only|True|

**Oem.Hpe.Moniker.IPROV**
Member of [ServiceRoot.v1_1_0.ServiceRoot](#serviceroot-v1_1_0-serviceroot)

| | |
|---|---|
|Description|Product name for provisioning and deployment suite.|
|Type|string|
|Read Only|True|

**Oem.Hpe.Moniker.PRODABR**
Member of [ServiceRoot.v1_1_0.ServiceRoot](#serviceroot-v1_1_0-serviceroot)

| | |
|---|---|
|Description|Abbreviated product name.|
|Type|string|
|Read Only|True|

**Oem.Hpe.Moniker.PRODFAM**
Member of [ServiceRoot.v1_1_0.ServiceRoot](#serviceroot-v1_1_0-serviceroot)

| | |
|---|---|
|Description|Full product family.|
|Type|string|
|Read Only|True|

**Oem.Hpe.Moniker.PRODGEN**
Member of [ServiceRoot.v1_1_0.ServiceRoot](#serviceroot-v1_1_0-serviceroot)

| | |
|---|---|
|Description|Abbreviated product name and generation.|
|Type|string|
|Read Only|True|

**Oem.Hpe.Moniker.PRODNAM**
Member of [ServiceRoot.v1_1_0.ServiceRoot](#serviceroot-v1_1_0-serviceroot)

| | |
|---|---|
|Description|Full product name.|
|Type|string|
|Read Only|True|

**Oem.Hpe.Moniker.PRODTAG**
Member of [ServiceRoot.v1_1_0.ServiceRoot](#serviceroot-v1_1_0-serviceroot)

| | |
|---|---|
|Description|Branded, abbreviated product name.|
|Type|string|
|Read Only|True|

**Oem.Hpe.Moniker.STDLIC**
Member of [ServiceRoot.v1_1_0.ServiceRoot](#serviceroot-v1_1_0-serviceroot)

| | |
|---|---|
|Description|Base licensed functionality tier name.|
|Type|string|
|Read Only|True|

**Oem.Hpe.Moniker.SUMABR**
Member of [ServiceRoot.v1_1_0.ServiceRoot](#serviceroot-v1_1_0-serviceroot)

| | |
|---|---|
|Description|Acronym for update deployment suite.|
|Type|string|
|Read Only|True|

**Oem.Hpe.Moniker.SUMGR**
Member of [ServiceRoot.v1_1_0.ServiceRoot](#serviceroot-v1_1_0-serviceroot)

| | |
|---|---|
|Description|Product name for update deployment suite.|
|Type|string|
|Read Only|True|

**Oem.Hpe.Moniker.SYSFAM**
Member of [ServiceRoot.v1_1_0.ServiceRoot](#serviceroot-v1_1_0-serviceroot)

| | |
|---|---|
|Description|Host system product family.|
|Type|string|
|Read Only|True|

**Oem.Hpe.Moniker.VENDABR**
Member of [ServiceRoot.v1_1_0.ServiceRoot](#serviceroot-v1_1_0-serviceroot)

| | |
|---|---|
|Description|Abbreviated vendor name (like stock ticker).|
|Type|string|
|Read Only|True|

**Oem.Hpe.Moniker.VENDNAM**
Member of [ServiceRoot.v1_1_0.ServiceRoot](#serviceroot-v1_1_0-serviceroot)

| | |
|---|---|
|Description|Full vendor name.|
|Type|string|
|Read Only|True|

**Oem.Hpe.Moniker.WWW**
Member of [ServiceRoot.v1_1_0.ServiceRoot](#serviceroot-v1_1_0-serviceroot)

| | |
|---|---|
|Description|Top level public internet vendor URI.|
|Type|string|
|Read Only|True|

**Oem.Hpe.Moniker.WWWAHSV**
Member of [ServiceRoot.v1_1_0.ServiceRoot](#serviceroot-v1_1_0-serviceroot)

| | |
|---|---|
|Description|Public internet vendor URI for Active Health viewer.|
|Type|string|
|Read Only|True|

**Oem.Hpe.Moniker.WWWBMC**
Member of [ServiceRoot.v1_1_0.ServiceRoot](#serviceroot-v1_1_0-serviceroot)

| | |
|---|---|
|Description|Public internet vendor URI for the management processor.|
|Type|string|
|Read Only|True|

**Oem.Hpe.Moniker.WWWDOC**
Member of [ServiceRoot.v1_1_0.ServiceRoot](#serviceroot-v1_1_0-serviceroot)

| | |
|---|---|
|Description|Public internet vendor URI for the management processor documentation / manuals.|
|Type|string|
|Read Only|True|

**Oem.Hpe.Moniker.WWWERS**
Member of [ServiceRoot.v1_1_0.ServiceRoot](#serviceroot-v1_1_0-serviceroot)

| | |
|---|---|
|Description|Public internet vendor URI for Embedded Remote Support.|
|Type|string|
|Read Only|True|

**Oem.Hpe.Moniker.WWWGLIS**
Member of [ServiceRoot.v1_1_0.ServiceRoot](#serviceroot-v1_1_0-serviceroot)

| | |
|---|---|
|Description|Public internet vendor URI for management processor licensing infrastructure.|
|Type|string|
|Read Only|True|

**Oem.Hpe.Moniker.WWWIOL**
Member of [ServiceRoot.v1_1_0.ServiceRoot](#serviceroot-v1_1_0-serviceroot)

| | |
|---|---|
|Description|Public internet vendor URI for Online Insight service.|
|Type|string|
|Read Only|True|

**Oem.Hpe.Moniker.WWWLIC**
Member of [ServiceRoot.v1_1_0.ServiceRoot](#serviceroot-v1_1_0-serviceroot)

| | |
|---|---|
|Description|Public internet vendor URI for the management processor.|
|Type|string|
|Read Only|True|

**Oem.Hpe.Moniker.WWWLML**
Member of [ServiceRoot.v1_1_0.ServiceRoot](#serviceroot-v1_1_0-serviceroot)

| | |
|---|---|
|Description|Public internet vendor URI for Learn More Links.|
|Type|string|
|Read Only|True|

**Oem.Hpe.Moniker.WWWPASS**
Member of [ServiceRoot.v1_1_0.ServiceRoot](#serviceroot-v1_1_0-serviceroot)

| | |
|---|---|
|Description|Public internet vendor URI for accessing support account.|
|Type|string|
|Read Only|True|

**Oem.Hpe.Moniker.WWWPRV**
Member of [ServiceRoot.v1_1_0.ServiceRoot](#serviceroot-v1_1_0-serviceroot)

| | |
|---|---|
|Description|Public internet vendor URI for privacy policy statement.|
|Type|string|
|Read Only|True|

**Oem.Hpe.Moniker.WWWQSPEC**
Member of [ServiceRoot.v1_1_0.ServiceRoot](#serviceroot-v1_1_0-serviceroot)

| | |
|---|---|
|Description|Public internet vendor URI for Quick Specs.|
|Type|string|
|Read Only|True|

**Oem.Hpe.Moniker.WWWRESTDOC**
Member of [ServiceRoot.v1_1_0.ServiceRoot](#serviceroot-v1_1_0-serviceroot)

| | |
|---|---|
|Description|Public internet vendor URI for REST API documentation.|
|Type|string|
|Read Only|True|

**Oem.Hpe.Moniker.WWWSUP**
Member of [ServiceRoot.v1_1_0.ServiceRoot](#serviceroot-v1_1_0-serviceroot)

| | |
|---|---|
|Description|Public internet vendor URI for management processor and product support.|
|Type|string|
|Read Only|True|

**Oem.Hpe.Moniker.WWWSWLIC**
Member of [ServiceRoot.v1_1_0.ServiceRoot](#serviceroot-v1_1_0-serviceroot)

| | |
|---|---|
|Description|Public internet vendor URI for vendor software licensing.|
|Type|string|
|Read Only|True|

### Oem.Hpe.Sessions
**Oem.Hpe.Sessions.CertCommonName**
Member of [ServiceRoot.v1_1_0.ServiceRoot](#serviceroot-v1_1_0-serviceroot)

| | |
|---|---|
|Description|The name of the management processor as it appears in the digital certificate when a secure web GUI session is established to the management processor.|
|Type|string|
|Read Only|True|

**Oem.Hpe.Sessions.CertificateLoginEnabled**
Member of [ServiceRoot.v1_1_0.ServiceRoot](#serviceroot-v1_1_0-serviceroot)

| | |
|---|---|
|Description|Specifies whether Certificate login is enabled.|
|Type|boolean|
|Read Only|True|

**Oem.Hpe.Sessions.KerberosEnabled**
Member of [ServiceRoot.v1_1_0.ServiceRoot](#serviceroot-v1_1_0-serviceroot)

| | |
|---|---|
|Description|Specifies whether Kerberos login is enabled.|
|Type|boolean|
|Read Only|True|

**Oem.Hpe.Sessions.LDAPAuthLicenced**
Member of [ServiceRoot.v1_1_0.ServiceRoot](#serviceroot-v1_1_0-serviceroot)

| | |
|---|---|
|Description|Specifies whether a valid license is installed for LDAP use.|
|Type|boolean|
|Read Only|True|

**Oem.Hpe.Sessions.LDAPEnabled**
Member of [ServiceRoot.v1_1_0.ServiceRoot](#serviceroot-v1_1_0-serviceroot)

| | |
|---|---|
|Description|Specifies whether LDAP login is enabled.|
|Type|boolean|
|Read Only|True|

**Oem.Hpe.Sessions.LocalLoginEnabled**
Member of [ServiceRoot.v1_1_0.ServiceRoot](#serviceroot-v1_1_0-serviceroot)

| | |
|---|---|
|Description|Specifies whether local users can log in.|
|Type|boolean|
|Read Only|True|

**Oem.Hpe.Sessions.LoginFailureDelay**
Member of [ServiceRoot.v1_1_0.ServiceRoot](#serviceroot-v1_1_0-serviceroot)

| | |
|---|---|
|Description|The delay (seconds) when a management processor login attempt has failed.|
|Type|integer|
|Read Only|True|

**Oem.Hpe.Sessions.LoginHint**
**Oem.Hpe.Sessions.LoginHint.Hint**
Member of [ServiceRoot.v1_1_0.ServiceRoot](#serviceroot-v1_1_0-serviceroot)

| | |
|---|---|
|Description|The information on how to log in to the management processor.|
|Type|string|
|Read Only|True|

**Oem.Hpe.Sessions.LoginHint.HintPOSTData**
**Oem.Hpe.Sessions.LoginHint.HintPOSTData.Password**
Member of [ServiceRoot.v1_1_0.ServiceRoot](#serviceroot-v1_1_0-serviceroot)

| | |
|---|---|
|Description|The password for logging in to the management processor.|
|Type|string|
|Read Only|True|

**Oem.Hpe.Sessions.LoginHint.HintPOSTData.UserName**
Member of [ServiceRoot.v1_1_0.ServiceRoot](#serviceroot-v1_1_0-serviceroot)

| | |
|---|---|
|Description|The user name for logging in to the management processor.|
|Type|string|
|Read Only|True|

**Oem.Hpe.Sessions.SecurityMessage**
Member of [ServiceRoot.v1_1_0.ServiceRoot](#serviceroot-v1_1_0-serviceroot)

| | |
|---|---|
|Description|The login security banner message that is displayed on the management processor Login page.|
|Type|string|
|Read Only|True|

**Oem.Hpe.Sessions.SecurityOverride**
Member of [ServiceRoot.v1_1_0.ServiceRoot](#serviceroot-v1_1_0-serviceroot)

| | |
|---|---|
|Description|Specifies whether the security override switch is enabled.|
|Type|boolean|
|Read Only|True|

**Oem.Hpe.Sessions.ServerName**
Member of [ServiceRoot.v1_1_0.ServiceRoot](#serviceroot-v1_1_0-serviceroot)

| | |
|---|---|
|Description|The name of the server that this management processor is managing.|
|Type|string|
|Read Only|True|

### Oem.Hpe.Time
Member of [ServiceRoot.v1_1_0.ServiceRoot](#serviceroot-v1_1_0-serviceroot)

| | |
|---|---|
|Description|The current Redfish service time.|
|Type|string or null|
|Read Only|True|

### RedfishVersion
Member of [ServiceRoot.v1_1_0.ServiceRoot](#serviceroot-v1_1_0-serviceroot)

| | |
|---|---|
|Description|The version of the Redfish service|
|Type|string|
|Read Only|True|

### Registries
The URI to this registries resource.
### SessionService
The URI to this sessions service resource.
### Systems
The URI to this systems resource.
### UUID
Member of [ServiceRoot.v1_1_0.ServiceRoot](#serviceroot-v1_1_0-serviceroot)

| | |
|---|---|
|Description|Unique identifier for a service instance.  This value should be an exact match of the UUID value returned in a 200OK from an SSDP M-SEARCH request during discovery.|
|Type|string or null|
|Read Only|True|

### UpdateService
The URI to this UpdateService resource.
## Session.v1_0_0.Session
```@odata.type: "#Session.v1_0_0.Session"```
### Resource Instances
|Uri|HTTP Allow|
|---|---|
|```/redfish/v1/sessionservice/sessions/{item}/```|GET DELETE |

### Oem.Hpe.AccessTime
Member of [Session.v1_0_0.Session](#session-v1_0_0-session)

| | |
|---|---|
|Description|User session last-access time|
|Type|string|
|Read Only|True|

### Oem.Hpe.LoginTime
Member of [Session.v1_0_0.Session](#session-v1_0_0-session)

| | |
|---|---|
|Description|User session login time|
|Type|string|
|Read Only|True|

### Oem.Hpe.MySession
Member of [Session.v1_0_0.Session](#session-v1_0_0-session)

| | |
|---|---|
|Description|Indicates whether this is a session I own.|
|Type|boolean|
|Read Only|True|

### Oem.Hpe.Privileges
**Oem.Hpe.Privileges.HostBIOSConfigPriv**
Member of [Session.v1_0_0.Session](#session-v1_0_0-session)

| | |
|---|---|
|Description|This privilege enables a user to configure Host Bios Settings.|
|Type|boolean|
|Read Only|True|

**Oem.Hpe.Privileges.HostNICConfigPriv**
Member of [Session.v1_0_0.Session](#session-v1_0_0-session)

| | |
|---|---|
|Description|This privilege enables a user to configure Host NIC Settings.|
|Type|boolean|
|Read Only|True|

**Oem.Hpe.Privileges.HostStorageConfigPriv**
Member of [Session.v1_0_0.Session](#session-v1_0_0-session)

| | |
|---|---|
|Description|This privilege enables a user to configure Host Storage Settings.|
|Type|boolean|
|Read Only|True|

**Oem.Hpe.Privileges.LoginPriv**
Member of [Session.v1_0_0.Session](#session-v1_0_0-session)

| | |
|---|---|
|Description|This privilege enables a user to log in to the management processor. All local accounts have the login privilege. This privilege is added automatically if it is not specified.|
|Type|boolean|
|Read Only|True|

**Oem.Hpe.Privileges.RemoteConsolePriv**
Member of [Session.v1_0_0.Session](#session-v1_0_0-session)

| | |
|---|---|
|Description|This privilege enables a user to remotely access the host system Remote Console, including video, keyboard, and mouse control.|
|Type|boolean|
|Read Only|True|

**Oem.Hpe.Privileges.SystemRecoveryConfigPriv**
Member of [Session.v1_0_0.Session](#session-v1_0_0-session)

| | |
|---|---|
|Description|This privilege enables a user to manage the critical recovery firmware images on the iLO Repository.|
|Type|boolean|
|Read Only|True|

**Oem.Hpe.Privileges.UserConfigPriv**
Member of [Session.v1_0_0.Session](#session-v1_0_0-session)

| | |
|---|---|
|Description|This privilege enables a user to add, edit, and delete local management processor user accounts. A user with this privilege can change privileges for all users.|
|Type|boolean|
|Read Only|True|

**Oem.Hpe.Privileges.VirtualMediaPriv**
Member of [Session.v1_0_0.Session](#session-v1_0_0-session)

| | |
|---|---|
|Description|This privilege enables a user to use the Virtual Media feature on the host system.|
|Type|boolean|
|Read Only|True|

**Oem.Hpe.Privileges.VirtualPowerAndResetPriv**
Member of [Session.v1_0_0.Session](#session-v1_0_0-session)

| | |
|---|---|
|Description|This privilege enables a user to power-cycle or reset the host system. These activities interrupt system availability. A user with this privilege can diagnose the system by using the Generate NMI to System button.|
|Type|boolean|
|Read Only|True|

**Oem.Hpe.Privileges.iLOConfigPriv**
Member of [Session.v1_0_0.Session](#session-v1_0_0-session)

| | |
|---|---|
|Description|This privilege enables a user to configure most management processor settings, including security settings, and to remotely update the management processor firmware. This privilege does not enable local user account administration.|
|Type|boolean|
|Read Only|True|

### Oem.Hpe.UserAccount
Member of [Session.v1_0_0.Session](#session-v1_0_0-session)

| | |
|---|---|
|Description|Login details of the user|
|Type|string|
|Read Only|True|

### Oem.Hpe.UserDistinguishedName
Member of [Session.v1_0_0.Session](#session-v1_0_0-session)

| | |
|---|---|
|Description|LDAP user is identified by its distinguished name (DN).|
|Type|string|
|Read Only|True|

### Oem.Hpe.UserExpires
Member of [Session.v1_0_0.Session](#session-v1_0_0-session)

| | |
|---|---|
|Description|User session expire time|
|Type|string|
|Read Only|True|

### Oem.Hpe.UserIP
Member of [Session.v1_0_0.Session](#session-v1_0_0-session)

| | |
|---|---|
|Description|IP address of the user|
|Type|string|
|Read Only|True|

### Oem.Hpe.UserTag
Member of [Session.v1_0_0.Session](#session-v1_0_0-session)

| | |
|---|---|
|Description|Session source|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|
|---|
|```Web UI```|
|```RBSU```|
|```Remote Console```|
|```SSH```|
|```IPMI/RMCP```|
|```SM-CLP```|
|```RIBCL```|
|```REST```|
|```Unknown```|

### Oem.Hpe.UserType
Member of [Session.v1_0_0.Session](#session-v1_0_0-session)

| | |
|---|---|
|Description|User type|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|
|---|
|```Local```|
|```Directory```|
|```Single Sign On```|
|```Kerberos```|
|```Trusted Key```|
|```Security Override```|
|```System```|
|```Federation```|

### UserName
Member of [Session.v1_0_0.Session](#session-v1_0_0-session)

| | |
|---|---|
|Description|Name to use to log in to the management processor.|
|Type|string|
|Read Only|True|

## SessionService.v1_0_0.SessionService
```@odata.type: "#SessionService.v1_0_0.SessionService"```

This is the schema definition for the Session Service.  It represents the properties for the service itself and has links to the actual list of sessions.
### Resource Instances
|Uri|HTTP Allow|
|---|---|
|```/redfish/v1/sessionservice/```|GET PATCH |

### Links to other Resources
|Link Name|Destination type
|---|---|
|```Sessions```|Collection of [Session](#session-v1_0_0-session)|

### ServiceEnabled
Member of [SessionService.v1_0_0.SessionService](#sessionservice-v1_0_0-sessionservice)

| | |
|---|---|
|Description|This indicates whether this service is enabled.|
|Type|boolean or null|
|Read Only|True|

### SessionTimeout
Member of [SessionService.v1_0_0.SessionService](#sessionservice-v1_0_0-sessionservice)

| | |
|---|---|
|Description|This is the number of seconds of inactivity that a session may have before the session service closes the session due to inactivity.|
|Type|integer|
|Read Only|False|

### Sessions
This property references a Collection resource of Sessions.
### Status
Member of [SessionService.v1_0_0.SessionService](#sessionservice-v1_0_0-sessionservice)
See the Redfish standard schema and specification for information on common Status object.

## SmartStorageConfig.v2_0_0.SmartStorageConfig
```@odata.type: "#SmartStorageConfig.v2_0_0.SmartStorageConfig"```

Smart Storage Configuration Schema
### Resource Instances
|Uri|HTTP Allow|
|---|---|
|```/redfish/v1/systems/{item}/smartstorageconfig/```|GET |
|```/redfish/v1/systems/{item}/smartstorageconfig/settings/```|GET PATCH |

### Links to other Resources
|Link Name|Destination type
|---|---|
|```@Redfish.Settings/SettingsObject```|[SmartStorageConfig](#smartstorageconfig-v2_0_0-smartstorageconfig)|

### Actions (array)
Member of [SmartStorageConfig.v2_0_0.SmartStorageConfig](#smartstorageconfig-v2_0_0-smartstorageconfig)
```Actions``` is an array containing elements of:

**Actions[{item}].Action**
Member of [SmartStorageConfig.v2_0_0.SmartStorageConfig](#smartstorageconfig-v2_0_0-smartstorageconfig)

| | |
|---|---|
|Description|The action to perform|
|Type|string|
|Read Only|False|

**Actions[{item}].ErasePattern**
Member of [SmartStorageConfig.v2_0_0.SmartStorageConfig](#smartstorageconfig-v2_0_0-smartstorageconfig)

| | |
|---|---|
|Description|The erase pattern used to erase the drive|
|Type|string|
|Read Only|False|

The following are the supported values:

|Value|Description|
|---|---|
|```SanitizeRestrictedBlockErase```|Use the restricted block erase sanitize block erase method to erase a drive|
|```SanitizeUnrestrictedBlockErase```|Use the unrestricted block erase sanitize method to erase a drive|
|```SanitizeRestrictedOverwrite```|Use the restricted overwrite sanitize method to erase a drive|
|```SanitizeUnrestrictedOverwrite```|Use the unrestricted overwrite sanitize method to erase a drive|
|```SanitizeRestrictedCryptoScramble```|Use the unrestricted cryptographic scramble sanitize method to erase a drive|
|```SanitizeUnrestrictedCryptoScramble```|Use the unrestricted cryptographic scramble sanitize method to erase a drive|
|```OnePass```|Use the controller-based one pass erase method that writes zeroes to every sector of the drive|
|```TwoPass```|Use the controller-based two pass erase method that writes random data to every sector of the drive on the first pass, and zeroes on the second pass|
|```ThreePass```|Use the controller-based three pass erase method that writes random data to every sector of the drive on the first two passes, and zeroes on the third pass|

**Actions[{item}].PhysicalDriveList (array)**
Member of [SmartStorageConfig.v2_0_0.SmartStorageConfig](#smartstorageconfig-v2_0_0-smartstorageconfig)
```PhysicalDriveList``` is an array containing elements of:


| | |
|---|---|
|Description|Physical drive in the format specified in DriveLocationFormat|
|Type|string|
|Read Only|True|

### CurrentParallelSurfaceScanCount
Member of [SmartStorageConfig.v2_0_0.SmartStorageConfig](#smartstorageconfig-v2_0_0-smartstorageconfig)

| | |
|---|---|
|Description|This indicates the number of parallel surface scans the controller allows|
|Type|integer or null|
|Read Only|False|

### DataGuard
Member of [SmartStorageConfig.v2_0_0.SmartStorageConfig](#smartstorageconfig-v2_0_0-smartstorageconfig)

| | |
|---|---|
|Description|The value of the field indicates whether or not data destructive actions are allowed on the controller|
|Type|string|
|Read Only|False|

The following are the supported values:

|Value|Description|
|---|---|
|```Strict```|Data destructive actions are not allowed|
|```Permissive```|Logical drive delete actions will be ignored|
|```Disabled```|Data destructive actions are allowed|

### DegradedPerformanceOptimization
Member of [SmartStorageConfig.v2_0_0.SmartStorageConfig](#smartstorageconfig-v2_0_0-smartstorageconfig)

| | |
|---|---|
|Description|Enables the controller to attempt to improve performance on RAID 5/50/6(ADG)/60 logical drives when one or more physical drives in the logical drive are failed|
|Type|string or null|
|Read Only|False|

The following are the supported values:

|Value|Description|
|---|---|
|```Enabled```|The controller will attempt to improve performance by buffering physical drive requests|
|```Disabled```|The controller will not buffer, which may result in reading from the same drive multiple times|

### DriveLocationFormat
Member of [SmartStorageConfig.v2_0_0.SmartStorageConfig](#smartstorageconfig-v2_0_0-smartstorageconfig)

| | |
|---|---|
|Description|The format of the physical drive locations on this controller|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```ControllerPort:Box:Bay[|ControllerPort:Box:Bay]```|The drives are specified in the <controller port: box: bay> format, with an optional alternate location delineated by a pipe|

### DriveWriteCache
Member of [SmartStorageConfig.v2_0_0.SmartStorageConfig](#smartstorageconfig-v2_0_0-smartstorageconfig)

| | |
|---|---|
|Description|Enables or disables the write cache of the physical drives attached to the controller|
|Type|string or null|
|Read Only|False|

The following are the supported values:

|Value|Description|
|---|---|
|```Enabled```|The write cache of the physical drives attached to the controller are enabled|
|```Disabled```|The write cache of the physical drives attached to the controller are enabled|

### ElevatorSort
Member of [SmartStorageConfig.v2_0_0.SmartStorageConfig](#smartstorageconfig-v2_0_0-smartstorageconfig)

| | |
|---|---|
|Description|Enables the controller to sort requests to a physical drive|
|Type|string or null|
|Read Only|False|

The following are the supported values:

|Value|Description|
|---|---|
|```Enabled```|The controller will sort the requests to minimize the amount of seeking the drive must perform in order to reduce seek times|
|```Disabled```|The controller will perform the requests as they are recieved in order to improve request throughput|

### EncryptionConfiguration
Member of [SmartStorageConfig.v2_0_0.SmartStorageConfig](#smartstorageconfig-v2_0_0-smartstorageconfig)

| | |
|---|---|
|Description|This indicates the type of encryption configured on the controller|
|Type|string|
|Read Only|False|

The following are the supported values:

|Value|Description|
|---|---|
|```ExpressLocal```|Express local encryption is configured and the controller is being encrypted with internally generated keys|
|```None```|Encryption is not configured on the controller|

### EncryptionEULA
Member of [SmartStorageConfig.v2_0_0.SmartStorageConfig](#smartstorageconfig-v2_0_0-smartstorageconfig)

| | |
|---|---|
|Description|The value of this field indicates whether or not the user has accepted the encryption EULA|
|Type|string or null|
|Read Only|False|

The following are the supported values:

|Value|Description|
|---|---|
|```Accept```|The user has read and accepted the encryption EULA|
|```Decline```|The user has not read and accepted the encryption EULA|

### ExpandPriority
Member of [SmartStorageConfig.v2_0_0.SmartStorageConfig](#smartstorageconfig-v2_0_0-smartstorageconfig)

| | |
|---|---|
|Description|The level of priority that transformations have over handling current operating system requests|
|Type|string or null|
|Read Only|False|

The following are the supported values:

|Value|Description|
|---|---|
|```High```|Transformations will complete as fast as possible at the expense of normal I/O|
|```Medium```|Transformations will perform with some impact on normal I/O|
|```Low```|Transformations will perform only when normal I/O is not occurring and may take longer to complete|

### FlexibleLatencySchedulerSetting
Member of [SmartStorageConfig.v2_0_0.SmartStorageConfig](#smartstorageconfig-v2_0_0-smartstorageconfig)

| | |
|---|---|
|Description|This allows the controller to process certain high-latency requests after a delay that may time out when elevator sorting|
|Type|string or null|
|Read Only|False|

The following are the supported values:

|Value|Description|
|---|---|
|```Default```|The controller will rely only on elevator sorting|
|```Low250```|The controller will apply a cutoff value of 250ms when suspending elevator sorting|
|```Middle100```|The controller will apply a cutoff value of 100ms when suspending elevator sorting|
|```Middle50```|The controller will apply a cutoff value of 50ms when suspending elevator sorting|
|```Aggressive30```|The controller will apply a cutoff value of 30ms when suspending elevator sorting|
|```Aggressive10```|The controller will apply a cutoff value of 10ms when suspending elevator sorting|

### InconsistencyRepairPolicy
Member of [SmartStorageConfig.v2_0_0.SmartStorageConfig](#smartstorageconfig-v2_0_0-smartstorageconfig)

| | |
|---|---|
|Description|Enables the controller to update data on RAID 6(ADG) and 60 volumes based on parity information when an inconsistency is discovered during surface scan|
|Type|string or null|
|Read Only|False|

The following are the supported values:

|Value|Description|
|---|---|
|```Enabled```|The controller will update the data on the drives based on the parity information|
|```Disabled```|The controller will only update the parity information and leave the data untouched|

### Location
Member of [SmartStorageConfig.v2_0_0.SmartStorageConfig](#smartstorageconfig-v2_0_0-smartstorageconfig)

| | |
|---|---|
|Description|The location of the controller|
|Type|string|
|Read Only|True|

### LocationFormat
Member of [SmartStorageConfig.v2_0_0.SmartStorageConfig](#smartstorageconfig-v2_0_0-smartstorageconfig)

| | |
|---|---|
|Description|The format of the Location property on this controller|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```PCISlot```|The location of the controller is given as a PCI slot number|

### LogicalDrives (array)
Member of [SmartStorageConfig.v2_0_0.SmartStorageConfig](#smartstorageconfig-v2_0_0-smartstorageconfig)
```LogicalDrives``` is an array containing elements of:

**LogicalDrives[{item}].Accelerator**
Member of [SmartStorageConfig.v2_0_0.SmartStorageConfig](#smartstorageconfig-v2_0_0-smartstorageconfig)

| | |
|---|---|
|Description|The acceleration method of the logical drive|
|Type|string|
|Read Only|False|

The following are the supported values:

|Value|Description|
|---|---|
|```None```|Logical drive acceleration is disabled|
|```ControllerCache```|Read and writes to the logical drive are being cached by the controller|
|```IOBypass```|For logical drives on SSDs, read and write information directly from the drive|

**LogicalDrives[{item}].Actions (array)**
Member of [SmartStorageConfig.v2_0_0.SmartStorageConfig](#smartstorageconfig-v2_0_0-smartstorageconfig)
```Actions``` is an array containing elements of:

**Actions[{item}].Action**
Member of [SmartStorageConfig.v2_0_0.SmartStorageConfig](#smartstorageconfig-v2_0_0-smartstorageconfig)

| | |
|---|---|
|Description|The action to perform|
|Type|string|
|Read Only|False|

**LogicalDrives[{item}].BlockSizeBytes**
Member of [SmartStorageConfig.v2_0_0.SmartStorageConfig](#smartstorageconfig-v2_0_0-smartstorageconfig)

| | |
|---|---|
|Description|The block size of the disk drive in bytes|
|Type|integer|
|Read Only|False|

**LogicalDrives[{item}].CapacityBlocks**
Member of [SmartStorageConfig.v2_0_0.SmartStorageConfig](#smartstorageconfig-v2_0_0-smartstorageconfig)

| | |
|---|---|
|Description|Total usable capacity available on this logical drive in block units. Set to -1 to use all remaining space for maximum size|
|Type|integer|
|Read Only|False|

**LogicalDrives[{item}].CapacityGiB**
Member of [SmartStorageConfig.v2_0_0.SmartStorageConfig](#smartstorageconfig-v2_0_0-smartstorageconfig)

| | |
|---|---|
|Description|Total usable capacity available on this logical drive in GiB units. Set to -1 to use all remaining space for maximum size|
|Type|integer|
|Read Only|False|

**LogicalDrives[{item}].DataDrives**
Member of [SmartStorageConfig.v2_0_0.SmartStorageConfig](#smartstorageconfig-v2_0_0-smartstorageconfig)
**LogicalDrives[{item}].DataDrives (array)**
Member of [SmartStorageConfig.v2_0_0.SmartStorageConfig](#smartstorageconfig-v2_0_0-smartstorageconfig)
```DataDrives``` is an array containing elements of:


| | |
|---|---|
|Description|Physical drive in the format specified in DriveLocationFormat|
|Type|string|
|Read Only|True|

**LogicalDrives[{item}].DataDrives**
**LogicalDrives[{item}].DataDrives.DataDriveCount**
Member of [SmartStorageConfig.v2_0_0.SmartStorageConfig](#smartstorageconfig-v2_0_0-smartstorageconfig)

| | |
|---|---|
|Description|Specify the number of data drives for this logical drive|
|Type|integer|
|Read Only|False|

**LogicalDrives[{item}].DataDrives.DataDriveInterfaceType**
Member of [SmartStorageConfig.v2_0_0.SmartStorageConfig](#smartstorageconfig-v2_0_0-smartstorageconfig)

| | |
|---|---|
|Description|Specify the interface type for the data drives for this logical drive|
|Type|string|
|Read Only|False|

The following are the supported values:

|Value|Description|
|---|---|
|```SAS```|Use SAS drives when creating the logical drive|
|```SATA```|Use SATA drives when creating the logical drive|

**LogicalDrives[{item}].DataDrives.DataDriveLocation**
Member of [SmartStorageConfig.v2_0_0.SmartStorageConfig](#smartstorageconfig-v2_0_0-smartstorageconfig)

| | |
|---|---|
|Description|Specify the location of the data drives for this logical drive|
|Type|string|
|Read Only|False|

The following are the supported values:

|Value|Description|
|---|---|
|```Internal```|Drives that are attached to an internal port of the controller (front drives)|
|```External```|Drives that are attached to an external port of the controller (JBOD drives)|

**LogicalDrives[{item}].DataDrives.DataDriveMediaType**
Member of [SmartStorageConfig.v2_0_0.SmartStorageConfig](#smartstorageconfig-v2_0_0-smartstorageconfig)

| | |
|---|---|
|Description|Specify the media type for the data drives for this logical drive|
|Type|string|
|Read Only|False|

The following are the supported values:

|Value|Description|
|---|---|
|```HDD```|Use spindle drives when creating the logical drive|
|```SSD```|Use solid state drives when creating the logical drive|

**LogicalDrives[{item}].DataDrives.DataDriveMinimumSizeGiB**
Member of [SmartStorageConfig.v2_0_0.SmartStorageConfig](#smartstorageconfig-v2_0_0-smartstorageconfig)

| | |
|---|---|
|Description|Specify the minimum size for the data drive(s) used to create the logical drive|
|Type|integer|
|Read Only|False|

**LogicalDrives[{item}].LegacyBootPriority**
Member of [SmartStorageConfig.v2_0_0.SmartStorageConfig](#smartstorageconfig-v2_0_0-smartstorageconfig)

| | |
|---|---|
|Description|The boot priority of this logical drive|
|Type|string|
|Read Only|False|

The following are the supported values:

|Value|Description|
|---|---|
|```Primary```|This logical drive is the primary boot volume|
|```Secondary```|This logical drive is the secondary boot volume|
|```All```|This logical drive is both the primary and secondary boot volume|
|```None```|This logical drive has no legacy boot priority|

**LogicalDrives[{item}].LogicalDriveName**
Member of [SmartStorageConfig.v2_0_0.SmartStorageConfig](#smartstorageconfig-v2_0_0-smartstorageconfig)

| | |
|---|---|
|Description|Label given to the logical drive|
|Type|string|
|Read Only|False|

**LogicalDrives[{item}].LogicalDriveNumber**
Member of [SmartStorageConfig.v2_0_0.SmartStorageConfig](#smartstorageconfig-v2_0_0-smartstorageconfig)

| | |
|---|---|
|Description|Logical drive number|
|Type|integer|
|Read Only|True|

**LogicalDrives[{item}].ParityGroupCount**
Member of [SmartStorageConfig.v2_0_0.SmartStorageConfig](#smartstorageconfig-v2_0_0-smartstorageconfig)

| | |
|---|---|
|Description|The number of parity groups to use in the logical drive; only valid for certain RAID levels|
|Type|integer|
|Read Only|False|

**LogicalDrives[{item}].ParityInitializationType**
Member of [SmartStorageConfig.v2_0_0.SmartStorageConfig](#smartstorageconfig-v2_0_0-smartstorageconfig)

| | |
|---|---|
|Description|When creating a logical drive with a RAID level that requires parity, parity blocks can be initialized with two different methods|
|Type|string|
|Read Only|False|

The following are the supported values:

|Value|Description|
|---|---|
|```Default```|Parity blocks are initialized in the background and the logical drive is available during this time|
|```Rapid```|Both data and parity blocks are initialized in the foreground and the logical drive will not be available to the operating system until initialization completes|

**LogicalDrives[{item}].Raid**
Member of [SmartStorageConfig.v2_0_0.SmartStorageConfig](#smartstorageconfig-v2_0_0-smartstorageconfig)

| | |
|---|---|
|Description|The current RAID level configured on the logical drive|
|Type|string|
|Read Only|False|

The following are the supported values:

|Value|Description|
|---|---|
|```Raid0```|There is no fault tolerance used on this logical drive|
|```Raid1```|Two sets of duplicate data is being stored on a pair of drives|
|```Raid1ADM```|Three sets of duplicate data is being stored on a trio of drives|
|```Raid10```|Data is duplicated and striped across pairs of disk drives|
|```Raid10ADM```|Data is duplicated and striped across trios of disk drives|
|```Raid5```|Fault tolerance is achieved by storing parity data across 3 or more disk drives|
|```Raid50```|Fault tolerance is achieved by storing parity data and striping the data across 6 or more disk drives|
|```Raid6```|Fault tolerance is achieved by storing multiple sets parity data across 4 or more disk drives|
|```Raid60```|Fault tolerance is achieved by storing multiple sets parity data and striping the data across 8 or more disk drives|

**LogicalDrives[{item}].SpareDrives**
Member of [SmartStorageConfig.v2_0_0.SmartStorageConfig](#smartstorageconfig-v2_0_0-smartstorageconfig)
**LogicalDrives[{item}].SpareDrives (array)**
Member of [SmartStorageConfig.v2_0_0.SmartStorageConfig](#smartstorageconfig-v2_0_0-smartstorageconfig)
```SpareDrives``` is an array containing elements of:


| | |
|---|---|
|Description|Physical drive in the format specified in DriveLocationFormat|
|Type|string|
|Read Only|True|

**LogicalDrives[{item}].SpareDrives**
**LogicalDrives[{item}].SpareDrives.SpareDriveCount**
Member of [SmartStorageConfig.v2_0_0.SmartStorageConfig](#smartstorageconfig-v2_0_0-smartstorageconfig)

| | |
|---|---|
|Description|Specify the number of spare drives for this logical drive|
|Type|integer|
|Read Only|False|

**LogicalDrives[{item}].SpareRebuildMode**
Member of [SmartStorageConfig.v2_0_0.SmartStorageConfig](#smartstorageconfig-v2_0_0-smartstorageconfig)

| | |
|---|---|
|Description|Type of spare drive used with this logical drive|
|Type|string|
|Read Only|False|

The following are the supported values:

|Value|Description|
|---|---|
|```Dedicated```|The spare drive temporarily takes over a failed data drive; when the failed data drive is replaced, the spare drive becomes idle again|
|```Roaming```|The spare drive replaces the failed data drive|

**LogicalDrives[{item}].StripSizeBytes**
Member of [SmartStorageConfig.v2_0_0.SmartStorageConfig](#smartstorageconfig-v2_0_0-smartstorageconfig)

| | |
|---|---|
|Description|The strip size of the logical drive in bytes|
|Type|integer|
|Read Only|False|

**LogicalDrives[{item}].StripeSizeBytes**
Member of [SmartStorageConfig.v2_0_0.SmartStorageConfig](#smartstorageconfig-v2_0_0-smartstorageconfig)

| | |
|---|---|
|Description|The stripe size of the logical drive in bytes|
|Type|integer|
|Read Only|False|

**LogicalDrives[{item}].VolumeUniqueIdentifier**
Member of [SmartStorageConfig.v2_0_0.SmartStorageConfig](#smartstorageconfig-v2_0_0-smartstorageconfig)

| | |
|---|---|
|Description|Logical drive volume unique identifier|
|Type|string|
|Read Only|True|

### MonitorAndPerformanceAnalysisDelaySeconds
Member of [SmartStorageConfig.v2_0_0.SmartStorageConfig](#smartstorageconfig-v2_0_0-smartstorageconfig)

| | |
|---|---|
|Description|This sets the monitor and performance delay on the controller. Valid values range from 0 to 1440 seconds. Set to 60 seconds for default settings and 0 seconds for video-on-demand optimized setting|
|Type|integer or null|
|Read Only|False|

### NoBatteryWriteCache
Member of [SmartStorageConfig.v2_0_0.SmartStorageConfig](#smartstorageconfig-v2_0_0-smartstorageconfig)

| | |
|---|---|
|Description|This indicates if the controller will continue to use write cache even if the backup power source is not available|
|Type|string or null|
|Read Only|False|

The following are the supported values:

|Value|Description|
|---|---|
|```Enabled```|The controller will continue to use write cache even if the backup power source is not available|
|```Disabled```|The controller will not continue to use write cache even if the backup power source is not available|

### PhysicalDrives (array)
Member of [SmartStorageConfig.v2_0_0.SmartStorageConfig](#smartstorageconfig-v2_0_0-smartstorageconfig)
```PhysicalDrives``` is an array containing elements of:

**PhysicalDrives[{item}].LegacyBootPriority**
Member of [SmartStorageConfig.v2_0_0.SmartStorageConfig](#smartstorageconfig-v2_0_0-smartstorageconfig)

| | |
|---|---|
|Description|The boot priority of this physical drive|
|Type|string|
|Read Only|False|

The following are the supported values:

|Value|Description|
|---|---|
|```Primary```|This physical drive is the primary boot volume|
|```Secondary```|This physical drive is the secondary boot volume|
|```All```|This physical drive is both the primary and secondary boot volume|
|```None```|This physical drive has no legacy boot priority|

**PhysicalDrives[{item}].PhysicalDriveNumber**
Member of [SmartStorageConfig.v2_0_0.SmartStorageConfig](#smartstorageconfig-v2_0_0-smartstorageconfig)

| | |
|---|---|
|Description|Physical drive number|
|Type|integer|
|Read Only|True|

### Ports (array)
Member of [SmartStorageConfig.v2_0_0.SmartStorageConfig](#smartstorageconfig-v2_0_0-smartstorageconfig)
```Ports``` is an array containing elements of:

**Ports[{item}].OperatingModeAfterReboot**
Member of [SmartStorageConfig.v2_0_0.SmartStorageConfig](#smartstorageconfig-v2_0_0-smartstorageconfig)

| | |
|---|---|
|Description|The operating mode of this port after a reboot|
|Type|string|
|Read Only|False|

The following are the supported values:

|Value|Description|
|---|---|
|```Mixed```|The port will be functioning in mixed mode after rebooting. Unassigned drives will be exposed to the OS|

**Ports[{item}].PortIndex**
Member of [SmartStorageConfig.v2_0_0.SmartStorageConfig](#smartstorageconfig-v2_0_0-smartstorageconfig)

| | |
|---|---|
|Description|The port index|
|Type|integer|
|Read Only|True|

### PowerModeAfterReboot
Member of [SmartStorageConfig.v2_0_0.SmartStorageConfig](#smartstorageconfig-v2_0_0-smartstorageconfig)

| | |
|---|---|
|Description|The power mode of the controller after a reboot|
|Type|string|
|Read Only|False|

The following are the supported values:

|Value|Description|
|---|---|
|```Invalid```|The controller will be operating in an unknown power mode after a reboot|
|```MinPower```|The controller will be operating in minimum power mode after a reboot|
|```Balanced```|The controller will be operating in a balanced mode after a reboot|
|```MaxPerformance```|The controller will be operating in maximum performance power mode after a reboot|

### PredictiveSpareRebuild
Member of [SmartStorageConfig.v2_0_0.SmartStorageConfig](#smartstorageconfig-v2_0_0-smartstorageconfig)

| | |
|---|---|
|Description|Enables or disables predictive spare rebuild mode|
|Type|string or null|
|Read Only|False|

The following are the supported values:

|Value|Description|
|---|---|
|```Enabled```|Spare drives will replace physical drives that are predicted to fail preemptively|
|```Disabled```|Spare drives will replace physical drives only when they fail|

### QueueDepth
Member of [SmartStorageConfig.v2_0_0.SmartStorageConfig](#smartstorageconfig-v2_0_0-smartstorageconfig)

| | |
|---|---|
|Description|This sets the maximum number of requests the controller will submit to a drive at any given time|
|Type|string or null|
|Read Only|False|

The following are the supported values:

|Value|Description|
|---|---|
|```Queue2```|2 requests|
|```Queue4```|4 requests|
|```Queue8```|8 requests|
|```Queue16```|16 requests|
|```Queue32```|32 requests|
|```Automatic```|Automatically determine the best queue depth for the controller|

### ReadCachePercent
Member of [SmartStorageConfig.v2_0_0.SmartStorageConfig](#smartstorageconfig-v2_0_0-smartstorageconfig)

| | |
|---|---|
|Description|This indicates the percentage of cache used for read cache on the controller, with the rest of the cache being used for write cache|
|Type|integer or null|
|Read Only|False|

### RebuildPriority
Member of [SmartStorageConfig.v2_0_0.SmartStorageConfig](#smartstorageconfig-v2_0_0-smartstorageconfig)

| | |
|---|---|
|Description|The level of priority that rebuilds have over handling current operating system requests|
|Type|string or null|
|Read Only|False|

The following are the supported values:

|Value|Description|
|---|---|
|```High```|Rebuilds will complete as fast as possible at the expense of normal I/O|
|```Medium```|Rebuilds will perform with some impact on normal I/O|
|```Low```|Rebuilds will perform only when normal I/O is not occurring and may take longer to complete|
|```RapidHigh```|Rebuilds will complete as fast as possible at the expense of normal I/O|
|```RapidMediumHigh```|Rebuilds will perform with an impact on normal I/O|
|```RapidMedium```|Rebuilds will perform with some impact on normal I/O|
|```RapidLow```|Rebuilds will perform only when normal I/O is not occurring and may take longer to complete|

### SurfaceScanAnalysisDelaySeconds
Member of [SmartStorageConfig.v2_0_0.SmartStorageConfig](#smartstorageconfig-v2_0_0-smartstorageconfig)

| | |
|---|---|
|Description|Sets the delay of the controller before beginning surface scan analysis. Only valid if SurfaceScanAnalysisPriority is Idle|
|Type|integer or null|
|Read Only|False|

### SurfaceScanAnalysisPriority
Member of [SmartStorageConfig.v2_0_0.SmartStorageConfig](#smartstorageconfig-v2_0_0-smartstorageconfig)

| | |
|---|---|
|Description|Priority that the controller takes to find and correct disk surface errors|
|Type|string or null|
|Read Only|False|

The following are the supported values:

|Value|Description|
|---|---|
|```Disabled```|Surface scan is disabled and may lead to data loss|
|```High```|Surface scan commands will be sent with the host I/O, resulting in faster scanning, but may inpact host I/O performance|
|```Medium```|Surface scan commands have a medium priority, and will have some impact on host I/O performance|
|```Low```|Surface scan commands have a low priority, and will have little impact on host I/O performance|
|```Idle```|Surface scan commands will ony be issued when no host I/O is present after a delay|

### SurvivalPowerMode
Member of [SmartStorageConfig.v2_0_0.SmartStorageConfig](#smartstorageconfig-v2_0_0-smartstorageconfig)

| | |
|---|---|
|Description|Enables or Disables survival mode|
|Type|string|
|Read Only|False|

The following are the supported values:

|Value|Description|
|---|---|
|```Enabled```|The controller will throttle dynamic power settings to their minimum when temperatures exceed the warning threshold|
|```Disabled```|The controller will not throttle dynamic power settings|

### WriteCacheBypassThresholdKiB
Member of [SmartStorageConfig.v2_0_0.SmartStorageConfig](#smartstorageconfig-v2_0_0-smartstorageconfig)

| | |
|---|---|
|Description|This value sets the write cache bypass threshold, ranging from 16 KiB to 1040 KiB in multiples of 16 KiB, where all writes larger than the specified value in KiB units will bypass the write cache and be written directly to the disk for non-parity RAID volumes|
|Type|integer or null|
|Read Only|False|

## SoftwareInventory.v1_0_0.SoftwareInventory
```@odata.type: "#SoftwareInventory.v1_0_0.SoftwareInventory"```
### Resource Instances
|Uri|HTTP Allow|
|---|---|
|```/redfish/v1/updateservice/firmwareinventory/{item}/```|GET |
|```/redfish/v1/updateservice/softwareinventory/{item}/```|GET |

### Oem.Hpe.DeviceClass
Member of [SoftwareInventory.v1_0_0.SoftwareInventory](#softwareinventory-v1_0_0-softwareinventory)

| | |
|---|---|
|Description|DeviceType GUID rendered by iLO for certain items iLO knows how to flash, and omitted for all other items.|
|Type|string or null|
|Read Only|True|

### Oem.Hpe.DeviceContext
Member of [SoftwareInventory.v1_0_0.SoftwareInventory](#softwareinventory-v1_0_0-softwareinventory)

| | |
|---|---|
|Description|Friendly text string - same as 'Location' in fw inventory - omitted if not available.|
|Type|string|
|Read Only|True|

### Oem.Hpe.DeviceInstance
Member of [SoftwareInventory.v1_0_0.SoftwareInventory](#softwareinventory-v1_0_0-softwareinventory)

| | |
|---|---|
|Description|UEFI Device Path if a PCI Device - omitted otherwise.|
|Type|string|
|Read Only|True|

### Oem.Hpe.Targets (array)
Member of [SoftwareInventory.v1_0_0.SoftwareInventory](#softwareinventory-v1_0_0-softwareinventory)
```Targets``` is an array containing elements of:


| | |
|---|---|
|Description|A GUID indicating iLO's knowledge of a possible correlation GUIDs vs. components.|
|Type|string or null|
|Read Only|True|

### Status
Member of [SoftwareInventory.v1_0_0.SoftwareInventory](#softwareinventory-v1_0_0-softwareinventory)
See the Redfish standard schema and specification for information on common Status object.

### Updateable
Member of [SoftwareInventory.v1_0_0.SoftwareInventory](#softwareinventory-v1_0_0-softwareinventory)

| | |
|---|---|
|Description|This is true if the item is updatable.|
|Type|boolean or null|
|Read Only|True|

### Version
Member of [SoftwareInventory.v1_0_0.SoftwareInventory](#softwareinventory-v1_0_0-softwareinventory)

| | |
|---|---|
|Description|same as 'VersionString' in existing FwSwVersionInventory|
|Type|string or null|
|Read Only|True|

## Storage.v1_0_0.Storage
```@odata.type: "#Storage.v1_0_0.Storage"```
### Resource Instances
|Uri|HTTP Allow|
|---|---|
|```/redfish/v1/systems/{item}/storage/{interface}/{item}/```|GET |

### Links to other Resources
|Link Name|Destination type
|---|---|
|```Volumes```|Collection of [Volume](#volume-v1_0_0-volume)|
|```Links/Enclosures[]```|[Chassis](#chassis-v1_2_0-chassis)|
|```StorageControllers[]```|[Storage](#storage-v1_0_0-storage)|
|```Drives[]```|[Drive](#drive-v1_0_0-drive)|

### Drives (array)
Member of [Storage.v1_0_0.Storage](#storage-v1_0_0-storage)
```Drives``` is an array containing elements of:

### Status
Member of [Storage.v1_0_0.Storage](#storage-v1_0_0-storage)
See the Redfish standard schema and specification for information on common Status object.

### StorageControllers (array)
Member of [Storage.v1_0_0.Storage](#storage-v1_0_0-storage)
```StorageControllers``` is an array containing elements of:

**StorageControllers[{item}].Manufacturer**
Member of [Storage.v1_0_0.Storage](#storage-v1_0_0-storage)

| | |
|---|---|
|Description|Controller Manufacturer name.|
|Type|string or null|
|Read Only|True|

**StorageControllers[{item}].Model**
Member of [Storage.v1_0_0.Storage](#storage-v1_0_0-storage)

| | |
|---|---|
|Description|Controller model name.|
|Type|string or null|
|Read Only|True|

**StorageControllers[{item}].SerialNumber**
Member of [Storage.v1_0_0.Storage](#storage-v1_0_0-storage)

| | |
|---|---|
|Description|Controller serial number.|
|Type|string or null|
|Read Only|True|

**StorageControllers[{item}].Status**
Member of [Storage.v1_0_0.Storage](#storage-v1_0_0-storage)
See the Redfish standard schema and specification for information on common Status object.

**StorageControllers[{item}].SupportedControllerProtocols (array)**
Member of [Storage.v1_0_0.Storage](#storage-v1_0_0-storage)
```SupportedControllerProtocols``` is an array containing elements of:


| | |
|---|---|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|
|---|
|```PCIe```|

**StorageControllers[{item}].SupportedDeviceProtocols (array)**
Member of [Storage.v1_0_0.Storage](#storage-v1_0_0-storage)
```SupportedDeviceProtocols``` is an array containing elements of:


| | |
|---|---|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|
|---|
|```USB```|
|```SATA```|
|```NVMe```|

**StorageControllers[{item}].UEFIDevicePath**
Member of [Storage.v1_0_0.Storage](#storage-v1_0_0-storage)

| | |
|---|---|
|Description|UEFI Device Path of the storage controller.|
|Type|string or null|
|Read Only|True|

### Volumes
A reference to the Volumes associated with this storage system.
## Thermal.v1_1_0.Thermal
```@odata.type: "#Thermal.v1_1_0.Thermal"```

The schema definition for the Thermal Metrics. It represents the properties for temperature and cooling.
### Resource Instances
|Uri|HTTP Allow|
|---|---|
|```/redfish/v1/chassis/{item}/thermal/```|GET |

### Fans (array)
Member of [Thermal.v1_1_0.Thermal](#thermal-v1_1_0-thermal)
```Fans``` is an array containing elements of:

**Fans[{item}].CorrelatableID**
Member of [Thermal.v1_1_0.Thermal](#thermal-v1_1_0-thermal)

| | |
|---|---|
|Description|The CorrelatableID for this fan.|
|Type|string or null|
|Read Only|True|

**Fans[{item}].LowerThresholdCritical**
Member of [Thermal.v1_1_0.Thermal](#thermal-v1_1_0-thermal)

| | |
|---|---|
|Description|Below normal range but not yet fatal.|
|Type|integer or null|
|Read Only|True|

**Fans[{item}].LowerThresholdFatal**
Member of [Thermal.v1_1_0.Thermal](#thermal-v1_1_0-thermal)

| | |
|---|---|
|Description|Below normal range and is fatal.|
|Type|integer or null|
|Read Only|True|

**Fans[{item}].LowerThresholdNonCritical**
Member of [Thermal.v1_1_0.Thermal](#thermal-v1_1_0-thermal)

| | |
|---|---|
|Description|Below normal range.|
|Type|integer or null|
|Read Only|True|

**Fans[{item}].MaximumValue**
Member of [Thermal.v1_1_0.Thermal](#thermal-v1_1_0-thermal)

| | |
|---|---|
|Description|Maximum value for CurrentReading.|
|Type|integer or null|
|Read Only|True|

**Fans[{item}].MinimumValue**
Member of [Thermal.v1_1_0.Thermal](#thermal-v1_1_0-thermal)

| | |
|---|---|
|Description|Minimum value for CurrentReading.|
|Type|integer or null|
|Read Only|True|

**Fans[{item}].Oem.Hpe.HotPluggable**
Member of [Thermal.v1_1_0.Thermal](#thermal-v1_1_0-thermal)

| | |
|---|---|
|Description|Indicates if the fan can be replaced while server is running.|
|Type|boolean|
|Read Only|True|

**Fans[{item}].Oem.Hpe.Location**
Member of [Thermal.v1_1_0.Thermal](#thermal-v1_1_0-thermal)

| | |
|---|---|
|Description|Indicates the component (i.e. CPU, Memory, and Storage) that the fan is being used to cool.|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|
|---|
|```System```|
|```System Board```|
|```I/O Board```|
|```CPU```|
|```Memory```|
|```Storage```|
|```Removable Media```|
|```Power Supply```|
|```Ambient```|
|```Chassis```|
|```Bridge Board```|
|```Exhaust```|
|```Processor Bay```|
|```IO Bay```|
|```Blade Slot```|
|```Virtual```|

**Fans[{item}].Oem.Hpe.Redundant**
Member of [Thermal.v1_1_0.Thermal](#thermal-v1_1_0-thermal)

| | |
|---|---|
|Description|Indicates if the fan is in a redundant configuration.|
|Type|boolean|
|Read Only|True|

**Fans[{item}].PhysicalContext**
Member of [Thermal.v1_1_0.Thermal](#thermal-v1_1_0-thermal)

| | |
|---|---|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```Room```|The room|
|```Intake```|The intake point of the chassis|
|```Exhaust```|The exhaust point of the chassis|
|```Front```|The front of the chassis|
|```Back```|The back of the chassis|
|```Upper```|The upper portion of the chassis|
|```Lower```|The lower portion of the chassis|
|```CPU```|A Processor (CPU)|
|```GPU```|A Graphics Processor (GPU)|
|```Backplane```|A backplane within the chassis|
|```SystemBoard```|The system board (PCB)|
|```PowerSupply```|A power supply|
|```VoltageRegulator```|A voltage regulator device|
|```StorageDevice```|A storage device|
|```NetworkingDevice```|A networking device|
|```ComputeBay```|Within a compute bay|
|```StorageBay```|Within a storage bay|
|```NetworkBay```|Within a networking bay|
|```ExpansionBay```|Within an expansion bay|
|```PowerSupplyBay```|Within a power supply bay|

**Fans[{item}].Reading**
Member of [Thermal.v1_1_0.Thermal](#thermal-v1_1_0-thermal)

| | |
|---|---|
|Description|The current speed of the fan.|
|Type|integer or null|
|Read Only|True|

**Fans[{item}].ReadingUnits**
Member of [Thermal.v1_1_0.Thermal](#thermal-v1_1_0-thermal)

| | |
|---|---|
|Description|Units for the CurrentReading.|
|Type|string or null|
|Read Only|True|

The following are the supported values:

|Value|
|---|
|```Null```|
|```Percent```|

**Fans[{item}].Status**
Member of [Thermal.v1_1_0.Thermal](#thermal-v1_1_0-thermal)
See the Redfish standard schema and specification for information on common Status object.

**Fans[{item}].UpperThresholdCritical**
Member of [Thermal.v1_1_0.Thermal](#thermal-v1_1_0-thermal)

| | |
|---|---|
|Description|Above normal range but not yet fatal.|
|Type|integer or null|
|Read Only|True|

**Fans[{item}].UpperThresholdFatal**
Member of [Thermal.v1_1_0.Thermal](#thermal-v1_1_0-thermal)

| | |
|---|---|
|Description|Above normal range and is fatal.|
|Type|integer or null|
|Read Only|True|

**Fans[{item}].UpperThresholdNonCritical**
Member of [Thermal.v1_1_0.Thermal](#thermal-v1_1_0-thermal)

| | |
|---|---|
|Description|Above normal range.|
|Type|integer or null|
|Read Only|True|

### Oem.Hpe.FanPercentAdjust
Member of [Thermal.v1_1_0.Thermal](#thermal-v1_1_0-thermal)

| | |
|---|---|
|Description|System-wide setting for fan +/- percentage adjustment.|
|Type|integer|
|Read Only|False|

### Status
Member of [Thermal.v1_1_0.Thermal](#thermal-v1_1_0-thermal)
See the Redfish standard schema and specification for information on common Status object.

### Temperatures (array)
Member of [Thermal.v1_1_0.Thermal](#thermal-v1_1_0-thermal)
```Temperatures``` is an array containing elements of:

**Temperatures[{item}].CorrelatableID**
Member of [Thermal.v1_1_0.Thermal](#thermal-v1_1_0-thermal)

| | |
|---|---|
|Description|The CorrelatableID for this temperature sensor.|
|Type|string or null|
|Read Only|True|

**Temperatures[{item}].LowerThresholdCritical**
Member of [Thermal.v1_1_0.Thermal](#thermal-v1_1_0-thermal)

| | |
|---|---|
|Description|Below normal range but not yet fatal.|
|Type|number or null|
|Read Only|True|

**Temperatures[{item}].LowerThresholdFatal**
Member of [Thermal.v1_1_0.Thermal](#thermal-v1_1_0-thermal)

| | |
|---|---|
|Description|Below normal range and is fatal.|
|Type|number or null|
|Read Only|True|

**Temperatures[{item}].LowerThresholdNonCritical**
Member of [Thermal.v1_1_0.Thermal](#thermal-v1_1_0-thermal)

| | |
|---|---|
|Description|Below normal range.|
|Type|number or null|
|Read Only|True|

**Temperatures[{item}].MaximumValue**
Member of [Thermal.v1_1_0.Thermal](#thermal-v1_1_0-thermal)

| | |
|---|---|
|Description|Maximum value for CurrentReading.|
|Type|integer or null|
|Read Only|True|

**Temperatures[{item}].MinimumValue**
Member of [Thermal.v1_1_0.Thermal](#thermal-v1_1_0-thermal)

| | |
|---|---|
|Description|Minimum value for CurrentReading.|
|Type|integer or null|
|Read Only|True|

**Temperatures[{item}].Oem.Hpe.LocationXmm**
Member of [Thermal.v1_1_0.Thermal](#thermal-v1_1_0-thermal)

| | |
|---|---|
|Description|The location of the sensor, in millimeters, along the X axis from the logical reference point.|
|Type|integer|
|Read Only|True|

**Temperatures[{item}].Oem.Hpe.LocationYmm**
Member of [Thermal.v1_1_0.Thermal](#thermal-v1_1_0-thermal)

| | |
|---|---|
|Description|The location of the sensor, in millimeters, along the Y axis from the logical reference point.|
|Type|integer|
|Read Only|True|

**Temperatures[{item}].Oem.Hpe.LocationZmm**
Member of [Thermal.v1_1_0.Thermal](#thermal-v1_1_0-thermal)

| | |
|---|---|
|Description|The location of the sensor, in millimeters, along the Z axis from the logical reference point.|
|Type|integer|
|Read Only|True|

**Temperatures[{item}].PhysicalContext**
Member of [Thermal.v1_1_0.Thermal](#thermal-v1_1_0-thermal)

| | |
|---|---|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```Room```|The room|
|```Intake```|The intake point of the chassis|
|```Exhaust```|The exhaust point of the chassis|
|```Front```|The front of the chassis|
|```Back```|The back of the chassis|
|```Upper```|The upper portion of the chassis|
|```Lower```|The lower portion of the chassis|
|```CPU```|A Processor (CPU)|
|```GPU```|A Graphics Processor (GPU)|
|```Backplane```|A backplane within the chassis|
|```SystemBoard```|The system board (PCB)|
|```PowerSupply```|A power supply|
|```VoltageRegulator```|A voltage regulator device|
|```StorageDevice```|A storage device|
|```NetworkingDevice```|A networking device|
|```ComputeBay```|Within a compute bay|
|```StorageBay```|Within a storage bay|
|```NetworkBay```|Within a networking bay|
|```ExpansionBay```|Within an expansion bay|
|```PowerSupplyBay```|Within a power supply bay|

**Temperatures[{item}].ReadingCelsius**
Member of [Thermal.v1_1_0.Thermal](#thermal-v1_1_0-thermal)

| | |
|---|---|
|Description|The current reading of the temperature sensor.|
|Type|integer or null|
|Read Only|True|

**Temperatures[{item}].SensorNumber**
Member of [Thermal.v1_1_0.Thermal](#thermal-v1_1_0-thermal)

| | |
|---|---|
|Description|A numerical identifier to represent the temperature sensor.|
|Type|integer or null|
|Read Only|True|

**Temperatures[{item}].Status**
Member of [Thermal.v1_1_0.Thermal](#thermal-v1_1_0-thermal)
See the Redfish standard schema and specification for information on common Status object.

**Temperatures[{item}].UpperThresholdCritical**
Member of [Thermal.v1_1_0.Thermal](#thermal-v1_1_0-thermal)

| | |
|---|---|
|Description|Above normal range but not yet fatal.|
|Type|number or null|
|Read Only|True|

**Temperatures[{item}].UpperThresholdFatal**
Member of [Thermal.v1_1_0.Thermal](#thermal-v1_1_0-thermal)

| | |
|---|---|
|Description|Above normal range and is fatal.|
|Type|number or null|
|Read Only|True|

**Temperatures[{item}].UpperThresholdNonCritical**
Member of [Thermal.v1_1_0.Thermal](#thermal-v1_1_0-thermal)

| | |
|---|---|
|Description|The noncritical temperature threshold.|
|Type|number or null|
|Read Only|True|

## UpdateService.v1_1_0.UpdateService
```@odata.type: "#UpdateService.v1_1_0.UpdateService"```
### Resource Instances
|Uri|HTTP Allow|
|---|---|
|```/redfish/v1/updateservice/```|GET POST PATCH |

### Links to other Resources
|Link Name|Destination type
|---|---|
|```Oem/Hpe/InstallSets```|Collection of [HpeComponentInstallSet](#hpecomponentinstallset-v1_0_1-hpecomponentinstallset)|
|```Oem/Hpe/ComponentRepository```|Collection of [HpeComponent](#hpecomponent-v1_0_0-hpecomponent)|
|```FirmwareInventory```|Collection of [SoftwareInventory](#softwareinventory-v1_0_0-softwareinventory)|
|```SoftwareInventory```|Collection of [SoftwareInventory](#softwareinventory-v1_0_0-softwareinventory)|
|```Oem/Hpe/UpdateTaskQueue```|Collection of [HpeComponentUpdateTask](#hpecomponentupdatetask-v1_0_1-hpecomponentupdatetask)|

### FirmwareInventory
Link to Firmware Inventory.
### HttpPushUri
Member of [UpdateService.v1_1_0.UpdateService](#updateservice-v1_1_0-updateservice)

| | |
|---|---|
|Description|The URI to which a client may POST an update image.|
|Type|string|
|Read Only|True|

### Oem.Hpe.ComponentRepository
Link to the Component Repository.
### Oem.Hpe.CurrentTime
Member of [UpdateService.v1_1_0.UpdateService](#updateservice-v1_1_0-updateservice)

| | |
|---|---|
|Description|ISO 8601 Redfish-style time string of the current iLO time (the reference for all scheduling)|
|Type|string|
|Read Only|True|

### Oem.Hpe.FirmwareIntegrity
**Oem.Hpe.FirmwareIntegrity.EnableBackgroundScan**
Member of [UpdateService.v1_1_0.UpdateService](#updateservice-v1_1_0-updateservice)

| | |
|---|---|
|Description|Enables or disables background scan of critical firmware.|
|Type|boolean|
|Read Only|False|

**Oem.Hpe.FirmwareIntegrity.LastFailedImageUri**
Member of [UpdateService.v1_1_0.UpdateService](#updateservice-v1_1_0-updateservice)

| | |
|---|---|
|Description|This is a link to the binary image of the firmware that failed an integrity check and is intended for diagnostic purposes.|
|Type|string or null|
|Read Only|True|

**Oem.Hpe.FirmwareIntegrity.LastScanResult**
Member of [UpdateService.v1_1_0.UpdateService](#updateservice-v1_1_0-updateservice)

| | |
|---|---|
|Description|The firmware integrity scan engine status.|
|Type|string or null|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```OK```|The last firmware integrity scan completed without finding any issues.|
|```Repaired```|The last firmware integrity scan successfully repaired an issue.  Refer to the event log for details.|
|```Failure```|The last firmware integrity scan failed to complete or repair an issue.  Refer to the event log for details.|
|```Stopped```|The last firmware integrity scan was stopped prior to completion.  Refer to the event log for details.|

**Oem.Hpe.FirmwareIntegrity.LastScanTime**
Member of [UpdateService.v1_1_0.UpdateService](#updateservice-v1_1_0-updateservice)

| | |
|---|---|
|Description|The time stamp of the last firmware integrity scan.|
|Type|string or null|
|Read Only|True|

**Oem.Hpe.FirmwareIntegrity.OnIntegrityFailure**
Member of [UpdateService.v1_1_0.UpdateService](#updateservice-v1_1_0-updateservice)

| | |
|---|---|
|Description|Sets the policy for how the firmware integrity check handles integrity failures.|
|Type|string|
|Read Only|False|

The following are the supported values:

|Value|Description|
|---|---|
|```LogOnly```|Log failures to the iLO event log but do not automatically attempt to repair.|
|```LogAndRepairAutomatically```|Log failures to the iLO event log and automatically attempt to repair.|

**Oem.Hpe.FirmwareIntegrity.ScanEveryDays**
Member of [UpdateService.v1_1_0.UpdateService](#updateservice-v1_1_0-updateservice)

| | |
|---|---|
|Description|Sets the interval between firmware integrity scans in 24 hour increments.|
|Type|integer or null|
|Read Only|False|

### Oem.Hpe.FlashProgressPercent
Member of [UpdateService.v1_1_0.UpdateService](#updateservice-v1_1_0-updateservice)

| | |
|---|---|
|Description|This is the percent complete for an iLO flash operation.  It is only valid when State is Updating.|
|Type|integer or null|
|Read Only|True|

### Oem.Hpe.InstallSets
Link to the Install Sets collection.
### Oem.Hpe.Result
**Oem.Hpe.Result.MessageArgs (array)**
Member of [UpdateService.v1_1_0.UpdateService](#updateservice-v1_1_0-updateservice)
```MessageArgs``` is an array containing elements of:


| | |
|---|---|
|Type|string|
|Read Only|True|

**Oem.Hpe.Result.MessageId**
Member of [UpdateService.v1_1_0.UpdateService](#updateservice-v1_1_0-updateservice)

| | |
|---|---|
|Description|The key for this message that can be used to look up the message in a message registry.|
|Type|string|
|Read Only|False|

### Oem.Hpe.State
Member of [UpdateService.v1_1_0.UpdateService](#updateservice-v1_1_0-updateservice)

| | |
|---|---|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```Idle```|The update service is idle.|
|```Uploading```|The update service is receiving a new component.|
|```Verifying```|The update service is verifying the integrity of a new component.|
|```Writing```|The update service is writing a new component to the iLO Repository.|
|```Updating```|The update service is updating (flashing) firmware.|
|```Complete```|The update service has completed up upload or update operation.|
|```Error```|The upload service encountered an error.  See Result for detail.|

### Oem.Hpe.UpdateTaskQueue
Link to the Update Task Queue.
### Oem.Hpe.UploadCurrentEtag
Member of [UpdateService.v1_1_0.UpdateService](#updateservice-v1_1_0-updateservice)

| | |
|---|---|
|Description|client-supplied etag (during component upload) indicating to what UploadStatus is reporting upon.|
|Type|string|
|Read Only|True|

### ServiceEnabled
Member of [UpdateService.v1_1_0.UpdateService](#updateservice-v1_1_0-updateservice)

| | |
|---|---|
|Description|Indicates if the Update Service is enabled.|
|Type|boolean or null|
|Read Only|True|

### SoftwareInventory
Link to Software Inventory.  This is only available when the Agentless Management Service is running.
### Actions

**UpdateService.SimpleUpdate**
Member of [UpdateService.v1_1_0.UpdateService](#updateservice-v1_1_0-updateservice)

**Parameters:**

**TransferProtocol (string)**

|Value|Description|
|---|---|
|FTP|File Transfer Protocol|
|HTTP|Hypertext Transfer Protocol|
|CIFS|Common Internet File System protocol|
|HTTPS|HTTP Secure protocol|
|NSF|Network File System protocol|
|OEM|A protocol defined by the manufacturer.|
|TFTP|Trivial File Transfer Protocol|
|SCP|Secure File Copy protocol|

**ImageURI (string)**

**HpeiLOUpdateServiceExt.DeleteInstallSets**
Member of [UpdateService.v1_1_0.UpdateService](#updateservice-v1_1_0-updateservice)

**Parameters:**

**IncludeRecoverySet (boolean)**

**HpeiLOUpdateServiceExt.DeleteUnlockedComponents**
Member of [UpdateService.v1_1_0.UpdateService](#updateservice-v1_1_0-updateservice)
There are no parameters for this action.

**HpeiLOUpdateServiceExt.SetDefaultLanguage**
Member of [UpdateService.v1_1_0.UpdateService](#updateservice-v1_1_0-updateservice)

**Parameters:**

**Language (string)**

Specifies one of the languages supported by the management processor to be set as default language used for the Web interface.

**HpeiLOUpdateServiceExt.StartFirmwareIntegrityCheck**
Member of [UpdateService.v1_1_0.UpdateService](#updateservice-v1_1_0-updateservice)
There are no parameters for this action.

**HpeiLOUpdateServiceExt.RemoveLanguagePack**
Member of [UpdateService.v1_1_0.UpdateService](#updateservice-v1_1_0-updateservice)

**Parameters:**

**Language (string)**

Specifies one of the languages supported by the management processor for removal. Please use HpeiLOUpdateServiceExt.AddFromUri or UpdateService.SimpleUpdate for adding language pack. NOTE: When language pack is removed, the Manager will reset automatically.

**HpeiLOUpdateServiceExt.DeleteUpdateTaskQueueItems**
Member of [UpdateService.v1_1_0.UpdateService](#updateservice-v1_1_0-updateservice)
There are no parameters for this action.

**HpeiLOUpdateServiceExt.AddFromUri**
Member of [UpdateService.v1_1_0.UpdateService](#updateservice-v1_1_0-updateservice)

**Parameters:**

**UpdateTarget (boolean)**

**UpdateRecoverySet (boolean)**

**UploadCurrentEtag (string)**

client-supplied etag (during component upload) indicating to what UploadStatus is reporting upon.

**UpdateRepository (boolean)**

**CompSigURI (string)**

**ImageURI (string)**

**TPMOverrideFlag (boolean)**
## VirtualMedia.v1_0_0.VirtualMedia
```@odata.type: "#VirtualMedia.v1_0_0.VirtualMedia"```

This is the schema definition for the Virtual Media service.
### Resource Instances
|Uri|HTTP Allow|
|---|---|
|```/redfish/v1/managers/{item}/virtualmedia/{item}/```|GET POST PATCH |

### ConnectedVia
Member of [VirtualMedia.v1_0_0.VirtualMedia](#virtualmedia-v1_0_0-virtualmedia)

| | |
|---|---|
|Description|Specifies how the virtual media is connected to the server.|
|Type|string or null|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```Null```|A value is temporarily unavailable|
|```NotConnected```|No current connection.|
|```URI```|Connected to a URI location.|
|```Applet```|Connected to a client application.|

### Image
Member of [VirtualMedia.v1_0_0.VirtualMedia](#virtualmedia-v1_0_0-virtualmedia)

| | |
|---|---|
|Description|The valid URI indicating the image that is mounted on this server. A null value indicates that no image exists.|
|Type|string or null|
|Read Only|False|

### ImageName
Member of [VirtualMedia.v1_0_0.VirtualMedia](#virtualmedia-v1_0_0-virtualmedia)

| | |
|---|---|
|Description|The name of the image that is mounted on this server. This is usually provided when a URL image is mounted through scripted virtual media.|
|Type|string or null|
|Read Only|True|

### Inserted
Member of [VirtualMedia.v1_0_0.VirtualMedia](#virtualmedia-v1_0_0-virtualmedia)

| | |
|---|---|
|Description|Indicates whether the virtual media is mounted on the server.|
|Type|boolean or null|
|Read Only|True|

### MediaTypes (array)
Member of [VirtualMedia.v1_0_0.VirtualMedia](#virtualmedia-v1_0_0-virtualmedia)
```MediaTypes``` is an array containing elements of:


| | |
|---|---|
|Description|The array of supported media types for this connection.|
|Type|string|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```CD```|A CD-ROM format (ISO) image.|
|```Floppy```|A floppy disk image.|
|```USBStick```|An emulation of a USB storage device.|
|```DVD```|A DVD-ROM format image.|

### Oem.Hpe.BootOnNextServerReset
Member of [VirtualMedia.v1_0_0.VirtualMedia](#virtualmedia-v1_0_0-virtualmedia)

| | |
|---|---|
|Description|If set to true, the server will boot to this image on the next server reboot. The image will be ejected automatically on the second server reboot so that the server does not boot to this image twice.|
|Type|boolean|
|Read Only|False|

### WriteProtected
Member of [VirtualMedia.v1_0_0.VirtualMedia](#virtualmedia-v1_0_0-virtualmedia)

| | |
|---|---|
|Description|Indicates whether the virtual media is protected against write operations.|
|Type|boolean or null|
|Read Only|True|

### Actions

**HpeiLOVirtualMedia.InsertVirtualMedia**
Member of [VirtualMedia.v1_0_0.VirtualMedia](#virtualmedia-v1_0_0-virtualmedia)

**Parameters:**

**Image (string)**

A URL for an ISO, BIN, or IMG file locating the virtual media image.

**Intent (string)**

A text description of the reason for this action invocation.

**Certificate (string)**

A PEM encoded X509 certificate used to validate the https server.

**Signature (string)**

A RSA2048 SHA-256 signature validating the provided Intent (Base64 encoded).

**HpeiLOVirtualMedia.EjectVirtualMedia**
Member of [VirtualMedia.v1_0_0.VirtualMedia](#virtualmedia-v1_0_0-virtualmedia)

**Parameters:**

**Intent (string)**

A text description of the reason for this action invocation.

**Signature (string)**

A RSA2048 SHA-256 signature validating the provided Intent (Base64 encoded).
## Volume.v1_0_0.Volume
```@odata.type: "#Volume.v1_0_0.Volume"```
### Resource Instances
|Uri|HTTP Allow|
|---|---|
|```/redfish/v1/systems/{item}/storage/{interface}/{item}/volumes/{item}/```|GET |

### Links to other Resources
|Link Name|Destination type
|---|---|
|```Links/Drives[]```|[Drive](#drive-v1_0_0-drive)|

### CapacityBytes
Member of [Volume.v1_0_0.Volume](#volume-v1_0_0-volume)

| | |
|---|---|
|Description|The size in bytes of this Volume|
|Type|integer or null|
|Read Only|True|

### Status
Member of [Volume.v1_0_0.Volume](#volume-v1_0_0-volume)
See the Redfish standard schema and specification for information on common Status object.

### VolumeType
Member of [Volume.v1_0_0.Volume](#volume-v1_0_0-volume)

| | |
|---|---|
|Description|The type of this volume.|
|Type|string or null|
|Read Only|True|

The following are the supported values:

|Value|Description|
|---|---|
|```RawDevice```|The volume is a raw physical device without any RAID or other virtualization applied|


### Base.1.0.AccessDenied
While attempting to access, connect to, or transfer to/from another resource, the service was denied access.

| | |
|:---|:---|
|Message Format|"While attempting to establish a connection to %1, the service was denied access."
|Severity|Critical
|Resolution|Verify that the URI is correct and that the service has the appropriate credentials.

### Base.1.0.AccountForSessionNoLongerExists
The account for current session is removed and the current session is also removed.

| | |
|:---|:---|
|Message Format|"The account for the session is removed and the current session is also removed."
|Severity|OK
|Resolution|Attempt to connect using a valid account.

### Base.1.0.AccountModified
The account was modified successfully.

| | |
|:---|:---|
|Message Format|"The account was modified successfully."
|Severity|OK
|Resolution|None.

### Base.1.0.AccountNotModified
The request was unable to modify the account.

| | |
|:---|:---|
|Message Format|"The account modification request did not complete."
|Severity|Warning
|Resolution|If the operation did not complete, check the authorization or the request body for issues and resubmit the request.

### Base.1.0.AccountRemoved
The account was removed successfully.

| | |
|:---|:---|
|Message Format|"The account was removed successfully."
|Severity|OK
|Resolution|None.

### Base.1.0.ActionNotSupported
The action supplied in the POST operation is not supported by the resource.

| | |
|:---|:---|
|Message Format|"The action %1 is not supported by the resource."
|Severity|Critical
|Resolution|The action was invalid or the wrong resource was the target. See the implementation documentation for assistance.

### Base.1.0.ActionParameterDuplicate
The action was submitted with a duplicate parameter in the request body.

| | |
|:---|:---|
|Message Format|"The action %1 was submitted with more than one value for the parameter %2."
|Severity|Warning
|Resolution|Resubmit the action with only one instance of the parameter in the request body.

### Base.1.0.ActionParameterMissing
The requested action is missing a parameter that is required to process the action.

| | |
|:---|:---|
|Message Format|"The action %1 requires that the parameter %2 be present in the request body."
|Severity|Critical
|Resolution|Resubmit the action with the required parameter in the request body.

### Base.1.0.ActionParameterNotSupported
The action parameter is not supported on the target resource.

| | |
|:---|:---|
|Message Format|"The parameter %1 for the action %2 is not supported on the target resource."
|Severity|Warning
|Resolution|If the operation did not complete, remove the parameter and resubmit the request.

### Base.1.0.ActionParameterUnknown
An action was submitted, but a supplied parameter did not match any of the known parameters.

| | |
|:---|:---|
|Message Format|"The action %1 was submitted with the invalid parameter %2."
|Severity|Warning
|Resolution|If the operation did not complete, correct the invalid parameter and resubmit the request.

### Base.1.0.ActionParameterValueFormatError
The value type is correct, but the format is not supported or the size/length is exceeded

| | |
|:---|:---|
|Message Format|"The value %1 for the parameter %2 in the action %3 is in a format that is not supported by the parameter."
|Severity|Warning
|Resolution|If the operation did not complete, correct the parameter value in the request body and resubmit the request.

### Base.1.0.ActionParameterValueTypeError
The parameter contains an incorrect value type. For example, a number value for a string parameter type.

| | |
|:---|:---|
|Message Format|"The value %1 for the parameter %2 in the action %3 is the incorrect parameter type."
|Severity|Warning
|Resolution|If the operation did not complete, correct the parameter value in the request body and resubmit the request.

### Base.1.0.CouldNotEstablishConnection
An attempt to access the resource, image, or file at the URI was unsuccessful because a session could not be established.

| | |
|:---|:---|
|Message Format|"The service was unable to establish a connection with the URI %1."
|Severity|Critical
|Resolution|Verify that the URI contains a valid and reachable node name, protocol information, and other URI components.

### Base.1.0.CreateFailedMissingReqProperties
A create operation was attempted on a resource, but a required property was missing from the request.

| | |
|:---|:---|
|Message Format|"The create operation did not complete because the required property %1 was missing from the request."
|Severity|Critical
|Resolution|If the operation did not complete, include the required property with a valid value in the request body and resubmit the request.

### Base.1.0.CreateLimitReachedForResource
No more resources can be created.

| | |
|:---|:---|
|Message Format|"No more resources can be created."
|Severity|Critical
|Resolution|If the operation did not complete, delete resources and resubmit the request.

### Base.1.0.Created
The resource has been created successfully.

| | |
|:---|:---|
|Message Format|"The resource has been created successfully."
|Severity|OK
|Resolution|None

### Base.1.0.EventSubscriptionLimitExceeded
The event subscription establishment has been requested, but the operation did not complete because the number of simultaneous subscriptions exceeded the maximum number allowed by the implementation.

| | |
|:---|:---|
|Message Format|"The event subscription did not complete because the number of simultaneous subscriptions exceeded the maximum number allowed by the implementation."
|Severity|Critical
|Resolution|Before attempting to establish the event subscription, reduce the number of subscriptions or increase the maximum number of simultaneous subscriptions allowed (if supported).

### Base.1.0.InsufficientPrivilege
The account or credentials associated with the current session are not authorized to perform the requested operation.

| | |
|:---|:---|
|Message Format|"The account or credentials associated with the current session are not authorized to perform the requested operation."
|Severity|Critical
|Resolution|Retry the operation with an authorized account or credentials.

### Base.1.0.InternalError
The request did not complete due to an unknown internal error, but the service is still operational.

| | |
|:---|:---|
|Message Format|"The request failed due to an internal service error, but the service is still operational."
|Severity|Critical
|Resolution|Resubmit the request. If the problem persists, consider resetting the service.

### Base.1.0.InvalidObject
The object is not valid.

| | |
|:---|:---|
|Message Format|"The object at %1 is not valid."
|Severity|Critical
|Resolution|If the operation did not complete, the object is malformed or the URI is incorrect. Make the appropriate corrections and resubmit the request.

### Base.1.0.MalformedJSON
The request body contains malformed JSON.

| | |
|:---|:---|
|Message Format|"The request body submitted is malformed JSON and cannot be parsed by the receiving service."
|Severity|Critical
|Resolution|Verify that the request body is valid JSON and resubmit the request.

### Base.1.0.NoValidSession
The operation did not complete because a valid session is required in order to access resources.

| | |
|:---|:---|
|Message Format|"There is no valid session established with the implementation."
|Severity|Critical
|Resolution|Establish a session before attempting any operations.

### Base.1.0.PropertyDuplicate
A duplicate property is in the request body.

| | |
|:---|:---|
|Message Format|"The property %1 is duplicated in the request."
|Severity|Warning
|Resolution|If the operation did not complete, remove the duplicate property from the request body and resubmit the request.

### Base.1.0.PropertyMissing
The request does not include a required property.

| | |
|:---|:---|
|Message Format|"The property %1 is a required property and must be included in the request."
|Severity|Warning
|Resolution|If the operation did not complete, verify the property is in the request body and has a valid value.

### Base.1.0.PropertyNotWritable
The request included a value for a read-only property.

| | |
|:---|:---|
|Message Format|"The property %1 is a read-only property and cannot be assigned a value."
|Severity|Warning
|Resolution|If the operation did not complete, remove the property from the request body and resubmit the request.

### Base.1.0.PropertyUnknown
An unknown property is in the request body.

| | |
|:---|:---|
|Message Format|"The property %1 is not valid for this resource."
|Severity|Warning
|Resolution|If the operation did not complete, remove the unknown property from the request body and resubmit the request.

### Base.1.0.PropertyValueFormatError
The value type is correct, but the format is not supported or the size/length is exceeded.

| | |
|:---|:---|
|Message Format|"The value %1 for the property %2 is in a format that is not supported by the property."
|Severity|Warning
|Resolution|If the operation did not complete, correct the property value in the request body and resubmit the request.

### Base.1.0.PropertyValueNotInList
The value type is correct, but the value is not supported.

| | |
|:---|:---|
|Message Format|"The value %1 for the property %2 is not valid."
|Severity|Warning
|Resolution|If the operation did not complete, choose a value from the enumeration list and resubmit your request.

### Base.1.0.PropertyValueTypeError
The property value contains an incorrect property type. For example, a number value for a string property type.

| | |
|:---|:---|
|Message Format|"The value %1 for the property %2 is the incorrect property type."
|Severity|Warning
|Resolution|If the operation did not complete, correct the property value in the request body and resubmit the request.

### Base.1.0.QueryNotSupported
The query is not supported by the implementation.

| | |
|:---|:---|
|Message Format|"Querying is not supported by the implementation."
|Severity|Warning
|Resolution|If the operation did not complete, remove the query parameter and resubmit the request.

### Base.1.0.QueryNotSupportedOnResource
The query is not supported on the resource. For example, a start/count query is attempted on a resource that is not a collection.

| | |
|:---|:---|
|Message Format|"Querying is not supported on the requested resource."
|Severity|Warning
|Resolution|If the operation did not complete, remove the query parameters and resubmit the request.

### Base.1.0.QueryParameterOutOfRange
The query parameter value is out of range for the resource. For example, a page is requested that is outside the valid page range.

| | |
|:---|:---|
|Message Format|"The value %1 for the query parameter %2 is out of range %3."
|Severity|Warning
|Resolution|Specify a query parameter value that is within range. For example, a page that is within the valid range of pages.

### Base.1.0.QueryParameterValueFormatError
The value type is correct, but the format is not supported or the size/length was exceeded.

| | |
|:---|:---|
|Message Format|"The value %1 for the parameter %2 is in a format that is not supported by the parameter."
|Severity|Warning
|Resolution|If the operation did not complete, correct the value for the query parameter in the request body and resubmit the request.

### Base.1.0.QueryParameterValueTypeError
The query parameter contains an incorrect value type. For example, a number supplied for a query parameter that requires a string.

| | |
|:---|:---|
|Message Format|"The value %1 for the query parameter %2 is the incorrect type of value for the query parameter."
|Severity|Warning
|Resolution|If the operation did not complete, correct the value for the query parameter in the request body and resubmit the request.

### Base.1.0.ResourceAlreadyExists
The create resource operation did not complete because the resource already exists.

| | |
|:---|:---|
|Message Format|"The requested resource already exists."
|Severity|Critical
|Resolution|Do not attempt the create operation because the resource already exists.

### Base.1.0.ResourceAtUriInUnknownFormat
The URI is valid, but the resource or image at that URI is in a format that is not supported by the service.

| | |
|:---|:---|
|Message Format|"The resource at %1 is in a format that is not supported by the service."
|Severity|Critical
|Resolution|Place a resource, image, or file that is supported by the service at the URI.

### Base.1.0.ResourceAtUriUnauthorized
An attempt to access the resource, image, or file at the URI is unauthorized.

| | |
|:---|:---|
|Message Format|"While accessing the resource at %1, the service received an authorization error %2."
|Severity|Critical
|Resolution|Verify that the appropriate access is provided for the service to access the URI.

### Base.1.0.ResourceCannotBeDeleted
A delete operation was attempted on a resource that cannot be deleted.

| | |
|:---|:---|
|Message Format|"The delete request did not complete because the resource cannot be deleted."
|Severity|Critical
|Resolution|Do not attempt to delete a resource that does not support the REST API DELETE operation.

### Base.1.0.ResourceInStandby
Indicates that the request could not be performed because the resource is in standby.

| | |
|:---|:---|
|Message Format|"The request could not be performed because the resource is in standby."
|Severity|Critical
|Resolution|Ensure that the resource is in the correct power state and resubmit the request.

### Base.1.0.ResourceInUse
The request to change the resource was rejected because the resource was in use or in transition.

| | |
|:---|:---|
|Message Format|"The change to the resource did not complete because the resource is in use or in transition."
|Severity|Warning
|Resolution|If the operation did not complete, wait until the resource is free and resubmit the request.

### Base.1.0.ResourceMissingAtURI
The operation expected an image or resource at the provided URI, but found none.

| | |
|:---|:---|
|Message Format|"The resource at the URI %1 was not found."
|Severity|Critical
|Resolution|Place a valid resource at the URI or correct the URI and resubmit the request.

### Base.1.0.ServiceInUnknownState
The operation did not complete because the service is in an unknown state and cannot take incoming requests.

| | |
|:---|:---|
|Message Format|"The operation did not complete because the service is in an unknown state and cannot take incoming requests."
|Severity|Critical
|Resolution|If the operation did not complete, restart the service and resubmit the request.

### Base.1.0.ServiceShuttingDown
The operation did not complete because the service is shutting down.

| | |
|:---|:---|
|Message Format|"The operation did not complete because the service is shutting down and cannot take incoming requests."
|Severity|Critical
|Resolution|If the operation did not complete, resubmit the request when the service is available.

### Base.1.0.ServiceTemporarilyUnavailable
The service is temporarily unavailable.

| | |
|:---|:---|
|Message Format|"The service is temporarily unavailable.  Retry in %1 seconds."
|Severity|Critical
|Resolution|Wait for the indicated retry duration and retry the operation.

### Base.1.0.SessionLimitExceeded
Session establishment has been requested, but the operation did not complete because the number of simultaneous sessions exceeded the maximum number allowed by the implementation.

| | |
|:---|:---|
|Message Format|"The session establishment did not complete because the number of simultaneous sessions exceeded the maximum number allowed by the implementation."
|Severity|Critical
|Resolution|Before attempting to establish the session, reduce the number of sessions or increase the maximum number of simultaneous sessions allowed (if supported).

### Base.1.0.SourceDoesNotSupportProtocol
While attempting to access, connect to, or transfer from another location, the other end of the connection did not support the specified protocol.

| | |
|:---|:---|
|Message Format|"The other end of the connection at %1 does not support the specified protocol %2."
|Severity|Critical
|Resolution|Change protocols or URIs. 

### Base.1.0.Success
The operation completed successfully.

| | |
|:---|:---|
|Message Format|"The operation completed successfully."
|Severity|OK
|Resolution|None

### Base.1.0.UnrecognizedRequestBody
The service detected a request body with malformed JSON.

| | |
|:---|:---|
|Message Format|"The service detected a request body with malformed JSON."
|Severity|Warning
|Resolution|If the operation did not complete, correct the request body and resubmit the request.

### HpeBiosMessageRegistry.1.0.MessagesMaxSizeExceeded
Indicates that the last configuration change attempted by the user resulted in a number of error messages that exceeded the maximum storage capacity alloted for messages corresponding to this resource.

| | |
|:---|:---|
|Message Format|"The messages array has been truncated because the last configuration change resulted in too many error messages."
|Severity|Warning
|Resolution|Inspect the last configuration change request for issues that may be generating errors, compare the request against the resource's schema, then retry the configuration change.

### HpeBiosMessageRegistry.1.0.UnsupportedAMPConfiguration
Indicates that the user provided Advanced Memory Protection (AMP) option is not appropriate for this memory configuration, as the underlying hardware does not support it.

| | |
|:---|:---|
|Message Format|"Underlying hardware does not support the requested AMP configuration, the settings are invalid."
|Severity|Warning
|Resolution|Ensure that the current memory configuration meets the requirements of the requested value before applying the settings.

### HpeBiosMessageRegistry.1.0.UnsupportedDramRaplValue
Indicates that the user provided Running Average Power Limit (RAPL) value could not be applied due to inherent DRAM power limitation. The value may be out of bounds or invalid.

| | |
|:---|:---|
|Message Format|"Underlying DRAM does not support the requested value."
|Severity|Warning
|Resolution|Ensure that the requested value is within the supported bounds before applying the settings.

### HpeBiosMessageRegistry.1.0.UnsupportedProcessorRaplValue
Indicates that the user provided Running Average Power Limit (RAPL) value could not be applied due to inherent processor power limitation. The value may be out of bounds or invalid.

| | |
|:---|:---|
|Message Format|"Underlying processor does not support the requested value."
|Severity|Warning
|Resolution|Ensure that the processor supports the requested value and that it is within the supported bounds before applying the settings.

### HpeCommon.2.0.ArrayPropertyOutOfBound
The items in the array exceed the maximum  number supported.

| | |
|:---|:---|
|Message Format|"An array %1 was supplied with %2 items that exceeds the maximum supported count of %3."
|Severity|Warning
|Resolution|Retry the operation using the correct number of items for the array.

### HpeCommon.2.0.ConditionalSuccess
A property value was successfully changed but the change may be reverted upon system reset.

| | |
|:---|:---|
|Message Format|"The property %1 was successfully changed to %2, but the change may be reverted upon system reset."
|Severity|Warning
|Resolution|Check the "SettingsResult" messages after the system has reset for errors referring to the corresponding property.

### HpeCommon.2.0.InternalErrorWithParam
The operation was not successful due to an internal service error (shown), but the service is still operational.

| | |
|:---|:---|
|Message Format|"The operation was not successful due to an internal service error (%1), but the service is still operational."
|Severity|Critical
|Resolution|Retry the operation. If the problem persists, consider resetting the service.

### HpeCommon.2.0.InvalidConfigurationSpecified
The specified configuration is not valid.

| | |
|:---|:---|
|Message Format|"The specified configuration is not valid."
|Severity|Warning
|Resolution|Correct the configuration, and then retry the operation.

### HpeCommon.2.0.PropertyValueExceedsMaxLength
The value for the property exceeds the maximum length.

| | |
|:---|:---|
|Message Format|"The value %1 for the property %2 exceeds the maximum length of %3."
|Severity|Warning
|Resolution|Correct the value for the property in the request body, and then retry the operation.

### HpeCommon.2.0.PropertyValueIncompatible
The value for the property is the correct type, but this value is incompatible with the current value of another property.

| | |
|:---|:---|
|Message Format|"The value %1 for the property %2 is incompatible with the value for property %3."
|Severity|Warning
|Resolution|Correct the value for the property in the request body, and then retry the operation.

### HpeCommon.2.0.PropertyValueOutOfRange
The value for the property is out of range.

| | |
|:---|:---|
|Message Format|"The value %1 for the property %2 is out of range %3."
|Severity|Warning
|Resolution|Correct the value for the property in the request body, and then retry the operation.

### HpeCommon.2.0.ResetInProgress
A device or service reset is in progress.

| | |
|:---|:---|
|Message Format|"A reset on %1 is in progress."
|Severity|Warning
|Resolution|Wait for device or service reset to complete, and then retry the operation.

### HpeCommon.2.0.ResetRequired
One or more properties were changed, but these changes will not take effect until the device or service is reset.

| | |
|:---|:---|
|Message Format|"One or more properties were changed, but these changes will not take effect until %1 is reset."
|Severity|Warning
|Resolution|To enable the changed properties, reset the device or service.

### HpeCommon.2.0.ResourceNotReadyRetry
The resource is present but is not ready to perform operations due to an internal condition such as initialization or reset.

| | |
|:---|:---|
|Message Format|"The resource is present but is not ready to perform operations.  The resource will be ready in %1 seconds."
|Severity|Warning
|Resolution|Retry the operation when the resource is ready.

### HpeCommon.2.0.SuccessFeedback
The operation completed successfully

| | |
|:---|:---|
|Message Format|"The operation completed successfully"
|Severity|OK
|Resolution|None

### HpeCommon.2.0.TaskCreated
A task was created in response to the operation.

| | |
|:---|:---|
|Message Format|"A task was created in response to the operation and is accessible at %1."
|Severity|OK
|Resolution|Perform an HTTP GET request on the supplied URI for task status.

### HpeCommon.2.0.UnsupportedHwConfiguration
A previously requested property value change was reverted because the current hardware configuration does not support it.

| | |
|:---|:---|
|Message Format|"The value %1 for property %2 was reverted because the current hardware configuration does not support it."
|Severity|Warning
|Resolution|Ensure that the system's hardware configuration supports the property value.

### iLO.2.2.AHSDisabled
Modifying AHS properties is not possible with AHS disabled.

| | |
|:---|:---|
|Message Format|"Modifying AHS properties is not possible with AHS disabled."
|Severity|Warning
|Resolution|Enable AHS, and then modify the AHS properties.

### iLO.2.2.Accepted
Indicates that one or more properties were correctly changed, but may not be in effect yet.

| | |
|:---|:---|
|Message Format|"Indicates that one or more properties were correctly changed, but may not be in effect yet."
|Severity|OK
|Resolution|None

### iLO.2.2.ActionParameterValueNotInList
Indicates that the correct value type was supplied for the action parameter, but the value is not supported. (The value is not in the enumeration list.)

| | |
|:---|:---|
|Message Format|"The value %1 for the property %2 is not in the list of valid values."
|Severity|Warning
|Resolution|Choose a value from the enumeration list and resubmit the request if the operation failed.

### iLO.2.2.AlertDestinationAssociationError
AlertDestination cannot be configured with both SNMPv1 and SNMPv3.

| | |
|:---|:---|
|Message Format|"AlertDestination cannot be configured with both SNMPv1 and SNMPv3."
|Severity|Warning
|Resolution|For SNMPv1 alert, configure SNMPAlertProtocol to SNMPv1. For SNMPv3 alert, configure SNMPAlertProtocol to SNMPv3.

### iLO.2.2.AlertMailFeatureDisabled
AlertMail feature is disabled.

| | |
|:---|:---|
|Message Format|"AlertMail feature is disabled."
|Severity|Warning
|Resolution|Enable AlertMail feature to send test alert message.

### iLO.2.2.AlreadyInProgress
An operation is already in progress.

| | |
|:---|:---|
|Message Format|"An operation is already in progress."
|Severity|Warning
|Resolution|Wait for the current operation to complete, and then retry the operation.

### iLO.2.2.AlreadyUpToDate


| | |
|:---|:---|
|Message Format|"The update did not occur because the component was already up to date."
|Severity|Warning
|Resolution|None.

### iLO.2.2.ApmPowerCapModeInUsed
Operation is currently unavailable because the power regulator is set to APM Power Capping Mode.

| | |
|:---|:---|
|Message Format|"Operation is currently unavailable because the power regulator is set to APM Power Capping Mode."
|Severity|Warning
|Resolution|Change the power regulator to other modes rather than APM Power Capping Mode through APM interface.

### iLO.2.2.ArrayPropertyAlreadyExists
Duplicate value.

| | |
|:---|:---|
|Message Format|"The property value %1 is already exists in index %2"
|Severity|Warning
|Resolution|If the operation did not complete, correct the property value in the request body and resubmit the request.

### iLO.2.2.ArrayPropertyOutOfBound
The number of items in the array exceeds the maximum number supported.

| | |
|:---|:---|
|Message Format|"An array %1 was supplied with %2 items that exceeds the maximum supported count of %3."
|Severity|Warning
|Resolution|Retry the operation using the correct number of items for the array.

### iLO.2.2.ArrayPropertyValueBadParam
The property value is not valid.

| | |
|:---|:---|
|Message Format|"The property value %1 in index %2 is not valid."
|Severity|Warning
|Resolution|Retry the operation using a corrected value.

### iLO.2.2.BatteryBackupUnitSettingsDisabled
Battery Backup Unit settings are currently disabled.

| | |
|:---|:---|
|Message Format|"Battery Backup Unit settings are disabled when the system is configured for Scalable Persistent Memory."
|Severity|Warning
|Resolution|To re-enable Battery Backup Unit settings, disable Scalable Persistent Memory functionality in the system ROM RBSU.

### iLO.2.2.BiosActionTBD
The BIOS action supplied in the POST operation is not yet implemented.

| | |
|:---|:---|
|Message Format|"The BIOS action %1 is not implemented yet."
|Severity|Critical
|Resolution|The action was invalid or the wrong resource was the target. See the implementation documentation for assistance.

### iLO.2.2.BiosPasswordInfoInvalid
The stored BIOS password information is invalid. A system reboot is neccessary to retore password defaults.

| | |
|:---|:---|
|Message Format|"The stored BIOS password information is invalid.  Reboot system."
|Severity|Critical
|Resolution|The system will need to be rebooted to restore BIOS password information to defaults.

### iLO.2.2.BiosPasswordMismatch
The provided OldPassword does not match the stored BIOS password.

| | |
|:---|:---|
|Message Format|"The provided OldPassword does not match the stored BIOS password."
|Severity|Critical
|Resolution|Retry the action with the matching password.

### iLO.2.2.CalibrateInProgress
Power calibrate is in progress.

| | |
|:---|:---|
|Message Format|"Power calibrate is in progress."
|Severity|Warning
|Resolution|Wait for previous power calibrate complete or stop previous power calibrate, and then retry the operation.

### iLO.2.2.CannotRemoveLanguagePack
Cannot remove language pack.

| | |
|:---|:---|
|Message Format|"Cannot remove %1 language pack."
|Severity|Warning
|Resolution|None.

### iLO.2.2.CannotRemoveLicense
Cannot remove the base license.

| | |
|:---|:---|
|Message Format|"The base license cannot be removed."
|Severity|Warning
|Resolution|None.

### iLO.2.2.ChassisPowerDataUnAvailable
Chassis power regulation data is currently unavailable.

| | |
|:---|:---|
|Message Format|"Chassis power regulation data is currently unavailable."
|Severity|Warning
|Resolution|Reset the management processor or chassis manager, and then retry the operation.

### iLO.2.2.ChassisResetRequired
The chassis properties were correctly changed, but will not take effect until the chassis is reset or all nodes in chassis remain powered off for at least 5 seconds.

| | |
|:---|:---|
|Message Format|"One or more properties were changed and will not take effect until chassis is reset or all nodes in chassis remain powered off for at least 5 seconds."
|Severity|Warning
|Resolution|Reset chassis or remain power off for all nodes in chassis for at least 5 seconds for the settings to take effect.

### iLO.2.2.ComponentUploadAlreadyInProgress
A component upload operation is already in progress.

| | |
|:---|:---|
|Message Format|"A component upload operation is already in progress."
|Severity|Warning
|Resolution|Wait for the current component upload to complete, and then retry the operation.

### iLO.2.2.ComponentUploadFailed
A component upload operation failed.

| | |
|:---|:---|
|Message Format|"A component upload operation failed."
|Severity|Warning
|Resolution|Wait for the current component upload to complete, and then retry the operation.

### iLO.2.2.DemoLicenseKeyPreviouslyInstalled
A license was previously activated and now a demo key may not be used.

| | |
|:---|:---|
|Message Format|"A license was previously activated."
|Severity|Warning
|Resolution|The system is no longer eligible for demo licenses.

### iLO.2.2.DeviceIsBusy
Device was not available for communication.

| | |
|:---|:---|
|Message Format|"Device communication response was busy."
|Severity|Warning
|Resolution|Retry the attempted operation after a delay.

### iLO.2.2.DeviceResetRequired
Indicates that one or more properties were correctly changed, but will not take effect until device is reset.

| | |
|:---|:---|
|Message Format|"One or more properties were changed and will not take effect until the device is reset."
|Severity|Warning
|Resolution|Reset the device for the settings to take effect.

### iLO.2.2.DiagsTestAlreadyRunning
A diagnostics self test is already running.

| | |
|:---|:---|
|Message Format|"A diagnostics self test is already running."
|Severity|Warning
|Resolution|Stop the running test and try again.

### iLO.2.2.ESKMServersNotConfigured
Enterprise Secure Key Manager Servers are not configured.

| | |
|:---|:---|
|Message Format|"Enterprise Secure Key Manager Servers are not configured."
|Severity|OK
|Resolution|None.

### iLO.2.2.ETagTooLong
The supplied ETag is too long. The maximum supported ETag length is 63 bytes.

| | |
|:---|:---|
|Message Format|"The supplied ETag is too long. The maximum supported ETag length is 63 bytes."
|Severity|Warning
|Resolution|Retry the operation using an ETag with a length of 63 bytes or less.

### iLO.2.2.EmptyDNSName
DNS name is empty.

| | |
|:---|:---|
|Message Format|"Empty DNS name."
|Severity|Warning
|Resolution|Retry the request with a valid DNS name.

### iLO.2.2.ErrorIntializingESKM
Failed to initialize ESKM.

| | |
|:---|:---|
|Message Format|"Failed to initialize ESKM."
|Severity|Warning
|Resolution|Check if Account Group, Local CA Certificate Name, Login Name and Password are correct and try again.

### iLO.2.2.EventLogCleared
Event log cleared successfully.

| | |
|:---|:---|
|Message Format|"Event log cleared successfully."
|Severity|OK
|Resolution|None.

### iLO.2.2.EventSubscriptionModified
The event subscription was modified successfully.

| | |
|:---|:---|
|Message Format|"The event subscription was modified successfully."
|Severity|OK
|Resolution|None.

### iLO.2.2.EventSubscriptionRemoved
The event subscription was removed successfully.

| | |
|:---|:---|
|Message Format|"The event subscription was removed successfully."
|Severity|OK
|Resolution|None.

### iLO.2.2.ExtendedInfo
Indicates that extended information is available.

| | |
|:---|:---|
|Message Format|"See @Message.ExtendedInfo for more information."
|Severity|OK
|Resolution|See @Message.ExtendedInfo for more information.

### iLO.2.2.FWFlashSuccessTPMOverrideEnabled
A Trusted Module is  detected in this system. If you have not performed the proper OS encryption procedures, you will lose access to your data if recovery key is not available. Recommended procedure is to suspend encryption software prior to System ROM or Option ROM firmware flash. TPMOverrideFlag is enabled and firmware flash initiated.

| | |
|:---|:---|
|Message Format|"CAUTION: A Trusted Module is detected in this system. Updating the System ROM or Option Card Firmware may have impact to measurements stored in the TM and may have impact to security functionality on the platform which depends on these measurements."
|Severity|OK
|Resolution|None.

### iLO.2.2.FWFlashSuccessTrustedModuleOverrideEnabled
A Trusted Module (type unspecified) is installed in the system and TPMOverrideFlag is enabled. Firmware flash initiated.

| | |
|:---|:---|
|Message Format|"CAUTION: A Trusted Module (type unspecified) has been detected in this system. If you have not performed the proper OS encryption procedures, you will lose access to your data if recovery key is not available. Recommended procedure for Microsoft Windows(R) BitLocker(TM) is to "suspend" BitLocker prior to System ROM or Option ROM firmware flash."
|Severity|OK
|Resolution|None.

### iLO.2.2.FWFlashTPMOverrideFlagRequired
A Trusted Module is  detected in this system. Failure to perform proper OS encryption procedures will result in loss of access to your data if recovery key is not available. Recommended procedure is to suspend encryption software prior to System ROM or Option ROM firmware flash. If you do not have your recovery key or have not suspended encryption software, cancel this firmware upload. Failure to follow these instructions will result in loss of access to your data. To continue with firmware flash TPMOverrideFlag is required.

| | |
|:---|:---|
|Message Format|"CAUTION: A Trusted Module is detected in this system. Updating the System ROM or Option Card Firmware may have impact to measurements stored in the TM and may have impact to security functionality on the platform which depends on these measurements."
|Severity|Warning
|Resolution|Please set the TPMOverrideFlag to true and try again.

### iLO.2.2.FWFlashTrustedModuleOverrideFlagRequired
A Trusted Module (type unspecified) is installed in the system, TPMOverrideFlag is required for firmware flash to proceed.

| | |
|:---|:---|
|Message Format|"CAUTION: A Trusted Module (type unspecified) has been detected in this system. Failure to perform proper OS encryption procedures will result in loss of access to your data if recovery key is not available. Recommended procedure for Microsoft Windows(R) BitLocker(TM) is to "suspend" BitLocker prior to System ROM or Option ROM firmware flash. If you do not have your recovery key or have not suspended BitLocker, exit this flash: Failure to follow these instructions will result in loss of access to your data."
|Severity|Warning
|Resolution|Please set the TPMOverrideFlag to true and try again.

### iLO.2.2.FirmwareFlashAlreadyInProgress
A firmware upgrade operation is already in progress.

| | |
|:---|:---|
|Message Format|"A firmware flash operation is already in progress."
|Severity|Warning
|Resolution|Wait for the current firmware flash to complete, and then retry the operation.

### iLO.2.2.GeneratingCertificate
Generating the X509 Certificate.

| | |
|:---|:---|
|Message Format|"X509 Certificate is being generated and the process might take up to 10 minutes."
|Severity|OK
|Resolution|None.

### iLO.2.2.HardDriveZoneFailure
Hard Drive Zoning was in error state.

| | |
|:---|:---|
|Message Format|"Hard Drive Zoning was in error state due to %1."
|Severity|Critical
|Resolution|Retry the operation. If the problem persists, consider resetting the entire chassis.

### iLO.2.2.ICRUInvalidAddress
ICRU returned invalid address for translation.

| | |
|:---|:---|
|Message Format|"ICRU returned invalid address for translation."
|Severity|Warning
|Resolution|Input valid address for translation.

### iLO.2.2.ICRUNotSupported
ICRU feature or function is not supported on the system.

| | |
|:---|:---|
|Message Format|"ICRU feature or function is not supported on the system."
|Severity|Warning
|Resolution|None.

### iLO.2.2.IPv6ConfigurationError
The specified IPv6 configuration caused an error.

| | |
|:---|:---|
|Message Format|"The specified IPv6 configuration was in error due to %1."
|Severity|Warning
|Resolution|Resolve the indicated error in the configuration data.

### iLO.2.2.ImportCertSuccessful
Import Certificate was successful.

| | |
|:---|:---|
|Message Format|"Import Certificate was successful."
|Severity|OK
|Resolution|None.

### iLO.2.2.ImportCertSuccessfuliLOResetinProgress
Import Certificate was successful and the management processor is being reset.

| | |
|:---|:---|
|Message Format|"Import Certificate was successful. Management Processor reset is in progress to enable the new certificate."
|Severity|Warning
|Resolution|None.

### iLO.2.2.ImportCertificateFailed
Failed importing Certificate.

| | |
|:---|:---|
|Message Format|"Failed importing the X509 Certificate."
|Severity|Warning
|Resolution|Retry the operation with proper Certificate information.

### iLO.2.2.ImportSSOParamError
Not a valid parameter.

| | |
|:---|:---|
|Message Format|"Invalid Parameter."
|Severity|Warning
|Resolution|Retry the request with valid parameters.

### iLO.2.2.ImportSSOUriError
Not a valid Uri to import SSO certificate.

| | |
|:---|:---|
|Message Format|"Invalid Uri."
|Severity|Warning
|Resolution|Retry the request with valid URI.

### iLO.2.2.IndicatorLedInvalidStateChange
The request to change the state of the Indicator LED cannot be granted because the current state is either Blinking or is Unknown.

| | |
|:---|:---|
|Message Format|"The Indicator LED cannot be changed when its state is Blinking or Unknown."
|Severity|Warning
|Resolution|Please wait until the server has completed its reserved state.

### iLO.2.2.InstallSetWriteError
The InstallSet write failed.

| | |
|:---|:---|
|Message Format|"The InstallSet write of %1 failed."
|Severity|Warning
|Resolution|Ensure a valid name for the item and that space exists to hold the item.

### iLO.2.2.InterfaceDisabledResetRequired
Disabling one or more interfaces/features will cause certain functionalities to be not available. Please refer to User Guide for details on the implications. Changes will not take effect until the management processor is reset

| | |
|:---|:---|
|Message Format|"CAUTION: Disabling one or more interfaces/features will cause certain functionalities to be not available. Please refer to User Guide for details on the implications. Changes will not take effect until the management processor is reset"
|Severity|OK
|Resolution|None.

### iLO.2.2.InternalErrorWithParam
The operation was not successful due to an internal service error (shown), but the service is still operational.

| | |
|:---|:---|
|Message Format|"The operation was not successful due to an internal service error (%1), but the service is still operational."
|Severity|Critical
|Resolution|Retry the operation. If the problem persists, consider resetting the service.

### iLO.2.2.InvalidConfigurationSpecified
The specified configuration is not valid.

| | |
|:---|:---|
|Message Format|"The specified configuration is not valid."
|Severity|Warning
|Resolution|Correct the configuration, and then retry the operation.

### iLO.2.2.InvalidConfigurationSpecifiedForFederation
iLO Federation Management cannot be supported in the current configuration.

| | |
|:---|:---|
|Message Format|"iLO Federation Management cannot be supported in the current configuration."
|Severity|Warning
|Resolution|Review the management processor network settings or Onboard Administrator settings and refer to the User Guide.

### iLO.2.2.InvalidEngineID
EngineID should be a hexadecimal number starting with 0x (for example, 0x0102030405abcdef). The string length should be an even number, greater than or equal to 6 characters (excluding the "0x"), and less than or equal to 32 characters.

| | |
|:---|:---|
|Message Format|"EngineID should be a hexadecimal number starting with 0x (for example, 0x0102030405abcdef). The string length should be an even number, greater than or equal to 6 characters (excluding the "0x"), and less than or equal to 32 characters."
|Severity|Warning
|Resolution|Retry the operation using an EngineID within the specified parameters.

### iLO.2.2.InvalidIndex
The Index is not valid.

| | |
|:---|:---|
|Message Format|"The Index provided is not valid."
|Severity|Warning
|Resolution|Adhere to the indexes supported in the self links.

### iLO.2.2.InvalidLicenseKey
The license key is not valid.

| | |
|:---|:---|
|Message Format|"The license key is not valid."
|Severity|Warning
|Resolution|Retry the operation using a valid license key.

### iLO.2.2.InvalidOperationForAutoPowerOnState
The operation was not successful because the current auto power on mode specifies power is to remain off.

| | |
|:---|:---|
|Message Format|"The auto power on delay cannot be set because power is configured to remain off."
|Severity|Warning
|Resolution|Verify that the system auto power on mode is set to turn power on or follow the previous power setting.

### iLO.2.2.InvalidOperationForSystemState
The operation was not successful due to the current power state (for example, attempting to turn the power off when it is already off).

| | |
|:---|:---|
|Message Format|"The operation was not successful due to the current power state."
|Severity|Warning
|Resolution|Verify that the system is in the correct power state, and then retry the operation.

### iLO.2.2.InvalidPassphraseLength
The passphrase must contain 8 to 49 characters.

| | |
|:---|:---|
|Message Format|"%1 must contain 8 to 49 characters."
|Severity|Warning
|Resolution|Correct the passphrase, and then retry the operation.

### iLO.2.2.InvalidPasswordLength
The password length is not valid.

| | |
|:---|:---|
|Message Format|"A valid password must contain between %1 to %2 characters."
|Severity|Critical
|Resolution|Retry the operation using a corrected password.

### iLO.2.2.LicenseKeyDenied
The license key activation was refused.  Includes details.

| | |
|:---|:---|
|Message Format|"The license activation key cannot be installed.  %1"
|Severity|Warning
|Resolution|Address the condition or use a valid license activation key.

### iLO.2.2.LicenseKeyNotSupported
The license key supplied is unsupported on this system.  The key may activate a different product or unsupported tier.

| | |
|:---|:---|
|Message Format|"The supplied license key is not supported on this system."
|Severity|Warning
|Resolution|None.

### iLO.2.2.LicenseKeyRequired
A license key is required to use this operation or feature.

| | |
|:---|:---|
|Message Format|"A license key is required to use this operation or feature."
|Severity|Warning
|Resolution|Install a license key to use this feature.

### iLO.2.2.LoginAttemptDelayed
The login was not successful, so the service enforces a delay before another login is allowed.

| | |
|:---|:---|
|Message Format|"The login was not successful, so the service enforces a delay before another login is allowed."
|Severity|Warning
|Resolution|Wait for the delay time to expire, and then retry the login.

### iLO.2.2.LoginAttemptDelayedSeconds
The login was not successful, so the service enforces a delay before another login is allowed.

| | |
|:---|:---|
|Message Format|"The login was not successful, so the service enforces a %1 second delay before another login is allowed."
|Severity|Warning
|Resolution|None.

### iLO.2.2.MaxProviders
The maximum number of providers are already registered.

| | |
|:---|:---|
|Message Format|"The maximum number of providers are already registered."
|Severity|Warning
|Resolution|None.

### iLO.2.2.MaxVirtualMediaConnectionEstablished
No more Virtual Media connections are available, because the maximum number of connections are already established.

| | |
|:---|:---|
|Message Format|"No more Virtual Media connections are available, because the maximum number of connections are already established."
|Severity|Warning
|Resolution|Close an established Virtual Media connection, and then retry creating or opening another connection.

### iLO.2.2.MembistVariablesNotSupported
Membist variables are not supported on the system.

| | |
|:---|:---|
|Message Format|"Membist variables are not supported on the system."
|Severity|Warning
|Resolution|None.

### iLO.2.2.NoEventSubscriptions
There are no event subscriptions registerd.

| | |
|:---|:---|
|Message Format|"The opeartion can not be completed because there are no event subscribers."
|Severity|Warning
|Resolution|

### iLO.2.2.NoPowerMetering
No support for power metering available on platform.

| | |
|:---|:---|
|Message Format|"No support for power metering available on platform."
|Severity|OK
|Resolution|Enable Power Metering on platform if supported.

### iLO.2.2.NoSNMPAlertDestinationsConfigured
No SNMP alert destinations configured or none of the configured destinations are associated with SNMPv1 protocol or SNMPv3 protocol and user.

| | |
|:---|:---|
|Message Format|"No SNMP alert destinations configured or none of the configured destinations are associated with SNMPv1 protocol or SNMPv3 protocol and user."
|Severity|Warning
|Resolution|Configure at least one SNMP alert destination and associate it with SNMPv1 protocol or SNMPv3 protocol and user.

### iLO.2.2.NoSamples
No power history samples are available.

| | |
|:---|:---|
|Message Format|"No power history samples are available."
|Severity|OK
|Resolution|To accumulate power history samples, power on the server, and then wait at least 5 minutes.

### iLO.2.2.NoScriptedVirtualMediaConnectionAvailable
No scripted virtual media connections exist to perform the operation.

| | |
|:---|:---|
|Message Format|"No scripted virtual media connections exist to perform the operation."
|Severity|Warning
|Resolution|Create or open a scripted virtual media connection, and then retry the operation.

### iLO.2.2.NoSpaceforDNSName
No space to store DNS name.

| | |
|:---|:---|
|Message Format|"No space to store DNS name."
|Severity|Warning
|Resolution|Make sure SSO database has enough space to store DNS name.

### iLO.2.2.NoVirtualMediaConnectionAvailable
No Virtual Media connections exist to perform the operation.

| | |
|:---|:---|
|Message Format|"No Virtual Media connections exist to perform the operation."
|Severity|Warning
|Resolution|Create or open a Virtual Media connection, and then retry the operation.

### iLO.2.2.NodeAssignedCrossRegion
Each zone can only manage the node in the same region, cannot manage overlap region.

| | |
|:---|:---|
|Message Format|"Each zone can only manage the node for range %1 or range %2, cannot manage overlap region."
|Severity|Warning
|Resolution|Correct the out of range value, and then retry the operation.

### iLO.2.2.NodeNotPresentInZone
Operation is currently unavailable because there is no node installed in the zone.

| | |
|:---|:---|
|Message Format|"Operation is currently unavailable because there is no node installed in the zone."
|Severity|Warning
|Resolution|Install at least one node in the zone and retry the operation.

### iLO.2.2.NotSupportedOnNIC
This property is not supported by the indicated network port.

| | |
|:---|:---|
|Message Format|"%1 is not supported on the %2 Network Port."
|Severity|Warning
|Resolution|Do not specify this property on the indicated network port.

### iLO.2.2.NotValidIPAddrOrDNS
The value for the property is not a valid IPv4/v6 address or DNS name.

| | |
|:---|:---|
|Message Format|"The value for property %1 is not a valid IPv4/v6 address or DNS name."
|Severity|Warning
|Resolution|Correct the IPv4/v6 address or DNS name, and then retry the operation.

### iLO.2.2.NotValidIPAddress
The value for the property is not a valid IP address.

| | |
|:---|:---|
|Message Format|"The value %1 is not a valid IP address for %2"
|Severity|Warning
|Resolution|Use a valid IP address.

### iLO.2.2.NotValidSubnetMask
The value for the property is not a valid subnet mask.

| | |
|:---|:---|
|Message Format|"The value %1 is not a valid subnet mask for %2"
|Severity|Warning
|Resolution|Use a valid subnet mask.

### iLO.2.2.OperationWillCompleteAfterSystemPOST
The value for the property will be applied after System BIOS POST completes.

| | |
|:---|:---|
|Message Format|"The value for property %1 will be changed after the System BIOS completes POST."
|Severity|Information
|Resolution|Wait to see the change in value until after the System BIOS completes POST.

### iLO.2.2.PowerCapOACntrld
The enclosure Onboard Administrator is currently managing the power cap.

| | |
|:---|:---|
|Message Format|"The enclosure Onboard Administrator is currently managing the power cap."
|Severity|Warning
|Resolution|Use Onboard Administrator to Manage the PowerCap

### iLO.2.2.PowerCapROMCntrld
The System ROM is currently managing the power cap.

| | |
|:---|:---|
|Message Format|"The System ROM is currently managing the power cap."
|Severity|Warning
|Resolution|Enable RESTful API management of the power cap in System ROM

### iLO.2.2.PowerLimitMayNotTakeEffect
One of power limit setpoint may become unreachable due to power limit range is unknown. It's not recommended configure power limit setpoint when power limit range is unknown.

| | |
|:---|:---|
|Message Format|"One of power limit setpoint may become unreachable due to power limit range is unknown. It's not recommended configure power limit setpoint when power limit range is unknown."
|Severity|Warning
|Resolution|Please execute calibrate action to get power limit range then reconfigure power limit setpoint.

### iLO.2.2.PowerRegulationNotDisable
Operation is currently unavailable because chassis power regulation is enabled.

| | |
|:---|:---|
|Message Format|"Operation is currently unavailable because chassis power regulation is enabled."
|Severity|Warning
|Resolution|Disable chassis power regulation, and then retry the operation.

### iLO.2.2.PowerSettingAdjustRequired
Indicates that one or more power limit setting were correctly changed, but will not take effect until power regulation enable and power regulator mode switch to user configurable mode.

| | |
|:---|:---|
|Message Format|"Indicates that one or more power limit setting were correctly changed, but will not take effect until power regulation enable and power regulator mode switch to user configurable mode."
|Severity|Warning
|Resolution|Enable power regulation and switch power regulator mode to user configurable mode for the settings to take effect.

### iLO.2.2.PowerValueBadParam
The power cap value is not valid.

| | |
|:---|:---|
|Message Format|"The power cap value is not valid."
|Severity|Warning
|Resolution|Retry the operation using a corrected value.

### iLO.2.2.PowerValueInvalidCalibrationData
The request to set the power cap failed. Invalid power cap calibration data. The Power Cap feature is currently unavailable.

| | |
|:---|:---|
|Message Format|"The request to set the power cap failed. Invalid power cap calibration data. The Power Cap feature is currently unavailable"
|Severity|Warning
|Resolution|Restart the server to retrieve calibration data from initial POST.

### iLO.2.2.PowerValueNotOptimal
Power caps set below the specified percentage threshold might become unreachable due to changes in the server. It is recommended to not set a cap for less than this threshold.

| | |
|:---|:---|
|Message Format|"Power caps set below the specified percentage threshold might become unreachable due to changes in the server. It is recommended to not set a cap for less than %1%."
|Severity|Warning
|Resolution|Please provide an optimal value in integer considering the power cap range.

### iLO.2.2.PowerValueUnAvailable
Advanced power capping is not currently available due to the system configuration or state.

| | |
|:---|:---|
|Message Format|"Advanced power capping is not currently available due to the system configuration or state."
|Severity|Warning
|Resolution|Change the system configuration or wait for the system to become fully initialized, and then retry the operation.

### iLO.2.2.PowerValueUnSupported
Advanced power capping is not supported on this system.

| | |
|:---|:---|
|Message Format|"Advanced power capping is not supported on this system."
|Severity|Warning
|Resolution|None.

### iLO.2.2.PrimaryESKMServerAccessible
Only the primary ESKM server is accessible.

| | |
|:---|:---|
|Message Format|"No redundancy. Only the primary ESKM server is accessible."
|Severity|OK
|Resolution|None.

### iLO.2.2.PrimarySecondaryAddressesResolveToSameServer
Primary and secondary ESKM server addresses resolve to the same server.

| | |
|:---|:---|
|Message Format|"No redundancy. Primary and secondary ESKM server addresses resolve to the same server."
|Severity|OK
|Resolution|None.

### iLO.2.2.PrimarySecondaryESKMServersAccessible
Both primary and secondary ESKM servers are accessible.

| | |
|:---|:---|
|Message Format|"Redundant solution: Both primary and secondary ESKM servers are accessible."
|Severity|OK
|Resolution|None.

### iLO.2.2.PropertyNotSupported
The property is not supported.

| | |
|:---|:---|
|Message Format|"The property %1 is not supported."
|Severity|Warning
|Resolution|Do not attempt to modify this property.

### iLO.2.2.PropertyNotWritableOrUnknown
The request included a value for a  read-only or unknown property.

| | |
|:---|:---|
|Message Format|"The property %1 is a read-only property and cannot be assigned a value, or not valid for this resource."
|Severity|Warning
|Resolution|If the operation did not complete, remove the property from the request body and resubmit the request.

### iLO.2.2.PropertyValueBadParam
The property value is not valid.

| | |
|:---|:---|
|Message Format|"The property value is not valid."
|Severity|Warning
|Resolution|Retry the operation using a corrected value.

### iLO.2.2.PropertyValueExceedsMaxLength
The value for the property exceeds the maximum length.

| | |
|:---|:---|
|Message Format|"The value %1 for the property %2 exceeds the maximum length of %3."
|Severity|Warning
|Resolution|Correct the value for the property in the request body, and then retry the operation.

### iLO.2.2.PropertyValueIncompatible
The value for the property is the correct type, but this value is incompatible with the current value of another property.

| | |
|:---|:---|
|Message Format|"The value %1 for the property %2 is incompatible with the value for property %3."
|Severity|Warning
|Resolution|Correct the value for the property in the request body, and then retry the operation.

### iLO.2.2.PropertyValueOutOfRange
The value for the property is out of range.

| | |
|:---|:---|
|Message Format|"The value %1 for the property %2 is out of range %3."
|Severity|Warning
|Resolution|Correct the value for the property in the request body, and then retry the operation.

### iLO.2.2.PropertyValueRequired
Indicates that a property was required but not specified.

| | |
|:---|:---|
|Message Format|"%1 requires Property %2 to be specified."
|Severity|Warning
|Resolution|Include the required property in the request body and then retry the operation.

### iLO.2.2.RecoveryInstallSetRequired
A recovery install set is required for this action.

| | |
|:---|:---|
|Message Format|"No recovery install set present."
|Severity|Critical
|Resolution|Create a recovery install set (install set with IsRecovery property set true).

### iLO.2.2.RepairNotSupported
IML event with this severity is not supported to be repaired. IML events with Critical or Warning severities can marked as repaired.

| | |
|:---|:---|
|Message Format|"IML event with %1 severity is not supported to be repaired. IML events with Critical or Warning severities can marked as repaired."
|Severity|Warning
|Resolution|Please do not try to repair IML events with severity other than Critical or Warning.

### iLO.2.2.RequiredPropertyMissing
Indicates that a required property is not specified.

| | |
|:---|:---|
|Message Format|"Required Property %1 needs to be specifed."
|Severity|Warning
|Resolution|Include the required property in the request body and then retry the operation.

### iLO.2.2.ResetInProgress
A management processor reset is in progress.

| | |
|:---|:---|
|Message Format|"A management processor reset is in progress."
|Severity|Warning
|Resolution|Wait for management processor reset to complete, and then retry the operation.

### iLO.2.2.ResetRequired
One or more properties were changed, but these changes will not take effect until the management processor is reset.

| | |
|:---|:---|
|Message Format|"One or more properties were changed, but these changes will not take effect until the management processor is reset."
|Severity|Warning
|Resolution|To enable the changed properties, reset the management processor.

### iLO.2.2.ResourceBeingFlashed
The change to the requested resource failed because the resource is being flashed.

| | |
|:---|:---|
|Message Format|"The change to the requested resource failed because the resource is being flashed."
|Severity|Warning
|Resolution|Retry the operation when the firmware upgrade has completed.

### iLO.2.2.ResourceInUseWithDetail
The change could not be made because the resource was in use or in a transitioning state.

| | |
|:---|:---|
|Message Format|"The change to the resource failed because the resource is in use or in transition."
|Severity|Warning
|Resolution|Retry the request.

### iLO.2.2.ResourceNotReadyRetry
The resource is present but is not ready to perform operations due to an internal condition such as initialization or reset.

| | |
|:---|:---|
|Message Format|"The resource is present but is not ready to perform operations.  The resource will be ready in %1 seconds."
|Severity|Warning
|Resolution|Retry the operation when the resource is ready.

### iLO.2.2.ResourceTemporarilyUnavailable
The resource is temporarily unavailable because the firmware is being flashed.

| | |
|:---|:---|
|Message Format|"The resource is temporarily unavailable because the firmware is being flashed."
|Severity|Warning
|Resolution|Retry the operation when the firmware upgrade has completed.

### iLO.2.2.SMBIOSRecordNotFound
The SMBIOS record type is not found or is not supported on the system.

| | |
|:---|:---|
|Message Format|"The SMBIOS record type %1 is not found or is not supported on the system."
|Severity|Warning
|Resolution|Reset the system to update the SMBIOS records. If the problem persists then the SMBIOS record type is not supported.

### iLO.2.2.SNMPAlertDisabled
The operation could not be completed because SNMP alerts are disabled.

| | |
|:---|:---|
|Message Format|"The operation could not be completed because SNMP alerts are disabled."
|Severity|Warning
|Resolution|Enable SNMP alerts and retry the operation.

### iLO.2.2.SNMPDisabled
Modifying SNMP properties is not possible with SNMP disabled.

| | |
|:---|:---|
|Message Format|"Modifying SNMP properties is not possible with SNMP disabled."
|Severity|Warning
|Resolution|Enable SNMP, and then modify the SNMP properties.

### iLO.2.2.SNMPTestAlertFailed
The SNMP Test Alert did not send successfully.

| | |
|:---|:---|
|Message Format|"The SNMP Test Alert did not send successfully."
|Severity|Warning
|Resolution|Verify the test alert content and retry.

### iLO.2.2.SNTPConfigurationManagedByDHCPAndIsReadOnly
SNTP configuration is currently managed by DHCP and is therefore read-only.

| | |
|:---|:---|
|Message Format|"%1 cannot be changed while DHCP is configured to provide SNTP settings."
|Severity|Warning
|Resolution|Disable SNTP configuration options in both DHCPv4 and DHCPv6 (see /Managers/n/NICs), and then reconfigure SNTP as desired with static settings.

### iLO.2.2.SSOCertficateEmpty
SSO Certificate is Empty.

| | |
|:---|:---|
|Message Format|"Empty SSO Certificate."
|Severity|Warning
|Resolution|None.

### iLO.2.2.SSOCertificateReadError
SSO Certificate Read Error.

| | |
|:---|:---|
|Message Format|"Error reading SSO certificate."
|Severity|Warning
|Resolution|Retry the request with valid SSO certificate.

### iLO.2.2.SSONoSpaceError
No space to store SSO certificate.

| | |
|:---|:---|
|Message Format|"No space to store SSO certificate."
|Severity|Warning
|Resolution|Make sure SSO database has enough space to store SSO certificate.

### iLO.2.2.SSORecordNotFound
SSO Record Not Found.

| | |
|:---|:---|
|Message Format|"SSO Record Not Found."
|Severity|Warning
|Resolution|None.

### iLO.2.2.SecondaryESKMServerAccessible
Only the secondary ESKM server is accessible.

| | |
|:---|:---|
|Message Format|"No redundancy. Only the secondary ESKM server is accessible."
|Severity|OK
|Resolution|None.

### iLO.2.2.SuccessFeedback
The operation completed successfully.

| | |
|:---|:---|
|Message Format|"The operation completed successfully."
|Severity|OK
|Resolution|None

### iLO.2.2.SyslogFeatureDisabled
Remote Syslog feature is disabled.

| | |
|:---|:---|
|Message Format|"Remote syslog feature is disabled."
|Severity|Warning
|Resolution|Enable remote syslog feature to send test syslog message.

### iLO.2.2.SystemPowerOffRequired
To perform this operation, power off the system. AutoPowerOn must be set to achieve a power restore.

| | |
|:---|:---|
|Message Format|"To perform this operation, power off the system."
|Severity|OK
|Resolution|To perform this operation, power off the system.

### iLO.2.2.SystemResetRequired
The system properties were correctly changed, but will not take effect until the system is reset.

| | |
|:---|:---|
|Message Format|"One or more properties were changed and will not take effect until system is reset."
|Severity|Warning
|Resolution|Reset system for the settings to take effect.

### iLO.2.2.TokenRequired
Proper 'X-HPRESTFULAPI-AuthToken' authorization token not provided.

| | |
|:---|:---|
|Message Format|"Proper 'X-HPRESTFULAPI-AuthToken' authorization token not provided."
|Severity|Critical
|Resolution|Create proper 'X-HPRESTFULAPI-AuthToken' authorization token. Send token in using the proper HTTP header.

### iLO.2.2.UnableModifyRights
Unable to modify user rights.

| | |
|:---|:---|
|Message Format|"Unable to modify user rights."
|Severity|Warning
|Resolution|None.

### iLO.2.2.UnableToModifyDueToMissingComponent
The value for the property cannot be changed because a related hardware component is not installed.

| | |
|:---|:---|
|Message Format|"The value for property %1 cannot be changed because a related hardware component is not installed."
|Severity|Warning
|Resolution|Install the hardware component and retry the operation.

### iLO.2.2.UnableToModifyDuringSystemPOST
The value for the property cannot be changed while the computer system BIOS is in POST.

| | |
|:---|:---|
|Message Format|"The value for property %1 cannot be changed while the computer system BIOS is in POST."
|Severity|Warning
|Resolution|After the computer system is either fully booted or powered off, retry the operation.

### iLO.2.2.UnauthorizedLoginAttempt
The login was not successful, because the supplied credentials could not be authorized.

| | |
|:---|:---|
|Message Format|"The login was not successful, because the supplied credentials could not be authorized."
|Severity|Warning
|Resolution|Log in with authorized user name and password credentials.

### iLO.2.2.UnsupportedOperation
This operation is not supported by RIS for the current system.

| | |
|:---|:---|
|Message Format|"This operation is not supported by RIS for the current system."
|Severity|Warning
|Resolution|None.

### iLO.2.2.UnsupportedOperationInChassisVersion
This operation is not supported by the current version of the XL Chassis firmware.

| | |
|:---|:---|
|Message Format|"This operation is not supported by the current version of the XL Chassis firmware."
|Severity|Warning
|Resolution|Please update the XL Chassis firmware to latest version.

### iLO.2.2.UnsupportedOperationInLegacyBootMode
This operation is not supported when the system Boot Mode is set to Legacy BIOS.

| | |
|:---|:---|
|Message Format|" This operation is not supported when the system Boot Mode is set to Legacy BIOS."
|Severity|Warning
|Resolution|Change the Boot Mode to UEFI and retry the operation.

### iLO.2.2.UnsupportedOperationInSystemBIOS
This operation is not supported by the current version of the system BIOS.

| | |
|:---|:---|
|Message Format|"This operation is not supported by the current version of the system BIOS."
|Severity|Warning
|Resolution|None.

### iLO.2.2.UpdateBadParameter


| | |
|:---|:---|
|Message Format|"The update failed because a bad parameter was supplied."
|Severity|Warning
|Resolution|Supply correct parameters to the component and retry the update.

### iLO.2.2.UpdateCancelled


| | |
|:---|:---|
|Message Format|"The update was canceled by the update process."
|Severity|Warning
|Resolution|Retry the update.

### iLO.2.2.UpdateDependencyFailure


| | |
|:---|:---|
|Message Format|"The update did not complete because the component failed a dependency check."
|Severity|Warning
|Resolution|Install any dependent components first and then retry this update.

### iLO.2.2.UpdateFailed


| | |
|:---|:---|
|Message Format|"The update failed with a component specific error (%1)."
|Severity|Warning
|Resolution|Retry the update after remedying the component error.

### iLO.2.2.UpdateInPOST


| | |
|:---|:---|
|Message Format|"System must not be booted past POST in order to perform this update"
|Severity|Warning
|Resolution|Boot to UEFI and retry the update.

### iLO.2.2.UpdateInterrupted


| | |
|:---|:---|
|Message Format|"The update was interrupted."
|Severity|Warning
|Resolution|Retry the update.

### iLO.2.2.UpdateInvalidFile


| | |
|:---|:---|
|Message Format|"The update operation failed because the file is not valid."
|Severity|Warning
|Resolution|Remove and re-add the component to the repository and try the operation again.

### iLO.2.2.UpdateInvalidOS


| | |
|:---|:---|
|Message Format|"The update did not occur because the running OS is not valid."
|Severity|Warning
|Resolution|Retry the update while running the correct OS.

### iLO.2.2.UpdateNotApplicable


| | |
|:---|:---|
|Message Format|"The task was not completed because the component was not applicable to this system."
|Severity|Warning
|Resolution|None.

### iLO.2.2.UpdateRepositoryUnavailable


| | |
|:---|:---|
|Message Format|"The update operation failed because the component repository is unavailable."
|Severity|Warning
|Resolution|None.

### iLO.2.2.UpdateTaskQueueFull
The Invoke action was not successful because the update task queue is full.

| | |
|:---|:---|
|Message Format|"The Invoke action was not successful because the update task queue is full."
|Severity|Critical
|Resolution|Remove completed tasks from the update task queue to retry the operation.

### iLO.2.2.UpdateTaskQueueWriteError
The UpdateTaskQueue write failed.

| | |
|:---|:---|
|Message Format|"The UpdateTaskQueue write of %1 failed."
|Severity|Warning
|Resolution|Ensure a valid name for the item and that space exists to hold the item.

### iLO.2.2.UpdateTemporarilyUnavailable


| | |
|:---|:---|
|Message Format|"The system is temporarily unable to perform this update"
|Severity|Warning
|Resolution|Retry the update, ensuring that power state is stable.

### iLO.2.2.UpdateWithPowerOff


| | |
|:---|:---|
|Message Format|"System power must be off to perform this update"
|Severity|Warning
|Resolution|Power system on and retry the update.

### iLO.2.2.UpdateWithPowerOn


| | |
|:---|:---|
|Message Format|"System power must be on to perform this update"
|Severity|Warning
|Resolution|Power system on and retry the update.

### iLO.2.2.UserAlreadyExist
The user or login user name already exists.

| | |
|:---|:---|
|Message Format|"The user or login user name already exists."
|Severity|Warning
|Resolution|Try a different user or login user name.

### iLO.2.2.UserNameAlreadyExists
Duplicate SNMPv3 User.

| | |
|:---|:---|
|Message Format|"The username %1 already exists in the list"
|Severity|Warning
|Resolution|Enter a different name and try again.

### iLO.2.2.VirtualMediaIsDisabled
Virtual Media has been disabled.

| | |
|:---|:---|
|Message Format|"Virtual Media has been disabled."
|Severity|Warning
|Resolution|Enable Virtual Media to perform this operation.

### iLO.2.2.ZonePowerLimitExceeded
The sum of zone power limit cannot be more than chassis power limit.

| | |
|:---|:---|
|Message Format|"The value %1 for the sum of %2 cannot be more than chassis power limit %3."
|Severity|Warning
|Resolution|Correct the value avoid the sum of power limit exceeds chassis power limit, and then retry the operation.

### iLO.2.2.iLOResetAndSystemRebootRequired
Indicates that one or more properties were correctly changed, but will not take effect until device is reset and system is rebooted.

| | |
|:---|:---|
|Message Format|"One or more properties were changed and will not take effect until the device is reset and system is rebooted"
|Severity|Warning
|Resolution|Reset the management processor and reboot the server.
