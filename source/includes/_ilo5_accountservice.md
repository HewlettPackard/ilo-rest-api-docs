# Managing iLO 5 Users
iLO 5 supports both local user authentication as well as directory authentication.

iLO 5 1.40 adds:

* Role based local user administration via Redfish
* Directory Authentication configuration via Redfish

All user account modifications require the client to be authenticated with the "Administer User Accounts" privilege (`UserConfigPriv` in the Redfish `ManagerAccount`)

## Local User Administration
iLO 5 has a local user database enabling consistent user management for all interfaces including the Web interface (GUI) as well as the Redfish API.  The iLO 5 local user accounts are managed in the AccountService (`/redfish/v1/AccountService`).  An `Accounts` collection in the AccountService enables clients to create, modify, or remove local user accounts.

> `GET /redfish/v1/AccountService/Accounts/`

```json
{
    "@odata.context": "/redfish/v1/$metadata#ManagerAccountCollection.ManagerAccountCollection",
    "@odata.etag": "W/\"21C260DB\"",
    "@odata.id": "/redfish/v1/AccountService/Accounts/",
    "@odata.type": "#ManagerAccountCollection.ManagerAccountCollection",
    "Description": "iLO User Accounts",
    "Name": "Accounts",
    "Members": [
        {
            "@odata.id": "/redfish/v1/AccountService/Accounts/1/"
        }
    ],
    "Members@odata.count": 1
}
```

A local user account consists of a user name, password, and a set of privileges.  The `RoleId` describes one of three defined Redfish roles based upon assigned privileges.  The `Oem/Hpe/LoginName` property is a description of the account.

NOTE:  Due to a terminology mismatch between the Redfish standard and historical iLO products, the Properties for `UserName` and `LoginName` are reversed in Redfish vs. the iLO 5 Web interface:

|Redfish Property|GUI Term|Description|Example|
|---|---|---|---|
|UserName|Login Name|The user identity string used with a password to log into iLO 5|jsmith|
|Oem/Hpe/LoginName|User Name|The descriptive name of the user|Jane Smith - Director of IT|


> `GET /redfish/v1/AccountService/Accounts/1/`

```json
{
    "@odata.context": "/redfish/v1/$metadata#ManagerAccount.ManagerAccount",
    "@odata.etag": "W/\"D9DF9F68\"",
    "@odata.id": "/redfish/v1/AccountService/Accounts/1/",
    "@odata.type": "#ManagerAccount.v1_1_3.ManagerAccount",
    "Id": "1",
    "Description": "iLO User Account",
    "Links": {
        "Role": {
            "@odata.id": "/redfish/v1/AccountService/Roles/Administrator/"
        }
    },
    "Name": "User Account",
    "Oem": {
        "Hpe": {
            "@odata.context": "/redfish/v1/$metadata#HpeiLOAccount.HpeiLOAccount",
            "@odata.type": "#HpeiLOAccount.v2_2_0.HpeiLOAccount",
            "LoginName": "Jane Smith - Director of IT",
            "Privileges": {
                "HostBIOSConfigPriv": true,
                "HostNICConfigPriv": true,
                "HostStorageConfigPriv": true,
                "LoginPriv": true,
                "RemoteConsolePriv": true,
                "SystemRecoveryConfigPriv": true,
                "UserConfigPriv": true,
                "VirtualMediaPriv": true,
                "VirtualPowerAndResetPriv": true,
                "iLOConfigPriv": true
            },
            "ServiceAccount": false
        }
    },
    "Password": null,
    "RoleId": "Administrator",
    "UserName": "jsmith"
}
```

> *Note that `Password` is always shown as `null` even though its PATCHable with a new password*

### Roles and Privileges

iLO 5 uses a set of privileges assigned to each user account to grant and restrict access to features.  iLO 5's privileges are:

|Redfish|iLO Web Interface (GUI)|
|---|---|
|LoginPriv|Login
|RemoteConsolePriv|Remote Console
|VirtualPowerAndResetPriv|Virtual Power and Reset
|VirtualMediaPriv|Virtual Media
|HostBIOSConfigPriv|Host BIOS
|iLOConfigPriv|Configure iLO Settings
|UserConfigPriv|Administer User Accounts
|HostNICConfigPriv|Host NIC
|HostStorageConfigPriv|Host Storage
|SystemRecoveryConfigPriv|Recovery Set

