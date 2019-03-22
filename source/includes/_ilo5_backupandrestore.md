# iLO Backup and Restore

The Backup & Restore feature allows you to restore the iLO configuration on a system with the same
hardware configuration as the system that was backed up. This feature is not meant to duplicate a
configuration and apply it to a different iLO system.

In general, it is not expected that you will need to perform an iLO restore operation. However, there are
cases in which having a backup of the configuration eases and expedites the return to a normal operating
environment.

As with any computer system, backing up your data is a recommended practice to minimize the impact
from failures. Hewlett Packard Enterprise recommends performing a backup each time that you update
the iLO firmware.

You might want to restore the iLO configuration in the following situations:

## Battery failure or removal

Various configuration parameters are stored in the battery-powered SRAM. Although rare, the battery
can fail. In some situations, battery removal and replacement might be required. To avoid the loss of
configuration information, restore the iLO configuration from a backup file after the battery is replaced.

## Reset to factory defaults

In some cases, you might need to reset iLO to the factory default settings to erase settings external to
iLO. Resetting iLO to the factory default settings erases the iLO configuration. To recover the iLO
configuration quickly, restore the configuration from a backup file after the reset to the factory default
settings is complete.

## Accidental or incorrect configuration change

In some cases, the iLO configuration might be changed incorrectly, causing important settings to be
lost. This situation might occur if iLO is set to the factory default settings or user accounts are deleted.
To recover the original configuration, restore the configuration from a backup file.

## System board replacement

If a system board replacement is required to address a hardware issue, you can use this feature to
transfer the iLO configuration from the original system board to the new system board.

## Lost license key

If a license key is accidentally replaced, or you reset iLO to the factory default settings, and you are
not sure which key to install, you can restore the license key and other configuration settings from a
backup file.

## What information is restored?

The iLO configuration includes many categories such as Power, Network, Security, the User Database,
and License Keys. Most configuration information is stored in the battery-powered SRAM memory device,
and it can be backed up and restored.

### Information that is not restored

Some information is not suitable to be restored. The information that cannot be restored is not part of the
iLO configuration, but instead is related to the iLO or server system state.

The following information is not backed up or restored:

* Security state—Allowing a restore operation to change the iLO security state would defeat the principles of security
and enforcement of security.
* Integrated Management Log—To preserve information about events that occurred between the backup and the time or event that
required the restore, this information is not restored.
* iLO Event Log—To preserve information about events that occurred between the backup and the time or event that
required the restore, this information is not restored.
* Active Health System data—To preserve the information recorded during the backup and restore process, this information is not
restored.
* Server state information— Server power state (ON/OFF), Server UID LED states, iLO and server clock settings.


## Backing up the iLO 5 configuration

> Find the information about the BackupRestoreService

> GET `/redfish/v1/Managers/1/BackupRestoreService`

```json
{
    "@odata.context": "/redfish/v1/$metadata#HpeiLOBackupRestoreService.HpeiLOBackupRestoreService",
    "@odata.etag": "W/\"D863AC37\"",
    "@odata.id": "/redfish/v1/Managers/1/BackupRestoreService",
    "@odata.type": "#HpeiLOBackupRestoreService.v2_2_0.HpeiLOBackupRestoreService",
    "Id": "BackupRestoreService",
    "BackupFileLocation": "/bkupdata/HPE_MXQ32200VV_20020928_0712.bak",
    "BackupFiles": {
        "@odata.id": "/redfish/v1/Managers/1/BackupRestoreService/BackupFiles"
    },
    "HttpPushUri": "/cgi-bin/uploadRestoreFile",
    "Name": "Backup Restore Service"
}
``` 

> GET the backup file based upon the `BackupFileLocation` URI

> GET `/bkupdata/HPE_MXQ32200VV_20020928_0712.bak`

The GET operation to the BackupFileLocation URI returns HTTP 200 with `Content Type: application/octet-stream`.  This is the binary image of the backup file.

## Restoring the iLO 5 configuration

> POST `/cgi-bin/uploadRestoreFile`

The content type of the POST must be Form Data and include the session key







