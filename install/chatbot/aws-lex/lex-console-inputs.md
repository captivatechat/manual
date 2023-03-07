# Lex Console Inputs

## Lex Session Attributes and Metadata

Session attributes are a part of the session state object of a Lex conversation and Captivate Hub uses this to save data available for chatbot developers to use throughout the session.

Chatbot developers can modify all parts of the session state but Captivate Hub will only modify the session attributes, this is to make sure that only chatbot developers are responsible for the flow of the bot responses. Session state will however stay updated in CH sessions every response from Lex which will be used for the next CH request to Lex, with possible modifications to session attributes only.

### Session Attributes content

Metadata from CH, includes both Inline and Internal metadata. Check this [page from Watson Assistant docs for the use-case](https://manual.captivat.io/install/chatbot/watson-assistant/the-captivate-hub-integration/metadata).

* JSON string format in`` `sessionState.sessionAttributes.metadata` ``, you may use this in your Lambda function after parsing.
* Flattened JSON available for use in Lex console directly.

Format and sample lambda event log for `sessionState`

![](<../../../.gitbook/assets/image (16).png>)

### Using the Session Attributes

1. Chatbot developers can use the entirety of the session state in the connected Lambda function however necessary.
2. Lex console can retrieve a session attribute by enclosing the property with square brackets. Using the session state in the event log above and configuring the closing response as in example below, the response message will be "Hello, John Doe".

![](<../../../.gitbook/assets/image (1).png>)

#### References from AWS Lex Documentation

* Session attributes management: [https://docs.aws.amazon.com/lexv2/latest/dg/context-mgmt-session-attribs.html](https://docs.aws.amazon.com/lexv2/latest/dg/context-mgmt-session-attribs.html)
* Session state model: [https://docs.aws.amazon.com/lexv2/latest/dg/API\_runtime\_SessionState.html](https://docs.aws.amazon.com/lexv2/latest/dg/API\_runtime\_SessionState.html)
* Managing session state:  [https://docs.aws.amazon.com/lexv2/latest/dg/using-sessions.html](https://docs.aws.amazon.com/lexv2/latest/dg/using-sessions.html)

## Lex Standard Response Formats Support

* **Text message** – supported.
* **Card group** – not yet supported. However, cards and buttons are supported in CH Special Response formats.
* **Custom payload** – supported templates are in Special Response and Outgoing Action section.
* **SSML** – not yet supported.
