# Managing Apollo Drive Bay Mapping
The HPE Apollo 2000 System with the HPE Apollo r2800 Chassis (including the Storage Expander Backplane) supports 24 SFF HPE SmartDrives. The SFF drive bays can be assigned to specific server nodes.

**CAUTION: Changing the drive bay mapping configuration might cause data loss or data corruption. For example, consider a configuration with drive bays two through seven assigned to node 1, with the drives configured as a RAID0 volume. Data corruption might occur if you change the drive bay mapping so that the configured drives are no longer available.**

## Prerequisites
* HPE iLO 5 firmware 1.20 or later 
* Storage enclosure processor firmware 1.00 or later
* Chassis firmware 1.2.10 or later

## Getting host port topology details
The HostPortsInfo JSON object displays the node number and SAS controller associated with each server host port. Before you change the drive bay mapping, HPE recommends using the following REST API to view and understand the PortNumber mapping: 
> GET /redfish/v1/Chassis/1/AccHddService

>This action returns the HostPortsInfo JSON object.

```json
{
    "HostPortsInfo": [
        {
            "NodeNumber": 1,
            "PortNumber": 1,
            "SlotNumber": 1
        },
        {
            "NodeNumber": 2,
            "PortNumber": 2,
            "SlotNumber": 1
        },
        {
            "NodeNumber": 3,
            "PortNumber": 3,
            "SlotNumber": 1
        },
        {
            "NodeNumber": 4,
            "PortNumber": 4,
            "SlotNumber": 1
        }
    ]
}
```

## Getting current and pending drive bay mapping

> GET /redfish/v1/Chassis/1/AccHddService/zone

This action returns the CurrentZoneConfiguration and PendingZoneConfiguration JSON objects.

> The CurrentZoneConfiguration JSON object displays the current drive bay mapping in the chassis.

```json
{
    "CurrentZoneConfiguration": {
        "HostPort": [
            {
                "BayNumber": [ 1, 2, 3, 4, 5, 6 ],
                "PortNumber": 1
            },
            {
                "BayNumber": [ 7, 8, 9, 10, 11, 12 ],
                "PortNumber": 2
            },
            {
                "BayNumber": [ 13, 14, 15, 16, 17, 18 ],
                "PortNumber": 3
            },
            {
                "BayNumber": [ 19, 20, 21, 22, 23, 24 ],
                "PortNumber": 4
            },
            {
                "PortNumber": null
            }
        ]
    }
}
```

***Note: The value PortNumber null indicates that a drive bay is not assigned.**

> The PendingZoneConfiguration JSON object displays the pending drive bay mapping configuration. This configuration will not be applied until all nodes remain powered off for at least 5 seconds.

```json
{
    "PendingZoneConfiguration": {
        "HostPort": [
            {
                "BayNumber": [ 1, 2, 3, 4 ],
                "PortNumber": 1
            },
            {
                "BayNumber": [ 7, 8, 9, 10 ],
                "PortNumber": 2
            },
            {
                "BayNumber": [ 13, 14, 15, 16 ],
                "PortNumber": 3
            },
            {
                "BayNumber": [ 19, 20, 21, 22 ],
                "PortNumber": 4
            },
            {
                "BayNumber": [ 5, 6, 11, 12, 17, 18, 23, 24 ],
                "PortNumber": null
            }
        ]
    }
}
```
***Note: The value PortNumber null indicates that a drive bay is not assigned.**

## Configuring drive bay mapping
You can make drive bay mapping configuration changes from any server node. The changes take effect when all server nodes in the Apollo 2000 system chassis are powered off and the Chassis firmware is able to reset the Storage Expander backplane. All nodes must remain powered off for at least 5 seconds after you initiate the configuration change.

The following example shows three drive bays assigned to each node.

> POST /redfish/v1/Chassis/1/AccHddService/Zone/Actions/HpeServerAccHddZone.ConfigureZone

```json
{
    "HostPort": [
      {
        "BayNumber": [
          1,
          2,
          3
        ],
        "PortNumber": 1
      },
      {
        "BayNumber": [
          7,
          8,
          9
        ],
        "PortNumber": 2
      },
      {
        "BayNumber": [
          13,
          14,
          15
        ],
        "PortNumber": 3
      },
      {
        "BayNumber": [
          19,
          20,
          21
        ],
        "PortNumber": 4
      }
    ]
}
```

This action returns a response indicating that all server nodes in the chassis must remain powered off for at least 5 seconds for the changes to take effect.

```json
{
    "error": {
        "code": "iLO.0.10.ExtendedInfo",
        "message": "See @Message.ExtendedInfo for more information.",
        "@Message.ExtendedInfo": [
            {
                "MessageId": "iLO.2.9.ChassisResetRequired"
            }
        ]
    }
}
```

## Setting drive bay mapping to the default configuration

The default configuration divides the 24 SFF drive bays by the number of server host ports in the Apollo 2000 Chassis. In a configuration with four 1U servers, the default drive bay configuration is six drive bays allocated to each of the four server slots. In a configuration with two 2U servers, the default drive bay configuration is 12 drive bays allocated to each of the two server slots.

POST an empty JSON object to URI to set drive bay mapping to the default configuration.

> POST /redfish/v1/Chassis/1/AccHddService/Zone/Actions/HpeServerAccHddZone.LoadDefault

```json
{}
```

This action returns a response indicating that all server nodes in the chassis must remain powered off for at least 5 seconds for the changes to take effect.

```json
{
    "error": {
        "code": "iLO.0.10.ExtendedInfo",
        "message": "See @Message.ExtendedInfo for more information.",
        "@Message.ExtendedInfo": [
            {
                "MessageId": "iLO.2.9.ChassisResetRequired"
            }
        ]
    }
}
```
