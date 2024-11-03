---
description: Set up your AI Assistant as a WhatsApp Chatbot
---

# Channel: WhatsApp

<figure><img src="../../../../.gitbook/assets/image (297).png" alt="After selecting an AI Chatbot in &#x22;Step 1: Select Chatbot,&#x22; choose &#x22;WhatsApp&#x22; in &#x22;Step 2: Select Channel&#x22; in the Chat Flow creation process. The button will be highlighted blue. Click &#x22;Next&#x22; to proceed."><figcaption><p>After selecting an AI Chatbot in "Step 1: Select Chatbot," choose "WhatsApp" in "Step 2: Select Channel" in the Chat Flow creation process. The button will be highlighted blue. Click "Next" to proceed.</p></figcaption></figure>

After _**Select Channel > WhatsApp**_, you will be taken to _**Configure WhatsApp**_. This is where you can start integrating your AI Assistant into WhatsApp as a Chatbot that people can converse with.&#x20;

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

***

## Configure WhatsApp

<figure><img src="../../../../.gitbook/assets/image (28) (1) (1).png" alt=""><figcaption><p>After selecting WhatsApp and clicking "Next" in "Step 2: Select Channel" of the Chat Flow creation process, you will go to the "Configure WhatsApp" page.</p></figcaption></figure>

You will be taken to a _**Configure WhatsApp**_ page after selecting WhatsApp in _**Step 2: Select Channel.**_&#x20;

This window contains the necessary information that have to be filled out before WhatsApp becomes integrated to your Chat Flow.

### Basic Information

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
