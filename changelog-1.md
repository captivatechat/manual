---
description: >-
  All changes to the Captivate Hub will be added here. Guides will be updated
  concurrently.
hidden: true
---

# 📕 Copy of Changelog



## 📆 v3.4.0 - 2025-01-03

### ✅ Added

* **Tutorials are live!** Learn the ropes in creating your AI Chatbots, Chat Flows, and Live Agent integrations within the Tutorial page of the Captivate Chat platform!
* **Meet our Guidebot!** We've deployed our Guidebot within the Captivate Chat platform! Once you log in to your account, you can ask our Guidebot for any advice as well as tips and tricks on how to best use Captivate Chat for your needs!
* We now support **SCA Stripe**. SCA, which stands for Strong Customer Authentication, allows us to offer more secure transactions when purchasing Captivate Chat Tokens or upgrading your subscriptions.
* **Mobile Optimization notice** appears when users to try to access Captivate Chat on mobile platforms.&#x20;
* **AI Chatbots:**
  * **Select Integrations** within AI Chatbots are now fully functional. User emails and names will be sent to the platforms you integrated into the AI Chatbot during the AI Chatbot Creation and AI Chatbot Update processes.
  * **URL Crawler** is now added under "Import Your Own Information" that auto-searches all URLs under a single URL. This will make importing groups of URLs under a "mother" URL much easier.&#x20;
  * You can now set **session expiration timers** within an AI Chatbot so they can automatically end an inactive session after your specified period of time.

### 🟧 Changed

* **Our Token Estimator now uses Server-Sent Events (SSEs)**. Thanks to SSEs, we should be experiencing faster and more efficient resource management. With SSEs, AI Chatbots should be able to ingest new information much faster.
* **Cost-Saving toggle for Chat Histories are available globally.** We will now provide a global toggle for users to choose if they want to view the full or AI-analyzed chat histories of their AI Chatbots.&#x20;
  * This is unlike in previous versions, where this toggle is placed inside each AI Chatbot.&#x20;
  * As per the previous version, the AI-analyzed chat histories will cost fewer tokens to produce.&#x20;

### 🆕 Tutorials

<figure><img src=".gitbook/assets/image (313).png" alt="The &#x22;Tutorial&#x22; page in the Captivate Chat platform contain videos that explain essential processes in using Captivate Chat. They are arranged in tiles, with a thumbnail and the name of the lesson."><figcaption><p>The "Tutorial" page in the Captivate Chat platform contain videos that explain essential processes in using Captivate Chat. They are arranged in tiles, with a thumbnail and the name of the lesson.</p></figcaption></figure>

Learning about Captivate Chat has never been easier!

Get in-depth tutorials on how to use the Captivate Chat platform using our **Tutorials** page! We have Tutorials for most of our processes in the platform, and we'll constantly update these Tutorials whenever we have major releases.&#x20;

To access our Tutorials, simply click the ![The "Tutorials" button on the left side of the dashboard leads to the "Tutorial" page. The The "Tutorial" page in the Captivate Chat platform contain videos that explain essential processes in using Captivate Chat. They are arranged in tiles, with a thumbnail and the name of the lesson.](<.gitbook/assets/image (315).png>) button on the left side of the Captivate Chat dashboard.

### 🆕 Select Integration

<figure><img src=".gitbook/assets/image (316).png" alt="The &#x22;Select Integration&#x22; page of the AI Chatbot creation process will let users choose what platform they want to use to receive data from AI Chatbots. This integration will store the emails and names of users that ask an AI Chatbot to connect them to a Live Agent."><figcaption><p>The "Select Integration" page of the AI Chatbot creation process will let users choose what platform they want to use to receive data from AI Chatbots. This integration will store the emails and names of users that ask an AI Chatbot to connect them to a Live Agent.</p></figcaption></figure>

The **Select Integration** page of the AI Chatbot creation process is now live. Users can use this page to customize where their AI Chatbots will send customer data whenever they ask AI Chatbots to connect them to Live Agents.&#x20;

We currently offer HubSpot, Email, and Google Sheets as our integration platforms. As of now, we can only collect a user's name and email address.&#x20;

