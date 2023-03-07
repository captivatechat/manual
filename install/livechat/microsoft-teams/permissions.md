# Permissions

#### In order to work correctly, Captivate needs to be able to assign chats to agents within Teams - this requires an understanding of who is in the group and who is available.  Captivate also must have knowledge of a user's email address and name as well as use of the user's photo for displaying in the chat.

#### Any information collected by Captivate is held within the Captivate Platform solely for these purposes under the laws of GDPR and is governed by the Teams Admin assigning users to the  Captivate Group.

The following information explains why Captivate needs these permisions and what they are:

* In order to automatically assign conversations to available team members/agents, the Captivate app needs to have the ability to check their presence/availability, which is why it requires the **"Read user's presence information"** permission or **`Presence.Read.All`** permission. This is a Microsoft Graph Delegated permission that allows the app to view the status of each member using the Presence Bot (presencebot@captivat.io), such as "Available," "Busy," or "Be right back".
* In order to programmatically **"Create Teams"** and **"Create channels"** for the team members connected to a hub specially for linking hub to teams, the Captivate app requires the "Create Teams and "Create Channel" permission or **`Team.Create`** and **`Channel.Create`** permission, which is a Microsoft Graph Application permission.
* In order to add members programmatically to the teams created for the agents, the Captivate app needs the "**Read Members the Members for All Teams**" permission or **`TeamMember.Read.All`** which is a Microsoft Graph Application Permission. This is the only permission related to team members that allows the app to add a member to a team that is also a member of the team connected to the hub.
* To verify that the team has been created programmatically for the user/agent, The Captivate  app requires the **"Get a List of all Teams"** permission or **"Team.ReadBasic.All"**, which is a Microsoft Graph Application Permission that allows the app to retrieve a list of the teams a specific user has joined.
* To modify and read channels to the agent teams group to display the users connected to the client, The Captivate  requires **"Read and write the names, descriptions, and settings of all channels"** and **"Read the names and descriptions of all channels"** or **`ChannelSettings.ReadWrite.All`**and **`Channel.ReadBasic.All`** , which is the most specific and lowest privilege permissions related to reading and modifying channels, specifically agent channels.
* To subscribe to messages changes (create, update, and delete) in the agent channels in real-time, the Captivate app requires the **"Read all channel message"** permission or **`ChannelMessage.Read.All`**, which is a Microsoft Application Permission that supports change notifications through its API
* To retrieve the files posted to the agent channels, Captivate requires to **"Access selected site collections"** and **"Read files in all site collections"**  or **`Sites.Selected`** permission is a Microsoft Graph Application permission that allows the app to retrieve information about a file and use the **`Files.Read.All`** permission to download it and send it to the channel connected to the hub.
* The **"Read all users profile"** or **`User.Read.All`** permission is a default permission that allows the app to read basic information of all agents inside the connected hub teams group, such as name, email, ID, and job title, primarily for identifying the agent to be escalated to the user.

### Permissions requested

The Captivate app has 13 permissions that need admin consent. Here's the list of permissions Captivate uses:

<figure><img src="../../../.gitbook/assets/image (41).png" alt=""><figcaption><p>Figure 1: Permission requested window of the teams application.</p></figcaption></figure>

### Purpose of using these Permissions



### Microsoft Graph Permissions

1. `Presence.Read.All`: This permission allows the user to read the presence status of all users in the organization.
2. `Sites.Selected`: This permission allows the user to access selected sites in the organization.
3. `Files.Read.All`: This permission allows the user to read all files in the organization.
4. `User.Read.All`: This permission allows the user to read all information about users in the organization.
5. `Channel.Create`: This permission allows the user to create channels within a team.
6. `ChannelSettings.ReadWrite.All`: This permission allows the user to read and write settings for all channels in the organization.
7. `Channel.ReadBasic.All`: This permission allows the user to read basic information about all channels in the organization.
8. `ChannelMessage.Read.All`: This permission allows the user to read all messages in all channels in the organization.
9. `Team.ReadBasic.All`: This permission allows the user to read basic information about all teams in the organization.
10. `TeamsAppInstallation.ReadWriteSelfForUser.All`: This permission allows the user to read and write Teams app installation information for all teams that the user is a member of.
11. `TeamsAppInstallation.ReadWriteSelfForTeam.All`: This permission allows a Teams app to read, install, upgrade, and uninstall itself in any team, without a signed-in user.
12. `Team.Create`: This permission allows the user to create teams within the organization.
13. `TeamMember.Read.All`: This permission allows the user to read information about all team members in the organization.

### In the Future

The Captivate Hub Teams Application will use RSC (Resources-Specific Consent) that reduces our global permissions and use these permissions

RSC permissions:

* TeamSettings.ReadWrite.Group
* Channel.Create.Group
* ChannelSettings.ReadWrite.Group
* ChannelMessage.Read.Group
* Team member.Read.Group
* Member.Read.Group
* File.Read.Group

Global Permissions:

* Presence.Read.All
* Sites.Selected
* Team.Create
* TeamsAppInstallation.ReadWriteSelfForUser.All

Currently, we can't implement it due to the restriction of RSC when we install our app programmatically on Microsoft Teams. to know more about this issue, visit [https://github.com/microsoftgraph/microsoft-graph-docs/issues/13349](https://github.com/microsoftgraph/microsoft-graph-docs/issues/13349)