#### Roles
In iLO 5 1.40 and later, you can use `RoleId` to create users with specific starting privileges.

On a GET of the local user account, `RoleId` is synthesized based upon the enabled privileges.  iLO 5 does not store a separate `RoleId` value.  For this reason, modifications to raw privileges may or may not result in a changed `RoleId` based upon iLO's mapping

If the PATCH includes both `RoleID` and individual privileges, the privileges corresponding to the RoleId are assigned to the local user account first, and then the explicit privileges are assigned.

> `PATCH /redfish/v1/AccountService/Accounts/{accountId}`

```json
{
    "RoleId": "Administrator",
    "Oem": {
        "Hpe": {
            "Privileges": {
                "SystemRecoveryConfigPriv": true
            }
        }
    }
}
```
> will set all iLO 5 privileges as long as the account performing the operation already has sufficient privilege to grant these privileges.

#### Privileges granted on Local Account Creation by RoleId
|RoleId|Privileges|
|---|---|
|Administrator|HostBIOSConfigPriv, HostNICConfigPriv, HostStorageConfigPriv, LoginPriv, RemoteConsolePriv, UserConfigPriv, VirtualMediaPriv, VirtualPowerAndResetPriv, iLOConfigPriv|
|Operator|HostBIOSConfigPriv, HostNICConfigPriv, HostStorageConfigPriv, LoginPriv, RemoteConsolePriv, VirtualMediaPriv, VirtualPowerAndResetPriv|
|ReadOnly|LoginPriv|

#### RoleId shown on an existing Local User Account by Privilege
The `RoleId` reported is the smallest superset of assigned privileges.

|Privileges|RoleId|
|----|----|
|LoginPriv only|ReadOnly|
|iLOConfigPriv or UserConfigPriv or SystemRecoveryConfigPriv and anything else|Administrator|
|any other combination|Operator|

### Creating a new Local User Account
The simplest possible new local user account create operation is to POST to the Accounts collection.

> `PATCH /redfish/v1/AccountService/Accounts/{accountId}`

```json
{
    "UserName": "jsmith",
    "Password": "passwordexample"
}
```
This will create a user account `jsmith` with default `ReadOnly` RoleId and only the iLO 5 Login privilege.  Notice that `Oem/Hpe/LoginName` defaults to the provided `UserName` unless it is specifically specified.

**NOTE:  Each local user account must have a unique `UserName`**

> `GET /redfish/v1/AccountService/Accounts/{accountId}`

```json
{
    "@odata.context": "/redfish/v1/$metadata#ManagerAccount.ManagerAccount",
    "@odata.etag": "W/\"B103601C\"",
    "@odata.id": "/redfish/v1/AccountService/Accounts/12/",
    "@odata.type": "#ManagerAccount.v1_1_3.ManagerAccount",
    "Id": "12",
    "Description": "iLO User Account",
    "Links": {
        "Role": {
            "@odata.id": "/redfish/v1/AccountService/Roles/ReadOnly/"
        }
    },
    "Name": "User Account",
    "Oem": {
        "Hpe": {
            "@odata.context": "/redfish/v1/$metadata#HpeiLOAccount.HpeiLOAccount",
            "@odata.type": "#HpeiLOAccount.v2_2_0.HpeiLOAccount",
            "LoginName": "jsmith",
            "Privileges": {
                "HostBIOSConfigPriv": false,
                "HostNICConfigPriv": false,
                "HostStorageConfigPriv": false,
                "LoginPriv": true,
                "RemoteConsolePriv": false,
                "SystemRecoveryConfigPriv": false,
                "UserConfigPriv": false,
                "VirtualMediaPriv": false,
                "VirtualPowerAndResetPriv": false,
                "iLOConfigPriv": false
            },
            "ServiceAccount": false
        }
    },
    "Password": null,
    "RoleId": "ReadOnly",
    "UserName": "jsmith"
}
```

### Creating a new Account using a RoleId
In iLO 5 1.40 and later, you may specify a `RoleId` with a new user account.

> `POST /redfish/v1/AccountService/Accounts/`

```json
{
    "UserName": "jsmith",
    "Password": "passwordexample",
    "RoleId": "Operator"
}
```

> This results in:
> `GET /redfish/v1/AccountService/Accounts/{accountId}`