### 🆕 URL Crawler

<figure><img src=".gitbook/assets/image (317).png" alt="The &#x22;Import Your Own Information&#x22; page of the AI Chatbot creation process now features a URL Crawler. This is accessed via pressing the &#x22;Import Button.&#x22; With this, users can now enter one URL and it will take the first layer of URLs sharing its section. "><figcaption><p>The "Import Your Own Information" page of the AI Chatbot creation process now features a URL Crawler. This is accessed via pressing the "Import Button." With this, users can now enter one URL and it will take the first layer of URLs sharing its section. </p></figcaption></figure>

We've added a **URL Crawler** to the "Import Your Own Information" page of the AI Chatbot creation process. Users can now choose to enter a URL and Captivate Chat will gather all relevant URLs of its similar section.

If you want to retrieve relevant URLs within a particular website layer, the URL Crawler can also be used with a **wildcard character or an asterisk (\*)**.&#x20;

### 🆕 Mobile Optimization Notice

<figure><img src=".gitbook/assets/image (318).png" alt="The Captivate Chat platform can be opened in mobile browsers but it&#x27;s not yet optimized for mobile devices. We&#x27;ve added a Mobile Optimization Notice to warn users that while they can proceed to the Captivate Chat platform, its functions might not work properly in their device."><figcaption><p>The Captivate Chat platform can be opened in mobile browsers but it's not yet optimized for mobile devices. We've added a Mobile Optimization Notice to warn users that while they can proceed to the Captivate Chat platform, its functions might not work properly in their device.</p></figcaption></figure>

We added a **Mobile Optimization Notice** for users trying to access our platform using their mobile devices.

As have yet to fully optimize the Captivate Chat platform for mobile users, this means many functions of the Captivate Chat platform might not work properly in mobile browsers. You can continue to use the platform normally via mobile by clicking "Continue to Site" when you see the Mobile Optimization Notice.

***

## 📆 v3.2.0 - 2024-10-02

### ✅ Added

* **Token Metrics** are now revealed for major AI Chatbot uses such as ingesting information, training, and various conversations to aid payment tracking.
* **AI Chatbots** now have a limiter and organizer to maximize Token usage without overwhelming their systems. This should lessen situations of AI Chatbots randomly slowing down.&#x20;

### 🟧 Changed

* **Web Widget Preview:** The Web Widget Preview now has a more noticeable _Page Settings_ button to access its features.
* **Import Your Own Information (AI Chatbots):** Pagination should now reveal ingested PDFs and URLs in sets of 10 for more efficient compilation and access to users.&#x20;

### ⚠️ Fixed

* Made minor adjustments to the UI to improve accessibility and encourage a more engaging experience.&#x20;
* Streamlined Token tracking so users are immediately notified if they have run out of Tokens.
* Ensured that **delete** information (URLs, PDFs, accounts) are permanently deleted as intended.&#x20;
* **Microsoft Teams:** Transcripts of the AI Chatbot's conversation with a user are now retained when their concern is escalated to a Live Chat agent in MS Teams.

### 🆕 Token Metrics

<figure><img src=".gitbook/assets/image (6) (1) (1) (1).png" alt="Tokens are now tracked throughout Captivate Chat features. The main Token count is revealed on the left side of the dashboard at all times, giving users an idea how many Tokens they have consumed, when their next Monthly Usage Reset would be, and any Extra Tokens they possess."><figcaption><p>Tokens are now tracked throughout Captivate Chat features. The main Token count is revealed on the left side of the dashboard at all times, giving users an idea how many Tokens they have consumed, when their next Monthly Usage Reset would be, and any Extra Tokens they possess.</p></figcaption></figure>

The Captivate Chat platform will now show **token metrics** to keep track of your Tokens whenever you use them across various parts of the platform. These include:

* Ingesting data that are uploaded into the system.
* Conversations between users and the AI Chatbots they create.
* Testing and deploying AI Chatbots in various platforms.

These token metrics can aid in managing your Captivate Chat plan, as major AI functionalities of the platform rely heavily in Token usage.

