# Skype

1. To enable skype, we would need an azure portal account. So Proceed to create one.
2. On your azure portal dashboard, navigate to the app services section, and add a Bot Channel Registration service.
3. Supply the details needed, and leave the default values behind. And don’t forget the messaging endpoint url: `https://channel.prod.captivat.io/api/skype/integration`
4. On your service, go to the channel section, and proceed to add a skype connection.
5. On the details page, feel free to edit the details as you see fit. The most important thing to remember is our `App ID`, and the `App Password`. To view the password, you will notice that behind the App ID label, there will be a Manage word, click that one.
6. Under the client secrets, add a new one, take note of the generated client secret as this is available only to be seen once.
7. Supply the details needed, and the `App ID`, and `App Password` earlier, select the bot you want to connect to. Then click add.
8. To verify its working, back on your portal azure dashboard, click the service you created earlier, and under the channel section, select Skype.
9. You will then be given the URL to add your configured bot. Add the bot to your contacts.
10. Start chatting with the bot, the bot should be replying now.
