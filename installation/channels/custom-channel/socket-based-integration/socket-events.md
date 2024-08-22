# Socket Events

Each event type below includes the following details, take _socket_\__connected_ event as an example.

1. action - marker if the message is incoming or outgoing from the client application.&#x20;
   * sendMessage - states if the event can be emitted from the client application. Marked as Emit: true in the event types.
   * receiveMessage - states if the event can be received by the client application. If received, the client application is responsible for the handling and acknowledgement of the event. Marked as Receive: true in the event types.
2. event - content of the event. Most events would have the same schema as below. Detailed payloads for each event type are in the next section.
   * event\_type - socket event type name
   * event\_payload - socket event payload
   * event\_id - socket event id
   * accespts\_response\_payload - feature not yet implemented, by default is false. (Once implemented, the client will be able to reply to a specific ID for applicable use cases.&#x20;

**Socket Event Example**

```javascript
{
    "action": "sendMessage || receiveMessage",
    "event": {
        "event_type" : "Socket event name.",
        "event_payload" : {}
        "event_id" : "Unique event id",
        "accepts_response_payload" : false 
    }
}
```