```json
{
    "@odata.context": "/redfish/v1/$metadata#ManagerAccount.ManagerAccount",
    "@odata.etag": "W/\"6C16FDE3\"",
    "@odata.id": "/redfish/v1/AccountService/Accounts/14/",
    "@odata.type": "#ManagerAccount.v1_1_3.ManagerAccount",
    "Id": "14",
    "Description": "iLO User Account",
    "Links": {
        "Role": {
            "@odata.id": "/redfish/v1/AccountService/Roles/Operator/"
        }
    },
    "Name": "User Account",
    "Oem": {
        "Hpe": {
            "@odata.context": "/redfish/v1/$metadata#HpeiLOAccount.HpeiLOAccount",
            "@odata.type": "#HpeiLOAccount.v2_2_0.HpeiLOAccount",
            "LoginName": "jsmith",
            "Privileges": {
                "HostBIOSConfigPriv": true,
                "HostNICConfigPriv": true,
                "HostStorageConfigPriv": true,
                "LoginPriv": true,
                "RemoteConsolePriv": true,
                "SystemRecoveryConfigPriv": false,
                "UserConfigPriv": false,
                "VirtualMediaPriv": true,
                "VirtualPowerAndResetPriv": true,
                "iLOConfigPriv": false
            },
            "ServiceAccount": false
        }
    },
    "Password": null,
    "RoleId": "Operator",
    "UserName": "jsmith"
}
```

### Creating a new Account with specific Privileges

You may also create a local user with specific privileges.

> `POST /redfish/v1/AccountService/Accounts/`

```json
{
    "UserName": "jsmith",
    "Password": "passwordexample",
    "Oem": {
    	"Hpe": {
    		"LoginName": "Director of IT",
    		"Privileges": {
	    		"LoginPriv": true,
	    		"VirtualMediaPriv": true,
	            "VirtualPowerAndResetPriv": true
    		}
    	}
    }
}
```

> This results in the following new local user account:
> `GET /redfish/v1/AccountService/Accounts/{accountId}`

```json
{
    "@odata.context": "/redfish/v1/$metadata#ManagerAccount.ManagerAccount",
    "@odata.etag": "W/\"E8037663\"",
    "@odata.id": "/redfish/v1/AccountService/Accounts/15/",
    "@odata.type": "#ManagerAccount.v1_1_3.ManagerAccount",
    "Id": "15",
    "Description": "iLO User Account",
    "Links": {
        "Role": {
            "@odata.id": "/redfish/v1/AccountService/Roles/Operator/"
        }
    },
    "Name": "User Account",
    "Oem": {
        "Hpe": {
            "@odata.context": "/redfish/v1/$metadata#HpeiLOAccount.HpeiLOAccount",
            "@odata.type": "#HpeiLOAccount.v2_2_0.HpeiLOAccount",
            "LoginName": "Director of IT",
            "Privileges": {
                "HostBIOSConfigPriv": false,
                "HostNICConfigPriv": false,
                "HostStorageConfigPriv": false,
                "LoginPriv": true,
                "RemoteConsolePriv": false,
                "SystemRecoveryConfigPriv": false,
                "UserConfigPriv": false,
                "VirtualMediaPriv": true,
                "VirtualPowerAndResetPriv": true,
                "iLOConfigPriv": false
            },
            "ServiceAccount": false
        }
    },
    "Password": null,
    "RoleId": "Operator",
    "UserName": "jsmith"
}
```
### Modifying a Local User Account
The following properties are modifiable on an existing local user account:
* `UserName`
* `Password` - this is always returned as null, but you may PATCH it with a value to change the password
* `RoleId` - PATCHing `RoleId` on an existing local user account will reset it’s existing privileges with those mapped to the RoleId.
* `Oem/Hpe/LoginName`
* `Oem/Hpe/Privileges/*` - any of the privileges may be modified with true or false

### Adding and Removing Privileges
Local user account privileges may be modified with a PATCH to the URI of the desired `ManagerAccount` resource.

> `PATCH /redfish/v1/AccountService/Accounts/{accountId}/`

```json
{
    "Oem": {
    	"Hpe": {
    		"Privileges": {
                "VirtualMediaPriv": true,
	            "VirtualPowerAndResetPriv": true
    		}
    	}
    }
}
```


### Changing Roles

> `PATCH /redfish/v1/AccountService/Accounts/{accountId}/`