In line with this new change, we are also going to **actively track** Token usage across the platform and notify users whenever they have to purchase more Tokens.&#x20;

### 🆕We revamped the Web Widget Preview

<figure><img src=".gitbook/assets/image (8) (1) (1).png" alt="The Web Widget Preview of Setup > Chat Flow > Channels > Web Widget is revamped with a more streamlined look."><figcaption><p>The Web Widget Preview of Setup > Chat Flow > Channels > Web Widget is revamped with a more streamlined look.</p></figcaption></figure>

We've upgraded the look of our **Web Widget Preview**!&#x20;

You can now preview your Web Widget Chat Flow with a completely revamped background.

<figure><img src=".gitbook/assets/image (7) (1) (1).png" alt="The Web Widget Preview of Setup > Chat Flow > Channels > Web Widget now has a more visible &#x22;Page Settings&#x22; button to edit the live preview."><figcaption><p>The Web Widget Preview of Setup > Chat Flow > Channels > Web Widget now has a more visible "Page Settings" button to edit the live preview.</p></figcaption></figure>

The ![](<.gitbook/assets/image (9) (1) (1).png>) button is now more visible and accessible, making it much easier for users to modify their live preview setup.&#x20;

***

## 📆 v3.1.1 - 2024-09-19

### ✅ Added

* **Makeover!** We've updated the Captivate Chat website to feature our new logos!
* **Edit AI Chatbots while making Chat Flows!** You can now directly modify your AI Chatbots while creating your Chat Flows.&#x20;

### 🟧 Changed

* **Transcripts** now feature a separate **Date Range** filter instead of the previous **By Date** sorting filter.&#x20;

### ⚠️ Fixed

* Fixed a bug that doesn't load the complete list of ingested content for some Chat Flows.
* **Chat Flow > Channel > Web Widget:** Fixed a typo. There is now an _"Embed Web Widget"_ option instead of the previous _"Embed Live Chat"_ option.

### 🆕 Website Makeover!

<figure><img src=".gitbook/assets/image (4) (1) (1) (1) (1).png" alt="The new Captivate Chat website featuring its updated logo with a blue color palette. "><figcaption><p>The new Captivate Chat website featuring its updated logo with a blue color palette. </p></figcaption></figure>

We're giving the Captivate Chat website a major makeover!&#x20;

This new update features **new logos** we've prepared for Captivate Chat, now featuring a sleek blue color palette designed to evoke a more professional and relaxing atmosphere.&#x20;

### 🆕 Edit your AI Chatbots while making Chat Flows

<figure><img src=".gitbook/assets/image (5) (1) (1) (1) (1).png" alt="Users can now click the three dots above their AI Chatbot choice in Setup > Chat Flow > My AI Chatbots to directly modify their AI Chatbots during the Chat Flow creation process."><figcaption><p>Users can now click the three dots above their AI Chatbot choice in Setup > Chat Flow > My AI Chatbots to directly modify their AI Chatbots during the Chat Flow creation process.</p></figcaption></figure>

We know that creating an AI Chatbot from scratch is wildly different when compared to connecting them to the rest of your Channels and Live Chats via a Chat Flow, as there are things you would only notice about your AI Chatbot after bringing everything together.

It's for this reason that we added a new feature that lets you **edit your AI Chatbots during the Chat Flow creation process**. After clicking _Setup > Chat Flow_, the list of AI Chatbots present in _My AI Chatbots_ menu now feature a three dots that enable you to edit them straight in the Chat Flow-creation process.

This means you no longer have to go all the way back to _Setup > AI Chatbot_ just to modify an AI Chatbot you'd use for your current Chat Flow - you can do everything in one convenient location.

***

## 📆 v3.0.0 - 2024-09-18

### ✅ Added

* **Incident Tracker** now informs users whenever Captivate Chat services are down.
* **Overwrite Warning** will inform users that changing the Channel of an existing Chat Flow will remove their current setup.&#x20;

### 🟧 Changed

* **Transcripts** now feature various options to simplify their use, such as sorting and deletion options.

### ⚠️ Fixed

