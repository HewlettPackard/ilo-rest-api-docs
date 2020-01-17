# Navigating the Data Model

The Redfish API is designed to be implemented on many different models of servers and other IT infrastructure devices for years to come.  These devices may be quite different from one another.  For this reason, the Redfish API does not specify the URIs to various resources. For example, a client cannot assume the BIOS version information is always at a particular URI.

This is more complex for the client, but is necessary to make sure the data model can change to accommodate various future server architectures without requiring specification changes. As an example, if the BIOS version is at `/redfish/v1/Systems/1`, and a client assumed it is always there, the client would then break when the interface is implemented on a different type of architecture with many compute nodes, each with its own BIOS version, or on other vendor implementations. 

## Redfish 1.6 (iLO 5 1.40 or later) URI Templates
As of Redfish 1.6, a number of resource types have URI template specifications to be compatible with OpenAPI 3.0.  Please see the Redfish 1.6 CSDL schema for details on URI templates for specific types.

A client must still perform GET operations on a Redfish API service in order to discover what resources are available.  For instance, just because a Chassis has a template of `/redfish/v1/Chassis/{ChassisId}` means that a client must still GET `/redfish/v1/Chassis` in order to find the valid values of `{ChassisId}`.

## Iterating Collections

```shell
curl https://{iLO}/redfish/v1/systems/ -i --insecure -u username:password -L
```

```python
import sys
import redfish

# When running remotely connect using the iLO address, iLO account name, 
# and password to send https requests
iLO_host = "https://{iLO}"
login_account = "admin"
login_password = "password"

## Create a REDFISH object
REDFISH_OBJ = redfish.RedfishClient(base_url=iLO_host,username=login_account, \
                          password=login_password, default_prefix='/redfish/v1')

# Login into the server and create a session
REDFISH_OBJ.login(auth="session")

# Do a GET on a given path
response = REDFISH_OBJ.get("/redfish/v1/systems/", None)

# Print out the response
sys.stdout.write("%s\n" % response)

# Logout of the current session
REDFISH_OBJ.logout()
```

> JSON response example:

```json
{
    "@odata.id": "/redfish/v1/systems/",
    "@odata.context": "/redfish/v1/$metadata/",
    "@odata.type": "#ComputerSystemCollection.ComputerSystemCollection",
    "Members@odata.count": 1,
    "Members": [
        {
            "@odata.id": "/redfish/v1/systems/1/"
        }
    ]
}
```

Many operations will require you to locate the resource you wish to use.  Most of these resources are members of "collections" (arrays of similar items).  The method to find collections members is consistent for compute nodes, chassis, management processors, and many other resources in the data model.

## Find a Compute Node

```shell
curl https://{host}/redfish/v1/systems/{item}/ -i --insecure -u username:password -L
```

```python
import sys
import redfish

# When running remotely connect using the iLO address, iLO account name, 
# and password to send https requests
iLO_host = "https://{iLO}"
login_account = "admin"
login_password = "password"

## Create a REDFISH object
REDFISH_OBJ = redfish.RedfishClient(base_url=iLO_host,username=login_account, \
                          password=login_password, default_prefix='/redfish/v1')

# Login into the server and create a session
REDFISH_OBJ.login(auth="session")

# Do a GET on a given path
response = REDFISH_OBJ.get("/redfish/v1/systems/{item}/", None)

# Print out the response
sys.stdout.write("%s\n" % response)

# Logout of the current session
REDFISH_OBJ.logout()
```

> JSON response example:

```json
{
	"@odata.context": "/redfish/v1/$metadata#Systems/Members/$entity",
	"@odata.id": "/redfish/v1/Systems/1/",
	"@odata.type": "#ComputerSystem.1.0.1.ComputerSystem",
	...
	
	...
	"SerialNumber": "Kappa",
	"Status": {
		"Health": "Warning",
		"State": "Enabled"
	},
	"SystemType": "Physical",
	"UUID": "00000000-0000-614B-7070-610000000000"
}
```

