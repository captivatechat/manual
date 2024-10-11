---
description: Connect your Chat Flow to Microsoft Teams
---

# Microsoft Teams integration

<figure><img src="../../.gitbook/assets/image (232).png" alt=""><figcaption></figcaption></figure>

In the textbox below, type `signin` to start the login process.

Under the first response, click ![](<../../.gitbook/assets/image (245).png>).  When the second message appears, click ![](<../../.gitbook/assets/image (250).png>).

<figure><img src="../../.gitbook/assets/image (251).png" alt=""><figcaption></figcaption></figure>

A new window will appear. You have to log in to your Captivate Chat account.

After you successfully logged in, you will see a list of things the Captivate Chat MS Teams App have to access in order to connect Chat Flows to your Teams organizations.  Click ![](<../../.gitbook/assets/image (252).png>).&#x20;

After providing consent, a new message will appear. You will be redirected to your chat in Microsoft Teams.&#x20;

{% hint style="info" %}
**We value your data!**

Captivate Chat won’t sell your information to third-party apps and services.&#x20;
{% endhint %}

<figure><img src="../../.gitbook/assets/image (236).png" alt=""><figcaption></figcaption></figure>

Clicking ![](<../../.gitbook/assets/image (237).png>) will prompt the app to check if your Microsoft Teams email is connected to an existing Captivate Chat account.&#x20;

If this is the case, the Captivate Chat MS Teams App will make an automatic connection.

Click Sign in via Teams.

\[]

Wait for a few moments. A new message will appear. You have successfully logged into your Captivate Chat account into Microsoft Teams.

\[]

It’s time to connect your Chat Flow!

In the same conversation with the Captivate Chat app, you will be prompted to connect a Chat Flow to Microsoft Teams.&#x20;

Click Link.

<figure><img src="../../.gitbook/assets/image (254).png" alt=""><figcaption></figcaption></figure>

Wait for the response. A new message called ![](<../../.gitbook/assets/image (210).png>) will appear that contains a drop-down list. This has all the Chat Flows you created in Captivate Chat so far.

<figure><img src="../../.gitbook/assets/image (253).png" alt=""><figcaption></figcaption></figure>

Choose the Chat Flow you want to connect to your Microsoft Teams account. In this example, we've chosen _**"Roof Buddy v2 ChatFlow."**_

Click ![](<../../.gitbook/assets/image (204).png>).

It will say ![](<../../.gitbook/assets/image (211).png>). Wait for this to finish.&#x20;

<figure><img src="../../.gitbook/assets/image (213).png" alt=""><figcaption></figcaption></figure>

A new message will say ![](<../../.gitbook/assets/image (214).png>)! This means you’ve finished connecting your Captivate Chat Flow to your Microsoft Teams account.

<figure><img src="../../.gitbook/assets/image (229).png" alt=""><figcaption></figcaption></figure>

To confirm the connection, go to your Captivate Chat account and check your list of Chat Flows. The Chat Flow you recently connected should have the Microsoft Teams under Live Chat.

### Your MS Teams Chat Flow

<figure><img src="../../.gitbook/assets/image (215).png" alt=""><figcaption></figcaption></figure>

Go to your Teams in your left-side dashboard. The following chats should be created:

* **Chat Flow Name (Chat Group):** A new chat group with the same name as your Captivate Chat Flow. In the above image, this is _**"Roof Buddy v2 ChatFlow."**_
* **Agent Name (Live Agent):** This is a conversation dedicated to a Live Agent assigned to respond to users in your Captivate Chat Flow. The first agent is named after you, the creator of the Chat Flow. In the above image, this is _**"CH Agent Rob."**_

### **Chat Flow Name**

This is a new chat group with the same name as your Captivate Chat Flow.

The chat group also contains the General chat. This contains all updates to the Chat Flow. All incoming conversations from users are sent here first before being reallocated to an agent.&#x20;

The General chat is where you can use commands to assign user conversations to Live Agents and make other adjustments to your Chat Flow from the Microsoft Teams side.

### **Agent Name**

This is a chat group dedicated to all user conversations that are transferred to the Live Agent via the Chat Flow. The first agent is named after you, the creator of the Chat Flow. It has the following components:&#x20;

* **General:** All changes that specifically happen to this Live Agent are listed here.&#x20;
* **User Name:** Each user assigned to this Live Agent gets a unique conversation within the chat group. Messages typed here are relayed to the AI Chatbot, which then relays the information to users via their conversation in the Channel.&#x20;

## Test your new MS Teams Chat Flow

Now that you’ve successfully integrated your Chat Flow to your Microsoft Teams, you have to test to see if it’s working.&#x20;

In order to do this, you have to do the following:

**Try requesting for a Live Agent via your Channel**

<figure><img src="../../.gitbook/assets/image (217).png" alt=""><figcaption></figcaption></figure>

Go to the Channel assigned to the Chat Flow you just connected.&#x20;

In this case, we used a Web Widget for "_**Roof Buddy v2 ChatFlow"**_ so we can preview it straight from the My Chat Flow list in the Captivate Chat website.

<figure><img src="../../.gitbook/assets/image (220).png" alt=""><figcaption></figcaption></figure>

Start a conversation with the AI Chatbot assigned to that Channel. Ask for a Live Agent. You can do this using these methods:

* **Type the request directly.** Write “I want to talk to an agent” or another derivative you can think of.
* **Click** ![](<../../.gitbook/assets/image (219).png>)**.** This option is available as a separate command on the Web Widget, but can be an interactive button in other Channels (Facebook, Instagram, WhatsApp).

<figure><img src="../../.gitbook/assets/image (221).png" alt=""><figcaption></figcaption></figure>

Wait for the AI Chatbot to respond. It will ask you for two things for record-keeping purposes:

* Your name
* Your email address

The AI Chatbot will give a default message asking for the user to wait.

{% hint style="warning" %}
**Use an alternate email for this test!**

When testing your MS Teams integration, make sure you’re using a different email when talking to your AI Chatbot. This allows you to recreate a scenario where a user with a personal email is inquiring to your AI Chatbot about your services.
{% endhint %}

## **Respond to the query via Microsoft Teams**

<figure><img src="../../.gitbook/assets/image (222).png" alt=""><figcaption></figcaption></figure>

Go to Microsoft Teams. Wait for the **Chat Flow > General** to receive an update.&#x20;

Since you’re the only Live Agent in your Chat Flow for now, the update will state that the test conversation will automatically be assigned to you.

<figure><img src="../../.gitbook/assets/image (225).png" alt=""><figcaption></figcaption></figure>

Greet the user.&#x20;

<figure><img src="../../.gitbook/assets/image (228).png" alt=""><figcaption></figcaption></figure>

After greeting the user, Captivate Chat will transition your chat with the user into a separate conversation under your **Agent Name** group chat. The new conversation will have the name of the user you're currently talking with.&#x20;

<figure><img src="../../.gitbook/assets/image (224).png" alt=""><figcaption></figcaption></figure>

Check the Channel to view the conversation between the AI Chatbot and your test user.&#x20;

There should be a message that says "_**Agent (Your Name) joins the conversation**_," alongside the greeting you sent over via Microsoft Teams.

<figure><img src="../../.gitbook/assets/image (226).png" alt=""><figcaption></figcaption></figure>

Back in Microsoft Teams, wait for the initial conversation between your AI Chatbot and user to load. This should give you enough context about the user’s needs.

Once all the messages have loaded, continue the conversation to test your AI Chatbot.&#x20;

\
