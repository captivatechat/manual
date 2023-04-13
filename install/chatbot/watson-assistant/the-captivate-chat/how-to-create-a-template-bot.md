# How to create a template bot

**How to create a template bot?**

* To create a template bot. Your chatbot developer will need to read data from the $botbuilder.metadata.internal.customizable object.&#x20;
* You can define which part of the chatbots are customizable or not.

Example object data of customizable in action

![](https://lh5.googleusercontent.com/7VYLplkozW13K9-ZquNg5\_ryv62z0LMAbV8fB-imhb7fT06kzHHOr9v7sfSywtYXswrdB1QzM01pemOnrFDjyj7fBtRBTDEySaLDq5bDy32ZHVb2UimvpH05Y-lOxA)

Your chatbot developers will then read those data and put them into the watson assistant skill

![Watson Screenshot 1: Initialize needed context](https://lh5.googleusercontent.com/rDMlxwf3FDU0MFuXX3avw2YVcS2UAHXuOGn06A7ahFHNsCvKIWW31BW-n-HLEto3d3HdRNVDptL7oqeqobeK4BYyMWPIp4jzyzMgmQE9NfFnPXvXmcY9n1C4V8gBjQ)

![Watson Screenshot 2: Default Data](https://lh4.googleusercontent.com/P0Rs7FprhPcuvMiUbsHSyeKTiRwHUGN3D3MO3US1\_6OyIi2C\_SUt1StVMPshp5z9W00WH6xgDP7XERka--ziAptPDh86JM0G677xk0m5-bTSHO8qRAfCHNbeSfSCAA)

![Watson Screenshot 3: Customized  Value](https://lh3.googleusercontent.com/-r7gu7avf3DbsPh0zZc4K8JPVFBlUhdYn-\_qcF3gc5sTqXbB5iJAZQSM30yYDeZDk4KMhIAT3f2jLsHoNRHjAz73u4ZvNN5\_VEPGqOqFHYce9-NlysE8XKlYQSybGQ)

Upon starting the template bot we initialize the values of the following context variables

* leave\_a\_contact&#x20;
* waiting\_message
* &#x20;escalate\_message&#x20;
* thank\_you\_message&#x20;
* connected\_to\_human\_message&#x20;
* send\_emails\_to

as you can see in the Watson Screenshot 1 after welcome node triggered it jumped to its  child node named “Default Data” where the default values for the sampled context variables are declared (see Watson Screenshot 2),Inside that child node there is also another child node named“Get Botbuilder - Pass here” that needs to be evaluated. Inside this node ( refer to the Watson Screenshot 3. Watson Assistant) Watson Assistant checks if the context variable $botbuilder.metadata.internal.customizable must have the set values that can used to replace the default values of the context variables  stated above  and if $botbuilder.metadata.internal.customizable is  undefined it will fallback to its parent node with the unchanged values of the context.

**As of now all templated bots are available to the public and all are applied through us manually. We are quickly making a User interface for this in our roadmap**



**CH User Profile**

&#x20; **Located at $botbuilder.metadata.internal.user**

1. fullName = variable which contains the full name of the user.&#x20;
2. Email = variable which contains the email of the user.&#x20;
3. Number = variable which contains the contact number of the user.&#x20;
4. Company = variable which contains the company name of the user.

Channel Metadata Located at $botbuilder.metadata.internal.channelMetadata Contains the details of the channels

We are still developing the Livechat metadata of this part. It will be updated in the next release.
