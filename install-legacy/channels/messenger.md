# Messenger

1. Create or choose a facebook page where you want to use.
2. To get the `Page ID`, follow this [How do I find my Facebook Page ID](https://www.facebook.com/help/1503421039731588) guide from Facebook.
3. Turn on messaging for your page. Follow this [How do I turn messaging on or off for my Page](https://www.facebook.com/help/307375982614147) from Facebook.
4. Create a facebook application.
5. You’ll be able to find your `Page Token` in the facebook application.
6. Go to the Facebook Developer Page.
7. Do all security checks. You will be redirected to your facebook developers app dashboard
8. Create a Messenger Product to the app by clicking the + sign beside Product section
9. Hover over the Messenger Product and click Setup.
10. Scroll down below until you see the webhook section.
11. Click subscribe to events beside the webhook section. Provided the channel gateway messenger webhook URL: `https://channel.prod.captivat.io/api/messenger/integration/` and Verify Token.
12. Subscribe to `Messages` and `Messages_postbacks`.
13. Click Verify and Save.
14. Connect the app to our Facebook page. Scroll down to the Webhook section and Select a Page.
15. Afterwards, the bot will be able to converse with the user.

