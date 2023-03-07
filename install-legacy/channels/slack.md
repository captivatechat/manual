# Slack

1. Create a Slack App.
2. Remember your `App ID` and `Bot Token`. The `App ID` can be seen on the app’s basic information section under app credentials. The Bot token can be seen on the oauth and permissions section.
3. Still on the same page, navigate to the Interactive Components section under the Features header, and supply the slack action channel gateway request url: `https://channel.prod.captivat.io/api/slack/integration/action`, to enable action events on your slack.
4. Navigate to the event subscriptions section, and supply the slack even channel gateway request url:&#x20;
   1. `https://channel.prod.captivat.io/api/slack/integration/event`. This will be the entry point, whenever someone messages on your slack.
5. Still on the same page, scroll down and under the subscribe to bot events section, subscribe to the following events: `im_open`, `message.channels`, `message.groups`, `message.im`, `app_mention`, and `file_shared`.
6. That’s it where done configuring the part on the slack. Now, go to our CH Dashboard, and add a channel.
7. Back to the hub, supply the `App ID` and `Bot Token` earlier.
8. To verify if it's working, try to message your created slack app directly, the bot should be able to reply now.
