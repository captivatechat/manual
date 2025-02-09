---
description: >-
  WebSocket Endpoints that correspond to processes that transform your Custom
  Channel into a fully functional AI Chatbot.
---

# WebSocket Endpoints

These are **WebSocket Endpoints** that are currently available and compatible with the Captivate Chat platform. These are all intended to create processes that will transform your Custom Channel into a full-blown AI Chatbot.

They are also available [here](https://www.npmjs.com/package/captivate-chat-api).

{% hint style="warning" %}
**REMINDER**

These WebSocket Endpoints are advisable to be used by developers familiar with the product or service you want to transform into a Custom Channel.&#x20;

Please provide this page to them so they can conduct proper testing with the Custom Channel you want to create.
{% endhint %}

***

### Basic Setup

Import and initialize the API client:

```
import { CaptivateChatAPI } from 'captivate-chat-api';

const api = new CaptivateChatAPI('YOUR_API_KEY');

// Connect to the WebSocket server
await api.connect();
```

### Create a Conversation

Create a new conversation with the following options:

1.  Basic setup with just a user ID:

    ```
    const conversation = await api.createConversation('user123');
    ```
2.  Include user information and custom data:

    ```
    const conversation = await api.createConversation(
      'user123',
      {
        name: 'John Doe',
        email: 'john@example.com'
      },
      {
        customField: 'value'
      },
      'user-first' // Start the conversation with user-first or bot-first mode
    );
    ```

### Send and Receive Messages

1.  Send a message to the conversation:

    ```
    await conversation.sendMessage('Hello!');
    ```
2.  Listen for responses:

    ```
    conversation.onMessage((message, type) => {
      console.log(`${type}: ${message}`);
    });
    ```

### Handle Events

Use event listeners to handle various updates, errors, or custom actions:

1.  Error handling:

    ```
    conversation.onError((error) => {
      console.error('Error:', error);
    });
    ```
2.  Updates on conversation status:

    ```
    conversation.onConversationUpdate((update) => {
      console.log('Conversation Update:', update);
    });
    ```
3.  Handling custom actions:

    ```
    conversation.onActionReceived((actions) => {
      console.log(`Actions:`, actions);
    });
    ```

### Get Conversation History

Retrieve the transcript of a conversation:

```
const transcript = await conversation.getTranscript();
console.log('Transcript:', transcript);
```

### Delete Conversation

Delete the current conversation

```
const transcript = await conversation.delete();
console.log('Deleted conversation');
```

### Retrieve User Conversations

Fetch a list of conversations associated with a specific user ID:

```
const conversations = await api.getUserConversations('user123');
console.log('User Conversations:', conversations);
/*
 Returns Conversation Object
 */
```

### Delete User Conversations

Delete list of conversations associated with a specific user ID:

```
const conversations = await api.deleteUserConversations('user123');
console.log('Conversations Deleted successfully');
/*
 Throws error if failed
 */
```
