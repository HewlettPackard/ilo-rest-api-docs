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
