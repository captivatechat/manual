---
description: Set up your AI Assistant as a WhatsApp Chatbot
---

# Submit your first WhatsApp Sender

<figure><img src="../../../../.gitbook/assets/image (30).png" alt="When users create a WhatsApp sender in Twilio for the first time, they will be taken to a Guided Signup window."><figcaption><p>When users create a WhatsApp sender in Twilio for the first time, they will be taken to a Guided Signup window.</p></figcaption></figure>

In this new **Guided Signup** window, click ![The "Create new sender" button in the Messaging > Senders > WhatsApp Senders page of Twilio will take users to the process of creating a WhatsApp Sender.](<../../../../.gitbook/assets/image (13).png>).&#x20;

{% hint style="warning" %}
**This is the same form when you create new senders**

The process below has the same forms to fill out when creating new senders beyond your first.&#x20;
{% endhint %}

***

### Request WhatsApp Senders

Follow the on-screen instructions to apply for WhatsApp access. These steps will mostly involve filling up the required details about your business so you can request access to the WhatsApp API.&#x20;

#### Client Information

<figure><img src="../../../../.gitbook/assets/image (14).png" alt="The first step of creating a first WhatsApp sender in Twilio is to fill up Client Information with the Business&#x27;s Legal Name, its email address, and its Meta Business Manager ID."><figcaption><p>The first step of creating a first WhatsApp sender in Twilio is to fill up Client Information with the Business's Legal Name, its email address, and its Meta Business Manager ID.</p></figcaption></figure>

Fill up your company's information.&#x20;

* **Client Business's Legal Name**
* **Client Email Address**
* **Client Meta Business Manager ID**

{% hint style="warning" %}
**Find the Meta Business Manager ID in the Meta Business Suite**

You can locate the Meta Business Manager ID via the Meta Business Suite. On the lower-left part of the screen, click _**Settings**_. When the new window loads, click the _**Business Portfolio Info**_ on the upper part of the screen. Copy the code under _**Business Portfolio ID**_.&#x20;
{% endhint %}

#### Select a Phone Number

<figure><img src="../../../../.gitbook/assets/image (15).png" alt="The second step of creating a first WhatsApp sender in Twilio is to Select a Phone Number. Users can choose an existing WhatsApp number by following special instructions or buy a new Twilio number."><figcaption><p>The second step of creating a first WhatsApp sender in Twilio is to Select a Phone Number. Users can choose an existing WhatsApp number by following special instructions or buy a new Twilio number.</p></figcaption></figure>

Choose a phone number. This will be **your company's designated WhatsApp number specifically for talking to your AI Chatbot.**

You have two options:

* You can **buy a Twilio phone number**. Access Twilio's list of available numbers via ![The Phone Numbers dropdown is located on the left-hand side of the Twilio screen.](<../../../../.gitbook/assets/image (18).png>), then clicking ![The Manage dropdown menu is located under Phone Numbers on the left-hand side of the Twilio dashboard.](<../../../../.gitbook/assets/image (19).png>) and selecting ![Buy a Twilio phone number by going to Phone Numbers > Manage in the Twilio dashboard then clicking "Buy a number."](<../../../../.gitbook/assets/image (20).png>).
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

<figure><img src="../../../../.gitbook/assets/image (16).png" alt="The third step of creating a first WhatsApp sender in Twilio is to fill up public WhatsApp Sender profile information with the company&#x27;s display name, address, email, websites, vertical, logo link, and an about statement."><figcaption><p>The third step of creating a first WhatsApp sender in Twilio is to fill up public WhatsApp Sender profile information with the company's display name, address, email, websites, vertical, logo link, and an about statement.</p></figcaption></figure>

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

***

### Accept the Request from Twilio in your Meta Business Suite

<figure><img src="../../../../.gitbook/assets/image (21).png" alt="After completing the form to create a first WhatsApp sender in Twilio, users should go to their Meta Business Suite and accept the request from Twilio. "><figcaption><p>After completing the form to create a first WhatsApp sender in Twilio, users should go to their Meta Business Suite and accept the request from Twilio. </p></figcaption></figure>

After setting up your **WhatsApp Sender**, you will receive a notification in your Meta Business Suite that says Twilio is asking for permissions to send messages on your behalf.&#x20;

To access this, go to your **Meta Business Suite**. From here:

1. Click ![To access requests in the Meta Business Suite, go to the Meta Business Suite and click the Settings button.](<../../../../.gitbook/assets/image (23).png>)
2. Go to ![Under the Settings in Meta Business Suite, access pending requests by clicking the Requests button.](<../../../../.gitbook/assets/image (24).png>)
3. Find and **accept** the Twilio request.&#x20;

***

### Find your new WhatsApp Sender

<figure><img src="../../../../.gitbook/assets/image (176).png" alt=""><figcaption><p>After accepting the request from Twilio in Meta Business Suite, users can go back to the Twilio dashboard and go to Messaging > Senders > WhatsApp Senders page. Their first WhatsApp sender should appear. </p></figcaption></figure>

After accepting the Twilio request, you should see your number in the list of WhatsApp Senders. Your WhatsApp number is now ready for integration in your Chat Flow.

To create another WhatsApp sender, click ![The "Create new sender" button in the Messaging > Senders > WhatsApp Senders page of Twilio will take users to the process of creating a WhatsApp Sender.](<../../../../.gitbook/assets/image (180).png>) on the upper-right part of the menu.
