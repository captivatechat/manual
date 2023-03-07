# Incoming Action

Incoming actions are set by Captivate Hub to trigger specific action or intents inside Lex. These are sent as part of [Lex request attributes](https://docs.aws.amazon.com/lexv2/latest/dg/context-mgmt-request-attribs.html).

### **Incoming action content**

1. id - the action’s title is set to the id property
2. data - the action’s payload is set to the data property

**Format and sample lambda event log for `requestAttributes`**

* JSON string format in `requestAttributes.incoming_action`, you may use this in your Lambda function after parsing.
* A flattened version is also sent, so that the variables can be [used directly in Lex Console](https://docs.aws.amazon.com/lex/latest/dg/howitworks-manage-prompts.html#msg-prompts-msg-types) if needed.

![Incoming action logs in requestAttributes of Lambda event](<../../../.gitbook/assets/image (63).png>)

### Incoming Action in Lex Console

Since incoming actions are configured by the Captivate Hub, it is not always necessary to have a user message. But in this documentation of [RecognizeText – Amazon Lex Runtime V2 Command](https://docs.aws.amazon.com/lexv2/latest/dg/API\_runtime\_RecognizeText.html), you will see that `text` is a required request body parameter. For this, we provide a message for the text parameter:

`CHSystemMessage--incoming_action_id--${Incoming Action ID here}`

For example:\
`` `CHSystemMessage--incoming_action_id--failedAgentAssignment` ``

### **Recommended Use**

One way to check if incoming message is a legitimate user message or a CH System message is to use Code Hooks. This is recommended especially for intents that have similar Sample Utterances like “system”, “message”, “incoming”, “action” etc.

![Code hooks in Lex Console](<../../../.gitbook/assets/image (51).png>)

Along with Code Hooks, make sure that your Lex Bot has a Fallback Intent configured. Before sending the default response for unknown user messages, check first if the message is an incoming action.

![Built-in Lex Fallback Intent](<../../../.gitbook/assets/image (36).png>)

For recommendations mentioned, you can verify if a message is a system action using the message and request attributes. Any CH message is prefixed with “CHSystemMessage” and if the message has an incoming action, you should be able to verify this in the Request Attributes.

### **Alternative Options**

Catching the CH System Messages as Sample Utterances is possible too, but testing proved that this can confuse your Lex bot especially if you have multiple intents for multiple incoming actions. If you are sure that this is okay for your bot, here goes.

Messages from Captivate Hub that are not from chatbot users will always be prefixed with `CHSystemMessage`, hence, chatbot developers to create an intent catcher for these. That is set `CHSystemMessage` as a sample utterance for the catcher and then use a Lamdba function to evaluate from Request Attributes which incoming action is received from CH and whatever should be the response of your bot.

![](<../../../.gitbook/assets/image (55).png>)

Another one, instead of just using `CHSystemMessage` as a sample utterance, the whole incoming action message can be set, for example `CHSystemMessage--incoming_action_id--failedAgentAssignment`. This eliminates the need for a Lambda function, but risks the recognition of the bot if there are similar utterances in the other intents.

![](<../../../.gitbook/assets/image (37).png>)

### Reserved Incoming actions

1. `failedAgentAssignment` - is sent when a user asks for a human live chat and chatbot tries to escalate to an agent but fails to find a human.
2. `agentIdleTimeout` - timeout after the agent has been assigned to the conversation but has not yet sent a message to the user.&#x20;
