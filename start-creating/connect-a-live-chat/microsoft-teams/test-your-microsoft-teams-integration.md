# Test your Microsoft Teams integration

Now that you’ve successfully integrated your Chat Flow to your Microsoft Teams, you have to test to see if it’s working.&#x20;

In order to do this, you have to do the following:

## **Request for a Live Agent via your Channel**

<figure><img src="../../../.gitbook/assets/image (217).png" alt="When you check the Channel of a MS Teams-connected Chat Flow, starting a conversation will reveal a blue &#x22;Chat to person&#x22; link just below their messages."><figcaption><p>When you check the Channel of a MS Teams-connected Chat Flow, starting a conversation will reveal a blue "Chat to person" link just below their messages.</p></figcaption></figure>

Go to the Channel assigned to the Chat Flow you just connected.&#x20;

In this case, we used a Web Widget for `"Roof Buddy v2".`

This means we can preview it straight from the My Chat Flow list in the Captivate Chat website.

{% hint style="info" %}
**Forgot how to preview a Web Widget?**

If you forgot how to preview a Web Widget, refer to [preview-your-web-widget.md](../../create-a-chat-flow/select-channel/channel-web-chat/preview-your-web-widget.md "mention")
{% endhint %}

<figure><img src="../../../.gitbook/assets/image (220).png" alt="Users can also ask an AI Chatbot to direct them to a Live Agent by saying &#x22;talk to human&#x22; or other similar messages."><figcaption><p>Users can also ask an AI Chatbot to direct them to a Live Agent by saying "talk to human" or other similar messages.</p></figcaption></figure>

Start a conversation with the AI Chatbot assigned to that Channel. Ask for a Live Agent. You can do this using these methods:

* **Type the request directly.** Write `"I want to talk to an agent"` or another derivative you can think of.
* **Click** ![The "Chat to person" link in the Channel of a Chat Flow will allow users to connect to a Live Agent after providing specific requirements.](<../../../.gitbook/assets/image (219).png>)**.** This option is available as a separate command on the Web Widget but can be an interactive button in other Channels (Facebook, Instagram, WhatsApp).

<figure><img src="../../../.gitbook/assets/image (221).png" alt="After telling the AI Chatbot that the user wants to talk to a Live Agent, the AI Chatbot is instructed to ask them for their name and their email address. This will be sent over to MS Teams."><figcaption><p>After telling the AI Chatbot that the user wants to talk to a Live Agent, the AI Chatbot is instructed to ask them for their name and their email address. This will be sent over to MS Teams.</p></figcaption></figure>

Wait for the AI Chatbot to respond. It will ask you for two (2) things for record-keeping purposes:

* Your name
* Your email address

The AI Chatbot will give a default message asking for the user to wait.

{% hint style="warning" %}
**Use an alternate email for this test!**

When testing your MS Teams integration, make sure you’re using a different email when talking to your AI Chatbot. This allows you to recreate a scenario where a user with a personal email is inquiring to your AI Chatbot about your services.
{% endhint %}

## **Respond to the query via Microsoft Teams**

<figure><img src="../../../.gitbook/assets/image (222).png" alt="The Captivate Chat MS Teams App will provide a notification in the connected Chat Flow&#x27;s General chat that a user wants to connect to a Live Agent."><figcaption><p>The Captivate Chat MS Teams App will provide a notification in the connected Chat Flow's General chat that a user wants to connect to a Live Agent.</p></figcaption></figure>

Go to Microsoft Teams. Wait for the **C**_**hat Flow > General**_ to receive an update.&#x20;

Since you’re the only Live Agent in your Chat Flow for now, the update will state that the test conversation will automatically be assigned to you.&#x20;

<figure><img src="../../../.gitbook/assets/image (225).png" alt="When the new user chat notification appears, clicking it will reveal a text box that agents can reply to in order to respond to the user."><figcaption><p>When the new user chat notification appears, clicking it will reveal a text box that agents can reply to in order to respond to the user.</p></figcaption></figure>

The notification will now contain a text box where you can type a greeting.&#x20;

Greet the user.&#x20;

<figure><img src="../../../.gitbook/assets/image (228).png" alt="Answering the first text box that appears with the new user chat notification will create a new chat under the Agent Name&#x27;s group chat. This will be named after the user who just asked a query. Their conversation will load in this chat, and agentscan reply using this chat."><figcaption><p>Answering the first text box that appears with the new user chat notification will create a new chat under the Agent Name's group chat. This will be named after the user who just asked a query. Their conversation will load in this chat, and agentscan reply using this chat.</p></figcaption></figure>

After greeting the user, Captivate Chat will transition your conversation into a separate chat under your _**Agent Name**_ group chat. The new conversation will have the name of the user you're currently talking to.&#x20;

## Check the dialogue in your Channel

<figure><img src="../../../.gitbook/assets/image (224).png" alt="Users will be notified that an agent has joined a conversation. All messages sent by the agent through the Captivate Chat MS Teams App will be sent to users in Channels via the AI Chatbots they are talking to. "><figcaption><p>Users will be notified that an agent has joined a conversation. All messages sent by the agent through the Captivate Chat MS Teams App will be sent to users in Channels via the AI Chatbots they are talking to. </p></figcaption></figure>

Check the Channel to view the conversation between the AI Chatbot and your test user.&#x20;

There should be a message that says `"Agent (Your Name) joins the conversation,"` alongside the greeting you sent over via Microsoft Teams.

## Wait for the MS Teams App to load your current conversation

<figure><img src="../../../.gitbook/assets/image (226).png" alt="Replies of users to the agent through the AI Chatbot will be sent to the Agent Group Chat > User&#x27;s Chat in the Captivate Chat MS Teams App. "><figcaption><p>Replies of users to the agent through the AI Chatbot will be sent to the Agent Group Chat > User's Chat in the Captivate Chat MS Teams App. </p></figcaption></figure>

Back in Microsoft Teams, wait for the initial conversation between your AI Chatbot and user to load. This should give you enough context about the user’s needs.

Once all the messages have loaded, continue the conversation to test your AI Chatbot. \
