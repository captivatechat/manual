# Socket Event Types

### socket\_connected

Successful creation of a channel session.\
**Emit :** No\
**Receive :** Yes\
**Payload**

```javascript
{
    "action": "receiveMessage",
    "event": {
        "event_type": "socket_connected",
        "event_id": "Vp6roFYZLPEFfcg=",
        "event_payload": {
            "socket_id": "Vp6roemHLPECFOQ="
        },
        "accepts_response_payload": false
    }
}
```

### conversation\_start

Send this event to start a new conversation in CH. On successful creation, expect to receive bot\_messages and be able to send user\_messages. \
**Emit** : Yes\
**Receive** : No\
**Payload** :

```javascript
{
    "action": "sendMessage",
    "event": {
        "event_type": "conversation_start",
        "event_payload": {
            // userId - optional. if not provided, CH will assign "anon" as the userId.
            "userId": "super-unique-user-id",
            // userBasicInfo - optional. if provided, basic info is sent in livechat and chatbot
            "userBasicInfo": { //optional
                "firstName": "John",
                "lastName": "Doe",
                "email": "john@sample.io"
            //DEV NOTE: Add phone number nalang here   
            },
            // userData - optional. if provided, basic info is sent in livechat and chatbot
            "userMetadata": {
            
            }
            //DEV NOTE: CHANGE TO userMetadata, metadata updates will be pushed here too.
        }
    }
}
```

### conversation\_start\_success

This event is received event to start a new conversation in CH. On successful creation, expect to receive bot\_messages immediately with the same conversation\_id received here. Consider this as a confirmation that conversation start request has been successful.\
**Emit** : No\
**Receive** : Yes\
**Payload** :

```javascript
{
    "action": "receiveMessage",
    "event": {
        "event_type": "conversation_start_success",
        "event_payload": {
            "conversation_id": "super-unique-user-id-d1816568-2b18-4e8b-a09e-ec6f86eeccfd"
        },
        "event_id": "Vp6xHFY9LPEFYXw=",
        "accepts_response_payload": false
    }
}
```

### user\_message

User messages sent from the client application.\
**Emit :** Yes\
**Receive :** No\
**Payload**

```javascript
{
    "action": "sendMessage",
    "event": {
        "event_type": "user_message",
        "event_payload": {
            "type": "message_create",
            "client_msg_id": "unique-message-id", // Unique message ID to be set by client, UUID type format is preferable.
            "conversation_id": "temp123-aaaaa-aaaa", //Unique conversation session ID from Captivate Hub
            "content": {
                "type" : "text", // current supported type
                "text": "hello"
            }
        }
    }
}
```

### bot\_message

Bot messages sent from Captivate Hub.\
**Emit** : No\
**Receive** : Yes\
\
**Payload showing the model of the bot\_message content**

```javascript
{
    "action": "receiveMessage",
    "event": {
        "event_type": "bot_message",
        "event_payload": {
            "type": "message_create",
            "ch_msg_id": "f14efe6e-773a-4a52-85f5-90b6d801f2d1",
            "bot": {},
            "content": [{
                // current supported types
                "type" : "text || buttons || cards",
                // sent only when type is "text"
                "text" : "bot text message",
                // sent only when type is "buttons"
                "buttons" : {},
                // sent only when type is "cards"
                "cards" : {}
            }]
        },
        "event_id": "Vp6x7GxOLPEFb7A=",
        "accepts_response_payload": false
    }
}

```

**Payload example**

```javascript
{
    "action": "receiveMessage",
    "event": {
        "event_type": "bot_message",
        "event_payload": {
            "type": "message_create",
            "ch_msg_id": "f14efe6e-773a-4a52-85f5-90b6d801f2d1",
            "bot": {},
            "content": [
                {
                    "text": "Hi. I'm the Captivate Bot.",
                    "type": "text"
                },
                {
                    "text": "You can leave us your contact details or you can chat to us directly now!",
                    "type": "text"
                },
                {
                    "type": "button",
                    "buttons": {
                        "title": "Please choose from one of the following:",
                        "options": [
                            {
                                "label": "Leave Contact Details",
                                "value": "Leave Contact Details"
                            },
                            {
                                "label": "Chat to Agent",
                                "value": "Chat to Agent"
                            }
                        ]
                    }
                }
            ]
        },
        "event_id": "Vp6x7GxOLPEFb7A=",
        "accepts_response_payload": false
    }
}
```

### livechat\_message

Livechat messages sent from the connected live chat application (Slack, MS Teams, Freshdesk, etc.).\
**Emit :** No\
**Receive :** Yes\
**Payload**

