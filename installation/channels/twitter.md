# Twitter

The twitter app should be accomplished first to be able to add a twitter channel in the frontend easily. Accomplishing the twitter app will give the required keys for the Channel Gateway, these keys will make the `Authorize App` button in the frontend work and automatically fill up all the required fields.

Follow these steps to create the app:

1. Apply for developer access [here](https://developer.twitter.com/en/apply-for-access.html). The approval process usually takes from minutes to a few days. Be sure to check your email as they may ask for additional information.
2. Once approved, create a twitter app.
3. In the twitter app [dashboard](https://developer.twitter.com/en/apps), you will find your newly created app.
4. Click the `Details` button, then go to the `Permissions` tab.
5. Update the permissions to enable `Read, Write, and Direct Messages`.
6. On the same page, go to the `Keys and Tokens` tab.
7. Generate `Consumer API keys` and `Access token & access token secret`, you will need these values for the Channel Gateway env variables.
8. Go to the `App details` tab, you will need to add the `frontend url` in the `Callback URL` list.
9. Go to the [dev environments page](https://developer.twitter.com/en/account/environments), you will need to create a `developer environment` for the webhook, this is also a variable needed for the Channel Gateway.

Once all the variables are obtained and Channel Gateway is up and running, you can easily click the `Authorize App` button and log in to the page where you want the hub to be bound to. By default, the chatbot is bound to the twitter direct messages but if you also want to bind a bot to reply to tweets, enable tweet bot and then supply the chatbot api key.
