# Setting up more WhatsApp Senders



<figure><img src="../../../../.gitbook/assets/image (178).png" alt="This time around, a &#x22;Getting started with WhatsApp&#x22; page will appear for all users who want to create WhatsApp senders after their first. The &#x22;Getting started with WhatsApp&#x22; window appears after clicking Messaging > Senders > WhatsApp Senders and clicking the &#x22;Create New Sender&#x22; button. Click &#x22;Get Started&#x22; to begin the process of creating another WhatsApp sender."><figcaption><p>This time around, a "Getting started with WhatsApp" page will appear for all users who want to create WhatsApp senders after their first. The "Getting started with WhatsApp" window appears after clicking Messaging > Senders > WhatsApp Senders and clicking the "Create New Sender" button. Click "Get Started" to begin the process of creating another WhatsApp sender.</p></figcaption></figure>



After going to the WhatsApp Senders menu, begin the process of creating your WhatsApp Sender. To do this, you have to:&#x20;

1. Click ![The "Get Started" button will appear in the "Get started with WhatsApp" page after if "Click New Sender" in Messaging > Senders > WhatsApp Senders is clicked by a user who already made their first WhatsApp sender.](<../../../../.gitbook/assets/image (179).png>)
2. Acknowledge and accept the Terms & Conditions presented in the new window.

### Select a Phone Number to register

<figure><img src="../../../../.gitbook/assets/image (181).png" alt="The first step to create a new WhatsApp Sender for users who already have existing senders is to select a phone number to register. They can use their own number by following special instructions or buy a Twilio phone number."><figcaption><p>The first step to create a new WhatsApp Sender for users who already have existing senders is to select a phone number to register. They can use their own number by following special instructions or buy a Twilio phone number.</p></figcaption></figure>

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

### Link WhatsApp Business Account with your number

<figure><img src="../../../../.gitbook/assets/image (182).png" alt="The second step to create a new WhatsApp Sender for users who already have existing senders is to link their chosen number to a WhatsApp business account."><figcaption><p>The second step to create a new WhatsApp Sender for users who already have existing senders is to link their chosen number to a WhatsApp business account.</p></figcaption></figure>

The next stage in the process involves **creating or select a pre-made WhatsApp Business Account** and verifying it to be used with Twilio.

#### 1. Link your WhatsApp Business Account

<figure><img src="../../../../.gitbook/assets/image (183).png" alt="In order to link a phone number to a WhatsApp Business Account in Twilio, click &#x22;Continue with Facebook&#x22; button in the &#x22;Create New Sender&#x22; procedure to open Facebook in a new window."><figcaption><p>In order to link a phone number to a WhatsApp Business Account in Twilio, click "Continue with Facebook" button in the "Create New Sender" procedure to open Facebook in a new window.</p></figcaption></figure>

You will be prompted to connect your chosen number to a WhatsApp Business Account. Click ![In order to link a phone number to a WhatsApp Business Account in Twilio, click "Continue with Facebook" button in the "Create New Sender" procedure to open Facebook in a new window.](<../../../../.gitbook/assets/image (184).png>) to start the setup process. Follow the instructions in the new window.

#### 2. Copy the phone number you want to register

<figure><img src="../../../../.gitbook/assets/image (185).png" alt="After &#x22;Continue with Facebook&#x22; button opens Facebook in a pop-up window, users can copy their selected phone number into the clipboard by clicking the &#x22;Copy&#x22; button beside it."><figcaption><p>After "Continue with Facebook" button opens Facebook in a pop-up window, users can copy their selected phone number into the clipboard by clicking the "Copy" button beside it.</p></figcaption></figure>

Part of the verification process will involve copying your designated phone number over to the Facebook pop-up window. Click ![After "Continue with Facebook" button opens Facebook in a pop-up window, users can copy their selected phone number into the clipboard by clicking the "Copy" button beside it.](<../../../../.gitbook/assets/image (186).png>) to place your chosen number in the clipboard.

#### 3. Verify the selected number with WhatsApp

<figure><img src="../../../../.gitbook/assets/image (187).png" alt="Users should press the &#x22;Send Code&#x22; in the Facebook pop-up window to send a verification code to the selected phone number. The code automatically appears in the blank spaces in the Twilio page of the WhatsApp Sender creation process."><figcaption><p>Users should press the "Send Code" in the Facebook pop-up window to send a verification code to the selected phone number. The code automatically appears in the blank spaces in the Twilio page of the WhatsApp Sender creation process.</p></figcaption></figure>

Press the **Send Code** over in the Faceobok pop-up window. A verification code should automatically appear on the blank spaces below.&#x20;

Twilio should be attempting to register the phone number to WhatsApp. The process generally takes a few moments. The upper-right of the screen will provide these status messages:

<figure><img src="../../../../.gitbook/assets/image (189).png" alt="Status updates will appear on the upper-right side of the Twilio dashboard during the WhatsApp number registration process. The first status will be an attempt to register the WhatsApp sender, and another is the confirmation of a successful registration."><figcaption><p>Status updates will appear on the upper-right side of the Twilio dashboard during the WhatsApp number registration process. The first status will be an attempt to register the WhatsApp sender, and another is the confirmation of a successful registration.</p></figcaption></figure>

***

### Find your new WhatsApp Sender

<figure><img src="../../../../.gitbook/assets/image (177).png" alt="After verifying the new WhatsApp number in the separate window, users will be redirected to the WhatsApp Senders page. Their new WhatsApp sender should appear. "><figcaption><p>After verifying the new WhatsApp number in the separate window, users will be redirected to the WhatsApp Senders page. Their new WhatsApp sender should appear. </p></figcaption></figure>

After verifying your new WhatsApp number, you will be redirected to your list of WhatsApp Senders. Your new WhatsApp sender should be in this list and ready to be integrated in a Captivate Chat Flow.

To create another WhatsApp sender, click ![The "Create new sender" button in the Messaging > Senders > WhatsApp Senders page of Twilio will take users to the process of creating a WhatsApp Sender.](<../../../../.gitbook/assets/image (180).png>) on the upper-right part of the menu.
