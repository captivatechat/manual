---
description: Set up your AI Assistant as a WhatsApp Chatbot
---

# Channel: WhatsApp

After _**Select Channel > WhatsApp**_, you will be taken to **Configure WhatsApp**. This is where you can start integrating your AI Assistant into WhatsApp as a Chatbot that people can converse with.&#x20;

<figure><img src="../../../../.gitbook/assets/image (28) (1) (1).png" alt=""><figcaption></figcaption></figure>

{% hint style="danger" %}
**Make sure you have a Facebook Business Account!**

Our integration only works if you have a Facebook Business Account.

Make sure it is a **verified** account by following the steps in this [guide from Meta](https://www.facebook.com/business/help/2058515294227817?id=180505742745347).
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

***

## Configure WhatsApp

<figure><img src="../../../../.gitbook/assets/image (4) (1).png" alt=""><figcaption></figcaption></figure>

Before you're able to integrate your AI Chatbot into WhatsApp, you have to fill up a few details:

* **Name:** This will be the assigned name of your AI Chatbot once it appears live on WhatsApp.
* **Description:** This is a short description assigned to your Chatbot.
* **Provider: Twilio** is set as the preset.

***

## Join Twilio

<figure><img src="../../../../.gitbook/assets/image (5).png" alt=""><figcaption></figcaption></figure>

In order to fill up the Account SID and Authentication Token, you have to **sign up for a Twilio** account.

Go to the **Twilio website** at [https://www.twilio.com/](https://www.twilio.com/)

{% hint style="info" %}
**What is Twilio?**

Twilio is a platform that uses web APIs to perform communication functions, such as text messaging and calls. Captivate Chat will automatically facilitate the connection between Twilio and your AI Chatbot.&#x20;
{% endhint %}

Click ![](<../../../../.gitbook/assets/image (6).png>) and follow the instructions to register a new account. You’ll need to provide your email address and set a password. Afterwards, you have to:

* **Verify your email.** Check your email for a verification link from Twilio and click on it to verify your account.&#x20;
* **Verify your phone number.** Twilio will ask you to **verify your phone number.** Just follow the on-screen instructions. It will involve receiving a validation code.&#x20;
* **Upgrade your account.** Your free trial won't be able to support Twilio to WhatsApp integrations that we need for Captivate Chat. Go to the upper part of your Twilio Console and click ![](<../../../../.gitbook/assets/image (175).png>), and follow the on-screen instructions to upgrade your account.&#x20;

***

## Creating a WhatsApp Sender

### Go to the Twilio Console (Dashboard)

<figure><img src="../../../../.gitbook/assets/image (8).png" alt=""><figcaption></figcaption></figure>

Log into Twilio. This will bring you to the **Twilio Console**, which serves as your main dashboard.

Alternatively, you can access the Twilio Console via [https://console.twilio.com/](https://console.twilio.com/)

### WhatsApp Senders

With your Twilio Paid Account, go to your Twilio Console and look for _**WhatsApp Senders**_. To do this, you have to:

1. Click ![](<../../../../.gitbook/assets/image (10).png>) in the left-hand menu.&#x20;
2. From the drop-down menu, find ![](<../../../../.gitbook/assets/image (11).png>) _**>**_ ![](<../../../../.gitbook/assets/image (12).png>)

Depending on the window that appears, follow either of these steps:&#x20;

{% content-ref url="setting-up-more-whatsapp-senders.md" %}
[setting-up-more-whatsapp-senders.md](setting-up-more-whatsapp-senders.md)
{% endcontent-ref %}

{% content-ref url="submit-your-first-whatsapp-sender.md" %}
[submit-your-first-whatsapp-sender.md](submit-your-first-whatsapp-sender.md)
{% endcontent-ref %}