```json
{
	"RoleId": "Operator"
}
```

> results in HTTPS status 200:

```json
{
    "error": {
        "code": "iLO.0.10.ExtendedInfo",
        "message": "See @Message.ExtendedInfo for more information.",
        "@Message.ExtendedInfo": [
            {
                "MessageId": "Base.1.0.AccountModified"
            }
        ]
    }
}
```

### Changing Password
Local user account passwords may be modified with a PATCH to the URI of the desired `ManagerAccount` resource.

> `PATCH /redfish/v1/AccountService/Accounts/{accountId}/`

```json
{
    "Password": "newpassword"
}
```

### Removing a Local User Account
A local user account can be removed with a DELETE to the URI of desired `ManagerAccount` resource

> `DELETE /redfish/v1/AccountService/Accounts/{accountId}/`

## Directory Authentication

### Enabling or Disabling Local User Accounts

> `PATCH /redfish/v1/AccountService/`

```json
{
	"LocalAccountAuth": "Disabled"
}
```
> or
```json
{
	"LocalAccountAuth": "Enabled"
}
```

**Note: Disabling local user accounts is not allowed if both Directory Authentication and Kerberos Authentication are disabled.**

### Configuring ActiveDirectory Authentication

> ```PATCH /redfish/v1/AccountService/```

> Example 1 (Using default ActiveDirectory server port 636):

```json
{
	"LDAP": {
        "ServiceEnabled": true,
        "ServiceAddresses": [
            "<Active Directory Server host name>"
        ]
    }
}
```

> Example 2 (Using explicit/custom ActiveDirectory server port):

```json
{
	"LDAP": {
        "ServiceEnabled": true,
        "ServiceAddresses": [
            "<Active Directory Server host name>:4646"
        ]
    }
}
```

### Configuring LDAP Authentication

> ```PATCH /redfish/v1/AccountService/```

> Example 1 (Using default OpenLDAP server port 636):

```json
{
    "LDAP": {
        "AccountProviderType": "LDAPService",
        "ServiceEnabled": true,
        "ServiceAddresses": [
            "<LDAP Server host name>"
        ]
    }
}
```

> Example 2 (Using explicit/custom OpenLDAP server port):

```json
{
    "LDAP": {
        "AccountProviderType": "LDAPService",
        "ServiceEnabled": true,
        "ServiceAddresses": [
            "<LDAP Server host name>:4646"
        ]
    }
}
```

### Disable ActiveDirectory and LDAP Authentication (Generic LDAP)

> ```PATCH /redfish/v1/AccountService/```

```json
{
    "LDAP": {
        "AccountProviderType": "ActiveDirectoryService",
        "ServiceEnabled": false,
    }
}
```

### Enable and Configure HPE Extended Schema Authentication (for ActiveDirectory only)

> ```PATCH /redfish/v1/AccountService/```

```json
{
    "LDAP": {
        "ServiceEnabled": true,
        "ServiceAddresses": [
            "<Active Directory Server host name>"
        ],
        "Authentication": {
            "Username": "CN=testdevice,CN=Users,DC=ilotest2,DC=com"
        }
    },
    "Oem": {
        "Hpe": {
            "DirectorySettings": {
                "LdapAuthenticationMode": "ExtendedSchema"
            }
        }
    }
}
```

### Add User Search Contexts

> ```PATCH /redfish/v1/AccountService/```

> Sample Payload-1 (Add two new User Search Contexts, with no existing User Search Context present):

```json
{
    "LDAP": {
        "LDAPService": {
            "SearchSettings": {
                "BaseDistinguishedNames": [
                    "CN=Users,DC=domain,DC=com",
                    "DC=domain,DC=com"
                ]
            }
        }
    }
}
```

> Sample Payload-2 (Add a new User Search Context, with two existing User Search Contexts present):

```json
{
    "LDAP": {
        "LDAPService": {
            "SearchSettings": {
                "BaseDistinguishedNames": [
                    "CN=Users,DC=domain,DC=com",
                    "DC=domain,DC=com",
                    "DC=testdomain,DC=com"
                ]
            }
        }
    }
}
```

### Delete User Search Contexts

> ```PATCH /redfish/v1/AccountService/```

> Sample Payload-1 (To delete one/multiple User Search Contexts):

