---
description: Finish setting up your WhatsApp Chat Flow
---

# Configure the Endpoint for Integration

<figure><img src="../../../../.gitbook/assets/image (29).png" alt="Clicking a specific WhatsApp Sender in the Messaging > Senders > WhatsApp Senders list in Twilio will reveal various technical information about this WhatsApp Sender."><figcaption><p>Clicking a specific WhatsApp Sender in the Messaging > Senders > WhatsApp Senders list in Twilio will reveal various technical information about this WhatsApp Sender.</p></figcaption></figure>

Once you have your WhatsApp Sender approved, they should appear in the _WhatsApp Senders_ list on Twilio. Access this again by going to your Twilio Console and:

1. Click ![The Messaging dropdown in the Twilio dashboard appears on the left-hand menu.](<../../../../.gitbook/assets/image (10) (1).png>) in the left-hand menu.&#x20;
2. From the drop-down menu, find ![After clicking the Messaging dropdown button, find the Senders drop down button and click it.](<../../../../.gitbook/assets/image (11) (1).png>) _**>**_ ![After going to Messaging > Senders in the Twilio Dashboard, find WhatsApp senders. Click it to open the WhatsApp senders page in Twilio.](<../../../../.gitbook/assets/image (12) (1).png>)

From this list on Twilio, click the WhatsApp number you dedicated to your AI Chatbot.

<figure><img src="../../../../.gitbook/assets/image (28).png" alt="In the WhatsApp Sender&#x27;s profile page in Messaging > Senders > WhatsApp Senders, go to &#x22;Endpoint Configuration&#x22; section and paste a specific Webhook URL from the Captivate Chat guide in the &#x22;Webhook URL for Incoming Messages.&#x22;"><figcaption><p>In the WhatsApp Sender's profile page in Messaging > Senders > WhatsApp Senders, go to "Endpoint Configuration" section and paste a specific Webhook URL from the Captivate Chat guide in the "Webhook URL for Incoming Messages."</p></figcaption></figure>

Find the section called **Endpoint Configuration** in the WhatsApp Sender's settings. Under the **Webhook URL for Incoming Messages**, paste the following:

```
https://channel.prod.captivat.io/api/whatsapp/twilio/integration 
```

After entering the URL, click _**Save**_ or _**Update**_ to apply the changes.&#x20;

***

## Copy the Account SID and Authentication Token

<figure><img src="../../../../.gitbook/assets/image (27).png" alt="Go to your Twilio dashboard. On the bottom side of the Twilio dashboard is an Account SID and Auth Token. Copy both these values and paste them in your WhatsApp Chat Flow in Captivate Chat."><figcaption><p>Go to your Twilio dashboard. On the bottom side of the Twilio dashboard is an Account SID and Auth Token. Copy both these values and paste them in your WhatsApp Chat Flow in Captivate Chat.</p></figcaption></figure>

Back on the Twilio Console, locate your **Account SID** and **Auth Token.**

They should be located on the ![The "Account Dashboard" button in Twilio takes users to the main Twilio dashboard.](<../../../../.gitbook/assets/image (31).png>).

***

## Paste the Account SID and Authentication Token in Captivate Chat

<figure><img src="../../../../.gitbook/assets/image (32).png" alt="In the WhatsApp Chat Flow in Captivate Chat, go to the &#x22;Configure WhatsApp&#x22; page as found in &#x22;Step 2: Channel&#x22; and paste the other information in the Account SID and Authentication Token from Twilio."><figcaption><p>In the WhatsApp Chat Flow in Captivate Chat, go to the "Configure WhatsApp" page as found in "Step 2: Channel" and paste the other information in the Account SID and Authentication Token from Twilio.</p></figcaption></figure>

Go back to Captivate Chat.&#x20;

1. Paste the copied Account SID and Authentication Token into the respective fields.
2. Click _**Next**_.

***

## Testing WhatsApp Configuration

<figure><img src="../../../../.gitbook/assets/image (34).png" alt=""><figcaption><p>After the WhatsApp Chat Flow has been finished, users can test the configuration by inputting their Twilio WhatsApp Sender's phone number in WhatsApp. The integration is working if the AI Chatbot is responding automatically.</p></figcaption></figure>

You should be ready to use WhatsApp on Twilio, thanks to Captivate Chat integration!

Locate your AI Chatbot by inputting the assigned WhatsApp number in your WhatsApp program.

Type a message and wait for your AI Chatbot to respond.&#x20;

***

## You're all set!

Doing all the steps above should get your Chatbot ready to be used with WhatsApp.
