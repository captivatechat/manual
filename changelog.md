---
description: >-
  All changes to the Captivate Hub will be added here. Guides will be updated
  concurrently.
---

# 📕 Changelog

## 📆 v2.2.3 - 2023-04-13

We'll be adding more changes soon!

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

You can now **activate **_**Manual Assignments**_ when configuring a Livechat.&#x20;

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

{% content-ref url="installation/channels/instagram.md" %}
[instagram.md](installation/channels/instagram.md)
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