> Assume you have three existing User Search Contexts, e.g. "CN=Users,DC=domain,DC=com", "DC=domain,DC=com" and "DC=testdomain,DC=com". To delete one, exclude it from the payload and keep the ones to be retained.

```json
{
    "LDAP": {
        "LDAPService": {
            "SearchSettings": {
                "BaseDistinguishedNames": [
                    "CN=Users,DC=domain,DC=com",
                    "DC=domain,DC=com"
                ]
            }
        }
    }
}
```

> Sample Payload-2 (To delete all User Search Contexts):

```json
{
    "LDAP": {
        "LDAPService": {
            "SearchSettings": {
                "BaseDistinguishedNames": [
                    ""
                ]
            }
        }
    }
}
```

### Import LDAP Server CA Certificate

> ```POST /redfish/v1/AccountService/ExternalAccountProviders/LDAP/Certificates/```

```json
{
    "CertificateString": "-----BEGIN CERTIFICATE-----
MIIEHTCCAwWgAwIBAgIQe8LmWgF5edKw01/avJg69DANBgkqhkiG9w0BAQsFADCB
…………………………………………………………………………………………………………………………………
…………………………………………………………………………………………………………………………………
Ow==
-----END CERTIFICATE-----"
}
```

### View LDAP Server CA Certificate Status

```GET /redfish/v1/AccountService/```

The property ```Oem/Hpe/DirectorySettings/LdapCaCertificateLoaded``` indicates the status of the certificate.

### View LDAP Server CA Certificate Details

> ```GET /redfish/v1/AccountService/ExternalAccountProviders/LDAP/Certificates/{certId}/```

> **NOTE:  The LDAP provider supports a single certficate**

```json
{
    "@odata.context": "/redfish/v1/$metadata#Certificate.Certificate",
    "@odata.etag": "W/\"A1110A63\"",
    "@odata.id": "/redfish/v1/AccountService/ExternalAccountProviders/LDAP/Certificates/1/",
    "@odata.type": "#Certificate.v0_9_0.Certificate",
    "Id": "1",
    "Issuer": "/C=US/O=Hewlett Packard Enterprise Company/OU=Infrastructure Services/CN=Hewlett Packard Enterprise Private Root CA",
    "Name": "LDAP Certificate",
    "SerialNumber": "7BC2E65A017979D2B0D35FDABC983AF4",
    "Subject": "/C=US/O=Hewlett Packard Enterprise Company/OU=Infrastructure Services/CN=Hewlett Packard Enterprise Private Root CA",
    "ValidNotAfter": "2025-03-16T23:59:59Z",
    "ValidNotBefore": "2015-03-17T00:00:00Z"
}
```

### Add new Directory Groups (No Existing Groups)

> ```PATCH /redfish/v1/AccountService/```

> Sample Payload: “Administrator” and “Operator” are predefined Redfish RoleIds. “LDAP” can also be used instead of “ActiveDirectory”.

```json
{
    "ActiveDirectory": {
        "RemoteRoleMapping": [
            {
                "LocalRole": "Administrator",
                "RemoteGroup": "TestGroup1"
            },
            {
                "LocalRole": "Operator",
                "RemoteGroup": "TestGroup2"
            }
        ]
    }
}
```

### View Directory Groups

> ```GET /redfish/v1/AccountService/```

> See the properties under ```RemoteRoleMapping``` created by the Add operation (fragment of the response):

```json
{
    "RemoteRoleMapping": [
        {
            "LocalRole": "dirgroup4c6c827762dd20dc530c52ef",
            "RemoteGroup": "TestGroup1"
        },
        {
            "LocalRole": "dirgroupeb9a3afc9cd9d126249c3aed",
            "RemoteGroup": "TestGroup2"
        }
    ]
}
```

### Add New Directory Groups to Existing Groups

> ```PATCH /redfish/v1/AccountService/```

> Assume two directory groups (TestGroup1 and TestGroup2 as in the steps above) are present. Use the LocalRole and RemoteGroup values for the existing directory groups from the step above in the payload. Add an additional group “TestGroup3” with “ReadOnly” Redfish Role. “LDAP” can also be used instead of “ActiveDirectory”.

