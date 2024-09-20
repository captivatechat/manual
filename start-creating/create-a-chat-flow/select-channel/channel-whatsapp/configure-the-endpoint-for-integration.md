---
description: Finish setting up your WhatsApp Chat Flow
---

# Configure the Endpoint for Integration

<figure><img src="../../../../.gitbook/assets/image (29).png" alt=""><figcaption></figcaption></figure>

Once you have your WhatsApp number approved, they should appear in the WhatsApp Senders list. Access this again by going to your Twilio Console and:

1. Click ![](<../../../../.gitbook/assets/image (10).png>) in the left-hand menu.&#x20;
2. From the drop-down menu, find ![](<../../../../.gitbook/assets/image (11).png>) _**>**_ ![](<../../../../.gitbook/assets/image (12).png>)

From this list, click the WhatsApp number you dedicated to your AI Chatbot.

<figure><img src="../../../../.gitbook/assets/image (28).png" alt=""><figcaption></figcaption></figure>

Find the section called **Endpoint Configuration**. Under the **Webhook URL for Incoming Messages**, paste the following:

```
https://channel.prod.captivat.io/api/whatsapp/twilio/integration 
```

After entering the URL, click _**Save**_ or _**Update**_ to apply the changes.&#x20;

***

### Copy the Account SID and Authentication Token

<figure><img src="../../../../.gitbook/assets/image (27).png" alt=""><figcaption></figcaption></figure>

Back in the Twilio Console, locate your **Account SID** and **Auth Token.**

They should be located on the ![](<../../../../.gitbook/assets/image (31).png>).

***

### Paste the Account SID and Authentication Token in Captivate Chat

<figure><img src="../../../../.gitbook/assets/image (32).png" alt=""><figcaption></figcaption></figure>

Go back to Captivate Chat.&#x20;

1. Paste the copied Account SID and Authentication Token into the respective fields.
2. Click _**Next**_.

***

### Testing WhatsApp Configuration

<figure><img src="../../../../.gitbook/assets/image (34).png" alt=""><figcaption></figcaption></figure>

You should be ready to use WhatsApp on Twilio, thanks to Captivate Chat integration!

Locate your AI Chatbot by inputting the assigned WhatsApp number in your WhatsApp program.

Type a message and wait for your AI Chatbot to respond.&#x20;

***

## You're all set!

Doing all the steps above should get your Chatbot ready to be used with WhatsApp.
