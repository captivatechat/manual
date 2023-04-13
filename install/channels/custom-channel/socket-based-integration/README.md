# Socket-based Integration

Socket-based integration is a new Captivate Hub API integration type that lets developers create their own chat widget or custom channel without providing a public Webhook endpoint.

Although our REST APIs remain available, with the use of WebSockets, any client (e.g. browser or mobile) or server application can communicate directly using a WebSockets URL with Captivate Hub servers in a real time manner.

This guide uses JavaScript/JSON syntax  as examples but developers are free to use any programming language or install a library that support the use of [WebSocket protocol](https://datatracker.ietf.org/doc/html/rfc6455).

### Creation of Channel API Key

Start with creating a hub using “Custom channel” then pick Socket Mode as the integration type. On successful channel creation, a **Channel API key** will be returned.

You can still toggle from Sockets mode to Webhooks mode by updating your channel. If you do so, this just means that messages from Captivate Hub (i.e., chatbot or livechat agent replies) will be sent to your configured Webhook URL via HTTP requests instead of WebSockets.

### Connect to the WebSocket

To successfully connect to Captivate Hub using Socket Mode, you need a valid Websocket URL.

Your **WebSocket URL** will consist of the Websockets Base URL of CH + your Channel API key  as a query parameter. WebSockets Base URL will be either be displayed in the CH dashboard too or provided by the CH team.

**Websocket URL Format**\
`<WebSockets Base wss:// URL>?apikey=<Your Custom Channel API Key>`

**Example Websocket URL**\
`wss://ch.channelgateway.com?apikey=sample-custom-channel-APIKey`

Here’s an example code of connecting to the WebSocket server. (another example implementation for a Flutter application in this [Flutter docs page](https://docs.flutter.dev/cookbook/networking/web-sockets).)

```javascript
let wssUrl = 'wss://ch.channelgateway.com?apikey=sample-custom-channel-APIKey';
let socket = new WebSocket(wssUrl);

socket.onopen = function(event) {
  // connection established
}

socket.onmessage = function(event) {
  // application received message
}
socket.onerror= function(event) {
  // application failed to connect or has been closed due to an error
}

```

If connection is not successful, this will be fired in the error event of the library you are using. For example, [Websocket API’s error event](https://developer.mozilla.org/en-US/docs/Web/API/WebSocket/error\_event).

Else, if successful connection, the client application will receive a socket session id through a socket message with type: “socket\_connected”. The socket\_id is not necessarily needed for the next steps, but is sent for reference. Details on Events is in the next step but for now this is an example connected message.

```javascript
{
    "event_type": "socket_connected",
    "event_id": "Vp6roFYZLPEFfcg=",
    "event_payload": {
        "socket_id": "Vp6roemHLPECFOQ="
    }
}
```

### Send and Receive Socket Events

General template of events include **event\_type and** **event\_payload**, more detailed format for event type is in the Socket Event Types section of this doc.

We’ll use **conversation\_start** and **conversation\_start\_success** event types as an example. Notice here that there are extra action and event wrappers to the event object when sending a socket message.

To start a conversation, you need to have a **conversation\_id** using the **conversation\_start** socket event. First, send a **conversation\_start** socket event**.**

\
**Send Socket Message Example**

```javascript
{
    "action": "sendMessage",
    "event": {
        "event_type": "conversation_start",
        "event_payload": {
            "userId": "super-unique-user-id", // Optional – if not sent, we assign “anon” as userId
            "userBasicInfo": {
                "firstName": "Sigrid",
                "lastName": "Ramos",
                "email": "sig@captivat.io"
            },
            "userData": {}
        }
    }
}

```

If that message has been successfully sent, you should receive a **conversation\_start\_success** event with the **conversation\_id** in the payload.

**Receive Socket Message Example**

```javascript
{
    "event_type": "conversation_start_success",
    "event_payload": {
        "conversation_id": "d1816568-2b18-4e8b-a09e-ec6f86eeccfd"
    },
    "event_id": "Vp6xHFY9LPEFYXw=",
    "accepts_response_payload": false
}
```

At this point, you now have a conversation\_id to emit messages for user\_message, action, metadata or any client emit-able event.

### Handling Disconnects and Reconnects

Client applications are responsible for handling disconnected sockets. To reconnect, just repeat the Connect to the Websocket step and if you already have a conversation\_id, you can get back to sending and receiving messages. If not, you may request for a new conversation\_id using conversation\_start event but note that this will be a new conversation session.

Developers should also note that session timeouts should be configured, more details on this will be provided on the next updates.