* AI Chatbots now properly recognizes postal codes of locations.
* AI Chatbots no longer declares in a separate chat message that they are checking for available Live Chat agents upon request, as we already have a preset message prepared when users ask to be escalated to a Live Chat agent.&#x20;
* **AI Chatbots > Select Type:** Removed a bug that triggers the _"Submit & Test"_ function whenever users select a tooltip.&#x20;

### 🆕 Overwrite Warning (Chat Flow)

<figure><img src=".gitbook/assets/image (5) (1) (1) (1).png" alt="Trying to change the Channel of an existing Chat Flow will now provide a warning to users that doing so will overwrite their existing data."><figcaption><p>Trying to change the Channel of an existing Chat Flow will now provide a warning to users that doing so will overwrite their existing data.</p></figcaption></figure>

We have included an **override warning** in Chat Flows that will activate whenever users try to change the Channel of an existing Chat Flow. Undergoing this process will overwrite their data, and any overwritten data can no longer be retrieved.

It's advisable for users to duplicate their existing Chat Flow before switching Channels, as doing so will force them to start creating their Chat Flow from scratch.&#x20;



### Transcript Options

<figure><img src=".gitbook/assets/image (3) (1) (1) (1) (1).png" alt="The Transcript page offers various features such as a Search function, as well as sorting through Filters such as Email, Channel, or Chat Flow. There are options to pick a Date to sort lists of conversations, as well as the option to check multiple conversations for deletion."><figcaption><p>The Transcript page offers various features such as a Search function, as well as sorting through Filters such as Email, Channel, or Chat Flow. There are options to pick a Date to sort lists of conversations, as well as the option to check multiple conversations for deletion.</p></figcaption></figure>

The **Transcript** page now offers different options for users to sort conversations detected by the Captivate Chat platform. These include the following:

* **Checkbox selection of conversations.** You can also mass-delete these conversations by pressing the _**Delete**_ button, although this is irreversible.
* **Sort by various filters**, such as Date the conversation occurred, the Email used, Channel where the conversation took place, and the Chat Flow that managed the conversation.

***

## 📆 v2.2.0-2 - 2022-02-02

It's now much easier to use the Captivate Hub for your **Livechat** needs!&#x20;

We're introducing new ways to modify your Livechat to automate certain tasks. Thanks to **Manual Assignment**, you can now set pre-determined messages that trigger after specific conditions - such as assigning chats based on an agent's MS Teams status.&#x20;

Agents can also use the new _**`"Reassign"`**_ command to transfer the chat to another available agent.&#x20;

### ✅ Added

* reCaptcha support on registration
  * Added new environmental variable on frontend `REACT_APP_GOOGLE_RECAPTCHA_KEY`
* Implementation of **Manual Assignment**
  * Added `manualAssign (bool)` `manualMessageUsersExist(string)` `manualMessageUsersNotExist (string)` `idleTimeoutBeforeAssign(int) (in minute)` `idleTimeoutAfterAssign(int) (in minute)` `idleMessageBeforeTimeout (string)` `idleMessageAfterTimeout (string)` to Hub properties.
* Implementation of **Agent Status**
  * Added `agentStatus (Array) [Available,Busy,Away,Offline]` to Hub properties.
* Implementation of **Reassign Agents**
* New React frontend
  * Added `GOOGLE_SECRET_KEY` to enviromental variable on chatbot
* **Livechat** configuration editor on frontend
* New Teams app permissions
  * `Site.Read.All` (for accessing files to teams and send it to channels)
  * `Group.ReadWrite.All` (for modifying teams channel permissions)

### 🟧 Changed

* All messages on channels to MS Teams is now tagged to selected agent

### 🟥 Removed

* Removed support for the legacy frontend. preferred the new React frontend

### ⚠️ Fixed

* Emojis and attachment message filter on agents' message
* Messages on direct mode is now properly sent to Teams Desktop and Teams Mobile

### 🆕 Agent Status (Livechat)

You can now **modify agent assignments** based on their **presence status** in MS Teams.&#x20;

Using the Livechat configuration, you can **set chat assignments** based on an agent's **status** or availability in MS Teams. Commands can affect agents who set themselves as `"Available",` `"Busy",` `"Away"` and `"Offline."`&#x20;

