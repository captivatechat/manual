---
description: Upload data for your AI Chatbot to ingest as part of its knowledgebase.
---

# Import Your Own Information

<figure><img src="../../.gitbook/assets/image (266).png" alt=""><figcaption><p>After giving your AI Chatbot a name and logo, you will be taken to "Import Your Own Information." This menu contains a list of resources you uploaded, and the option to upload new data.</p></figcaption></figure>

It's in the _**Import Your Own Information**_ page where you will establish your AI Chatbot's knowledgebase by uploading data.&#x20;

Importing your own information or uploading your data is the most important step in AI Chatbot creation. This is what the bot uses to answer user questions.

Make sure the information you will include has everything you want the Chatbot to use as a reference. In-depth sources can provide more accurate and reliable responses from your new Chatbot.&#x20;

{% hint style="info" %}
**The more the merrier!**

Think of this process as building the encyclopedia your Chatbot will rely on when answering customers. Since your Chatbot is an "intelligent" model, it knows how to combine information from different sources. This is where you come in. \
\
The more resources you provide, the more information your Chatbot can access when creating responses!
{% endhint %}

To start adding data to your chatbot, click  !["Import Your Own Information" button leads to the "Import Your Own Information" page. This is where you can upload data or resources to build your AI Chatbot's knowledgebase.](<../../.gitbook/assets/image (19) (1).png>)

### Adding files and URLs to import

<figure><img src="../../.gitbook/assets/image (6) (1) (1) (1).png" alt="Use the blue &#x22;Import&#x22; button to open the &#x22;Import&#x22; menu in order to add files and/or URLs to your Chatbot&#x27;s database"><figcaption><p>Use the blue "Import" button to open the "Import" menu in order to add files and/or URLs to your Chatbot's database</p></figcaption></figure>

An _**Import**_ pop-up window should appear. You can either:

* **Import:** Click or drag **PDF files** (up to 100MB) that contains important information that your Chatbot should know. You can drag multiple files at once by selecting a group of files and dragging them all to the file import area.
* **URL(s):** List a set of URLs (one URL per line) that will become the basis of the knowledge of your Chatbot.&#x20;

Once you have completed the files or webpages you want to import click on the ![Use the blue "Import" button to open the "Import" menu in order to add files and/or URLs to your Chatbot's database](<../../.gitbook/assets/image (25) (1).png>)button.

<figure><img src="../../.gitbook/assets/image (1) (1).png" alt="After you upload your data and click the &#x22;Import&#x22; button in the &#x22;Import&#x22; menu, you will be taken to the &#x22;Proceed with Ingestion?&#x22; window. You will be given an estimated number of tokens required to ingest the data you just uploaded. Click &#x22;Import Selected&#x22; to proceed."><figcaption><p>After you upload your data and click the "Import" button in the "Import" menu, you will be taken to the "Proceed with Ingestion?" window. You will be given an estimated number of tokens required to ingest the data you just uploaded. Click "Import Selected" to proceed.</p></figcaption></figure>

You will be asked to pay a number of tokens to ingest the URL or PDF you've just uploaded. Click ![ Click "Import Selected" in "Proceed with Ingestion?" menu to start ingesting your uploaded information or data.](<../../.gitbook/assets/image (255).png>) to proceed.

{% hint style="danger" %}
**Import limit**

We limit the number of imports to support **a combination of up to 20 Files and URLs.**
{% endhint %}

{% hint style="warning" %}
**Only PDF files allowed**

We only support **PDF files** as of the moment. If you have data in some other format such as a **DOCX** (MS Word) or **PPTX** (MS Powerpoint) file, simply save those files as **PDFs** and import the PDF file.
{% endhint %}

### The import process

<figure><img src="../../.gitbook/assets/image (26) (1).png" alt=""><figcaption><p>A list of recently-uploaded resources are not clickable as they are still being ingested by the AI Chatbot. This process will go to "Allocating resources" then "Ingesting" before a successful ingestion. </p></figcaption></figure>

After clicking the ![ Click "Import Selected" in "Proceed with Ingestion?" menu to start ingesting your uploaded information or data.](<../../.gitbook/assets/image (255).png>) button, you will then see a list of the files or URL(s) being imported. Wait patiently as the information is ingested. Here are the status updates throughout the importation process:

<figure><img src="../../.gitbook/assets/image (27) (1).png" alt="The ingestion process of newly-uploaded data/resources starts with an &#x22;Allocating resources&#x22; message in &#x22;Import Your Own Information.&#x22; This will take a few minutes."><figcaption><p>The ingestion process of newly-uploaded data/resources starts with an "Allocating resources" message in "Import Your Own Information." This will take a few minutes.</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (30) (1).png" alt="After a few minutes of &#x22;Allocating resources&#x22; in &#x22;Import Your Own Information,&#x22; the system will give a message that ingestion has been completed."><figcaption><p>After a few minutes of "Allocating resources" in "Import Your Own Information," the system will give a message that ingestion has been completed.</p></figcaption></figure>

Please be patient. The time taken to import a PDF file or URL is dependent upon the size of the file or webpage.  You can return to import further information or remove information at any time. &#x20;

{% hint style="warning" %}
**Import again whenever you make updates!**

When you upload your resources to an AI Chatbot, they are only ingested **in their instance as of that moment.** This means the AI Chatbot doesn't auto-ingest your URL or PDF if you make any updates.

If you make any major changes to your resources, disable their original iteration and import the updated versions to your AI Chatbot.
{% endhint %}

### Restrict Data from Internet

<figure><img src="../../.gitbook/assets/image.png" alt="A &#x22;Restrict Data from Internet&#x22; toggle is located in the &#x22;Import Your Own Information&#x22; page during AI Chatbot setup. Toggle this to &#x22;Active&#x22; to restrict AI Chatbots into just using the information it contains, and toggle this it &#x22;Inactive&#x22; to allow AI Chatbots to search the internet for information."><figcaption><p>A "Restrict Data from Internet" toggle is located in the "Import Your Own Information" page during AI Chatbot setup. Toggle this to "Active" to restrict AI Chatbots into just using the information it contains, and toggle this it "Inactive" to allow AI Chatbots to search the internet for information.</p></figcaption></figure>

One additional feature is the ability to force your AI Chatbot to only use data it can gather from your resources instead of getting more insights from the internet. This can be done by toggling **Active/Inactive** at the right-hand side of the screen.&#x20;

The AI Chatbot will take note of this and behave as requested in most circumstances but like us humans may not be able to help itself sometimes. Adjust any prompts accordingly to maximize the functionality of this toggle.

Once your data has been imported, click ![Click "Next: AI Chatbot Type" button from "Import Your Own Information" page to proceed to the next stage that involves choosing a template for the new AI Chatbot.](<../../.gitbook/assets/image (267).png>).

***

##