A Compute node represents a logical computer system with attributes such as processors, memory, BIOS, power state, firmware version, etc.  To find a compute node `GET /redfish/v1/systems` and iterate the "Members" array in the returned JSON.  Each member has a link to a compute node.

Find a compute node by iterating the systems collection at `/redfish/v1/systems/`.

You can then GET the compute node, PATCH values, or perform Actions.

## Find a Chassis

```shell
curl https://{host}/redfish/v1/chassis/{item}/ -i --insecure -u username:password -L
```

```python
import sys
import redfish

# When running remotely connect using the iLO address, iLO account name, 
# and password to send https requests
iLO_host = "https://{iLO}"
login_account = "admin"
login_password = "password"

## Create a REDFISH object
REDFISH_OBJ = redfish.RedfishClient(base_url=iLO_host,username=login_account, \
                          password=login_password, default_prefix='/redfish/v1')

# Login into the server and create a session
REDFISH_OBJ.login(auth="session")

# Do a GET on a given path
response = REDFISH_OBJ.get("/redfish/v1/chassis/{item}/", None)

# Print out the response
sys.stdout.write("%s\n" % response)

# Logout of the current session
REDFISH_OBJ.logout()
```

> JSON response example:

```json
{
	"@odata.context": "/redfish/v1/$metadata#Chassis/Members/$entity",
	"@odata.id": "/redfish/v1/Chassis/1/",
	"@odata.type": "#Chassis.1.0.0.Chassis",
	"ChassisType": "RackMount",
	...
	
	...
	"Status": {
		"Health": "Warning",
		"State": "Enabled"
	},
	"Thermal": {
		"@odata.id": "/redfish/v1/Chassis/1/Thermal/"
	}
}
```

A Chassis represents a physical or virtual container of compute resources with attrbutes such as FRU information, power supplies, temperature, etc.  To find a chassis `GET /redfish/v1/chassis` and iterate the "Members" array in the returned JSON.  Each member has a link to a chassis.

Find a chassis by iterating the chassis collection at `/redfish/v1/chassis/`.

You can then GET the chassis, PATCH values, or perform Actions.

## Find the iLO 5 Management Processor

```shell
curl https://{host}/redfish/v1/managers/{item}/ -i --insecure -u username:password -L
```

```python
import sys
import redfish

# When running remotely connect using the iLO address, iLO account name, 
# and password to send https requests
iLO_host = "https://{iLO}"
login_account = "admin"
login_password = "password"

## Create a REDFISH object
REDFISH_OBJ = redfish.RedfishClient(base_url=iLO_host,username=login_account, \
                          password=login_password, default_prefix='/redfish/v1')

# Login into the server and create a session
REDFISH_OBJ.login(auth="session")

# Do a GET on a given path
response = REDFISH_OBJ.get("/redfish/v1/managers/{item}/", None)

# Print out the response
sys.stdout.write("%s\n" % response)

# Logout of the current session
REDFISH_OBJ.logout()
```

> JSON response example:

```json
{
	"@odata.context": "/redfish/v1/$metadata#Managers/Members/$entity",
	"@odata.id": "/redfish/v1/Managers/1/",
	"@odata.type": "#Manager.1.0.0.Manager",
	...
	
	...
	"Status": {
		"State": "Enabled"
	},
	"UUID": null,
	"VirtualMedia": {
		"@odata.id": "/redfish/v1/Managers/1/VirtualMedia/"
	}
}
```

A Manager represents a management processor (or "BMC") that manages chassis and compute resources.  For HPE Gen10 Servers, the manager is iLO 5.  Managers contain attributes such as networking state and configuration, management services, security configuration, etc.  To find a manager `GET /redfish/v1/managers` and iterate the "Members" array in the returned JSON.  Each member has a link to a chassis.

Find a manager by iterating the manager collection at `/redfish/v1/managers/`.

You can then GET the manager, PATCH values, or perform Actions.

