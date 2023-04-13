# Incoming Action

Incoming action ($incoming\_action) is set by Conversational Hub to trigger specific action or flow inside Watson Assistant.&#x20;

1. id - the action’s title is set to the id property ($incoming\_action.id)&#x20;
2. data - the action’s payload is set to the data property ($incoming\_action.data)

Incoming Action can also be set after an Outgoing Action (API call). It acts as a signal inside the Watson Assistant that the API call is completed.

![](https://lh6.googleusercontent.com/JEJRymnpanGlUuxW4x4h04mvFNrYyrcNVULBp4NuzNbbwhv\_BheiGV6A9tDaCQVFUi2BRC8pybEiPjXrsoNFMf0pCqcPbqJf9yse5D1gEMWZ3Oxc-PEdjL5kOwIrgh0vFTPdt3k)

**Reserved Incoming action**

1. **failedAgentAssignment** - Is sent when a user asks for a human live chat and chatbot  tries to escalate to an agent but fails to find a human.

