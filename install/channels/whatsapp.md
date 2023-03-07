# WhatsApp

## Installation

1. On dashboard, click **"Create now"** or **"Create conversation"**

![Figure 1: The Captivate Hub Dashboard](https://1215041517-files.gitbook.io/\~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2F-Mi0FFC-4Qd4Qxv4dQte%2Fuploads%2FF1gnvyEpXZ0LGyf98f4h%2Fimage.png?alt=media\&token=06e5b3c7-6944-4a42-b92a-3df091a1fe34)

2\. Choose the **WhatsApp** as channel

![Figure 2: Supported Channels](https://1215041517-files.gitbook.io/\~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2F-Mi0FFC-4Qd4Qxv4dQte%2Fuploads%2FvIRE7X37JFKyfmNJlwug%2Fimage.png?alt=media\&token=0399206c-92f2-4317-be94-a34c86944808)



### Sandbox

1. Create a Twilio account.
2. Take note of your `Account SID`, and `Auth Token` on your account page.
3. Enable Whatsapp sandbox for Twilio.
4. Supply the channel webhook url: `https://channel.prod.captivat.io/api/whatsapp/twilio/integration`.
5. Remember the whatsapp number, and the key to join the sandbox.
6. Supply the `Account SID` and `Auth Token` on the hub.
7. To verify if it's working, open your whatsapp app, then message the whatsapp number in your sandbox, send the code given to join the sandbox. The chatbot should reply now.

### WhatsApp for Business

1. Go to Programmable Messaging and select Senders. be sure you have phone number already on the twilio account.
2. Click WhatsApp Senders and supply the necessity information
3. Apply for WhatsApp for Business for twilio by answering this form [https://www.twilio.com/whatsapp/request-access](https://www.twilio.com/whatsapp/request-access)
4. After activation of the WhatsApp request. follow the sandbox instruction but on the WhatsApp sender this time.
