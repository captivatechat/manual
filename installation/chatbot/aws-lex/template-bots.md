# Template Bots

CH Template Bots allow you to create these customizable messages, for example Welcome Messages. Template bots solve the following use cases:

1. If you need multiple bots with the same flow but just need some slight different tweak of messages.
2. If you want your own customers to easily configure some messages in your chatbot.

### Customizable Messages

Customizable data are accessible in the Lex Console or Lambda function through Session Attributes, the access instructions are available in [Lex Console Inputs](lex-console-inputs.md) - Lex Session Attributes and Metadata page.

![Bot Template Customizable Messages](<../../../.gitbook/assets/image (49).png>)

The key name for each customizable variable is `metadata_internal_customizables_*.`This screenshot below shows the customizable messages in the sessionAttributes object of the sessionState of a Lex event.

![](<../../../.gitbook/assets/image (64).png>)

By default, available customizable variables are:

* metadata\_internal\_customizables\_thank\_you\_message
* metadata\_internal\_customizables\_escalate\_message
* metadata\_internal\_customizables\_leave\_a\_contact
* metadata\_internal\_customizables\_connected\_to\_human\_mesage
* metadata\_internal\_customizables\_send\_emails\_to

**Note: As of now all template bots are available to the public and all are applied through us manually. We are quickly making a User interface for this in our roadmap.**



**References from Watson Assistant Implementation**

[CH Customizable Data](../watson-assistant/the-captivate-chat/ch-customizable-data.md)

[How to Create Template](../watson-assistant/the-captivate-chat/how-to-create-a-template-bot.md)

