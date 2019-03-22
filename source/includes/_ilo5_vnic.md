# Managing the iLO Redfish Host Interface ("Virtual NIC")
iLO 5 1.40 adds a virtual network interface to access iLO's HTTPS resources (including the Redfish API and the Web GUI) to the host.  This interface is disabled by default in Gen10 servers but may be enabled by default in future servers.

When accessing iLO 5 through the virtual network interface, authentication is enforced.

## Enabling the Virtual NIC
The Virtual NIC (also known as the Redfish Host API) is disabled by default but may be enabled either though the Web GUI or by a Redfish operation.  An iLO reset is required for this change to take effect.

> PATCH /redfish/v1/Managers/{managerId}/

```json
{
    "Oem": {
        "Hpe": {
            "VirtualNICEnabled": true
        }
    }
}
```

## Using the Virtual NIC
When enabled, software running on the server operating system may access the iLO 5 Web GUI or Redfish API using IP address `16.1.15.1`.  Normal authentication is required.

**NOTE:  The Virtual NIC does NOT act as a passthru to traffic on the iLO 5 network connection.  It is a separate network connection into iLO's resources.**

## Disabling the Virtual NIC
The Virtual NIC may be disabled either though the Web GUI or by a Redfish operation.  An iLO reset is required for this change to take effect.

> PATCH /redfish/v1/Managers/{managerId}/

```json
{
    "Oem": {
        "Hpe": {
            "VirtualNICEnabled": false
        }
    }
}
```
