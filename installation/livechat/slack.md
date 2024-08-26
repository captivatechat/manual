# Slack

The Captivate Hub app lets your agent communicate with users between Slack and any [channel](../channels/), e.g., messenger, whatsapp, twitter.&#x20;

## Please follow all the instruction thoroughly and do not skip any instructions on the Installation part.

If you have any suggestions on this page please email us at support@captivat.io



{% hint style="danger" %}
The Captivate Hub Slack Apps requires [**Workspace Admins**](https://slack.com/help/articles/360018112273-Types-of-roles-in-Slack) permission to install
{% endhint %}

{% tabs %}
{% tab title="Installation" %}
{% hint style="warning" %}
If you are on the last step of the creation of the Hub (Figure 1.0), please follow the instruction below and do not close the page. If you haven't yet set up your Hub, please go to [Get Started](../../get-started.md). If it's easier there's a corresponding step by step video per instruction.
{% endhint %}

![Figure 1: Slack installation window after creating the hub](<../../.gitbook/assets/image (55) (1).png>)

### App Installation.

* Click [this link](https://slack.com/oauth/v2/authorize?client\_id=266934262400.3543747458869\&scope=app\_mentions:read,channels:history,channels:read,chat:write,chat:write.customize,chat:write.public,commands,files:read,groups:history,groups:read,groups:write,im:history,mpim:read,users.profile:read,users:read\&user\_scope=) or click the "Add to Slack button" below and install the Slack app. and press  the "Allow" button

[![add-slack](https://susume.captivat.io/ebvjr/img/slack.png)](https://slack.com/oauth/v2/authorize?client\_id=266934262400.3543747458869\&scope=app\_mentions:read,channels:history,channels:read,chat:write,chat:write.customize,chat:write.public,commands,files:read,groups:history,groups:read,groups:write,im:history,mpim:read,users.profile:read,users:read\&user\_scope=)

![](<../../.gitbook/assets/image (66).png>)

### Authentication

* You will be see the **"The Captivate Hub"** on your apps. click the app and on the topside click the **"Messages"**. on the first message of the Slack app. click the **"Authorize"** button. The application will ask you another permission. please click allow.

![Figure 2: Accessing the Captivate Hub for Authentication](<../../.gitbook/assets/image (56) (1).png>)

![Figure 3: Slack app is requesting again new permissions](<../../.gitbook/assets/image (93).png>)

* After the authorization of the Slack app. type the command '/signin' to the Message and it will display **"Sign-in"** button. it will open a browser and login your account credentials on the Hub.

![Figure 4: Output of /signin on the Slack app](<../../.gitbook/assets/image (46) (1).png>)

### Hub Installation

* Now that you are logged in to The Hub, [**create a new channel**](https://slack.com/help/articles/201402297-Create-a-channel) giving it a name you will associate with using The Hub (e.g. The Hub Live Chat). after creating the channel, select the new created channel and get the channel details by clicking its header. copy the **"Channel ID"**

![Figure 5: Channel information on Slack](<../../.gitbook/assets/image (68).png>)

* Go to the app messages again (Figure 2) and type the command /link. it will display a new window asking for your Channel ID and Hub. paste the Channel ID you copied on Figure 5 and select the Hub will be connected to Slack and press **"Submit"**

![Figure 6: Link window](<../../.gitbook/assets/image (76).png>)

Congratulations, you have now connected your Hub to Slacks!
{% endtab %}

{% tab title="App Commands" %}
If you're sending account commands please message The Captivate Hub via App Chat.



Available Commands:

* Signin your Captivate Account: /signin
* Signout your Captivate Account: /signout
* Link your Hub to Slack: /link
* Unlink your Hub from Slack: /unlink
{% endtab %}

{% tab title="Agent Commands" %}
To use these commands you need to mention the Bot first, e.g., @The Captivate Hub es. Available Commands:

* End Livechat: /es or /endSession
* Redirect conversation to a different agent: /reassign
{% endtab %}
{% endtabs %}

{% embed url="https://www.captivat.io/privacy-policy/" %}
Read Privacy Policy
{% endembed %}