```javascript
{
    "action": "receiveMessage",
    "event": {
        "event_type": "livechat_message",
        "event_payload": {
            "type": "message_create",
            "conversation_id": "",
            "content": [ // array of agent messages
                {
                    "text": "hello",
                    "type": "text"
                },
                {
                    "files": [
                        {
                            "type": "image",
                            "url": "https://fc-euc1-00-pics-bkt-00.s3.eu-central-1.amazonaws.com/9ca67af811a929e146797ca9a098a7baa924f5f3f97462ea995a15f3f6ef6b39/f_marketingpicFull/u_c3f0d156af45b476c0be56a8d22f56bc4df846910c1b1a5b6ff1d8f4577b4d9d/img_37o2ah9f8j_309cbb43ff98c47af2ee993cb95fe23f9349f6e2386d9d188cf23b0fe8c336ec.jpeg",
                            "mimetype": "image",
                            "filename": null
                        }
                    ],
                    "type": "files"
                }
            ]
        },
        "event_id": "103fb31a-a70c-4b16-977c-917956ff12ae",
        "accepts_response_payload": false
    }
}
```

### metadata

Metadata that can be set from the client application. This [CH document](https://manual.captivat.io/install/chatbot/watson-assistant/the-captivate-hub-integration/metadata) details how and why metadata is used in Captivate Hub. Examples of metadata that can be set are channel user data and sending preconfigured data depending on where the user is in the website. This metadata will be saved in CH sessions and can be if required.\
**Emit :** Yes\
**Receive :** No\
**Payload**

```javascript
{
    "action": "sendMessage",
    "event": {
        "event_type": "metadata",
        "event_payload": {
            "metadata": { //Object to contain any custom metadata
                "sample_metadata": "Sample metadata"
            },
            "target" : "default || bot || live || bot_live",
            "client_msg_id": "unique-message-id",Javasc
            "conversation_id": "temp123-aaaaa-aaaa"
        }
    }
}
```

### action

Aside from messages, actions can also be exchanged by the client application and Captivate Hub. Actions can be used for triggering events on both sides.

For example, a reserved CH action “escalateToHuman” can be emitted from the client application for this example scenario:

> There is button in the chat widget that the user can click to ask for a livechat agent for assistance. Client application should then emit an action to CH, and CH will handle the action accordingly.

It is also possible to receive an action from CH for an example scenario:

> A user asks the chatbot “How do I reach you”, the chatbot then recognizes this and sends an [outgoing action](https://manual.captivat.io/install/chatbot/watson-assistant/the-captivate-hub-integration/outgoing-action)  back to the channel with a title “redirectToContactUs”. It is up to the client application developer then to utilize the action received.

**Emit** : Yes\
**Receive** : Yes\
**Payload**

```javascript
{
    "action": "sendMessage",
    "event": {
        "event_type": "action",
        "event_payload": {
            "type": "normal", // type can be utilized by developers, but by default this is set to "normal"
            "id": "escalateToHuman", // Action ID Java
            "data": {}, //Object to contain any custom supporting data for the action
            "conversation_id": "temp123-aaaaa-aaaa"
        }
    }
}
```

### conversation\_transcript\_request

Send this event to request for the conversation transcripts associated with a socket connection. Expect to receive a conversation\_transcript event as a response.\
**Emit** : Yes\
**Receive** : No\
**Payload** :

```javascript
{
    "action": "sendMessage",
    "event": {
        "event_type": "conversation_transcript_request",
        "event_payload": {
            "conversation_id": "assigned conversation id"
        }Javasc
    }
}
```

### conversation\_transcript

The returned transcript in response to conversation\_transcript\_request __ event_._

**Emit** : No\
**Receive** : Yes\
**Payload** :

```javascript
{
    "action": "receiveMessage",
    "event": {
        "event_type": "conversation_transcript",
        "event_payload": {
            "conversation_id": "hart_acb3b13e-4818-40fa-b57e-d8a80feba5c1",
            "transcript": [
                {
                    "event_id": "event id",
                    "messages": [
                        {
                            "actions": [], // if there are actions
                            "files": [], // if there are files
                            "from": "user || chatbot || livechat",
                            "chatbotName": "Name of chatbot in your hub if there is",
                            "channelName": "Name of channel in your hub",
                            "livechatName": "Name of livechat in your hub if there is",
                            //Array of chronological message contents
                            "messages": [
                                {
                                    "type": "text || buttons || cards",
                                    "text": "Actual message if type is text",
                                    "buttons": {
                                        // buttons if type is buttons
                                        "title": "Choose from the following:",
                                        "options": [
                                            {
                                                "label": "button label 1",
                                                "value": "button value 1"
                                            }
                                        ]
                                    }
                                }
                            ]
                        }
                    ]
                }
            ]
        },
        "event_id": "WvVB-EB6rPEFkJQ=",
        "accepts_response_payload": false
    }
}
```

**Payload example with user, agent, and bot messages:**

```javascript
{
    "action": "receiveMessage",
    "event": {
        "event_type": "conversation_transcript",
        "event_payload": {
            "conversation_id": "hart_acb3b13e-4818-40fa-b57e-d8a80feba5c1",
            "messages": [
                {
                    "from": "user",
                    "messages": [{ "type": "text", "text": "hello" }],
                    "channelName": "test custom channel",
                    "chatbotName": "AWS-LEX-QORBITAL-DEMO"
                },
                {
                    "from": "bot",
                    "messages": {
                        "idChat": "hart_acb3b13e-4818-40fa-b57e-d8a80feba5c1",
                        "messages": [
                            {
                                "text": "Hi. I'm the Captivate Bot.",
                                "type": "text"
                            }
                        ],
                        "actions": []
                    },
                    "channelName": "test custom channel",
                    "chatbotName": "AWS-LEX-QORBITAL-DEMO"
                },
                {
                    "from": "user",
                    "messages": [{ "type": "text", "text": "agent" }],
                    "channelName": "test custom channel",
                    "chatbotName": "AWS-LEX-QORBITAL-DEMO"
                },
                {
                    "from": "bot",
                    "messages": {
                        "idChat": "hart_acb3b13e-4818-40fa-b57e-d8a80feba5c1",
                        "messages": [
                            {
                                "text": "Please wait while I connect you to the support team.",
                                "type": "text"
                            }
                        ],
                        "actions": [
                            { "type": "normal", "title": "escalateToHuman" }
                        ]
                    },
                    "actions": [
                        { "type": "normal", "title": "escalateToHuman" }
                    ],
                    "channelName": "test custom channel",
                    "chatbotName": "AWS-LEX-QORBITAL-DEMO"
                },
                {
                    "from": "user",
                    "messages": [{ "type": "text", "text": "hello" }],
                    "channelName": "test custom channel",
                    "chatbotName": "AWS-LEX-QORBITAL-DEMO"
                },
                {
                    "from": "user",
                    "messages": [{ "type": "text", "text": "hello" }],
                    "channelName": "test custom channel",
                    "chatbotName": "AWS-LEX-QORBITAL-DEMO"
                },
                {
                    "from": "agent ",
                    "messages": {
                        "idChat": "hart_acb3b13e-4818-40fa-b57e-d8a80feba5c1",
                        "messages": [
                            {
                                "type": "text",
                                "text": "Our agents are currently busy at the moment."
                            }
                        ],
                        "actions": []
                    },
                    "channelName": "custom-channel",
                    "chatbotName": "AWS-LEX-QORBITAL-DEMO"
                }
            ]
        },
        "event_id": "WvVB-EB6rPEFkJQ=",
        "accepts_response_payload": false
    }
}
```

### conversation\_update

Updates specific to a conversation session. Details for updates types will be provided in the next docs.&#x20;

Emit : No \
Receive : Yes \
Payload :

```javascript
{
    "action": "receiveMessage",
    "event": {
        "event_type": "conversation_update",
        "event_payload": {
            "type": "failedAgentAssignment || livechatAgentConnected || livechatAgentDisconnected",
            "conversation_id": "Captivate Hub Session ID",
            "data": {} // data relevant to the type of conversation update, for example, if update is livechatAgentConnected, then this would contain the agentInfo
        }
    }
}
```

### general\_error

Sent during errors.

Emit : No \
Receive : Yes \
Payload \


```javascript
{
    "action": "receiveMessage",
    "event": {
        "event_type": "conversation_update",
        "event_payload": {
            "event_type": "general_error",
            "event_payload": {
                "conversation_id": "Conversation ID",
                "error_code": "Error code",
                "error_desc": "Error Description"
            },
            "event_id": "event_id"
        }
    }
}
```

**Example –** at the moment, this Invalid conversation\_Id is the only possible error returned.

```javascript
{
    "action": "receiveMessage",
    "event": {
        "event_type": "general_error",
        "event_payload": {
            "conversation_id": "sasa-5beb-4a96-a0d6-8c3369e82627",
            "error_code": 400,
            "error_desc": "Invalid conversation_id"
        },
        "event_id": "WJ8pqG9gLPEF9ng=",
        "accepts_response_payload": false
    }
}
```
