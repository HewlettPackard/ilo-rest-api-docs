# One-button secure erase

<aside class="warning">

* **One-button secure erase should be used with extreme caution, and only when a system is being decommissioned.** The One-button secure erase process resets iLO and deletes all licenses stored there, resets BIOS settings, and deletes all AHS and warranty data stored on the system. The secure erase process also erases supported non-volatile storage data and deletes any deployment settings profiles. iLO reboots multiple times after the process is initiated.

* **Disconnect any FCoE, iSCSI, external SAS, and Fibre Channel storage before using One-button secure erase.**

**NOTE: Securely erasing the server can take up to a day to complete.**

</aside>


One-button secure erase erases supported non-volatile storage data and returns the server to the
manufacturing default state. The feature complies with specification NIST SP 800-88 Rev.1 (Dec. 2014). For more information about NIST SP 800-88, see https://nvlpubs.nist.gov/nistpubs/specialpublications/nist.sp.800-88r1.pdf.

To view what was erased successfully, view the ROM displays. The process can take up to a day to fully erase and reset all user data.  When you activate One-button secure erase, iLO 5 does not allow firmware update or reset operations. **DO NOT perform any iLO 5 configuration changes until this process is completed.**

## Prerequisites
* User account must have all iLO 5 permissions, including `SystemRecoveryConfigPriv`.
* iLO Advanced license.
* Set the iLO security setting on the system maintenance switch to the OFF position.
* Disconnect any FCoE, iSCSI, external SAS, and Fibre Channel storage before using One-button secure erase.
* Disable **Server Configuration Lock**.  For instructions, see the *UEFI System Utilities User Guide for HPE ProLiant Gen10 Servers and HPE Synergy*.
* Disable **Smart Storage Encryption**.  For instructions, see the "Clearing the encryption configuration" section in the *HPE Smart Array SR Secure Encryption Installation and User Guide*.
* For c-Class and Synergy users:  Remove HPE OneView or Virtual Connect profiles assigned to the system.


## Process Flow

1. User initiates One-button secure erase
2. Upon reboot, BIOS erases configuration, system time, TPM configuration and user data (drives and persistent memory).  The system powers off after completion
3. iLO 5 then erases key NVRAM and NAND data, and then automatically resets.

## Initiating One-button secure erase from the REST API

Execute the `HpeComputerSystemExt.SecureSystemErase` action on the computer system resource.

> POST `/redfish/v1/Systems/{id}/Actions/Oem/Hpe/#HpeComputerSystemExt.SecureSystemErase`

```json
{
    "SystemROMAndiLOErase": true,
    "UserDataErase": true
}
```

This returns a response indicating that a server system reset is required.

> returns

```json
{
    "error": {
        "code": "iLO.0.10.ExtendedInfo",
        "message": "See @Message.ExtendedInfo for more information.",
        "@Message.ExtendedInfo": [
            {
                "MessageId": "iLO.2.7.SystemResetRequired"
            }
        ],
    }
}
```

The client must then initiate a server reset using the Reset action in the ComputerSystem resourse.

> POST `/redfish/v1/Systems/{id}/Actions/ComputerSystem.Reset`

```json
{
    "ResetType": "ForceRestart"
}
```
At this point the UEFI BIOS will begin erasing configuration information.

## Impacts to the server after One-button secure erase completes

The server will need to be re-provisioned to be used after this operation.

* All data on impacted storage drives and persistent memory will be erased and is not recoverable.
  * All RAID settings, disk partitions and OS installations will be lost.

* BIOS and iLO 5 settings will be reset to defaults
  * iLO 5 network and other settings will need to be reconfigured.
  * iLO 5 Language Pack will be removed and iLO 5 will respond in English only.
  * iLO 5 license reverts to “Standard”.
  * The System Recovery Set will need to be recreated.
  * iLO 5 user accounts will be removed and will revert to the default factory Administrator account and password.
  * Active Health System, Integrated Management Log, and iLO 5 Event Logs will be cleared.
  * BIOS and SmartStorage Redfish API data will be removed and recreated on the next boot.
  * Secure Boot will be disabled and any enrolled certificates will be removed (other than the factory installed certificates).
  * Boot options and BIOS User Defined Defaults are removed.
  * Passwords, pass-phrases and/or encryption keys stored in the TPM or BIOS will be removed.
  * Date, time, DST, and time zone will be reset.
  * System will boot the most recent BIOS revision flashed.
* Intelligent Provisioning will not boot and will need to be reinstalled.

## Troubleshooting

In some situations the One-button secure erase function may return an HTTP 500 Internal Server Error.

> HTTP 500 Internal Server Error


```json
{
    "error": {
        "code": "iLO.0.10.ExtendedInfo",
        "message": "See @Message.ExtendedInfo for more information.",
        "@Message.ExtendedInfo": [
            {
                "MessageId": "Base.1.0.InternalError"
            }
        ],
    }
}

```
In the event of this error:

1)	Check if the installed BIOS firmware supports One-button secure erase. Note: This feature is supported only on Gen10 servers and above that have been updated with SPP version 2019.03.0 or later.
2)	If the system is already updated with the correct BIOS firmware version, then reboot the server. Once the system booted, execute the One-button secure erase again using POST action URI.

For more troubleshooting tips and One-button secure erase FAQ, please refer *“Intelligent Provisioning User Guide for HPE ProLiant Gen10 Servers and HPE Synergy”*
https://support.hpe.com/hpsc/doc/public/display?docId=a00017037en_us 