This example video demonstrates a Livechat configured to only assign chats to someone set as `"Busy".` Check it out:&#x20;

{% embed url="https://www.youtube.com/watch?v=gG1GO2aHJAs" %}
Agent status demonstration
{% endembed %}

### 🆕 Manual Assignment (Livechats)

You can now **activate&#x20;**_**Manual Assignments**_ when configuring a Livechat.&#x20;

This allows **pre-made messages** to be sent after **meeting certain conditions**. Here are the properties you can modify:

*   `manualMessageUsersExist(string)`&#x20;

    Displays a message **if there is an available agent** to respond to the client.
*   `manualMessageUsersNotExist (string)`&#x20;

    Displays a message **if there are no agents available** to respond to the client.&#x20;
*   `idleTimeoutBeforeAssign(int) (in minute)`&#x20;

    A value **(in minutes)** before a timeout is declared, **should a conversation not be escalated** to an agent.&#x20;
*   `idleTimeoutAfterAssign(int) (in minute)`&#x20;

    A value **(in minutes)** before a timeout is declared, **if there's an agent assigned but neither agent nor client is responding** to each other.
*   `idleMessageBeforeTimeout (string)`&#x20;

    Displays a message when `idleTimeoutBeforeAssign(int)` elapses.
*   `idleMessageAfterTimeout (string)`&#x20;

    Display a message when \`\`idleTimeoutAfterAssign(int)\` elapses.&#x20;

#### ➦ Default Values

Here are the **default Manual Assignment** values:&#x20;

* `manualAssign (bool):` false
* `manualMessageUsersExist(string):` “Our agents know you’re waiting and will chat here as soon as they’re free.”
* `manualMessageUsersNotExist (string):` “Our agents is currently busy at the moment.”
* `idleTimeoutBeforeAssign(int) (in minute):` 5
* `idleTimeoutAfterAssign(int) (in minute):` 10
* `idleMessageBeforeTimeout (string):` “Our agents is currently busy at the moment.”
* `idleMessageAfterTimeout (string):` “Livechat Ended”

#### ➦ Example Scenarios

You might find this manual assignment feature useful if you encounter the following scenarios:&#x20;

*   **There are available users.**\
    Displays: **manualMessageUsersExist(string)**

    \
    Suppose Teams Group A is connected to the Captivate Hub web widget, and the channel is asking if there are any agents available. Agent A (Busy) and Agent B (Available) are currently online.\
    \
    If Manual Assignment exists that assigns a chat to anyone set as "Available" (Agent B), then the channel has to declare that there's at least one agent (Agent B) that might be available to assist them. \

* **There are no available users.**\
  Displays: **manualMessageUsersNotExist(string)** \
  \
  Suppose Teams Group A has an active channel asking if there are agents available. However, both Agent A (Busy) and Agent B (Busy) are both occupied. \
  \
  If only "Available" agents are programmed to receive chat assignments, then the channel declares there are no available agents to assist them. \

* **Time has elapsed and no users managed to assist them.**\
  Runs: **idleTimeoutBeforeAssign**\
  Displays: **idleMessageBeforeTimeout**\
  \
  Suppose Teams Group A has an active channel asking for agents, and Agent B (Available) is not busy. This will have the channel declare that an agent will assist the client soon. Until such a time that Agent B responds to the client, the chatbot will run the Idle Timeout counter. \
  \
  If the assigned time elapses and Agent B hasn't responded, a message explains that chat will be put on time out due to the lack of agent response. \

* **Time has elapsed that the agent and client didn't speak to each other.**\
  Runs: **idleTimeoutAfterAssign**\
  Displays: **idleMessageAfterTimeout**\
  \
  Suppose Teams Group A has an active channel asking for agents, and Agent B (Available) managed to respond to the client's questions. After some time, someone in the conversation hasn't responded. This triggers a background Idle Timeout counter.\
  \
  If the assigned time elapses, a message appears that states one of the parties have yet to respond and the chat will be put on time out.&#x20;

{% embed url="https://www.youtube.com/watch?v=4p1kpHahDmk" %}
Manual Assignment Demo
{% endembed %}

### 🆕 Reassign Agent

You can now use the _**`"Reassign"`**_ command to **reassign agents within the same Teams group.**&#x20;

Normally, a Support Chatbot is assigned to an available Live Support Agent so they can answer client queries on their behalf. However, not all Live Support Agents can answer a client's questions. This is where _**Reassign**_ comes in.&#x20;

Should the need arise to transfer control of the Support Chatbot to another Live Support Agent, do this **in the MS Teams chat:**

1. Type _**`"@TheCaptivateHub"`**_ to tag the Captivate Hub
2. Type _**`"Reassign"`**_ and press _Enter_.
3. An automated message will appear alongside a drop down of available team members.
4. Select the desired team member to transfer the Support Chatbot.

Check out the video below:

{% embed url="https://www.youtube.com/watch?v=l1JoTW5_ZG8" %}
Reassign agent demo
{% endembed %}



***

## 📆 v2.2.0-1 - 2021-08-26

**Instagram support is now live!**&#x20;

You can now use Captivate Hub to create chatbots for Instagram via the Watson Assistant. Before you create your Instagram chatbots, make sure your Instagram account is a Business Account and that it is connected to your Facebook Page.&#x20;

We made updates to the documentation to reflect these new changes.

### ✅ Added

* **Instagram** support
* Add bot templates support on Watson Assistant
* New enviromental variable for app-ecb-frontend (frontend / legacy)
  * `REACT_APP_FACEBOOK_APPID` - Facebook Application ID
* New enviromental variable for app-chatbot (chatbot)
  * `FACEBOOK_APPID` - Facebook Application ID
  * `FACEBOOK_SECRET` - Facebook Application Secret Key
* New permissions added to Facebook Application
  * `instagram_manage_messages`
  * `instagram_basic`
  * `pages_manage_metadata`
  * `pages_show_list`

### 🟧 Changed

* Using Facebook OAuth to add Facebook / Instagram as channels (same as Twitter now)
* Enabled public registration
* Update Microsoft Teams permissions for AppSource ([https://appsource.microsoft.com/en-us/product/office/WA200003575?tab=DetailsAndSupport](https://appsource.microsoft.com/en-us/product/office/WA200003575?tab=DetailsAndSupport))

### 🆕 Instagram Integrations

Before attempting integrations, please ensure that you're using an **Instagram Business Account**. This account has to be **connected to your Facebook page**. For more information, please click [here](https://www.facebook.com/business/help/898752960195806).

#### ➦ Facebook Developers Advance Access

* public\_profile
* pages\_messaging
* Business Asset User Profile Access
* instagram\_manage\_messages
* instagram\_basic
* pages\_manage\_metadata
* pages\_show\_list

#### ➦ Facebook Developers Valid OAuth Redirect URLs

* Your app-channel-gateway Public URL (ex: [https://hub.captivat.io/gateways/channel](https://hub.captivat.io/gateways/channel))

#### ➦ Facebook Developers Allowed Domains for the JavaScript SDK

* Your frontend Public URL (ex: [https://hub.captivat.io/](https://hub.captivat.io/))

To add Instagram to the Hub, you click the link below:

{% content-ref url="broken-reference" %}
[Broken link](broken-reference)
{% endcontent-ref %}

### ⚠️ Teams Application Permission

* Channel.Create
* Channel.Delete.All
* Channel.ReadBasic.All
* ChannelMessage.Read.All
* Chat.ReadWrite
* Group.Read.All
* Presence.Read.All
* Team.Create
* Team.ReadBasic.All
* TeamMember.ReadWrite.All
* TeamActivity.Send
* TeamAppInstallation.TeadWrite
* User.ReadBasic.All

***

## 📆 v2.2.0 - 2021-08-26

This is the Initial release of the **Captivate Hub** to the public.

### ✅ Added

* Bot Template setup
* Registration

### 🟧 Changed

* Changed frontend ([https://hub.captivat.io](https://hub.captivat.io)) to the new design
* Old frontend will be hosted on legacy.
* Moved [https://manual.captivat.io](https://manual.captivat.io) to Gitbook