```json
{
    "ActiveDirectory": {
        "RemoteRoleMapping": [
            {
                "LocalRole": "dirgroup4c6c827762dd20dc530c52ef",
                "RemoteGroup": "TestGroup1"
            },
            {
                "LocalRole": "dirgroupeb9a3afc9cd9d126249c3aed",
                "RemoteGroup": "TestGroup2"
            },
            {
                "LocalRole": "ReadOnly",
                "RemoteGroup": "TestGroup3"
            }
        ]
    }
}
```

### Delete Directory Groups

> ```PATCH /redfish/v1/AccountService/```

> Sample Payload-1 (To delete one/multiple Directory Groups):
Assume you have three existing directory groups, e.g. "TestGroup1", "TestGroup2" and "TestGroup3". To delete "TestGroup3", exclude it from the payload and keep the ones to be retained. “LDAP” can also be used instead of “ActiveDirectory”.

```json
{
    "ActiveDirectory": {
        "RemoteRoleMapping": [
            {
                "LocalRole": "dirgroup4c6c827762dd20dc530c52ef",
                "RemoteGroup": "TestGroup1"
            },
            {
                "LocalRole": "dirgroupeb9a3afc9cd9d126249c3aed",
                "RemoteGroup": "TestGroup2"
            }
        ]
    }
}
```

> Sample Payload-2 (To delete all Directory Groups): “LDAP” can also be used instead of “ActiveDirectory”.

```json
{
    "ActiveDirectory": {
        "RemoteRoleMapping": [
            {}
        ]
    }
}
```

### View Directory Group Privileges

> ```GET /redfish/v1/AccountService/Roles/```

```json
{
    "@odata.context": "/redfish/v1/$metadata#RoleCollection.RoleCollection",
    "@odata.etag": "W/\"08A22FCA\"",
    "@odata.id": "/redfish/v1/AccountService/Roles/",
    "@odata.type": "#RoleCollection.RoleCollection",
    "Description": "iLO Roles Collection",
    "Name": "Roles",
    "Members": [
        {
            "@odata.id": "/redfish/v1/AccountService/Roles/Administrator/"
        },
        {
            "@odata.id": "/redfish/v1/AccountService/Roles/Operator/"
        },
        {
            "@odata.id": "/redfish/v1/AccountService/Roles/ReadOnly/"
        },
        {
            "@odata.id": "/redfish/v1/AccountService/Roles/dirgroup4c6c827762dd20dc530c52ef/"
        },
        {
            "@odata.id": "/redfish/v1/AccountService/Roles/dirgroupeb9a3afc9cd9d126249c3aed/"
        }
    ],
    "Members@odata.count": 5
}
```

> ```GET /redfish/v1/AccountService/Roles/{directoryGroupId}/```

```json
{
    "@odata.context": "/redfish/v1/$metadata#Role.Role",
    "@odata.etag": "W/\"D17157B3\"",
    "@odata.id": "/redfish/v1/AccountService/Roles/dirgroup4c6c827762dd20dc530c52ef/",
    "@odata.type": "#Role.v1_2_1.Role",
    "Id": "dirgroup4c6c827762dd20dc530c52ef",
    "AssignedPrivileges": [
        "Login",
        "ConfigureSelf",
        "ConfigureManager",
        "ConfigureUsers"
    ],
    "Description": "iLO Directory Group Role",
    "IsPredefined": false,
    "Name": "Group Role",
    "Oem": {
        "Hpe": {
            "@odata.context": "/redfish/v1/$metadata#HpeDirectoryGroup.HpeDirectoryGroup",
            "@odata.type": "#HpeDirectoryGroup.v1_0_0.HpeDirectoryGroup",
            "GroupDn": "TestGroup1",
            "GroupSid": ""
        }
    },
    "OemPrivileges": [
        "RemoteConsolePriv",
        "VirtualMediaPriv",
        "VirtualPowerAndResetPriv",
        "HostBIOSConfigPriv",
        "HostNICConfigPriv",
        "HostStorageConfigPriv"
    ],
    "RoleId": "dirgroup4c6c827762dd20dc530c52ef"
}
```

### Modify Directory Group Privileges

> ```PATCH /redfish/v1/AccountService/Roles/{directoryGroupId}/```

> Sample Payload-1 (Update AssignedPrivileges): Add/Remove the privileges in the AssignedPrivileges[] array.

```json
{
    "AssignedPrivileges": [
        "Login",
        "ConfigureSelf",
        "ConfigureUsers"
    ]
}
```

> Sample Payload-2 (Update OemPrivileges): Add/Remove the privileges in the OemPrivileges[] array.

