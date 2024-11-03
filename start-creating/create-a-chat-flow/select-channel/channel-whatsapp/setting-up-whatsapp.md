---
description: Set up your AI Assistant as a WhatsApp Chatbot
---

# Setting up WhatsApp

<figure><img src="../../../../.gitbook/assets/image (28) (1) (1).png" alt=""><figcaption><p>After selecting WhatsApp and clicking "Next" in "Step 2: Select Channel" of the Chat Flow creation process, you will go to the "Configure WhatsApp" page.</p></figcaption></figure>

You will be taken to a _**Configure WhatsApp**_ page after selecting WhatsApp in _**Step 2: Select Channel.**_&#x20;

This window contains the necessary information that have to be filled out before WhatsApp becomes integrated to your Chat Flow.

## Configure WhatsApp

<figure><img src="../../../../.gitbook/assets/image (4) (1) (1).png" alt="Basic information that have to be filled out for a successful WhatsApp integration include the public name of the WhatsApp Chat Flow, a basic description, and a Provider that is set to Twilio by default."><figcaption><p>Basic information that have to be filled out for a successful WhatsApp integration include the public name of the WhatsApp Chat Flow, a basic description, and a Provider that is set to Twilio by default.</p></figcaption></figure>

Before you're able to integrate your AI Chatbot into WhatsApp, you have to fill up a few details:

* **Name:** This will be the assigned name of your AI Chatbot once it appears live on WhatsApp.
* **Description:** This is a short description assigned to your Chatbot.
* **Provider: Twilio** is set as the preset.

***

## Join Twilio

<figure><img src="../../../../.gitbook/assets/image (5).png" alt="The upper right side of the screen of the Twilio homepage has &#x22;Start for Free&#x22; button that leads to the registration process."><figcaption><p>The upper right side of the screen of the Twilio homepage has "Start for Free" button that leads to the registration process.</p></figcaption></figure>

In order to fill up the Account SID and Authentication Token, you have to **sign up for a Twilio** account.

Go to the **Twilio website** at [https://www.twilio.com/](https://www.twilio.com/)

{% hint style="info" %}
**What is Twilio?**

Twilio is a platform that uses web APIs to perform communication functions, such as text messaging and calls. Captivate Chat will automatically facilitate the connection between Twilio and your AI Chatbot.&#x20;
{% endhint %}

Click ![The upper right side of the screen of the Twilio homepage has "Start for Free" button that leads to the registration process.](<../../../../.gitbook/assets/image (6).png>) and follow the instructions to register a new account. You’ll need to provide your email address and set a password. Afterwards, you have to:

* **Verify your email.** Check your email for a verification link from Twilio and click on it to verify your account.&#x20;
* **Verify your phone number.** Twilio will ask you to **verify your phone number.** Just follow the on-screen instructions. It will involve receiving a validation code.&#x20;
* **Upgrade your account.** Your free trial won't be able to support Twilio to WhatsApp integrations that we need for Captivate Chat. Go to the upper part of your Twilio Console and click ![A new user will have a "Trial" status on the upper part of their Twilio dashboard and an "Upgrade" link beside it. Click the "Upgrade" link and follow its instructions to upgrade a user account.](<../../../../.gitbook/assets/image (175).png>), and follow the on-screen instructions to upgrade your account.&#x20;

***

## Creating a WhatsApp Sender

### Go to the Twilio Console (Dashboard)

<figure><img src="../../../../.gitbook/assets/image (8).png" alt="The Twilio dashboard."><figcaption><p>The Twilio dashboard.</p></figcaption></figure>

Log into Twilio. This will bring you to the **Twilio Console**, which serves as your main dashboard.

Alternatively, you can access the Twilio Console via [https://console.twilio.com/](https://console.twilio.com/)

### WhatsApp Senders

With your Twilio Paid Account, go to your Twilio Console and look for _**WhatsApp Senders**_. To do this, you have to:

1. Click ![The Messaging dropdown in the Twilio dashboard appears on the left-hand menu.](<../../../../.gitbook/assets/image (10).png>) in the left-hand menu.&#x20;
2. From the drop-down menu, find ![After clicking the Messaging dropdown button, find the Senders drop down button and click it.](<../../../../.gitbook/assets/image (11).png>) _**>**_ ![After going to Messaging > Senders in the Twilio Dashboard, find WhatsApp senders. Click it to open the WhatsApp senders page in Twilio.](<../../../../.gitbook/assets/image (12).png>)

Depending on what you've already done with Twilio, follow either of these steps:&#x20;

{% content-ref url="submit-your-first-whatsapp-sender.md" %}
[submit-your-first-whatsapp-sender.md](submit-your-first-whatsapp-sender.md)
{% endcontent-ref %}

{% content-ref url="setting-up-more-whatsapp-senders.md" %}
[setting-up-more-whatsapp-senders.md](setting-up-more-whatsapp-senders.md)
{% endcontent-ref %}
