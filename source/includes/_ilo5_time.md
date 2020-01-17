# Managing Time in iLO 5

iLO 5 obtains the date and time from one of several sources and is not manually configurable.

* Network Time Protocol (NTP) Servers
* System UEFI during Boot
* BladeSystem C-Class Onboard Administrator

The configurable iLO 5 Time/Date related configuration properties are:

* Time zone
* Network Time Protocol Server addresses
* Option to synchronize the host to iLO 5's date and time during first boot after AC power is applied (`PropagateTimeToHost` boolean)

## iLO 5 Date and Time

iLO 5 current date and time is available in the main `Manager` resource at `/redfish/v1/Managers/{id}`

> GET /redfish/v1/Managers/{id}

```json
    "DateTime": "2019-01-06T17:11:53Z",
    "DateTimeLocalOffset": "-06:00",
```

### Date/Time Service Resource

A link exists in `/redfish/v1/Managers/{id}` to the iLO 5 Date/Time Service.  See `Oem/Hpe/Links/DateTimeService`.  This points to a DateTime resource at `/redfish/v1/Managers/{id}/DateTime`.

## Time Zone Management
Time Zone configuration is performed with a PATCH to the `DateTime` resource at `/redfish/v1/Managers/{id}/DateTime`.

The available time zones are available in the `TimeZoneList` property.  Take note of the `Index` value of the time zone you wish iLO 5 to be configured with.  Then `PATCH` the `TimeZone.Index` property:

> PATCH /redfish/v1/Managers/{id}/DateTime

```json
{
    "TimeZone": {
        "Index": 4
    }
}
```

If the operation is successful, iLO 5 will respond with `HTTP 200 OK` and `ResetRequired`.  An iLO 5 reset is required for date and time operations to be applied.  After a successful PATCH the `ConfigurationSettings` property will contain `SomePendingReset` indicating that some settings have changed but will not take effect until iLO 5 is reset.

If the time zone is configured to be managed by DHCP, iLO 5 will respond with `HTTP 400` and `SNTPConfigurationManagedByDHCPAndIsReadOnly` (see Using DHCP Supplied Time Settings).

## Configuring Network Time Protocol (NTP)
The currently configured Network Time Protocol (NTP) servers are available in the `DateTime` resource at `/redfish/v1/Managers/{id}/DateTime`.

> GET /redfish/v1/Managers/{id}/DateTime

```json
{
    "NTPServers": [
        "<NTP server 1>",
        "<NTP server 2>"
    ]
}
```

If NTP is not being managed by DHCP, you may PATCH server addresses into the `StaticNTPServers` array.

> PATCH /redfish/v1/Managers/{id}/DateTime

```json
{
    "StaticNTPServers": [
        "<NTP server 1>",
        "<NTP server 2>"        
    ]
}
```

> or to set one address

```json
{
    "StaticNTPServers": [
        "<NTP server 1>"
    ]
}
```


If the operation is successful, iLO 5 will respond with `HTTP 200 OK` and `ResetRequired`.  An iLO 5 reset is required for date and time operations to be applied.  After a successful PATCH the `ConfigurationSettings` property will contain `SomePendingReset` indicating that some settings have changed but will not take effect until iLO 5 is reset.

If the time zone is configured to be managed by DHCP, iLO 5 will respond with `HTTP 400` and `SNTPConfigurationManagedByDHCPAndIsReadOnly` (see Using DHCP Supplied Time Settings).
