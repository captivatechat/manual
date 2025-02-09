---
description: Test the functionality of your Custom Channel with our Socket Tester.
---

# Socket Conversation Testing

We created a **Socket Conversation Testing** environment where you can plug in your existing Custom Channel and test Endpoints if they are currently working as intended.&#x20;

You may access the **Socket Conversation Testing** site [here](https://captivatechat.github.io/widget-test/socket/sockets.html).

{% hint style="warning" %}
**REMINDER**

These WebSocket Endpoints are advisable to be used by developers familiar with the product or service you want to transform into a Custom Channel.&#x20;

Please provide this page to them so they can conduct proper testing with the Custom Channel you want to create.
{% endhint %}

***

## Socket Conversation Testing

<figure><img src="../../../../.gitbook/assets/image (38).png" alt="Opening the Socket Conversation Testing webpage reveals this webpage. It has instructions on how to use this testing environment. The section to the right is where users can plug in their WSS URL with the API Key to access their Custom Channel, a JSON textbox for their WebSocket Endpoints, and Send Message to test them. There is an empty box below that will be filled with the Chatbot&#x27;s response."><figcaption><p>Opening the Socket Conversation Testing webpage reveals this webpage. It has instructions on how to use this testing environment. The section to the right is where users can plug in their WSS URL with the API Key to access their Custom Channel, a JSON textbox for their WebSocket Endpoints, and Send Message to test them. There is an empty box below that will be filled with the Chatbot's response.</p></figcaption></figure>

This is the **Socket Conversation Testing** website that is accessible via the URL above. It reveals a simple webpage where developers can test their existing Custom Channel's functionalities.&#x20;

It is comprised of three sections:

* **Instructions:** The left side contains instructions on how to use this webpage.
* **Choose an Action:** This is the active testing area. It has these components:
  * **WSS URL:** This is the unique URL of your Custom Channel. It contains your API key.
  * **Enter your JSON here...:** This textbox is where you will plug in WebSocket Endpoints listed in the Instructions to test your Custom Channel.
* **Response Area:** This is the white area below the _Send Message_ button where your Custom Channel should respond.

***

## Open Socket Connection

<figure><img src="../../../../.gitbook/assets/image (39).png" alt=""><figcaption></figcaption></figure>

Before you can use the Socket Conversation Testing page, you need to plug in your Custom Channel first. You do this within the **WSS URL** textbox below _Choose an Action_.

You have to copy a WSS URL into the text box.

If you're using it for **production:**

```
wss://channel.wss.captivatechat.ai/dev?apiKey=API_KEY
```

If you're using it for **development:**

```
wss://channel-dev.wss.captivatechat.ai/dev?apiKey=API_KEY
```

Take note that `API_KEY` here corresponds to the API Key you will receive when you create a Custom Channel in [.](./ "mention")

After doing so, click _**Open Socket Connection**_. If your Custom Channel is working, you should get a `socket_connected` event.

***

## Test with Client Actions

<figure><img src="../../../../.gitbook/assets/image (343).png" alt="This &#x22;Enter your JSON here...&#x22; textbox in the Socket Conversation Testing  is where you have to input events in JSON format. When you click &#x22;Send Message&#x22;, you should receive a response appropriate to the expected outcome as indicated in the &#x22;Instructions&#x22; segment of the Socket Conversation Testing page."><figcaption><p>This "Enter your JSON here..." textbox in the Socket Conversation Testing  is where you have to input events in JSON format. When you click "Send Message", you should receive a response appropriate to the expected outcome as indicated in the "Instructions" segment of the Socket Conversation Testing page.</p></figcaption></figure>

After you connected your WSS URL, your Custom Channel will be responsive to your **events**. You can test them by plugging them into the _"Enter your JSON here..."_ textbox, customizing its parameters, and clicking _**Send Message**_.&#x20;

<figure><img src="../../../../.gitbook/assets/image (344).png" alt="The empty box below the &#x22;Enter your JSON here...&#x22; textbox will return a response after you click &#x22;Send Message.&#x22;"><figcaption><p>The empty box below the "Enter your JSON here..." textbox will return a response after you click "Send Message."</p></figcaption></figure>

When the empty box below the _"Enter your JSON here..."_ textbox returns a response appropriate to your event, then it is working as intended.

***

## Client Actions

<figure><img src="../../../../.gitbook/assets/image (345).png" alt="An example of a Client Action listed in the Socket Conversation Testing webpage. Plug them into the &#x22;Enter your JSON here...&#x22; textbox, customize its parameters, and click &#x22;Send Message&#x22; to check if your Custom Channel can interpret it properly."><figcaption><p>An example of a Client Action listed in the Socket Conversation Testing webpage. Plug them into the "Enter your JSON here..." textbox, customize its parameters, and click "Send Message" to check if your Custom Channel can interpret it properly.</p></figcaption></figure>

The Socket Conversation Testing webpage has a list of **Client Actions** you can copy and paste into the _"Enter your JSON here..."_ textbox for testing. You can customize its parameters before clicking _"Send Message."_&#x20;

The response in the white box below will determine if your Custom Channel is working properly.
