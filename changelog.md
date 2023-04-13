# 📕 Changelog

## v2.2.3 - 2023-04-13

Changes will be added soon

## v2.2.0-2 - 2022-02-02

### Added

* reCaptcha support on registration
  * Added new enviromental variable on frontend `REACT_APP_GOOGLE_RECAPTCHA_KEY`
* Implementation of Manual Assignment
  * Added `manualAssign (bool)` `manualMessageUsersExist(string)` `manualMessageUsersNotExist (string)` `idleTimeoutBeforeAssign(int) (in minute)` `idleTimeoutAfterAssign(int) (in minute)` `idleMessageBeforeTimeout (string)` `idleMessageAfterTimeout (string)` to hub properties.
* Implementation of Agent Status
  * Added `agentStatus (Array) [Available,Busy,Away,Offline]` to hub properties.
* Re-assign agents
* New React frontend
  * Added `GOOGLE_SECRET_KEY` to enviromental variable on chatbot
* Livechat configuration editor on frontend
* New teams app permissions
  * `Site.Read.All` (for accessing files to teams and send it to channels)
  * `Group.ReadWrite.All` (for modifying teams channel permissions)

### Changed

* All messages on channels to Microsoft teams is now tagged to selected agent

### Removed

* Removed support for the legacy frontend. preferred the new react frontend

### Fixed

* Emojis and attachment message filter on agents message
* Messages on direct mode is now properly send to Teams Desktop and Teams Mobile

### Agent Status

You can now modify the the agent assignment based on their presence information on teams such as Available, Busy, Away and Offline. on this demo video we demonstrate on live chat configuration, we only select the busy agent status and it will only assign the agent available with busy status while when we change it to away it doesn’t assign the escalation to the agent.

{% embed url="https://www.youtube.com/watch?v=gG1GO2aHJAs" %}
Agent status demonstration
{% endembed %}

### Manual Assignment

Conversation will now display as manual assignment if this configuration is enabled. you can now set the properties

* `manualMessageUsersExist(string)` display the message on the channel if there’s available agent exist
* `manualMessageUsersNotExist (string)` display the message on the channel if theres’s no available agent
* `idleTimeoutBeforeAssign(int) (in minute)` is timeout when the conversation is not assigned before escalation
* `idleTimeoutAfterAssign(int) (in minute)` is timeout when the conversation assigned but both agent and client is not sending message to each other.
* `idleMessageBeforeTimeout (string)` display the message when `idleTimeoutBeforeAssign(int)` elapse.
* `idleMessageAfterTimeout (string)` display the message when \`\`idleTimeoutAfterAssign(int)\` elapse

Default values

* `manualAssign (bool):` false
* `manualMessageUsersExist(string):` “Our agents know you’re waiting and will chat here as soon as they’re free.”
* `manualMessageUsersNotExist (string):` “Our agents is currently busy at the moment.”
* `idleTimeoutBeforeAssign(int) (in minute):` 5
* `idleTimeoutAfterAssign(int) (in minute):` 10
* `idleMessageBeforeTimeout (string):` “Our agents is currently busy at the moment.”
* `idleMessageAfterTimeout (string):` “Livechat Ended”

Example Scenarios

* If User A (Busy) and User A (Available) is on the Teams group A connected to The Captivate Hub web widget, if the channel is asking for an agent and override exist for Available and Busy users, it will display manualMessageUsersExist(string) since there’s an 2 available users.
* If User A (Busy) and User B (Busy) is on the Teams group A connected to The Captivate Hub web widget, if the channel is asking for an agent and override doesn’t exist, it will display manualMessageUsersNotExist(string) since there’s no agent available to accept it’s message.
* If User A (Available) and User B (Busy) is on the Teams group A connected The Captivate Hub web widget, after displaying the manualMessageUsersExist it will check for idleTimeoutBeforeAssign, if there’s no assigned agent after idleTimeoutBeforeAssign then it will send a message idleMessageBeforeTimeout.
* If User A (Available) and User B (Busy) is on the Teams group A connected The Captivate Hub web widget, after displaying the manualMessageUsersExist and it was Assgined to User A, after assignment it will check for idleTimeoutAfterAssign, if the agent OR user doesn’t reply to and it exceed to the time of idleTimeoutAfterAssign it will send the idleMessageAfterTimeout message and end the conversation.

{% embed url="https://www.youtube.com/watch?v=4p1kpHahDmk" %}
Manual Assignment Demo
{% endembed %}

### Reassign Agent

You can now reassign agent with same teams groups by typing the reassign command

{% embed url="https://www.youtube.com/watch?v=l1JoTW5_ZG8" %}
Reassign agent demo
{% endembed %}

## v2.2.0-1 - 2021-08-26

Updated documentation

### Added

* Instagram Support
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

### Changed

* Using Facebook OAuth to add Facebook / Instagram as channels (Same as twitter now)
* Enabled public registration.
* Update Microsoft Teams permissions for AppSource ([https://appsource.microsoft.com/en-us/product/office/WA200003575?tab=DetailsAndSupport](https://appsource.microsoft.com/en-us/product/office/WA200003575?tab=DetailsAndSupport))

### Instagram

Be sure the instagram account is **connected to facebook page and it is a business account**. for more information please click [here](https://www.facebook.com/business/help/898752960195806).

Facebook Developers Advance Access:

* public\_profile
* pages\_messaging
* Business Asset User Profile Access
* instagram\_manage\_messages
* instagram\_basic
* pages\_manage\_metadata
* pages\_show\_list

Facebook Developers Valid OAuth Redirect URIs

* Your app-channel-gateway public url (ex: [https://hub.captivat.io/gateways/channel](https://hub.captivat.io/gateways/channel))

Facebook Developers Allowed Domains for the JavaScript SDK

* Your frontend public url (ex: [https://hub.captivat.io/](https://hub.captivat.io/))

To add instagram to the hub click the link below:

{% content-ref url="install/channels/instagram.md" %}
[instagram.md](install/channels/instagram.md)
{% endcontent-ref %}

### Teams Application Permission

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

## v2.2.0 - 2021-08-26

Initial release of The Captivate Hub to public

### Added

* Bot Template setup
* Registration

### Changed

* Changed frontend ([https://hub.captivat.io](https://hub.captivat.io)) to the new design
* Old frontend will be hosted on legacy.
* Moved [https://manual.captivat.io](https://manual.captivat.io) to Gitbook
