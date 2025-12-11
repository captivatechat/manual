# Integrate a Google Sheet to AI Chatbot

<figure><img src="../../../.gitbook/assets/image (312).png" alt="Under the &#x22;Select Integration&#x22; page, selecting &#x22;Google Sheets&#x22; and clicking &#x22;Configure&#x22; will take users to a &#x22;Customize Integration&#x22; page where they have to insert their Google Sheet&#x27;s Sheet ID. After that, they should click &#x22;Next&#x22; to finish the integration process."><figcaption><p>Under the "Select Integration" page, selecting "Google Sheets" and clicking "Configure" will take users to a "Customize Integration" page where they have to insert their Google Sheet's Sheet ID. After that, they should click "Next" to finish the integration process.</p></figcaption></figure>

You can also select **Google Sheets** as your AI Chatbot integration. With this selected, users who want to transition to a Live Agent will have their name and email address auto-populate the sheet named "Customers" within your Google Sheet file.&#x20;

{% hint style="danger" %}
**Your Google Sheet needs to be editable by everyone**

Before you start the integration process that connects your Google Sheet to your AI Chatbot, make sure that your selected Google Sheet has its permissions set to be editable by everyone!&#x20;

To do this, please follow the steps in [this link](https://www.youtube.com/watch?v=Dv8s4QxZlDk).&#x20;

You can also simply click the blue _"Share"_ button on the upper right of your Google Sheet. Under _"General Access,"_ click _"Anyone with the link"_ and select _"Can edit."_&#x20;
{% endhint %}

{% hint style="danger" %}
**You need to create a "Customers" sheet first!**

Before you integrate your Google Sheet into your AI Chatbot, your selected Google Sheet needs to have its _"Sheet 1"_ renamed as `Customers`.&#x20;

This is where we will send the user data gathered by your AI Chatbot.
{% endhint %}

To integrate Google Sheets into your AI Chatbot:

1. Select the Google Sheets icon under "Select Integration."
2. Click ![The "Configure" button in the "Select Integration" page will let users configure the information of the platform they selected. The "Select Integration" page within the AI Chatbot creation process can assign the AI Chatbot to get user data from their conversations and store them in a selected integration platform: HubSpot, Email, or Google Sheets.](<../../../.gitbook/assets/image (308).png>).
3. Enter your **the Sheet ID** of your preferred Google Sheets file.&#x20;
4. Click !["Next" in the context of Select Integration > Google Sheet > Configure > Customize Integration will integrate the selected Google Sheet into the AI Chatbot. ](<../../../.gitbook/assets/image (310).png>).

{% hint style="info" %}
**Where is my Sheet ID?**

Your Google Sheet ID is located in the URL:&#x20;

_docs.google.ocm/spreadsheets/d/_`<this-is-the-sheet-id>` _/edit?gid=0#gid=0_
{% endhint %}

{% hint style="warning" %}
**Only the user's names and emails will be sent to your Google Sheets file**

Please note that, at this time, the Captivate Chat Google Sheet Integration **only captures the user’s name and email**.&#x20;

Any future improvements, such as support for custom forms, may be added in future updates and releases.
{% endhint %}

***



Once you're done placing your integration, click ![If you made it to the "Select Integration" page of the AI Chatbot creation process, leave it be and click "Update AI Chatbot" to finish the AI Chatbot creation process.](<../../../.gitbook/assets/image (3) (1) (1) (1) (1) (1) (1) (1).png>)  to finish the AI Chatbot setup.
