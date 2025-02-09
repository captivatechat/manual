---
description: Set up your AI Assistant as a WhatsApp Chatbot
---

# Channel: WhatsApp

<figure><img src="../../../../.gitbook/assets/image (18).png" alt="After selecting an AI Chatbot in &#x22;Step 1: Select Chatbot,&#x22; choose &#x22;WhatsApp&#x22; in &#x22;Step 2: Select Channel&#x22; in the Chat Flow creation process. The button will be highlighted blue. Click &#x22;Next&#x22; to proceed."><figcaption><p>After selecting an AI Chatbot in "Step 1: Select Chatbot," choose "WhatsApp" in "Step 2: Select Channel" in the Chat Flow creation process. The button will be highlighted blue. Click "Next" to proceed.</p></figcaption></figure>

After _**Select Channel > WhatsApp**_, you will be taken to _**Configure WhatsApp**_. This is where you can start integrating your AI Assistant into WhatsApp as a Chatbot that people can converse with.&#x20;

{% hint style="info" %}
**SUMMARY**

Connecting your Chat Flow to WhatsApp needs some back and forth between another app called Twilio. Here are the steps:

1. **Set up a Twilio Paid Account:** You need a Twilio Paid Account to assign a phone number to WhatsApp that connects to your Chat Flow.
2. **Create a WhatsApp Sender on Twilio:** On the Twilio dashboard, go to _Messaging > Senders > WhatsApp Senders._ Follow the prompts in the new page to start setting up your WhatsApp Sender.
3. **Fill out basic information on Twilio:** The WhatsApp Sender setup process on Twilio requires you to fill out data. Make sure this is accurate.
4. **Select a phone number on Twilio:** Enter a reserve phone number unconnected to WhatsApp or buy one from Twilio.&#x20;
5. **Connect to WhatsApp:** For your first WhatsApp Sender, you have to put additional information about your business on Twilio and then go to Meta Business Suite to accept the pending Twilio connection request. If you're making your subsequent WhatsApp Senders, use a button on Twilio to sign into Meta and verify your phone number.
6. **Configure the Endpoint:** Go to your recently created WhatsApp Sender on Twilio. Copy the Webhook URL from this guide and paste it onto the Webhook URL text box on the WhatsApp Sender's settings.
7. **Finish the WhatsApp Chat Flow on Captivate Chat:** Copy the Account SID and Authorization Token from your Twilio dashboard and paste it on the necessary fields back in your WhatsApp Chat Flow on Captivate Chat.&#x20;
8. **Test the WhatsApp Chat Flow:** Find your WhatsApp Chat Flow on WhatsApp via the phone number you used on Twilio. It should create automated responses.&#x20;
{% endhint %}

{% hint style="danger" %}
**REQUIREMENTS**

Before proceeding with the rest of the WhatsApp integration process, make sure you have the following:

* **Twilio Paid Account:** While you can register for a free Twilio account, you need to have a Paid Account to access functionalities needed to integrate WhatsApp into Captivate Chat.&#x20;
* **Phone Number not connected to WhatsApp:** You need to have an extra number not connected to WhatsApp. You can have one prepared or buy one from Twilio. It's important that the number is **not connected to WhatsApp** or the process won't work.&#x20;
* **Facebook Business Account:** Our integration only works if you have a Facebook Business Account. Make sure it is a **verified** account by following the steps in this [guide from Meta](https://www.facebook.com/business/help/2058515294227817?id=180505742745347).
{% endhint %}

{% hint style="danger" %}
**Get a Twilio Paid Account!**

Crucial steps in this process, such as being able to create a WhatsApp Sender, is only possible with a Twilio Paid Account. After registering for your Twilio Free Account, please upgrade to a Twilio Paid Account.

You cannot use Captivate Chat to integrate your AI Chatbots to WhatsApp without Twilio.
{% endhint %}

{% hint style="warning" %}
**Check for guide updates!**

Unlike other Chat Flows, connecting your AI Chatbot to WhatsApp needs you to use other platforms (Twilio, Meta Business Suite). Make sure to read updated guides and documentation about their processes for more in-depth instructions.&#x20;
{% endhint %}
