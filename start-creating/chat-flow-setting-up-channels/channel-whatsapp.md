---
description: Set up your AI Assistant as a WhatsApp Chatbot
---

# Channel: WhatsApp

After _**Select Channel > WhatsApp**_, you will be taken to **Configure WhatsApp**. This is where you can start integrating your AI Assistant into WhatsApp as a Chatbot that people can converse with.&#x20;

<figure><img src="../../.gitbook/assets/image (28) (1).png" alt=""><figcaption></figcaption></figure>

{% hint style="danger" %}
**Make sure you have a Facebook Business Account!**

Our integration only works if you have a Facebook Business Account.
{% endhint %}

## Configure WhatsApp

Before you're able to integrate your AIChatbot into WhatsApp, you have to fill up a few details:

<pre><code><strong>image
</strong></code></pre>

* **Name:** This will be the assigned name of your AI Chatbot once it appears live on WhatsApp.
* **Description:** This is a short description assigned to your Chatbot.
* **Provider: Twilio** is set as the preset.

***

### Join Twilio

```
image
```

In order to fill up the Account SID and Authentication Token, you have to **sign up for a Twilio** account.

Go to the **Twilio website** at [https://www.twilio.com/](https://www.twilio.com/)

{% hint style="info" %}
**What is Twilio?**

Twilio is a platform that uses web APIs to perform communication functions, such as text messaging and calls. Captivate Chat will automatically facilitate the connection between Twilio and your AI Chatbot.&#x20;
{% endhint %}

<pre><code><strong>image
</strong></code></pre>

Click _**Sign Up**_ and follow the instructions to register a new account. You’ll need to provide your email address and set a password.&#x20;

**Verify your email.** Check your email for a verification link from Twilio and click on it to verify your account.&#x20;

<pre><code><strong>image
</strong></code></pre>

Log into Twilio. This will bring you to the **Twilio Console**, which serves as your main dashboard.

Twilio might ask you to **verify your phone number.** Just follow the on-screen instructions.&#x20;

### Request Access to the WhatsApp API

<pre><code><strong>image
</strong></code></pre>

**Locate the WhatsApp option in Twilio**.&#x20;

To do this, you have to:

1. Click _**Messaging**_ in the left-hand menu.&#x20;
2. From the drop down menu, find _**Senders > WhatsApp Senders**_
3. Click _**Create New Sender**_

<pre><code><strong>image
</strong></code></pre>

Follow the on-screen instructions to apply for WhatsApp access.&#x20;

These steps will mostly involve filling up the required details about your business so you can request access to the WhatsApp API.&#x20;

After doing this, Twilio will handle the actual setup process with WhatsApp.&#x20;

### Link a WhatsApp Number

<pre><code><strong>image
</strong></code></pre>

Once your request to link Twilio and WhatsApp is approved, you need to **add a phone number to use for WhatsApp messaging**.

<pre><code><strong>image
</strong></code></pre>

In order to add a new number:

1. In the Twilio Console (dashboard), click _**Messaging > Senders > WhatsApp Senders.**_
2. Click _**Create New Sender**_.&#x20;

This will reveal on-screen instructions on how to link a phone number to your WhatsApp account.

### Link your Facebook Business Account

<pre><code><strong>image
</strong></code></pre>

After setting up your **New WhatsApp Sender**, Twilio will prompt you to link your account to an existing **Facebook Business Manager** account. This is a requirement from WhatsApp.&#x20;

<pre><code><strong>image
</strong></code></pre>

Follow the instructions that Twilio provides on the screen.&#x20;

This will involve providing permissions to access the Facebook Page you want to connect to WhatsApp.&#x20;

***

### Configure the Endpoint for Integration

<pre><code><strong>image
</strong></code></pre>

Once you connect your Facebook Page to WhatsApp and Twilio, it's time to bring everything together!&#x20;

Back in the **Twilio Console**, do the following:

1. Go to _**Messaging > Services**_
2. Select your **Messaging Service**. This will be the service that corresponds to your WhatsApp number. If it doesn't exist, **create a new one**.&#x20;

<pre><code><strong>image
</strong></code></pre>

Find the section labeled _**Inbound Settings**_ or _**Incoming Messages**_.&#x20;

Enter the following endpoing URL under the **Webhook URL** field:

```
ruby 
Copy code 
https://channel.prod.captivat.io/api/whatsapp/twilio/integration 
```

After entering the URL, click _**Save**_ or _**Update**_ to apply the changes.&#x20;

### Copy the Account SID and Authentication Token

<pre><code><strong>image
</strong></code></pre>

Back in the **Twilio Console**, locate your **Account SID** and **Authentication Token.**

They should be located on either the Twilio Console itself or under the **Account** section.&#x20;

### Paste the Account SID and Authentication Token in Captivate Chat

<pre><code><strong>image
</strong></code></pre>

Go back to **Captivate Chat**.&#x20;

1. Under _**Setup > Chat Flows**_, select the Chat Flow where you want to connect WhatsApp.&#x20;
2. Go to _**Select**_ _**Channel > WhatsApp**_&#x20;
3. Paste the copied Account SID and Authentication Token into the respective fields.
4. Click _**Save Settings**._

***

### Testing WhatsApp Configuration

You should be ready to use WhatsApp on Twilio, thanks to Captivate Chat integration!

<pre><code><strong>image
</strong></code></pre>

Wait for your WhatsApp integration to be fully approved.

<pre><code><strong>image
</strong></code></pre>

After approval, try to locate your AI Assistant on WhatsApp and send a message.

If the integration is successful, your Chatbot should be able to respond.&#x20;

***

## You're all set!

Doing all the steps above should get your Chatbot ready to be used with WhatsApp.
