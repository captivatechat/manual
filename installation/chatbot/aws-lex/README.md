# AWS Lex

Captivate Hub supports [Amazon Lex V2](https://docs.aws.amazon.com/lexv2/latest/dg/what-is.html). The integration covers the requirement for the connection between CH supported channels and Lex. Features like using [Lambda Functions](https://docs.aws.amazon.com/lexv2/latest/dg/lambda.html), [managing conversation contexts](https://docs.aws.amazon.com/lexv2/latest/dg/using-contexts.html) and [other features](https://docs.aws.amazon.com/lexv2/latest/dg/building-bots.html) that are specific to managing the bot conversation flow are left for the chatbot developers to explore and utilize.

## **Required Parameters for Lex Bot Integration**

* Name – any name for your lex bot
* Description – any description for your lex bot
* Bot Alias ID – is the ID of the _Alias_ with the intended _Associated Version_
* Bot ID – is the ID found in the _Bot Details_
* Locale ID – each bot version can have multiple languages, language ID should be one of the following in this from the [languages and locales supported by Amazon Lex V2](https://docs.aws.amazon.com/lexv2/latest/dg/how-languages.html?icmpid=docs\_console\_unmapped) and should be existing within your Lex bot.&#x20;
* AWS Credentials
  * Access Key ID – part of IAM user credentials
  * Secret Access Key – part of IAM user credentials
  * User ID – part of IAM user credentials
  * Region – region where the bot exists

![](<../../../.gitbook/assets/image (50).png>)

## On multiple bot  languages and deployments

For each Lex bot there are multiple languages and multiple Aliases (Deployments) but will keep everything simple for now in the models. Each bot in the Captivate Hub can be connected to one language and one version only.

*   If the CH user wants to use both English and Spanish versions of a Lex Bot: that will be two bots in the Captivate Hub.

    1. My First Lex Bot - English - Prod Version
    2. My First Lex Bot - Spanish - Prod Version


* If the CH user wants to use both English and Spanish versions of a Lex Bot, and for each language two versions (dev and prod)
  1. My First Lex Bot - English - Prod Version
  2. My First Lex Bot - Spanish - Prod Version
  3. My First Lex Bot - English - Dev Version
  4. My First Lex Bot - Spanish- Dev Version

## Build me a Bot

For us to build your bot please check our contact information here

{% content-ref url="../../../support.md" %}
[support.md](../../../support.md)
{% endcontent-ref %}
