# Introduction

The iLO RESTful API for HPE iLO 5 is a programming interface enabling state-of-the-art server management. This document contains helpful information about how to interact with the iLO RESTful API. The iLO RESTful API uses the basic HTTP operations (GET, PUT, POST, DELETE, and PATCH) to submit or return a JSON formatted resource to or from a URI on iLO 5.

With modern scripting languages, you can easily write simple REST clients for RESTful APIs. Most languages, like Python, can transform JSON into internal-data structures, like dictionaries, allowing for easy access to data. This enables you to write custom code directly to the iLO RESTful API, instead of using intermediate tools such as HPE’s HPQLOCFG or CONREP.
 
## Redfish Conformance

iLO 5's Redfish conformance details are available in this document in the "**iLO 5 Adaptation Guide**" section.

## iLO 5 1.40 New Features and Changes

iLO 5 1.40 adds support for several Redfish features:

* Redfish 1.6 support for the OpenAPI standard
* Support for the `?only` query parameter for easier access to key data
* Directory Services Configuration (`ExternalAccountProvider`)
* Local account roles (`Role`)
* TelemetryService support for CPU utilization (`TelemetryService`)
* Persistent Memory support (`MemoryDomains` and `MemoryChunks`)
* Improved `EthernetInterfaces` implementation for iLO's network
* Redfish host interface

Additionally, it includes support for new iLO 5 1.40 features:

* One-button secure erase (in `ComputerSystem` HPE OEM schema)
* iLO Configuration Backup and Restore (new `HpeiLOBackupRestoreService` HPE OEM schema)
* Configuration support for firmware downgrade policy (in `UpdateService` HPE OEM schema)
* Workload Performance advisor (new `HpeWorkloadPerformanceAdvisor` HPE OEM schema)

### Redfish 1.6 and OpenAPI

iLO 5 version 1.40 and later is conformant with the new Redfish 1.6 requirement to fix certain resource URIs in the data model.

Several resource URIs have been changed to conform to Redfish 1.6.  A properly written Redfish client which traverses the data model and finds the URIs dynamically should not be affected, but clients which make assumptions about URIs may require modififications.

#### Trailing Slashes on URIs

iLO 5 versions prior to 1.40 would return an HTTP 308 Redirect back to clients who requested URIs without a trailing slash.  Clients must follow 308 Redirect to the alternate URI (the same URI path with a trailing slash.)  In order to conform to Redfsh 1.6, iLO 5 1.40 changes this behavior and aliases the same resources at both URIs.  Requesting a URI with or without a trailing slash will return similar results with the exception that URIs in the returned data will be different.  GETs of URIs with trailing slash will return links (@odata.id) with trailing slashes, and GETs of URIs without trailing slashes will return links without trailing slashes.

|Version|Behavior|
|---|---|
|1.10-1.3x|`GET /redfish/v1/Systems` redirects (308) to `/redfish/v1/Systems/`|
|1.40-later|`GET /redfish/v1/Systems` returns result similar to `GET /redfish/v1/Systems/`|

#### Changed URIs

The following URIs have changed in iLO 5 1.40 and later to conform to Redfish 1.6:

|Old URI in iLO 5 1.10-1.3x|New URI Required by Redfish 1.6|
|---|---|
|`/redfish/v1/Chassis/{chassisId}/Drives/{interface}/{driveId}`|`/redfish/v1/Chassis/{systemId}/Drives/{driveId}`|
|`/redfish/v1/Systems/{systemId}/Storage/{interface}/{storageId}`|`/redfish/v1/Systems/{systemId}/Storage/{storageId}`|
|`/redfish/v1/Systems/{systemId}/Storage/{interface}/{storageId}/Volumes/{volumeId}`|`/redfish/v1/Systems/{systemId}/Storage/{storageId}/Volumes/{volumeId}`|
|`/redfish/v1/Systems/{systemId}/NetworkInterfaces/{nId}/NetworkDeviceFunctions/{ndfId}`|`/redfish/v1/Chassis/{chassisId}/NetworkAdapters/{nId}/NetworkDeviceFunctions/{ndfId}`|
|`/redfish/v1/Systems/{systemId}/NetworkInterfaces/{nicId}/NetworkPorts/{nportId}`|`/redfish/v1/Chassis/{chassisId}/NetworkAdapters/{Id}/NetworkPorts/{nportId}`|
|`/redfish/v1/Schemas/{Id}/`|`/redfish/v1/JsonSchemas/{Id}`|
|`/redfish/v1/Schemas/`|`/redfish/v1/JsonSchemas`|
|`/redfish/v1/Managers/{managerId}/NetworkService/`|`/redfish/v1/Managers/{managerId}/NetworkProtocol`|

#### New `?only` Query Parameter
Starting in iLO 5 1.40, appending `?only` to GETs on single-member collections returns the one and only member instead.  This is a convenient and efficient way to get to important data faster.

`GET /redfish/v1/Systems?only` returns the one and only `ComputerSystem` resource instead of the collection that includes it.

This works for collections that have only one member.  Otherwise the GET returns the collection as if the query parameter was omitted.

## Key benefits of the iLO RESTful API

The iLO RESTful API is becoming the main management interface for Hewlett Packard Enterprise servers with iLO 5. Its feature set will become larger than the existing iLO XML API (RIBCL) and IPMI interfaces. Using the iLO RESTful API, you can take full inventory of the server, control power and reset, configure BIOS and iLO settings, fetch event logs, as well as many other functions.

The iLO RESTful API follows the trend of the Internet in moving to a common pattern for new software interfaces. Many web services in a variety of industries use REST APIs because they are easy to implement, easy to consume, and offer scalability advantages over previous technologies.

HPE OneView, OpenStack, and many other server management APIs are now REST APIs. Most Hewlett Packard Enterprise Management software offerings, as well as the entire Software Defined Infrastructure, are built upon REST APIs.

The iLO RESTful API has the additional advantage of consistency across all present and projected server architectures. The same data model works for traditional rack-mount servers, blades, as well as newer types of systems. This advantage comes because the data model is designed to self-describe the service’s capabilities to the client and has room for flexibility designed in from the start

