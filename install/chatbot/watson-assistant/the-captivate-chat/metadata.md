# METADATA

There are 2 types of metadata. _**Inline**_ and _**Internal**_. Both are in the object $botbuilder.metadata

1.  **Inline Metadata** is set on the frontend. These is commonly use in conjunction with the Widget API.

    **Use cases include**

    1. Sending User & Login Session data to watson&#x20;
    2. Sending preconfigured modes depending on where the user is in the website.

    There are many use case for this feature and it is up to the developers to maximize its use case
2.  **Internal Metadata** are mostly metadata that is set and used by CH Backend. The data you set inside internal metadata are stored in the systems database.

    **Use case include**

    1. Preconfigured data you want for your chatbots that you do not want to configure in the Watson NLP.&#x20;
    2. You have multiple versions of bots you want deployed per channel and you want to just switch them with different configurations. Those configurations can be stored in this internal metadata object.
    3. Captivate Hub's own Template bots were made possible because of this. Will be discuss in the next section.
    4. Reading user data from 3rd party channels like Facebook,WhatsApp,Instagram and etc.
    5. Reading agent data from 3rd party live chat like teams,liveengage,click4assistance,slack and etc.

It is up for the developers to again maximize the use case for this feature

