# Resource Map
|URI|Type|
|:---|:---|
|`/redfish/v1/`|[ServiceRoot](#serviceroot-v1_5_0-serviceroot)|
|`/redfish/v1/AccountService`|[AccountService](#accountservice-v1_3_0-accountservice)|
|`/redfish/v1/AccountService/Accounts`|Collection of [ManagerAccount](#manageraccount-v1_1_3-manageraccount)|
|`/redfish/v1/AccountService/Accounts/{item}`|[ManagerAccount](#manageraccount-v1_1_3-manageraccount)|
|`/redfish/v1/AccountService/DirectoryTest`|[HpeDirectoryTest](#hpedirectorytest-v1_0_0-hpedirectorytest)|
|`/redfish/v1/AccountService/ExternalAccountProviders/LDAP/Certificates`|Collection of [Certificate](#certificate-v0_9_0-certificate)|
|`/redfish/v1/AccountService/ExternalAccountProviders/LDAP/Certificates/{item}`|[Certificate](#certificate-v0_9_0-certificate)|
|`/redfish/v1/AccountService/Roles`|Collection of [Role](#role-v1_2_1-role)|
|`/redfish/v1/AccountService/Roles/{item}`|[Role](#role-v1_2_1-role)|
|`/redfish/v1/AccountService/UserCertificateMapping`|Collection of [HpeiLOAccountCertificateMap](#hpeiloaccountcertificatemap-v1_0_1-hpeiloaccountcertificatemap)|
|`/redfish/v1/AccountService/UserCertificateMapping/{item}`|[HpeiLOAccountCertificateMap](#hpeiloaccountcertificatemap-v1_0_1-hpeiloaccountcertificatemap)|
|`/redfish/v1/Chassis`|Collection of [Chassis](#chassis-v1_6_0-chassis)|
|`/redfish/v1/Chassis/{item}`|[Chassis](#chassis-v1_6_0-chassis)|
|`/redfish/v1/Chassis/{item}/AccHddService`|[HpeServerAccHddService](#hpeserveracchddservice-v1_0_0-hpeserveracchddservice)|
|`/redfish/v1/Chassis/{item}/AccHddService/Zone`|[HpeServerAccHddZone](#hpeserveracchddzone-v1_0_0-hpeserveracchddzone)|
|`/redfish/v1/Chassis/{item}/Devices`|Collection of [HpeServerDevice](#hpeserverdevice-v2_0_0-hpeserverdevice)|
|`/redfish/v1/Chassis/{item}/Devices/{item}`|[HpeServerDevice](#hpeserverdevice-v2_0_0-hpeserverdevice)|
|`/redfish/v1/Chassis/{item}/Drives/{interface}/{item}`|[Drive](#drive-v1_0_0-drive)|
|`/redfish/v1/Chassis/{item}/NetworkAdapters`|Collection of [NetworkAdapter](#networkadapter-v1_2_0-networkadapter)|
|`/redfish/v1/Chassis/{item}/NetworkAdapters/{item}`|[NetworkAdapter](#networkadapter-v1_2_0-networkadapter)|
|`/redfish/v1/Chassis/{item}/NetworkAdapters/{item}/NetworkDeviceFunctions`|Collection of [NetworkDeviceFunction](#networkdevicefunction-v1_3_0-networkdevicefunction)|
|`/redfish/v1/Chassis/{item}/NetworkAdapters/{item}/NetworkDeviceFunctions/{item}`|[NetworkDeviceFunction](#networkdevicefunction-v1_3_0-networkdevicefunction)|
|`/redfish/v1/Chassis/{item}/NetworkAdapters/{item}/NetworkDeviceFunctions/{item}/Settings`|[NetworkDeviceFunction](#networkdevicefunction-v1_3_0-networkdevicefunction)|
|`/redfish/v1/Chassis/{item}/NetworkAdapters/{item}/NetworkPorts`|Collection of [NetworkPort](#networkport-v1_2_0-networkport)|
|`/redfish/v1/Chassis/{item}/NetworkAdapters/{item}/NetworkPorts/{item}`|[NetworkPort](#networkport-v1_2_0-networkport)|
|`/redfish/v1/Chassis/{item}/NetworkAdapters/{item}/NetworkPorts/{item}/HpeEVB`|[HpeNetworkPortEVB](#hpenetworkportevb-v1_1_1-hpenetworkportevb)|
|`/redfish/v1/Chassis/{item}/NetworkAdapters/{item}/NetworkPorts/{item}/HpeLLDP`|[HpeNetworkPortLLDP](#hpenetworkportlldp-v1_1_1-hpenetworkportlldp)|
|`/redfish/v1/Chassis/{item}/NetworkAdapters/{item}/NetworkPorts/{item}/Settings`|[NetworkPort](#networkport-v1_2_0-networkport)|
|`/redfish/v1/Chassis/{item}/NetworkAdapters/{item}/Settings`|[NetworkAdapter](#networkadapter-v1_2_0-networkadapter)|
|`/redfish/v1/Chassis/{item}/Power`|[Power](#power-v1_3_0-power)|
|`/redfish/v1/Chassis/{item}/Power/AccPowerService`|[HpeServerAccPowerService](#hpeserveraccpowerservice-v1_0_0-hpeserveraccpowerservice)|
|`/redfish/v1/Chassis/{item}/Power/AccPowerService/Calibration`|[HpeServerAccPowerCalibration](#hpeserveraccpowercalibration-v1_0_0-hpeserveraccpowercalibration)|
|`/redfish/v1/Chassis/{item}/Power/AccPowerService/NodesInfo`|[HpeServerAccPowerNodesInfo](#hpeserveraccpowernodesinfo-v1_0_0-hpeserveraccpowernodesinfo)|
|`/redfish/v1/Chassis/{item}/Power/AccPowerService/PowerLimit`|[HpeServerAccPowerLimit](#hpeserveraccpowerlimit-v1_0_0-hpeserveraccpowerlimit)|
|`/redfish/v1/Chassis/{item}/Power/AccPowerService/Zone`|[HpeServerAccPowerZone](#hpeserveraccpowerzone-v1_0_0-hpeserveraccpowerzone)|
|`/redfish/v1/Chassis/{item}/Power/FastPowerMeter`|[HpePowerMeter](#hpepowermeter-v2_0_1-hpepowermeter)|
|`/redfish/v1/Chassis/{item}/Power/FederatedGroupCapping`|[HpeiLOFederatedGroupCapping](#hpeilofederatedgroupcapping-v2_0_0-hpeilofederatedgroupcapping)|
|`/redfish/v1/Chassis/{item}/Power/PowerMeter`|[HpePowerMeter](#hpepowermeter-v2_0_1-hpepowermeter)|
|`/redfish/v1/Chassis/{item}/Thermal`|[Thermal](#thermal-v1_1_0-thermal)|
|`/redfish/v1/EventService`|[EventService](#eventservice-v1_0_8-eventservice)|
|`/redfish/v1/EventService/CACertificates`|Collection of [HpeCertificate](#hpecertificate-v0_9_0-hpecertificate)|
|`/redfish/v1/EventService/CACertificates/{item}`|[HpeCertificate](#hpecertificate-v0_9_0-hpecertificate)|
|`/redfish/v1/EventService/Subscriptions`|Collection of [EventDestination](#eventdestination-v1_0_0-eventdestination)|
|`/redfish/v1/EventService/Subscriptions/{item}`|[EventDestination](#eventdestination-v1_0_0-eventdestination)|
|`/redfish/v1/JsonSchemas`|Collection of [JsonSchemaFile](#jsonschemafile-v1_0_4-jsonschemafile)|
|`/redfish/v1/JsonSchemas/{item}`|[JsonSchemaFile](#jsonschemafile-v1_0_4-jsonschemafile)|
|`/redfish/v1/Managers`|Collection of [Manager](#manager-v1_3_3-manager)|
|`/redfish/v1/Managers/{item}`|[Manager](#manager-v1_3_3-manager)|
|`/redfish/v1/Managers/{item}/ActiveHealthSystem`|[HpeiLOActiveHealthSystem](#hpeiloactivehealthsystem-v2_3_0-hpeiloactivehealthsystem)|
|`/redfish/v1/Managers/{item}/BackupRestoreService`|[HpeiLOBackupRestoreService](#hpeilobackuprestoreservice-v2_2_0-hpeilobackuprestoreservice)|
|`/redfish/v1/Managers/{item}/BackupRestoreService/BackupFiles`|Collection of [HpeiLOBackupFile](#hpeilobackupfile-v1_0_0-hpeilobackupfile)|
|`/redfish/v1/Managers/{item}/BackupRestoreService/BackupFiles/{item}`|[HpeiLOBackupFile](#hpeilobackupfile-v1_0_0-hpeilobackupfile)|
|`/redfish/v1/Managers/{item}/DateTime`|[HpeiLODateTime](#hpeilodatetime-v2_0_0-hpeilodatetime)|
|`/redfish/v1/Managers/{item}/EmbeddedMedia`|[HpeiLOEmbeddedMedia](#hpeiloembeddedmedia-v2_0_0-hpeiloembeddedmedia)|
|`/redfish/v1/Managers/{item}/EthernetInterfaces`|Collection of [EthernetInterface](#ethernetinterface-v1_4_1-ethernetinterface)|
|`/redfish/v1/Managers/{item}/EthernetInterfaces/{item}`|[EthernetInterface](#ethernetinterface-v1_4_1-ethernetinterface)|
|`/redfish/v1/Managers/{item}/FederationGroups`|Collection of [HpeiLOFederationGroup](#hpeilofederationgroup-v2_0_0-hpeilofederationgroup)|
|`/redfish/v1/Managers/{item}/FederationGroups/{item}`|[HpeiLOFederationGroup](#hpeilofederationgroup-v2_0_0-hpeilofederationgroup)|
|`/redfish/v1/Managers/{item}/FederationPeers`|Collection of [HpeiLOFederationPeers](#hpeilofederationpeers-v2_0_0-hpeilofederationpeers)|
|`/redfish/v1/Managers/{item}/FederationPeers/{item}`|[HpeiLOFederationPeers](#hpeilofederationpeers-v2_0_0-hpeilofederationpeers)|
|`/redfish/v1/Managers/{item}/HostInterfaces`|Collection of [HostInterface](#hostinterface-v1_1_1-hostinterface)|
|`/redfish/v1/Managers/{item}/HostInterfaces/{item}`|[HostInterface](#hostinterface-v1_1_1-hostinterface)|
|`/redfish/v1/Managers/{item}/LicenseService`|Collection of [HpeiLOLicense](#hpeilolicense-v2_1_1-hpeilolicense)|
|`/redfish/v1/Managers/{item}/LicenseService/{item}`|[HpeiLOLicense](#hpeilolicense-v2_1_1-hpeilolicense)|
|`/redfish/v1/Managers/{item}/LogServices`|Collection of [LogService](#logservice-v1_0_0-logservice)|
|`/redfish/v1/Managers/{item}/LogServices/IEL`|[LogService](#logservice-v1_0_0-logservice)|
|`/redfish/v1/Managers/{item}/LogServices/IEL/Entries`|Collection of [LogEntry](#logentry-v1_0_0-logentry)|
|`/redfish/v1/Managers/{item}/LogServices/IEL/Entries/{item}`|[LogEntry](#logentry-v1_0_0-logentry)|
|`/redfish/v1/Managers/{item}/NetworkProtocol`|[ManagerNetworkProtocol](#managernetworkprotocol-v1_0_0-managernetworkprotocol)|
|`/redfish/v1/Managers/{item}/RemoteSupportService`|[HpeRemoteSupport](#hperemotesupport-v2_3_0-hperemotesupport)|
|`/redfish/v1/Managers/{item}/RemoteSupportService/ServiceEventLogs`|Collection of [LogEntry](#logentry-v1_0_0-logentry)|
|`/redfish/v1/Managers/{item}/RemoteSupportService/ServiceEventLogs/{item}`|[LogEntry](#logentry-v1_0_0-logentry)|
|`/redfish/v1/Managers/{item}/SecurityService`|[HpeSecurityService](#hpesecurityservice-v2_2_0-hpesecurityservice)|
|`/redfish/v1/Managers/{item}/SecurityService/CertificateAuthentication`|[HpeCertAuth](#hpecertauth-v1_1_0-hpecertauth)|
|`/redfish/v1/Managers/{item}/SecurityService/CertificateAuthentication/CACertificates`|Collection of [HpeCertificate](#hpecertificate-v0_9_0-hpecertificate)|
|`/redfish/v1/Managers/{item}/SecurityService/CertificateAuthentication/CACertificates/{item}`|[HpeCertificate](#hpecertificate-v0_9_0-hpecertificate)|
|`/redfish/v1/Managers/{item}/SecurityService/ESKM`|[HpeESKM](#hpeeskm-v2_0_0-hpeeskm)|
|`/redfish/v1/Managers/{item}/SecurityService/HttpsCert`|[HpeHttpsCert](#hpehttpscert-v2_0_0-hpehttpscert)|
|`/redfish/v1/Managers/{item}/SecurityService/SSO`|[HpeiLOSSO](#hpeilosso-v2_0_0-hpeilosso)|
|`/redfish/v1/Managers/{item}/SecurityService/SecurityDashboard`|[HpeiLOSecurityDashboard](#hpeilosecuritydashboard-v1_0_0-hpeilosecuritydashboard)|
|`/redfish/v1/Managers/{item}/SecurityService/SecurityDashboard/SecurityParams`|Collection of [HpeiLOSecurityParam](#hpeilosecurityparam-v1_0_0-hpeilosecurityparam)|
|`/redfish/v1/Managers/{item}/SecurityService/SecurityDashboard/SecurityParams/{item}`|[HpeiLOSecurityParam](#hpeilosecurityparam-v1_0_0-hpeilosecurityparam)|
|`/redfish/v1/Managers/{item}/SnmpService`|[HpeiLOSnmpService](#hpeilosnmpservice-v2_2_0-hpeilosnmpservice)|
|`/redfish/v1/Managers/{item}/SnmpService/SNMPAlertDestinations`|Collection of [HpeSNMPAlertDestination](#hpesnmpalertdestination-v2_0_0-hpesnmpalertdestination)|
|`/redfish/v1/Managers/{item}/SnmpService/SNMPAlertDestinations/{item}`|[HpeSNMPAlertDestination](#hpesnmpalertdestination-v2_0_0-hpesnmpalertdestination)|
|`/redfish/v1/Managers/{item}/SnmpService/SNMPUsers`|Collection of [HpeSNMPUser](#hpesnmpuser-v2_1_0-hpesnmpuser)|
|`/redfish/v1/Managers/{item}/SnmpService/SNMPUsers/{item}`|[HpeSNMPUser](#hpesnmpuser-v2_1_0-hpesnmpuser)|
|`/redfish/v1/Managers/{item}/VirtualMedia`|Collection of [VirtualMedia](#virtualmedia-v1_2_0-virtualmedia)|
|`/redfish/v1/Managers/{item}/VirtualMedia/{item}`|[VirtualMedia](#virtualmedia-v1_2_0-virtualmedia)|
|`/redfish/v1/Registries`|Collection of [MessageRegistryFile](#messageregistryfile-v1_0_4-messageregistryfile)|
|`/redfish/v1/Registries/{item}`|[MessageRegistryFile](#messageregistryfile-v1_0_4-messageregistryfile)|
|`/redfish/v1/ResourceDirectory`|[HpeiLOResourceDirectory](#hpeiloresourcedirectory-v2_0_0-hpeiloresourcedirectory)|
|`/redfish/v1/SessionService`|[SessionService](#sessionservice-v1_0_0-sessionservice)|
|`/redfish/v1/SessionService/Sessions`|Collection of [Session](#session-v1_0_0-session)|
|`/redfish/v1/SessionService/Sessions/{item}`|[Session](#session-v1_0_0-session)|
|`/redfish/v1/Systems`|Collection of [ComputerSystem](#computersystem-v1_4_0-computersystem)|
|`/redfish/v1/Systems/{item}`|[ComputerSystem](#computersystem-v1_4_0-computersystem)|
|`/redfish/v1/Systems/{item}/BaseNetworkAdapters`|Collection of [HpeBaseNetworkAdapter](#hpebasenetworkadapter-v2_0_0-hpebasenetworkadapter)|
|`/redfish/v1/Systems/{item}/BaseNetworkAdapters/{item}`|[HpeBaseNetworkAdapter](#hpebasenetworkadapter-v2_0_0-hpebasenetworkadapter)|
|`/redfish/v1/Systems/{item}/Bios`|[Bios](#bios-v1_0_0-bios)|
|`/redfish/v1/Systems/{item}/Bios/Settings`|[Bios](#bios-v1_0_0-bios)|
|`/redfish/v1/Systems/{item}/Bios/baseconfigs`|[HpeBaseConfigs](#hpebaseconfigs-v2_0_0-hpebaseconfigs)|
|`/redfish/v1/Systems/{item}/Bios/boot`|[HpeServerBootSettings](#hpeserverbootsettings-v2_0_0-hpeserverbootsettings)|
|`/redfish/v1/Systems/{item}/Bios/boot/Settings`|[HpeServerBootSettings](#hpeserverbootsettings-v2_0_0-hpeserverbootsettings)|
|`/redfish/v1/Systems/{item}/Bios/boot/baseconfigs`|[HpeBaseConfigs](#hpebaseconfigs-v2_0_0-hpebaseconfigs)|
|`/redfish/v1/Systems/{item}/Bios/hpescalablepmem`|[HpeScalablePmem](#hpescalablepmem-v1_0_0-hpescalablepmem)|
|`/redfish/v1/Systems/{item}/Bios/hpescalablepmem/Settings`|[HpeScalablePmem](#hpescalablepmem-v1_0_0-hpescalablepmem)|
|`/redfish/v1/Systems/{item}/Bios/iscsi`|[HpeiSCSISoftwareInitiator](#hpeiscsisoftwareinitiator-v2_0_0-hpeiscsisoftwareinitiator)|
|`/redfish/v1/Systems/{item}/Bios/iscsi/Settings`|[HpeiSCSISoftwareInitiator](#hpeiscsisoftwareinitiator-v2_0_0-hpeiscsisoftwareinitiator)|
|`/redfish/v1/Systems/{item}/Bios/iscsi/baseconfigs`|[HpeBaseConfigs](#hpebaseconfigs-v2_0_0-hpebaseconfigs)|
|`/redfish/v1/Systems/{item}/Bios/mappings`|[HpeBiosMapping](#hpebiosmapping-v2_0_0-hpebiosmapping)|
|`/redfish/v1/Systems/{item}/Bios/tlsconfig`|[HpeTlsConfig](#hpetlsconfig-v1_0_0-hpetlsconfig)|
|`/redfish/v1/Systems/{item}/Bios/tlsconfig/Settings`|[HpeTlsConfig](#hpetlsconfig-v1_0_0-hpetlsconfig)|
|`/redfish/v1/Systems/{item}/Bios/tlsconfig/baseconfigs`|[HpeBaseConfigs](#hpebaseconfigs-v2_0_0-hpebaseconfigs)|
|`/redfish/v1/Systems/{item}/EthernetInterfaces`|Collection of [EthernetInterface](#ethernetinterface-v1_4_1-ethernetinterface)|
|`/redfish/v1/Systems/{item}/EthernetInterfaces/{item}`|[EthernetInterface](#ethernetinterface-v1_4_1-ethernetinterface)|
|`/redfish/v1/Systems/{item}/LogServices`|Collection of [LogService](#logservice-v1_0_0-logservice)|
|`/redfish/v1/Systems/{item}/LogServices/IML`|[LogService](#logservice-v1_0_0-logservice)|
|`/redfish/v1/Systems/{item}/LogServices/IML/Entries`|Collection of [LogEntry](#logentry-v1_0_0-logentry)|
|`/redfish/v1/Systems/{item}/LogServices/IML/Entries/{item}`|[LogEntry](#logentry-v1_0_0-logentry)|
|`/redfish/v1/Systems/{item}/Memory`|Collection of [Memory](#memory-v1_7_0-memory)|
|`/redfish/v1/Systems/{item}/Memory/{item}`|[Memory](#memory-v1_7_0-memory)|
|`/redfish/v1/Systems/{item}/MemoryDomains`|Collection of [MemoryDomain](#memorydomain-v1_2_1-memorydomain)|
|`/redfish/v1/Systems/{item}/MemoryDomains/{item}`|[MemoryDomain](#memorydomain-v1_2_1-memorydomain)|
|`/redfish/v1/Systems/{item}/MemoryDomains/{item}/MemoryChunks`|Collection of [MemoryChunks](#memorychunks-v1_2_2-memorychunks)|
|`/redfish/v1/Systems/{item}/MemoryDomains/{item}/MemoryChunks/{item}`|[MemoryChunks](#memorychunks-v1_2_2-memorychunks)|
|`/redfish/v1/Systems/{item}/NetworkInterfaces`|Collection of [NetworkInterface](#networkinterface-v1_1_1-networkinterface)|
|`/redfish/v1/Systems/{item}/NetworkInterfaces/{item}`|[NetworkInterface](#networkinterface-v1_1_1-networkinterface)|
|`/redfish/v1/Systems/{item}/NetworkInterfaces/{item}/NetworkDeviceFunctions`|Collection of [NetworkDeviceFunction](#networkdevicefunction-v1_3_0-networkdevicefunction)|
|`/redfish/v1/Systems/{item}/NetworkInterfaces/{item}/NetworkDeviceFunctions/{item}`|[NetworkDeviceFunction](#networkdevicefunction-v1_3_0-networkdevicefunction)|
|`/redfish/v1/Systems/{item}/NetworkInterfaces/{item}/NetworkPorts`|Collection of [NetworkPort](#networkport-v1_2_0-networkport)|
|`/redfish/v1/Systems/{item}/NetworkInterfaces/{item}/NetworkPorts/{item}`|[NetworkPort](#networkport-v1_2_0-networkport)|
|`/redfish/v1/Systems/{item}/NetworkInterfaces/{item}/NetworkPorts/{item}/HpeEVB`|[HpeNetworkPortEVB](#hpenetworkportevb-v1_1_1-hpenetworkportevb)|
|`/redfish/v1/Systems/{item}/NetworkInterfaces/{item}/NetworkPorts/{item}/HpeLLDP`|[HpeNetworkPortLLDP](#hpenetworkportlldp-v1_1_1-hpenetworkportlldp)|
|`/redfish/v1/Systems/{item}/NetworkInterfaces/{item}/NetworkPorts/{item}/Settings`|[NetworkPort](#networkport-v1_2_0-networkport)|
|`/redfish/v1/Systems/{item}/PCIDevices`|Collection of [HpeServerPciDevice](#hpeserverpcidevice-v2_0_0-hpeserverpcidevice)|
|`/redfish/v1/Systems/{item}/PCIDevices/{item}`|[HpeServerPciDevice](#hpeserverpcidevice-v2_0_0-hpeserverpcidevice)|
|`/redfish/v1/Systems/{item}/PCISlots`|Collection of [HpeServerPCISlot](#hpeserverpcislot-v2_1_0-hpeserverpcislot)|
|`/redfish/v1/Systems/{item}/PCISlots/{item}`|[HpeServerPCISlot](#hpeserverpcislot-v2_1_0-hpeserverpcislot)|
|`/redfish/v1/Systems/{item}/Processors`|Collection of [Processor](#processor-v1_0_0-processor)|
|`/redfish/v1/Systems/{item}/Processors/{item}`|[Processor](#processor-v1_0_0-processor)|
|`/redfish/v1/Systems/{item}/SecureBoot`|[SecureBoot](#secureboot-v1_0_0-secureboot)|
|`/redfish/v1/Systems/{item}/SmartStorage`|[HpeSmartStorage](#hpesmartstorage-v2_0_0-hpesmartstorage)|
|`/redfish/v1/Systems/{item}/SmartStorage/ArrayControllers`|Collection of [HpeSmartStorageArrayController](#hpesmartstoragearraycontroller-v2_2_0-hpesmartstoragearraycontroller)|
|`/redfish/v1/Systems/{item}/SmartStorage/ArrayControllers/{item}`|[HpeSmartStorageArrayController](#hpesmartstoragearraycontroller-v2_2_0-hpesmartstoragearraycontroller)|
|`/redfish/v1/Systems/{item}/SmartStorage/ArrayControllers/{item}/DiskDrives`|Collection of [HpeSmartStorageDiskDrive](#hpesmartstoragediskdrive-v2_1_0-hpesmartstoragediskdrive)|
|`/redfish/v1/Systems/{item}/SmartStorage/ArrayControllers/{item}/DiskDrives/{item}`|[HpeSmartStorageDiskDrive](#hpesmartstoragediskdrive-v2_1_0-hpesmartstoragediskdrive)|
|`/redfish/v1/Systems/{item}/SmartStorage/ArrayControllers/{item}/LogicalDrives`|Collection of [HpeSmartStorageLogicalDrive](#hpesmartstoragelogicaldrive-v2_3_0-hpesmartstoragelogicaldrive)|
|`/redfish/v1/Systems/{item}/SmartStorage/ArrayControllers/{item}/LogicalDrives/{item}`|[HpeSmartStorageLogicalDrive](#hpesmartstoragelogicaldrive-v2_3_0-hpesmartstoragelogicaldrive)|
|`/redfish/v1/Systems/{item}/SmartStorage/ArrayControllers/{item}/LogicalDrives/{item}/DataDrives`|Collection of [HpeSmartStorageDiskDrive](#hpesmartstoragediskdrive-v2_1_0-hpesmartstoragediskdrive)|
|`/redfish/v1/Systems/{item}/SmartStorage/ArrayControllers/{item}/StorageEnclosures`|Collection of [HpeSmartStorageStorageEnclosure](#hpesmartstoragestorageenclosure-v2_0_0-hpesmartstoragestorageenclosure)|
|`/redfish/v1/Systems/{item}/SmartStorage/ArrayControllers/{item}/StorageEnclosures/{item}`|[HpeSmartStorageStorageEnclosure](#hpesmartstoragestorageenclosure-v2_0_0-hpesmartstoragestorageenclosure)|
|`/redfish/v1/Systems/{item}/SmartStorage/ArrayControllers/{item}/UnconfiguredDrives`|Collection of [HpeSmartStorageDiskDrive](#hpesmartstoragediskdrive-v2_1_0-hpesmartstoragediskdrive)|
|`/redfish/v1/Systems/{item}/SmartStorage/ArrayControllers/{item}/UnconfiguredDrives/{item}`|[HpeSmartStorageDiskDrive](#hpesmartstoragediskdrive-v2_1_0-hpesmartstoragediskdrive)|
|`/redfish/v1/Systems/{item}/SmartStorage/HostBusAdapters`|Collection of [HpeSmartStorageHostBusAdapter](#hpesmartstoragehostbusadapter-v2_0_0-hpesmartstoragehostbusadapter)|
|`/redfish/v1/Systems/{item}/SmartStorage/HostBusAdapters/{item}`|[HpeSmartStorageHostBusAdapter](#hpesmartstoragehostbusadapter-v2_0_0-hpesmartstoragehostbusadapter)|
|`/redfish/v1/Systems/{item}/SmartStorage/HostBusAdapters/{item}/DiskDrives`|Collection of [HpeSmartStorageDiskDrive](#hpesmartstoragediskdrive-v2_1_0-hpesmartstoragediskdrive)|
|`/redfish/v1/Systems/{item}/SmartStorage/HostBusAdapters/{item}/DiskDrives/{item}`|[HpeSmartStorageDiskDrive](#hpesmartstoragediskdrive-v2_1_0-hpesmartstoragediskdrive)|
|`/redfish/v1/Systems/{item}/SmartStorageConfig`|[SmartStorageConfig](#smartstorageconfig-v2_0_0-smartstorageconfig)|
|`/redfish/v1/Systems/{item}/SmartStorageConfig/Settings`|[SmartStorageConfig](#smartstorageconfig-v2_0_0-smartstorageconfig)|
|`/redfish/v1/Systems/{item}/Storage`|Collection of [Storage](#storage-v1_1_0-storage)|
|`/redfish/v1/Systems/{item}/Storage/{interface}/{item}`|[Storage](#storage-v1_1_0-storage)|
|`/redfish/v1/Systems/{item}/Storage/{interface}/{item}/Volumes`|Collection of [Volume](#volume-v1_0_0-volume)|
|`/redfish/v1/Systems/{item}/Storage/{interface}/{item}/Volumes/{item}`|[Volume](#volume-v1_0_0-volume)|
|`/redfish/v1/Systems/{item}/USBDevices`|Collection of [HpeUSBDevice](#hpeusbdevice-v2_0_0-hpeusbdevice)|
|`/redfish/v1/Systems/{item}/USBDevices/{item}`|[HpeUSBDevice](#hpeusbdevice-v2_0_0-hpeusbdevice)|
|`/redfish/v1/Systems/{item}/USBPorts`|Collection of [HpeUSBPort](#hpeusbport-v2_0_0-hpeusbport)|
|`/redfish/v1/Systems/{item}/USBPorts/{item}`|[HpeUSBPort](#hpeusbport-v2_0_0-hpeusbport)|
|`/redfish/v1/Systems/{item}/WorkloadPerformanceAdvisor`|Collection of [v1_0_0](#v1_0_0)|
|`/redfish/v1/Systems/{item}/WorkloadPerformanceAdvisor/{item}`|[HpeWorkloadPerformanceAdvisor](#hpeworkloadperformanceadvisor-v1_0_0-hpeworkloadperformanceadvisor)|
|`/redfish/v1/TaskService`|[TaskService](#taskservice-v1_1_1-taskservice)|
|`/redfish/v1/TaskService/Tasks`|Collection of [Task](#task-v1_3_0-task)|
|`/redfish/v1/TaskService/Tasks/{item}`|[Task](#task-v1_3_0-task)|
|`/redfish/v1/TelemetryService`|[TelemetryService](#telemetryservice-v1_0_0-telemetryservice)|
|`/redfish/v1/TelemetryService/MetricDefinitions`|Collection of [MetricDefinition](#metricdefinition-v1_0_0-metricdefinition)|
|`/redfish/v1/TelemetryService/MetricDefinitions/{item}`|[MetricDefinition](#metricdefinition-v1_0_0-metricdefinition)|
|`/redfish/v1/TelemetryService/MetricReportDefinitions`|Collection of [MetricReportDefinition](#metricreportdefinition-v1_0_0-metricreportdefinition)|
|`/redfish/v1/TelemetryService/MetricReportDefinitions/{item}`|[MetricReportDefinition](#metricreportdefinition-v1_0_0-metricreportdefinition)|
|`/redfish/v1/TelemetryService/MetricReports/{item}`|[MetricReport](#metricreport-v1_0_0-metricreport)|
|`/redfish/v1/TelemetryService/MetricsReport`|Collection of [MetricReport](#metricreport-v1_0_0-metricreport)|
|`/redfish/v1/TelemetryService/Triggers`|Collection of [Trigger](#trigger-v1_0_0-trigger)|
|`/redfish/v1/TelemetryService/Triggers/{item}`|[Triggers](#triggers-v1_0_0-triggers)|
|`/redfish/v1/UpdateService`|[UpdateService](#updateservice-v1_1_0-updateservice)|
|`/redfish/v1/UpdateService/ComponentRepository`|Collection of [HpeComponent](#hpecomponent-v1_0_1-hpecomponent)|
|`/redfish/v1/UpdateService/ComponentRepository/{item}`|[HpeComponent](#hpecomponent-v1_0_1-hpecomponent)|
|`/redfish/v1/UpdateService/FirmwareInventory`|Collection of [SoftwareInventory](#softwareinventory-v1_0_0-softwareinventory)|
|`/redfish/v1/UpdateService/FirmwareInventory/{item}`|[SoftwareInventory](#softwareinventory-v1_0_0-softwareinventory)|
|`/redfish/v1/UpdateService/InstallSets`|Collection of [HpeComponentInstallSet](#hpecomponentinstallset-v1_0_3-hpecomponentinstallset)|
|`/redfish/v1/UpdateService/InstallSets/{item}`|[HpeComponentInstallSet](#hpecomponentinstallset-v1_0_3-hpecomponentinstallset)|
|`/redfish/v1/UpdateService/InvalidImageRepository`|Collection of [HpeInvalidImage](#hpeinvalidimage-v1_0_0-hpeinvalidimage)|
|`/redfish/v1/UpdateService/InvalidImageRepository/{item}`|[HpeInvalidImage](#hpeinvalidimage-v1_0_0-hpeinvalidimage)|
|`/redfish/v1/UpdateService/MaintenanceWindows`|Collection of [HpeMaintenanceWindow](#hpemaintenancewindow-v1_0_1-hpemaintenancewindow)|
|`/redfish/v1/UpdateService/MaintenanceWindows/{item}`|[HpeMaintenanceWindow](#hpemaintenancewindow-v1_0_1-hpemaintenancewindow)|
|`/redfish/v1/UpdateService/SoftwareInventory`|Collection of [SoftwareInventory](#softwareinventory-v1_0_0-softwareinventory)|
|`/redfish/v1/UpdateService/SoftwareInventory/{item}`|[SoftwareInventory](#softwareinventory-v1_0_0-softwareinventory)|
|`/redfish/v1/UpdateService/UpdateTaskQueue`|Collection of [HpeComponentUpdateTask](#hpecomponentupdatetask-v1_0_2-hpecomponentupdatetask)|
|`/redfish/v1/UpdateService/UpdateTaskQueue/{item}`|[HpeComponentUpdateTask](#hpecomponentupdatetask-v1_0_2-hpecomponentupdatetask)|