```json
{
    "OemPrivileges": [
        "RemoteConsolePriv",
        "VirtualPowerAndResetPriv",
        "HostNICConfigPriv",
        "HostStorageConfigPriv"
    ]
}
```

### Enable, Configure, Disable Kerberos Authentication

> ```PATCH /redfish/v1/AccountService/```

> Disable

```json
{
    "ActiveDirectory": {
        "ServiceEnabled": false
    }
}
```

> Enable Sample Payload-1 (Using default KDC server port 88):

> Where `“TESTKDCREALM.COM”` is the Kerberos Realm.

```json
{
    "ActiveDirectory": {
        "ServiceEnabled": true,
        "ServiceAddresses": [
            "testkdc.hpe.com@TESTKDCREALM.COM"
        ]
    }
}
```

> Enable Sample Payload-2 (Using explicit/custom KDC server port):

```json
{
    "ActiveDirectory": {
        "ServiceEnabled": true,
        "ServiceAddresses": [
            "testkdc.hpe.com:8888@TESTKDCREALM.COM"
        ]
    }
}
```

### Import Kerberos Keytab File

> ```POST /redfish/v1/AccountService/Actions/Oem/Hpe/HpeiLOAccountService.ImportKerberosKeytab/```

```json
{
    "ImportUri": "http://<URI of keytab file>"
}
```

## Start Directory Test

> ```POST on /redfish/v1/AccountService/DirectoryTest/Actions/HpeDirectoryTest.StartTest/```

> Sample Payload-1 (No parameters):

```json
{
}
```

> Sample Payload-2 (with Test User Name and password):

```json
{
	"TestUserName": "TestUser1",
	"TestUserPassword": "TestPassword1"
}
```

> Sample Payload-3 (with all parameters):

```json
{
	"TestUserName": "TestUser1",
	"TestUserPassword": "TestPassword1",
	"DirectoryAdminDn": "CN=Administrator,CN=Users,DC=ilotest2,DC=com",
	"DirectoryAdminPassword": "AdminPassword"
}
```

### Stop Directory Test

> ```POST /redfish/v1/AccountService/DirectoryTest/Actions/HpeDirectoryTest.StopTest/```

> (empty payload)

```json
{
}
```

### View Directory Test Result

> ```GET /redfish/v1/AccountService/DirectoryTest/```

```json
{
    "@odata.context": "/redfish/v1/$metadata#HpeDirectoryTest.HpeDirectoryTest",
    "@odata.etag": "W/\"6B3F28F1\"",
    "@odata.id": "/redfish/v1/AccountService/DirectoryTest/",
    "@odata.type": "#HpeDirectoryTest.v1_0_0.HpeDirectoryTest",
    "Id": "DirectoryTest",
    "Actions": {
        "#HpeDirectoryTest.StartTest": {
            "target": "/redfish/v1/AccountService/DirectoryTest/Actions/HpeDirectoryTest.StartTest/"
        },
        "#HpeDirectoryTest.StopTest": {
            "target": "/redfish/v1/AccountService/DirectoryTest/Actions/HpeDirectoryTest.StopTest/"
        }
    },
    "OverallStatus": "NotRun",
    "TestResults": [
        {
            "Notes": "",
            "Status": "NotRun",
            "TestName": "Directory Server DNS Name"
        },
        {
            "Notes": "",
            "Status": "NotRun",
            "TestName": "Ping Directory Server"
        },
        {
            "Notes": "",
            "Status": "NotRun",
            "TestName": "Connect to Directory Server"
        },
        {
            "Notes": "",
            "Status": "NotRun",
            "TestName": "Connect using SSL"
        },
        {
            "Notes": "",
            "Status": "NotRun",
            "TestName": "Bind to Directory Server"
        },
        {
            "Notes": "",
            "Status": "NotRun",
            "TestName": "Directory Administrator login"
        },
        {
            "Notes": "",
            "Status": "NotRun",
            "TestName": "User Authentication"
        },
        {
            "Notes": "",
            "Status": "NotRun",
            "TestName": "User Authorization"
        },
        {
            "Notes": "",
            "Status": "NotRun",
            "TestName": "Directory User Contexts"
        },
        {
            "Notes": "",
            "Status": "NotRun",
            "TestName": "LOM Object exists"
        }
    ]
}
```

