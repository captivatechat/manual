# Outgoing Action

Aside from messages, actions can also be sent by the chatbot. Actions can be used for triggering certain events within Captivate Hub. For AWS Lex, just like Special Responses, these can be configured in the Custom Payload Response.

## Outgoing Action in Lex Console

Outgoing actions should be a valid JSON with `outgoing_actions` as the key with value of either an array of responses or a single object response. You can configure multiple custom payloads with outgoing actions using array and/or object format as needed. Outgoing actions can also be sent along with standard Lex responses and special responses.

### **Examples in Lex Console**

![Multiple outgoing actions](<../../../.gitbook/assets/image (70).png>)



## **Types and Use cases of Outgoing action**

For outgoing action types and use cases, refer to [this article from Watson Assistant section](https://manual.captivat.io/install/chatbot/watson-assistant/the-captivate-hub-integration/outgoing-action)**.**&#x20;

