---
description: Set up your AI Assistant as a WhatsApp Chatbot
---

# Channel: WhatsApp

After _**Select Channel > WhatsApp**_, you will be taken to **Configure WhatsApp**. This is where you can start integrating your AI Assistant into WhatsApp as a Chatbot that people can converse with.&#x20;

<figure><img src="../../.gitbook/assets/image (28) (1) (1).png" alt=""><figcaption></figcaption></figure>

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

## Configure WhatsApp

<figure><img src="../../.gitbook/assets/image (4).png" alt=""><figcaption></figcaption></figure>

Before you're able to integrate your AI Chatbot into WhatsApp, you have to fill up a few details:

* **Name:** This will be the assigned name of your AI Chatbot once it appears live on WhatsApp.
* **Description:** This is a short description assigned to your Chatbot.
* **Provider: Twilio** is set as the preset.

***

### Join Twilio

<figure><img src="../../.gitbook/assets/image (5).png" alt=""><figcaption></figcaption></figure>

In order to fill up the Account SID and Authentication Token, you have to **sign up for a Twilio** account.

Go to the **Twilio website** at [https://www.twilio.com/](https://www.twilio.com/)

{% hint style="info" %}
**What is Twilio?**

Twilio is a platform that uses web APIs to perform communication functions, such as text messaging and calls. Captivate Chat will automatically facilitate the connection between Twilio and your AI Chatbot.&#x20;
{% endhint %}

Click ![](<../../.gitbook/assets/image (6).png>) and follow the instructions to register a new account. You’ll need to provide your email address and set a password. Afterwards, you have to:

* **Verify your email.** Check your email for a verification link from Twilio and click on it to verify your account.&#x20;
* Twilio might ask you to **verify your phone number.** Just follow the on-screen instructions.&#x20;

### Go to the Twilio Console (Dashboard)

<figure><img src="../../.gitbook/assets/image (8).png" alt=""><figcaption></figcaption></figure>

Log into Twilio. This will bring you to the **Twilio Console**, which serves as your main dashboard.

Alternatively, you can access the Twilio Console via [https://console.twilio.com/](https://console.twilio.com/)

### Create your WhatsApp Sender

<figure><img src="../../.gitbook/assets/image (30).png" alt=""><figcaption></figcaption></figure>

With your Twilio Paid Account, go to your Twilio Console and look for _**WhatsApp Senders**_. To do this, you have to:

1. Click ![](<../../.gitbook/assets/image (10).png>) in the left-hand menu.&#x20;
2. From the drop-down menu, find ![](<../../.gitbook/assets/image (11).png>) _**>**_ ![](<../../.gitbook/assets/image (12).png>)
3. Click ![](<../../.gitbook/assets/image (13).png>)

Follow the on-screen instructions to apply for WhatsApp access. These steps will mostly involve filling up the required details about your business so you can request access to the WhatsApp API.&#x20;

#### Client Information

<figure><img src="../../.gitbook/assets/image (14).png" alt=""><figcaption></figcaption></figure>

Fill up your company's information.&#x20;

* **Client Business's Legal Name**
* **Client Email Address**
* **Client Meta Business Manager ID**

{% hint style="warning" %}
**Find the Meta Business Manager ID in the Meta Business Suite**

You can locate the Meta Business Manager ID via the Meta Business Suite. On the lower-left part of the screen, click _**Settings**_. When the new window loads, click the _**Business Portfolio Info**_ on the upper part of the screen. Copy the code under _**Business Portfolio ID**_.&#x20;
{% endhint %}

#### Select a Phone Number

<figure><img src="../../.gitbook/assets/image (15).png" alt=""><figcaption></figcaption></figure>

Choose a phone number. This will be **your company's designated WhatsApp number specifically for talking to your AI Chatbot.**

You have two options:

* You can **buy a Twilio phone number**. Access Twilio's list of available numbers via ![](<../../.gitbook/assets/image (18).png>), then clicking ![](<../../.gitbook/assets/image (19).png>) and selecting ![](<../../.gitbook/assets/image (20).png>).
* You can **use your own number**. Twilio calls this process as **BYON (Bring Your Own Number)**. Please follow the instructions in [this Twilio guide](https://help.twilio.com/articles/360052171393-Can-I-register-my-own-phone-number-for-WhatsApp-on-Twilio-?\_gl=1\*br9h2a\*\_gcl\_au\*MTY0OTYxMjg3OC4xNzI0MjQ2Mzc5\*\_ga\*NjAwMDE0NDcuMTcyNDI0NjM3OQ..\*\_ga\_RRP8K4M4F3\*MTcyNTM3MzY2MS43LjEuMTcyNTM3Mzg0Ni4wLjAuMA..).

Twilio has its own [Guided Onboarding document](https://www.twilio.com/docs/whatsapp/guided-onboarding) for a more in-depth look on this process, especially for steps outside Captivate Chat.

{% hint style="warning" %}
**Before selecting a number**

Take note of the Twilio warning before proceeding. Twilio has separate instructions if your phone number:

* ...is already connected to the WhatsApp consumer or small business app
* ...is already connected to the WhatsApp Business Platform via a different provider
{% endhint %}

{% hint style="info" %}
**Buy a Twilio number according to your needs**

If you plan on purchasing a Twilio number, do take note that the service allows you to buy a phone number using different filters. You can choose according to country, capabilities (Voice, SMS, MMS, Fax), and advanced filters such as address requirements.
{% endhint %}

{% hint style="danger" %}
**Get a phone number with SMS enabled**

Since we are going to integrate an AI Chatbot with WhatsApp, prioritize choosing a number with SMS enabled.&#x20;
{% endhint %}

#### Fill Out Your Public WhatsApp Sender Profile Information

<figure><img src="../../.gitbook/assets/image (16).png" alt=""><figcaption></figcaption></figure>

Fill up your business information. This data will be **submitted in order to request for WhatsApp to provide API access**.

* **Business Display Name**
* **Company Address**
* **Company Email**
* **Website**
* **Additional Website**
* **Vertical**
* **Link to Logo**
* **Profile About**

After filling up items in these steps, Twilio will handle the actual setup process with WhatsApp.&#x20;

{% hint style="danger" %}
**WhatsApp API is crucial to the integration**

This step is perhaps **the most important** when it comes to WhatsApp integration. WhatsApp needs to give you access to its API so we can place your AI Chatbot in the system.&#x20;
{% endhint %}

{% hint style="info" %}
**Visible to end users**

Some text boxes you have to fill up are indicated as **visible to end users**. This means the information placed here will be available for end users to see while interacting with your AI Chatbot.&#x20;
{% endhint %}

{% hint style="warning" %}
**Submitting a wrong business display can cause 2-4 week delays**

Before submitting your request, make sure you're submitting the right information about your business. This is especially the case with the **Business Display Name**. Follow [WhatsApp's Display Name Guidelines](https://www.facebook.com/business/help/338047025165344#display-name-guidelines).
{% endhint %}

### Accept the Request from Twilio in your Meta Business Suite

<figure><img src="../../.gitbook/assets/image (21).png" alt=""><figcaption></figcaption></figure>

After setting up your **WhatsApp Sender**, you will receive a notification in your Meta Business Suite that says Twilio is asking for permissions to send messages on your behalf.&#x20;

To access this, go to your **Meta Business Suite**. From here:

1. Click ![](<../../.gitbook/assets/image (23).png>)
2. Go to ![](<../../.gitbook/assets/image (24).png>)
3. Find and **accept** the Twilio request.&#x20;

***

### Configure the Endpoint for Integration

<figure><img src="../../.gitbook/assets/image (29).png" alt=""><figcaption></figcaption></figure>

Once you have your WhatsApp number approved, they should appear in the WhatsApp Senders list. Access this again by going to your Twilio Console and:

1. Click ![](<../../.gitbook/assets/image (10).png>) in the left-hand menu.&#x20;
2. From the drop-down menu, find ![](<../../.gitbook/assets/image (11).png>) _**>**_ ![](<../../.gitbook/assets/image (12).png>)

From this list, click the WhatsApp number you dedicated to your AI Chatbot.

<figure><img src="../../.gitbook/assets/image (28).png" alt=""><figcaption></figcaption></figure>

Find the section called **Endpoint Configuration**. Under the **Webhook URL for Incoming Messages**, paste the following:

```
https://channel.prod.captivat.io/api/whatsapp/twilio/integration 
```

After entering the URL, click _**Save**_ or _**Update**_ to apply the changes.&#x20;

### Copy the Account SID and Authentication Token

<figure><img src="../../.gitbook/assets/image (27).png" alt=""><figcaption></figcaption></figure>

Back in the Twilio Console, locate your **Account SID** and **Auth Token.**

They should be located on the ![](<../../.gitbook/assets/image (31).png>).

### Paste the Account SID and Authentication Token in Captivate Chat

<figure><img src="../../.gitbook/assets/image (32).png" alt=""><figcaption></figcaption></figure>

Go back to Captivate Chat.&#x20;

1. Paste the copied Account SID and Authentication Token into the respective fields.
2. Click _**Next**_.

***

### Testing WhatsApp Configuration

<figure><img src="../../.gitbook/assets/image (34).png" alt=""><figcaption></figcaption></figure>

You should be ready to use WhatsApp on Twilio, thanks to Captivate Chat integration!

Locate your AI Chatbot by inputting the assigned WhatsApp number in your WhatsApp program.

Type a message and wait for your AI Chatbot to respond.&#x20;

***

## You're all set!

Doing all the steps above should get your Chatbot ready to be used with WhatsApp.
