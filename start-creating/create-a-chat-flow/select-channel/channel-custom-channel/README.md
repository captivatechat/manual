---
description: >-
  Set your AI Assistant as a Chatbot of a Custom Channel, whether a unique app,
  social media platform, website, or other means.
---

# Channel: Custom Channel

<figure><img src="../../../../.gitbook/assets/image (32).png" alt=""><figcaption><p>The "Step 2: Select Channel" page will have Custom Channel highlighted in blue when you click it.</p></figcaption></figure>

After _**Select Channel > Custom Channel**_, you will be taken to _**Configure Custom Channel**_. This is where you can integrate your AI Chatbot as the assigned bot of your Custom Channel.

{% hint style="info" %}
**SUMMARY**

Creating a Custom Channel Chat Flow involves these steps:

1. **Choose Custom Channel** In _Step 2: Select Channel_, choose "Custom Channel." This brings you to the _Configure Custom Channel_ window.
2. **Give your Chat Flow a name and description:** Provide a Name and Description for your Custom Channel. This will its description within Captivate Chat.
3. **Get API Key:** Click _Create Channel_ after putting a Name and a Description. This creates the Custom Channel and gives you a unique API Key.
4. **Plug in the API Key into your developer environment:** Use the API Key in your developer environment alongside our Captivate Chat WebSocket tools.
{% endhint %}

{% hint style="danger" %}
**REQUIREMENTS**

Before proceeding with the rest of the Custom Channel integration process, make sure you have the following:

* **Access to our WebSocket tools:** Get our WebSocket package in [this link](https://www.npmjs.com/package/captivate-chat-api).
* **An active developer environment:** Our Custom Channel is not an independent tool. Rather, it has to be plugged into an existing developer environment.
{% endhint %}

{% hint style="warning" %}
**REMINDER**

The Custom Channel is a **development-heavy tool**. It needs more active testing compared to our other Channel types.&#x20;

It is advisable that you assign a developer to create a Custom Channel with Captivate Chat using this process.

Please contact our Support Team if you need assistance in implementing a Custom Channel in your producs and services.
{% endhint %}

***

## Configure Custom Channel

<figure><img src="../../../../.gitbook/assets/image (33).png" alt=""><figcaption><p>Clicking  "Custom Channel" in "Step 2: Select Channel" and clicking "Next" will take users to "Configure Custom Channel." You have to fill out the information on this page (Next, Description) to finish the setup process.</p></figcaption></figure>

Before you can fully integrate your AI Chatbot with your Custom Channel, you have to fill in the following information in _**Configure Custom Channel**_:

* **Name:** This is the name of the AI Chatbot as it will appear on your Custom Channel
* **Description:** Give your AI Chatbot a short description.

After you give your Custom Channel a name and a description, click _Create Channel._

### API Key

<figure><img src="../../../../.gitbook/assets/image (34).png" alt="You will get an API Key after clicking &#x22;Create Channel&#x22; in the &#x22;Configure Custom Channel.&#x22; "><figcaption><p>You will get an API Key after clicking "Create Channel" in the "Configure Custom Channel." </p></figcaption></figure>

<figure><img src="../../../../.gitbook/assets/image (35).png" alt="After clicking &#x22;Create Channel&#x22; under &#x22;Configure Custom Channel,&#x22; you can now view your API Key once more with the &#x22;Show API key&#x22; button. However, when you make changes to your Custom Channel&#x27;s Name and/or Description, you have to click &#x22;Create Channel&#x22; again to save those changes, which then generates a new API Key."><figcaption><p>After clicking "Create Channel" under "Configure Custom Channel," you can now view your API Key once more with the "Show API key" button. However, when you make changes to your Custom Channel's Name and/or Description, you have to click "Create Channel" again to save those changes, which then generates a new API Key.</p></figcaption></figure>

When you make your Custom Channel, you will now get a special API Key. You can view it whenever you want via the new _**Show API Key**_ button that appears on the page.

However, when you edit your Custom Channels' Name and/or Description, you have to click _**Create Channel**_ again to save your changes, which then generates a new API Key you have to plug in to your website or app.

***

## You're all set!

Doing all the steps above should get your Chatbot ready to be used with your Custom Channel. You may proceed with the following:

{% content-ref url="websocket-endpoints.md" %}
[websocket-endpoints.md](websocket-endpoints.md)
{% endcontent-ref %}

{% content-ref url="socket-conversation-testing.md" %}
[socket-conversation-testing.md](socket-conversation-testing.md)
{% endcontent-ref %}
