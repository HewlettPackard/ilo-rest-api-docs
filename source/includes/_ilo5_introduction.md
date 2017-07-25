# Introduction

The iLO RESTful API for HPE iLO 5 is a programming interface enabling state-of-the-art server management. This document contains helpful information about how to interact with the iLO RESTful API. The iLO RESTful API uses the basic HTTP operations (GET, PUT, POST, DELETE, and PATCH) to submit or return a JSON formatted resource to or from a URI on iLO 5.

With modern scripting languages, you can easily write simple REST clients for RESTful APIs. Most languages, like Python, can transform JSON into internal-data structures, like dictionaries, allowing for easy access to data. This enables you to write custom code directly to the iLO RESTful API, instead of using intermediate tools such as HPE’s HPQLOCFG or CONREP.
 
## Redfish Conformance

The iLO RESTful API was first released with iLO 4 2.00 on HPE Gen9 servers. The iLO RESTful API also functioned as the starting point for the new Redfish 1.0 DMTF standard at [http:// www.dmtf.org/standards/redfish](http://www.dmtf.org/standards/redfish)

Since the introduction of the iLO RESTful API, a number of changes were introduced into the Redfish standard by the DMTF SPMF members.

iLO 4 2.30 and later was the first generation of iLO to support the Redfish API.  Because the standard is moving, iLO 5 supports a 2nd generation REST API that removes portions that were not part of the standard, while keeping and enhancing the HPE extensions.

iLO 4 achieved Redfish 1.0 conformance and backward compatibility by:

1. Mirroring the resource model at both /redfish/v1/ and /rest/v1.
1. Returning both compatibility and Redfish properties by default.
1. Returning only Redfish conformant properties (with Hewlett Packard Enterprise extensions) if the Redfish-required OData header is included in the request (`OData-Version: 4.0`).

Full details on how Redfish 1.0 was implemented in iLO 4 2.30 and how it impacts clients written for previous versions is found here:  [http://www8.hp.com/h20195/V2/GetDocument.aspx?docname=4AA6-1727ENW&cc=us&lc=en](http://www8.hp.com/h20195/V2/GetDocument.aspx?docname=4AA6-1727ENW&cc=us&lc=en "Redfish Implementation on HP RESTful API for HPE iLO 4 - Technical White Paper")

iLO 5's Redfish conformance details are available in this document in the "**iLO 5 Adaptation Guide**" section.


## REST APIs Architected using HATEOS

Representational State Transfer (REST) is a web service that uses basic CRUD (Create, Read, Update, Delete, and Patch) operations performed on resources using HTTP commands such as POST, GET, PUT, PATCH, and DELETE. The iLO RESTful API is designed using a REST architecture called HATEOS (Hypermedia as the Engine of Application State). This architecture allows the client to interact with iLO through a simple fixed URL (rest/v1) and several other top-level URIs documented in the iLO Data Model. The rest of the data model is discoverable by following clearly identified “links” in the data. This has the advantage that the client does not need to know a set of fixed URLs. When you create a script to automate tasks using the iLO RESTful API, you only need to hardcode this simple URL and design the script to discover the REST API URLs that are needed to complete a task. To learn more about REST and HATEOAS concepts, see:

* [http://en.wikipedia.org/wiki/Representational_state_transfer](http://en.wikipedia.org/wiki/Representational_state_transfer)
* [http://en.wikipedia.org/wiki/HATEOAS](http://en.wikipedia.org/wiki/HATEOAS)

## Key benefits of the iLO RESTful API

The iLO RESTful API is becoming the main management interface for Hewlett Packard Enterprise servers with iLO 5. Its feature set will become larger than the existing iLO XML API (RIBCL) and IPMI interfaces. Using the iLO RESTful API, you can take full inventory of the server, control power and reset, configure BIOS and iLO settings, fetch event logs, as well as many other functions.

The iLO RESTful API follows the trend of the Internet in moving to a common pattern for new software interfaces. Many web services in a variety of industries use REST APIs because they are easy to implement, easy to consume, and offer scalability advantages over previous technologies.

HPE OneView, OpenStack, and many other server management APIs are now REST APIs. Most Hewlett Packard Enterprise Management software offerings, as well as the entire Software Defined Infrastructure, are built upon REST APIs.

The iLO RESTful API has the additional advantage of consistency across all present and projected server architectures. The same data model works for traditional rack-mount servers, blades, as well as newer types of systems. This advantage comes because the data model is designed to self-describe the service’s capabilities to the client and has room for flexibility designed in from the start

