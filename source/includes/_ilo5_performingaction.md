# Performing Actions

> Example of a system resource advertising an available action:

```json
  {
  	"Actions": {
  		"#ComputerSystem.Reset": {
  			"ResetType@Redfish.AllowableValues": [
  				"On",
  				"ForceOff",
  				"ForceRestart",
  				"Nmi",
  				"PushPowerButton"
  			],
  			"target": "/redfish/v1/Systems/1/Actions/ComputerSystem.Reset"
  		}
  	}
  }
```

> This action may be invoked by performing:

```shell
curl --header "Content-Type: application/json" --request POST --data '{"ResetType": "ForceRestart"}' https://{iLO}/redfish/v1/Systems/1/Actions/ComputerSystem.Reset -u username:password --insecure
```

REST resources usually support HTTP GET to read the current state, and some support modification and removal with HTTP POST, PUT, PATCH, or DELETE.

There are some resources that support other types of operations not easily mapped to HTTP operations.  For this reason the Redfish specification defines "Actions".  Actions are HTTP POST operations with a specifically formatted JSON request including the operation to perform and any parameters.  For instance, it is not enough to simply tell a server to reset, but it is also necessary to specify the type of reset:  cold boot, warm boot, PCI reset, etc.  Actions are often used when the operation causes iLO 5 not just to update a value, but to change system state.

In Redfish, the available actions that can be invoked are identified by a "target" property in the resource's "Actions" object definitions.  The parameters identify the supported values with the annotation @Redfish.AllowableValues.

<aside class="information">

When writing new Redfish REST client code, the first example is the recommended way to invoke actions.

</aside>

## Actions on HPE-specific Extensions

Actions on HPE-specific extentions are invoked in the same way.  Find the `target` URI for the action and POST a JSON request with parameters.

```shell
curl --header "Content-Type: application/json" --request POST --data '{"PushType": "PressAndHold"}' https://{iLO}//redfish/v1/Systems/1/Actions/Oem/Hpe/HpeComputerSystemExt.PowerButton/ -u username:password --insecure
```

The embedded extensions may also have Actions not specified by the Redfish standard.  They are invoked in a similar way.  The POST URI may include indicate the HPE specific nature of the action.

The older pre-Redfish form of the Action invokation requires you to specify `"Target": "/Oem/Hp"` as one of the properties in the body of the request.

It is recommended that you use the Redfish version of the action invocation.

