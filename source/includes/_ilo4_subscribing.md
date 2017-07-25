# RESTful Events and the Event Service
Starting with iLO 4 2.30, iLO now features a new event subscription service that enables you to
subscribe to receive notifications when the REST data changes or when certain alerts occur.
These notifications are in the form of HTTPS POST operations to a URI of your choice.

The event service is located in the data model at `/redfish/v1/EventService.` This resource includes
a link to a collection of subscriptions (called `EventSubscriptions` located at
`/redfish/v1/EventService/EventSubscriptions`).

## Subscribing for Events examples
> POST /redfish/v1/EventService/EventSubscriptions/

```json
{
	"Destination": "https://myeventreciever/eventreceiver",
	"EventTypes": [
		"ResourceAdded",
		"ResourceRemoved",
		"ResourceUpdated",
		"StatusChange",
		"Alert"
	],
	"HttpHeaders": {
		"Header": "HeaderValue"
	},
	"TTLCount": 1440,
	"TTLUnits": "minutes",
	"Context": "context string",
	"Oem": {
		"Hp": {
			"DeliveryRetryIntervalInSeconds": 30,
			"RequestedMaxEventsToQueue": 20,
			"DeliveryRetryAttempts": 5,
			"RetireOldEventInMinutes": 10
		}
	}
}
```

In order to receive events, you must provide an HTTPS server accessible to iLO’s network with
a URI you designate as the target for iLO-initiated HTTPS POST operations.

Construct a JSON object conforming to the type `ListenerDestination` (see example) and
POST this to the collection indicated by the `EventSubscriptions` link at
`/redfish/v1/EventService/EventSubscriptions.` If you receive an HTTP 201 Created
response, a new subscription has been added. Note that iLO does not test the destination URI
during this phase, so if the indicated URI is not valid, this will not be flagged until events are
emitted and the connection to the destination fails.

**Example POST payload to create a new subscription**

Much of the above content depends entirely upon your needs and setup:

* `Destination` must be an HTTPS URI accessible to iLO’s network.
* `EventTypes` in the example is everything but you could remove types from the array.
* `HttpHeaders` gives you an opportunity to specify any arbitrary HTTP headers you need
for the event POST operation. Note that the subscription is readable via GET to an authorized
iLO user.
* `Context` may be any string.

Consult the `ListenerDestination` schema for more details on each property. The subscription
will automatically expire after the TTL information specified and must be renewed.


