# Overview

The Captivate Hub has four major components, one for the frontend and for backend, chatbot, channel gateway and live chat gateway and two microservice for handing Microsoft Teams connections and Widget for custom chatbot widget.

### Frontend

Frontend handles the site where chatbots, channels, live chats and hubs are configured.

### Chatbot

Chatbot serves as the backend for the frontend site handling the database controllers. It is responsible for communicating with chatbot providers and returning the responses. It handles all the tools and services / microservices related to language / conversation.

### Channel Gateway

Channel Gateway handles the communication to and from the channels. This handles the channel - chatbot compatibility making sure that responses can be returned to the corresponding channel. If there is a live chat solution configured to the hub, Channel Gateway also is responsible for sending the intended messages to the Live chat Gateway.

### Livechat Gateway

Livechat Gateway makes the communication to and from the live chat vendors / solutions possible. It handles the sending and receiving of messages from the live chat to and from the Channel Gateway.

### Microsoft Teams Bot

Microsoft Teams Bot handles the communication to the Azure Web App Bot, it is responsible for receiving data from the Azure Web App Bot via webhooks and sending it to Livechat Gateway, it is also resposible for Presence Bot for checking the status of teams client to escalate users to the channels.

Microsoft Teams Agent handles the Agent to Channel communication by retrieving the messages of teams client to channels.

### Widget

Widget is another custom channel to create custom chatbot widget to user webpage. it is using websockets to communicate thru the chatbot and livechat gateway.
