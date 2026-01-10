---
description: >-
  All changes to the Captivate platform will be added here. Guides will be
  updated concurrently.
---

# 📕 Changelog

***

## v5.0.4

### 📆2025-12-05

### ⚠️ Fixed

* **Athena**
  * **General**
    * **Athena bot late attendance:** Fixed a bug where Athena is late in calls.&#x20;
  * **During**
    * **Late transcriptions:** Fixed a bug where live transcriptions are not being updated as the call happens.
    * **AI Suggestions errors:** Fixed a bug where AI Suggestions aren't appearing despite having an in-depth transcript.&#x20;
  * **After**
    * **Meeting scheduling errors:** Fixed a bug where meetings aren't being scheduled based on the date and time provided.&#x20;

### 📆2025-11-20

### ✅ Added

* **Athena**
  * **General**
    * **Opportunity Name:** Calls in Athena are now organised into a group of meetings called an "Opportunity" - a reflection of the fact that securing a deal with a company doesn't just happen within a single meeting, but often in a series of calls.&#x20;
  * **Before**
    * **Invite Athena to meetings manually:** Users can now invite the Athena bot into the specific call with a button.&#x20;
    * **More manual editable features:** Before module now has more manually-editable features, making meeting setups much easier.&#x20;
  * **During**
  * **After**&#x20;
    * **Meeting Scheduler:** The After module now includes the ability to schedule next meetings, with the date and time either lifted from the transcript or manually set up by users.&#x20;

### 🟧 Changed

* **Athena**
  * **General**
    * **Tighter text:** Made sure that text throughout the Athena platform are succinct and brief to aid users get information as fast as possible
    * **Light mode:** Light mode now selected as default color
    * **No more auto-inviting Athena:** With the button to invite Athena now existing in Before, it's up to users to manually invite Athena into their meeting as they see fit.&#x20;
  * **Before**
    * **Mini Course sources improvement:** Mini Course now also use the Meeting Description and the core Knowledge Bot as a basis of its topics.
  * **During**
    * **AI Suggestion page finder:** A textbox exists should users want to switch to a very specific suggestion they have encountered, and if they remember the page.&#x20;

### ⚠️ Fixed

* **Athena**
  * **General**
    * **Registration errors:** Fixed a bug that results in faulty registration.&#x20;
  * **Call Pilot**
    * **Name change:** "Call Planner" is now named "Call Pilot"
    * **Email additions error:** Fixed a bug where adjusting attendees in the main calendar doesn't reflect in the Call Planner.
  * **Before**
    * **Mini Course appearance:** Fixed bugs that don't cause the Mini Course to appear based on different actions.
  * **During**
    * **Live Transcription error:** Fixed a bug that doesn't make the transcript update itself live during a call.
    * **AI Suggestions appear too quickly:** Fixed a bug that caused many Live Suggestions to appear.&#x20;
  * **After**
    * **Retention error:** Fixed an error that removes a pre-existing generated After report.&#x20;

### 📆2025-10-30

### ✅ Added

* **AI Chatbots**
  * **Compliance!** A new integration that allows users to test the quality of their AI Chatbots based on specific standards.&#x20;

### ⚠️ Fixed

* **General**
  * **Inconsistent Registration:** Fixed an error where accounts aren't properly registering in the platform.
  * **Email Fixes:** Fixed the text that appears during registration emails.&#x20;
* **Agent Groups**
  * **Agent Group Listing:** Fixed a bug where Agent Groups don't appear in the list after making them.
* **Captivate Organisations**
  * **Same Company, different Organisation:** Fixed a bug where the same company has two different Organisations with user lists.

### 📆2025-10-16

### ✅ Added

* **Chat Flows**
  * **Athena User and Mini Course List:** Have an interface within the Chat Flows view that lets users obtain a list of registered users in an Athena as well as the list of Mini Courses generated in an Athena.
* **Athena**
  * **General**
    * **Edit with AI:** Most items in the Before/During/After modules can be edited with AI using a simple text prompt.&#x20;
  * **Call Calendar (Call Pilot)**
    * **Calendar Syncing:** Users can see their calendars linked within the Call Calendar (Call Pilot), with non-Athena calls marked grey and Athena calls marked blue. Athena calls can be organised and utilised in live conversations as a **Call Plan**.&#x20;
  * **Before**
    * **Meeting Description:** Non-Athena calls that users want to transform into Athena calls will prompt users to add a Meeting Description that will be used as a basis of the meeting information.
    * **Build Call Plan:** Athena can now build **Call Plans** based on the Meeting Description. The main "starting information" of a Call Plan is located within the Before module. The Call Plan will provide information like agenda items, predicted objections, analysed pain points, as well as background data of companies and contacts involved in the call.&#x20;
  * **During**
    * **Pull data from Before:** Ticked items from Before are carried over in During.&#x20;
    * **Embedded Assistant:** The Knowledge Bot can now be accessed in the During module as a chatbot that users can converse with during meetings.
    * **Live Transcript:** An Athena bot will automatically join a designated Athena meeting and begin transcribing the call.&#x20;
    * **AI Suggestions:** The Knowledge Bot can offer live suggestions based on the transcript of the call.&#x20;
    * **Generate After/Re-Generate After:** Users can generate an After module report based on the current transcript with the "Generate After". Meanwhile, existing After reports could be overwritten with "Re-Generate After" - useful when the initial After report has been created while a call is ongoing.&#x20;
  * **After**
    * **AI-based drafting:** Based on the transcript of the call, Athena will create a meeting summary, draft follow-up emails, and suggest action items.&#x20;

### ⚠️ Fixed

* **Athena**
  * **General**
    * **Text fixes:** Tightened the language across the platform
  * **Call Planner**
    * **Inconsistent call details:** Fixed a bug where the Host and Attendees are being shown incorrectly
    * **Inconsistent calendar visualisation:** Fixed some visual errors where some details are not showing up properly.&#x20;
  * **During**
    * **Visual fixes in transcription:** Fixed a bug that makes it difficult to see the actual transcript of the call.&#x20;
    * **Athena avatar for the bot:** The attendee bot to take transcriptions now use the official Athena avatar for easy identification.&#x20;
    * **Live Suggestions navigation:** Navigating the Live Suggestions interface has become easier with new buttons.&#x20;

### 🆕 Introducing Call Pilot (Athena)&#x20;

<figure><img src=".gitbook/assets/image (14).png" alt="A preview of the Captivate Athena interface, showcasing the view of the main Athena Chat alongside the Mini Course Library, Suggested Questions, Call Pilot, Feedback, and Tutorials."><figcaption><p>A preview of the Captivate Athena interface, showcasing the view of the main Athena Chat alongside the Mini Course Library, Suggested Questions, Call Pilot, Feedback, and Tutorials.</p></figcaption></figure>

**Call Pilot** (previously the "Call Calendar") is the most integral part of Captivate Athena's AI sales execution functionality, as it's the feature that directly ties into sales assistance. Aside from studying materials via Mini Courses and conversing with the Knowledge Bot, it's the Call Pilot where users can plan and engage in their calls with Captivate's proprietary AI sales execution assistance.&#x20;

* **Call Pilot:** After connecting your calendar, Call Pilot lets you transform meetings into "Athena calls" that offer AI assistance in any stage of the call process.&#x20;
* **Call Plan:** When accessed in preparation for a meeting, an Athena call is known as a **Call Plan**. They contain:
  * **Before Module:** This is your pre-call study layer, where AI takes your meeting description and surfaces contact information, company information, agenda items, pain points, potential objections, and meeting-focused Mini Courses that you can study.
  * **During Module:** This is your in-call layer, where AI can generate live transcripts and provide live suggestions based on both context and items selected in the Before Module.&#x20;
  * **After Module:** This is the post-call layer, where AI can take the existing call's transcript and organise next steps. These include auto-updating the CRM as well as providing a call summary, creating a draft email to be sent after the call, listing tasks to be distributed across attendees, and even scheduling the next call.&#x20;

### 📆2025-09-22

### ✅ Added

* **Captivate Organisations:**
  * **RBAC (Role-Based Access Control):** Users can now become part of an organisation when they join Captivate via any work email. They can invite users, as well as create and edit roles with Read, Write, and Delete features. Features are divided across User Management, User Role Management, Chat Flows, Reports, and Chat Transcripts.&#x20;



***

## v5.0.3

### 📆2025-08-22

### ✅ Added

* **AI Chatbots**
  * **Custom Tags & Metadata (for&#x20;**_**AI Chatbot > Add Data**_**):** Allow users to filter ingested docs using custom keywords. You can test this in the Import Your Information/Add Data step of AI Chatbot creation.

### 🆕 Custom Tags and Metadata

<figure><img src=".gitbook/assets/image (405).png" alt="After uploading new data in AI Chatbots > Import Your Own Information, you will be prompted if you want to add metadata. This &#x22;Add New Metadata tags&#x22; menu is where you will set metadata identifiers so your data is easily organised and sorted."><figcaption><p>After uploading new data in AI Chatbots > Import Your Own Information, you will be prompted if you want to add metadata. This "Add New Metadata tags" menu is where you will set metadata identifiers so your data is easily organised and sorted.</p></figcaption></figure>

You can now sort ingested information using metadata tags. This is extremely useful for large quantities of content, as you can now add categories (**Metadata Tag**) and identifiers **(Value)** that the platform can auto-assign to relevant content. You may freely edit this within _**AI Chatbots > Importy Your Own Information.**_&#x20;

***

## v5.0.2

### 📆2025-08-14

### ✅ Added

* **General**
  * **AI Agent Groups (Beta):** With Developer Mode on you can now create AI Agent Groups comprised of many AI Chatbots. Attach this to your Chat Flow and your conversations get auto-routed to the appropriate AI Chatbot.&#x20;
* **AI Chatbots**
  * **Enable Mini Course Integration (AI Chatbot > Integration):** Start creating Mini Courses based on your bot’s ingested knowledge.

### 🆕 Agent Groups (Beta)

<figure><img src=".gitbook/assets/image (406).png" alt="The &#x22;Agent Group&#x22; window showing a specific Agent Group. When showing the details of an Agent Group, users can see the Agents (AI Chatbots) selected for the group, their original AI Chatbot names, their Provider (LLM), and Example Queries used to toggle the AI router to switch between them."><figcaption><p>The "Agent Group" window showing a specific Agent Group. When showing the details of an Agent Group, users can see the Agents (AI Chatbots) selected for the group, their original AI Chatbot names, their Provider (LLM), and Example Queries used to toggle the AI router to switch between them.</p></figcaption></figure>

**Agent Groups** make use of the platform's unique AI router feature, where users can be rerouted to appropriate sources of information (AI Chatbots/Agents) based purely on context. With Developer Mode turned on, users can group existing AI Chatbots into an Agent Group. This Agent Group becomes the equivalent of an "AI Chatbot" that can be used within a Chat Flow.&#x20;

Instead of choosing just one AI Chatbot with limited knowledge, an Agent Group is the "representative" of a network of AI Chatbots.&#x20;

### 🆕 Enable Mini Course Integration

<figure><img src=".gitbook/assets/image (407).png" alt="&#x22;Mini Course Integration&#x22; window as accessed via AI Chatbots > Integration > Mini Course. This is the main menu that activates the course generation API of Captivate, allowing an AI Chatbot to create Mini Courses when attached to an Athena Channel."><figcaption><p>"Mini Course Integration" window as accessed via AI Chatbots > Integration > Mini Course. This is the main menu that activates the course generation API of Captivate, allowing an AI Chatbot to create Mini Courses when attached to an Athena Channel.</p></figcaption></figure>

Users can now designate any AI Chatbot as a source of Mini Courses when attached to an Athena Channel.&#x20;

Accessed within _**AI Chatbots > Integration > Mini Course**_, any AI Chatbot with this integration enabled can be used with an Athena, with the chat interface now allowing users to create 5-minute bite-sized Mini Courses about any information ingested by the chatbot.&#x20;



***

## v5.0.1

### 📆2025-08-04

### ✅ Added

* **General**
  * **Developer Mode:** Users can now enjoy more advanced features from Captivate by toggling the Developer Mode in their Account Settings.
* **AI Chatbots**
  * **External Bots:** Use an API endpoint to turn third-party chatbots into bots compatible with Captivate Chat Flows. This selection can be toggled once Developer Mode is activated.    \
    Add Data supports more file types: Aside from PDFs and URLs, you can now upload DOCX, XPS, RTF, TXT, PPTX, XLSX, XLS, and CSV files.
  * **Markdown format now set as default:** Get more visually-consistent conversations with Captivate bots as we've set Markdown as the default format of responses.    \
    Select Type Summarized View: Identify your AI Chatbot's selected chatbot Type easier with the modified Select Type view. Users will also receive a warning before choosing another Type.
*   **Chat Flows**



    * **Atomization of edits:** Editing Chat Flows will now open a selector that lets you choose which specific Chat Flow component you want to edit - whether the AI Chatbot, Channel, Livechat, or all of them at once.
*   **Athena**



    *      **Product Rename:** The **"Full Chat"** Channel is now **Athena**, our AI sales execution platform. Create a mini-site within our platform that allows you to focus on selling, complete with our sales execution suite.&#x20;
    * **Badges now available:** Passing a Knowledge Test now rewards users with a course Badge. They no longer will be able to retake the Knowledge Test.



    * **Add Feedback options:** Create a list of suggested subject lines and emails where user feedback is automatically sent, allowing you to respond to user suggestions and complaints much faster.
    * **Add Terms and Conditions:** Attach Terms and Conditions to your Full Chat to accommodate specific legal requirements by your team.
    * **Start Chat Toggle (You and AI):** Use a toggle to choose whether you or your AI Chatbot will start a conversation in your Full Chat. This is set to your AI Chatbot by default.
    * **Multi-Select Languages:** Choose which languages you want your Full Chat to appear in, auto-translating components based on the language the user selects.      \
      Back to Library button: Use a "Back" button inside a Mini Course to go back to your Mini Course Library.
    * **Sidebar View Toggle:** Hide the Full Chat sidebar to get a more focused view of your current section.
    * **Unread Chats now numbered: Y**ou can now see the number of unread chats in your Full Chat within the dedicated "Unread Chats" part of the interface.

### 🟧 Changed

* **Chat Flows**
  * **Full Chat icon is now Athena: Y**ou will now see Athena's headshot as the icon for Full Chat.    \
    Add Suggested Questions for your Full Chat: Create Suggested Questions for your Full Chat users, giving them examples of prompts to ask your AI Chatbot.
  * **Updated Full Chat subdomain URLs:** Full Chats created in Captivate now appear as "\[subdomain].athena.captivate.com"
  * **Suggestion Questions lead straight to chats:** Clicking a Suggested Question in your Full Chat will now create a new chat with your bot, with that specific question as your first query.
  * **Unique Knowledge Test per take:** Knowledge Tests now feature non-repeating questions and answers, ensuring every test iteration is different.
  * **Notifications are now clickable:** Clicking a Notification will send you to the conversation associated with it, letting you access responses much faster.

### ⚠️ Fixed

* **General**
  * **Removed legacy dependencies:** We have removed legacy dependencies from our codebase repository, as most of them are either broken or outdated.
* **AI Chatbots**
  * **Incorrect token count:** Fixed instances of incorrect token counts being reflected on specific bots.    \
    Estimated Token Cost on Add Data: Fixed an error where ingested files are auto-computed for token consumption. Now, only selected files for pre-ingestion will get an Estimated Token Cost.
*

    **Athena**

    * **Visual fixes:** Adjusted the extra space to Tools selections, fixed theme color errors, correct profile images reflected across conversations and settings, renamed components for better UX.
    * **Chat rename on refresh:** Fixed instances where new chats are auto-renamed on refresh. New chats now automatically get renamed based on conversation context as users converse with AI Chatbots.
    * **Double language options**: Fixed a bug that causes the appearance of multiple instances of the same language in the Language selection dropdown.

### 🆕 Full Chat is now Athena

<figure><img src=".gitbook/assets/image (2) (1).png" alt="A preview of the Captivate Athena interface, showcasing the view of the main Athena Chat alongside the Mini Course Library, and Feedback."><figcaption><p>A preview of the Captivate Athena interface, showcasing the view of the main Athena Chat alongside the Mini Course Library, and Feedback.</p></figcaption></figure>

We've renamed our Full Chat channel into **Athena**, our AI sales execution platform.

When you create an Athena inside _**Chat Flow > Channels**_, we will provide a "mini-site" you and your sales representatives can use to help your sales process. It comes with these features:

* **Knowledge Base:** The AI Chatbot attached to the Athena will become the primary Knowledge Base of your Athena. Conversations here will be based on knowledge ingested by your AI Chatbot, so you can create a dedicated AI Chatbot for your Athena that will ingest your marketing and sales materials.&#x20;
* **Mini Course:** Through the _**AI Chatbot > Integration > Mini Course**_ feature, your AI Chatbot can create bite-sized Mini Courses that Athena users can study in preparation for their sales calls. These Mini Courses will be based on your AI Chatbot's knowledge.

***

## v4.0.0

### 📆2025-03-21

### ✅ Added

* **Full Chat Channels are live!** If you want your AI Chatbot to have a dedicated webpage, you can finally create a full-sized messaging page with our Full Chat Channels.&#x20;
* **Markdown now supported by Web Chats!** Expect more visual flair when conversing with our Web Chats thanks to markdown language support.&#x20;
* **Speech Options make Web Chats for accessible!** Use Speech Options with Web Chats to add options to talk to AI Chatbots with your built-in microphone or even hear their responses.&#x20;
* **Other Options provide more customizability to Web Chats!** Customize more specific aspects of your Web Chat such as strings that indicate _"text sent by"_ or text to _"download transcript_."&#x20;

### 🟧 Changed

* **Transcripts**
  * **Replaced Name with Last Chat Message:** Instead of listing the _Name_ of the users who conversed with an AI Chatbot in the Transcripts, we're listing their _Last Chat Message_ instead.&#x20;
* **Import Your Own Information**
  * **More Filter Options:** You can now sort your data more intuitively with updated filter options inside AI Chatbots > Add Information. In the Import Your Own Information window, you can now filter columns in ascending or descending order, and filter the types of data displayed based on their status.&#x20;
  * **File Folders with URL Crawler:** Use Captivate Chat's built-in URL Crawler feature to find file folders, making the data ingestion process more efficient.&#x20;

### ⚠️ Fixed

* Fixed a bug where the button to request for Live Agents are not visible when opened using Safari.
* Fixed a bug that doesn't reset the checkbox of a deleted Transcript.
* Fixed a bug where mass ingestion via Chatbot > Add Information suddenly stops while still incomplete.
* Fixed a bug where ingestion via Chatbot > Add Information didn't make any progress at all.

### 🆕 Full Chat Channels will dedicate a webpage for your AI Chatbot

<figure><img src=".gitbook/assets/image (350).png" alt="Create a &#x22;Full Chat&#x22; Channel within Chat Flows > Channels will set up an AI Chatbot that occupies an entire webpage. "><figcaption><p>Create a "Full Chat" Channel within Chat Flows > Channels will set up an AI Chatbot that occupies an entire webpage. </p></figcaption></figure>

While our Web Chat Channels can be expanded to occupy a larger portion of your screen, they're still technically a part of whatever page you assigned them to.&#x20;

This all changes with **Full Chat Channels**, as this lets you set up an AI Chatbot that will occupy an entire webpage! You can finally direct your users to a webpage dedicated to a chatbot - great for interactive sessions!&#x20;

### 🆕 Markdown Syntax now supported by Web Chats

<figure><img src=".gitbook/assets/image (353).png" alt="Web Chats now support Markdown syntax, allowing AI Chatbots to provide more structured and visually appealing responses."><figcaption><p>Web Chats now support Markdown syntax, allowing AI Chatbots to provide more structured and visually appealing responses.</p></figcaption></figure>

Our Web Chats now support **Markdown** syntax, allowing AI Chatbots to provide more structured responses. Enjoy tables, headers, and other formatting options when conversing with your AI Chatbots.

### 🆕 Customize Web Chats further with Other Options!

<figure><img src=".gitbook/assets/image (348).png" alt="The &#x22;Other Options&#x22; menu under Chat Flow > Channels > Web Chat will now let users change specific values of text fields of their web chats and widgets, adding more variety to messages."><figcaption><p>The "Other Options" menu under Chat Flow > Channels > Web Chat will now let users change specific values of text fields of their web chats and widgets, adding more variety to messages.</p></figcaption></figure>

We've incorporated **Other Options** in Configure Web Chat, giving you the opportunity to provide specific string values to other parts of your AI Chatbot's web chats or web widgets.&#x20;

Unlike values such as your AI Chatbot's name or organization name, Other Options can let you customize more UI-leaning elements, specifically what your Web Chat says when...&#x20;

* ...you want to download the transcript
* ...it tells the date "today"
* ...you want to chat with a Live Agent
* ...you want to send a message to your Web Chat
* ...you want to start a conversation

And many more!

### 🆕 Speech Options make Web Chats more convenient!

<figure><img src=".gitbook/assets/image (349).png" alt="&#x22;Speech Options&#x22; in Chat Flows > Channel > Configure Web Chat will allow users to toggle options that will let them talk to AI Chatbots via their microphone (Enable Voice In) and/or hear spoken responses (Enable Read Out)."><figcaption><p>"Speech Options" in Chat Flows > Channel > Configure Web Chat will allow users to toggle options that will let them talk to AI Chatbots via their microphone (Enable Voice In) and/or hear spoken responses (Enable Read Out).</p></figcaption></figure>

Thanks to **Speech Options** within Configure Web Chat, we can now toggle more advanced and accessible audio options when interacting with our AI Chatbots. Depending on your preference, you can:

* **Enable Voice In:** This will let users use their microphone to talk to your AI Chatbot.
* **Enable Read Out:** This will let users get their AI Chatbot's responses in audio form.

### 🆕 Last Chat Message in Transcripts

<figure><img src=".gitbook/assets/image (351).png" alt="&#x22;Last Chat Message&#x22; replaces &#x22;Name&#x22; in Transcripts, allowing users to see the last chat message sent before being logged into the Transcript for that specific time period."><figcaption><p>"Last Chat Message" replaces "Name" in Transcripts, allowing users to see the last chat message sent before being logged into the Transcript for that specific time period.</p></figcaption></figure>

We've removed the "Name" column in Transcripts and replaced them with **Last Chat Message**, giving you the last message sent to the conversation before it was logged by the system.&#x20;

### 🆕 Filter Options now available in Import Your Own Information

<figure><img src=".gitbook/assets/image (352).png" alt=""><figcaption><p>AI Chatbots > Add Data will bring users to an updated Import Your Own Information page, where there's a Filter for Status (Active/Other States) and Type (Web/PDF) as well as the option to sort things in ascending and descending order.</p></figcaption></figure>

Users can now filter and sort their data more efficiently in the "Import Your Own Information" page. New options include:

* **Filter:** Only reveal data based on their **Status (Active or Other Statuses)** and/or their **Type (Web or PDF)**
* **Sort:** Select arrows beside the name of the column you want to sort in descending or ascending order.

***

## v3.5.1

### 📆2025-02-10

### ✅ Added

* **Custom Channels are here!** If you want to integrate Captivate Chat functionalities into your own Channel outside our offerings, you can finally do so!
* **Citations are now live!** You can make your AI Chatbot provide sources of its data whenever it provides responses to users.
* **Token Estimation errors** are now reported! The platform will now let you know if a URL you plan on ingesting isn't available for processing.&#x20;
* **Asynchronous messages** are now saved in Transcripts. Messages that are via the Chatbot directly from agents (without using the Chat Flow) are now stored alongside traditional messages.
* **Session Expiry** can now be set in select Channels. This will end inactive chats after a set number of days.

### 🟧 Changed

* Changed a button in the Edit Data section of the Create AI Chatbot process.&#x20;

### ⚠️ Fixed

* **Smileys are back!** We fixed a chat error regarding emojis, so now you can add emojis to your conversations with AI Chatbots!
* Fixed a bug where pages are forcibly refreshed after the user uploads a file of the same file name multiple times during the Web Widget Test.
* Fixed a delay between the time users choose files to ingest and the system starts ingesting it.
* Fixed a bug that delays the Add Information section of the Create AI Chatbot process after an ingestion procedure is cancelled.
* Fixed a bug that doubles the URLs ingested when using the Captivate Chat URL Crawler.&#x20;

### 🆕 Custom Channels

<figure><img src=".gitbook/assets/image (341).png" alt="Select &#x22;Custom Channel&#x22; under Chat Flows > Channel in order to show your AI Chatbot in your very own Channel of choice outside our regular options. "><figcaption><p>Select "Custom Channel" under Chat Flows > Channel in order to show your AI Chatbot in your very own Channel of choice outside our regular options. </p></figcaption></figure>

**Custom Channels** are now available as a Channel option for Captivate Chat users. Select this if you want to show our AI Chatbot and connect your users to Live Agents in a different platform outside of our offerings.

This will require some manual setup, which we will provide in our guide!

### 🆕 Citations

<figure><img src=".gitbook/assets/image (339).png" alt="In the &#x22;Import Your Own Information&#x22; window, you can toggle &#x22;Enable Citations&#x22; so your AI Chatbot will send an extra message after each response that contains the sources of its answers."><figcaption><p>In the "Import Your Own Information" window, you can toggle "Enable Citations" so your AI Chatbot will send an extra message after each response that contains the sources of its answers.</p></figcaption></figure>

**Citations** are now available in your Captivate Chat bots! This takes the form of a simple but powerful toggle in _AI Chatbots > Add Information._&#x20;

If you turn on this toggle, your AI Chatbot will provide an extra response that contains the sources of their answers.

### 🆕 Token Estimation Errors

<figure><img src=".gitbook/assets/image (342).png" alt="Faulty URLs will now be flagged during the Token Estimation process of the AI Chatbot > Add Information part of the AI Chatbot Creation process.  "><figcaption><p>Faulty URLs will now be flagged during the Token Estimation process of the AI Chatbot > Add Information part of the AI Chatbot Creation process.  </p></figcaption></figure>

We now have **Token Estimation Errors** that will appear as error messages when trying to ingest faulty URLs.&#x20;

These errors will come with tooltips that explain why these URLs haven't been ingested, which range from inaccessible URLs to incompatible formats.

### 🆕 Session Expiry

<figure><img src=".gitbook/assets/image (340).png" alt="When editing Channels, you can change the &#x22;Session Timeout (Days)&#x22; of Instagram, Facebook Messenger, and WhatsApp. This will dictate the number of days before an existing inactive conversation is closed."><figcaption><p>When editing Channels, you can change the "Session Timeout (Days)" of Instagram, Facebook Messenger, and WhatsApp. This will dictate the number of days before an existing inactive conversation is closed.</p></figcaption></figure>

**Session Expiry** can now be modified in your Channels. This dictates the number of days before an existing (but inactive) conversation with your AI Chatbot on Instagram, Facebook Messenger, or WhatsApp is closed.

***

## v3.5.0

### 📆2025-01-29

### ✅ Added

* We now support **SCA Stripe**. SCA, which stands for Strong Customer Authentication, allows us to offer more secure transactions when purchasing Captivate Chat Tokens or upgrading your subscriptions.
* **Web Widgets:**
  * **Full Screen Embeds** are now available for Web Widget Chat Flows! Simply customize a special iframe code with your Web Widget's API and put that into the HTML of the webpage where you want a full screen AI Chatbot to greet your customers.&#x20;
* **Metadata:**
  * Will now have **conversation dates** added by default, helping you keep track of important information much faster.
  * Initial metadata will be stored in custom metadata, making data retrieval more efficient.
* **Captivate AI & LLM API** will now make it easier for AI devs to integrate with AIs with Captivate Chat.
* **Custom Channels:**
  * **New APIs** are available to make conversation deletions in the index (not the real sessions) much easier to manage if you're using our **Custom Channels:**
    * Use the `conversation_id` of that specific conversation to delete it from the index.
    * Use the `user_id` of the user in question to delete all their conversations from the index.
    * Asyncrhonous messaging via `send_message` can now handle file attachments.

### 🟧 Changed

* **Free and Basic Accounts** now get **1,000,000 Tokens!** This leaves you more room to try Captivate Chat for your projects.&#x20;
* **AI Chatbots:**
  * Clicking any AI Chatbot will immediately reveal the list of modifications you can do to them.

### ⚠️ Fixed

* Fixed some UI inconsistencies to provide a more seamless experience.&#x20;
* Fixed deep crawler issues, so it now:
  * Shows results in the estimator (instead of no results).&#x20;
  * Is not case sensitive (it was previously)
  * It doesn't need "www." (it previously did)
* Fixed issues involving the ingestion of at least 100 URLs.&#x20;
* Fixed issues involving the creation of an AI Chatbot directly from the Chat Flow process.

### 🆕 Captivate AI & LLM API

<figure><img src=".gitbook/assets/image (338).png" alt="This is a Python Package Index (PyPI) screenshot of the Captivate AI &#x26; LLM API, an API developed by Captivate Chat to handle its API formats."><figcaption><p>This is a Python Package Index (PyPI) screenshot of the Captivate AI &#x26; LLM API, an API developed by Captivate Chat to handle its API formats.</p></figcaption></figure>

We have released the **Captivate AI & LLM API.** Access it [here](https://pypi.org/project/captivate-ai-api/).&#x20;

We developed the Captivate AI & LLM API to handle Captivate Chat's API formats. This flexible messaging and metadata management system is built using Pydantic models and designed to handle complex communication scenarios with robust checking and validation.

Its main features include dynamic metadata handling, immutable session and chat properties, flexible message type support, custom metadata manipulation, and conversation title management. &#x20;

### 🆕 Full Screen Embed Code

<figure><img src=".gitbook/assets/image (333).png" alt="A Web Widget adjusted to fit a full screen resolution thanks to the Full Screen Embed Code. If you fill up a special iframe code with your Web Widget API and paste that code into the HTML of your assigned webpage, that particular webpage becomes a full-screen AI Chatbot."><figcaption><p>A Web Widget adjusted to fit a full screen resolution thanks to the Full Screen Embed Code. If you fill up a special iframe code with your Web Widget API and paste that code into the HTML of your assigned webpage, that particular webpage becomes a full-screen AI Chatbot.</p></figcaption></figure>

We have made a **Full Screen Embed Code** for you to use with your Web Widget Chat Flows!

Unlike our traditional embeds that provide you with an interactive AI Chatbot within a webpage, our Full Screen Embed Code will "fill" the webpage with your AI Chatbot. In order to do this, simply put your Web Widget API into a special iframe code you can access in [channel-web-chat](start-creating/create-a-chat-flow/select-channel/channel-web-chat/ "mention")

***

## v3.4.1

### 📆2025-01-10

### ✅ Added

* **AI Chatbots:**
  * **Select Type** now has a toggle for **Full Chat History**, letting you decide if you want your AI Chatbot to respond based on previous conversations with the user or to treat every conversation as a completely new one.&#x20;
  * You can now set **session expiration timers** within an AI Chatbot so they can automatically end an inactive session after your specified period of time.

### 🆕 Full Chat History

<figure><img src=".gitbook/assets/image (326).png" alt="The &#x22;Use Full Chat History For AI Context&#x22; toggle in &#x22;Select Type&#x22; when creating your own AI Chatbot will determine if the specific AI Chatbot in question will use all prior conversations with the user as the contextual basis of the current session. Toggling yes will do so, and toggling no on Full Chat History will treat each session as a completely new one."><figcaption><p>The "Use Full Chat History For AI Context" toggle in "Select Type" of the AI Chatbot creation process. This will determine if the specific AI Chatbot in question will use all prior conversations with the user as the contextual basis of the current session. Toggling yes will do so, and toggling no on Full Chat History will treat each session as a completely new one.</p></figcaption></figure>

We've added a **Full Chat History** toggle in the "Select Type" page of the AI Chatbot creation process.&#x20;

Taking the form of the "Use Full Chat History for AI Context" button, this will toggle whether the AI Chatbot in question will use all prior sessions with the user as context for its current responses. Doing so will cost more tokens, but will provide maximum accuracy.

## v3.4.0

### 📆2025-01-03

### ✅ Added

* **Tutorials are live!** Learn the ropes in creating your AI Chatbots, Chat Flows, and Live Agent integrations within the Tutorial page of the Captivate Chat platform!
* **Meet our Guidebot!** We've deployed our Guidebot within the Captivate Chat platform! Once you log in to your account, you can ask our Guidebot for any advice as well as tips and tricks on how to best use Captivate Chat for your needs!
* **Mobile Optimization notice** appears when users to try to access Captivate Chat on mobile platforms.&#x20;
* **AI Chatbots:**
  * **URL Crawler** is now added under "Import Your Own Information" that auto-searches all URLs under a single URL. This will make importing groups of URLs under a "mother" URL much easier.&#x20;

### 🟧 Changed

* **Our Token Estimator now uses Server-Sent Events (SSEs)**. Thanks to SSEs, we should be experiencing faster and more efficient resource management. With SSEs, AI Chatbots should be able to ingest new information much faster.
* **Cost-Saving toggle for Chat Histories are available globally.** We will now provide a global toggle for users to choose if they want to view the full or AI-analyzed chat histories of their AI Chatbots.&#x20;
  * This is unlike in previous versions, where this toggle is placed inside each AI Chatbot.&#x20;
  * As per the previous version, the AI-analyzed chat histories will cost fewer tokens to produce.&#x20;

### 🆕 Tutorials

<figure><img src=".gitbook/assets/image (313).png" alt="The &#x22;Tutorial&#x22; page in the Captivate Chat platform contain videos that explain essential processes in using Captivate Chat. They are arranged in tiles, with a thumbnail and the name of the lesson."><figcaption><p>The "Tutorial" page in the Captivate Chat platform contain videos that explain essential processes in using Captivate Chat. They are arranged in tiles, with a thumbnail and the name of the lesson.</p></figcaption></figure>

Learning about Captivate Chat has never been easier!

Get in-depth tutorials on how to use the Captivate Chat platform using our **Tutorials** page! We have Tutorials for most of our processes in the platform, and we'll constantly update these Tutorials whenever we have major releases.&#x20;

To access our Tutorials, simply click the ![The "Tutorials" button on the left side of the dashboard leads to the "Tutorial" page. The The "Tutorial" page in the Captivate Chat platform contain videos that explain essential processes in using Captivate Chat. They are arranged in tiles, with a thumbnail and the name of the lesson.](<.gitbook/assets/image (315).png>) button on the left side of the Captivate Chat dashboard.

### 🆕 URL Crawler

<figure><img src=".gitbook/assets/image (317).png" alt="The &#x22;Import Your Own Information&#x22; page of the AI Chatbot creation process now features a URL Crawler. This is accessed via pressing the &#x22;Import Button.&#x22; With this, users can now enter one URL and it will take the first layer of URLs sharing its section. "><figcaption><p>The "Import Your Own Information" page of the AI Chatbot creation process now features a URL Crawler. This is accessed via pressing the "Import Button." With this, users can now enter one URL and it will take the first layer of URLs sharing its section. </p></figcaption></figure>

We've added a **URL Crawler** to the "Import Your Own Information" page of the AI Chatbot creation process. Users can now choose to enter a URL and Captivate Chat will gather all relevant URLs of its similar section.

If you want to retrieve relevant URLs within a particular website layer, the URL Crawler can also be used with a **wildcard character or an asterisk (\*)**.&#x20;

### 🆕 Mobile Optimization Notice

<figure><img src=".gitbook/assets/image (318).png" alt="The Captivate Chat platform can be opened in mobile browsers but it&#x27;s not yet optimized for mobile devices. We&#x27;ve added a Mobile Optimization Notice to warn users that while they can proceed to the Captivate Chat platform, its functions might not work properly in their device."><figcaption><p>The Captivate Chat platform can be opened in mobile browsers but it's not yet optimized for mobile devices. We've added a Mobile Optimization Notice to warn users that while they can proceed to the Captivate Chat platform, its functions might not work properly in their device.</p></figcaption></figure>

We added a **Mobile Optimization Notice** for users trying to access our platform using their mobile devices.

As have yet to fully optimize the Captivate Chat platform for mobile users, this means many functions of the Captivate Chat platform might not work properly in mobile browsers. You can continue to use the platform normally via mobile by clicking "Continue to Site" when you see the Mobile Optimization Notice.

***

## v3.2.0

### 📆 2024-10-02

### ✅ Added

* **Token Metrics** are now revealed for major AI Chatbot uses such as ingesting information, training, and various conversations to aid payment tracking.
* **AI Chatbots** now have a limiter and organizer to maximize Token usage without overwhelming their systems. This should lessen situations of AI Chatbots randomly slowing down.&#x20;

### 🟧 Changed

* **Web Widget Preview:** The Web Widget Preview now has a more noticeable _Page Settings_ button to access its features.
* **Import Your Own Information (AI Chatbots):** Pagination should now reveal ingested PDFs and URLs in sets of 10 for more efficient compilation and access to users.&#x20;

### ⚠️ Fixed

* Made minor adjustments to the UI to improve accessibility and encourage a more engaging experience.&#x20;
* Streamlined Token tracking so users are immediately notified if they have run out of Tokens.
* Ensured that **delete** information (URLs, PDFs, accounts) are permanently deleted as intended.&#x20;
* **Microsoft Teams:** Transcripts of the AI Chatbot's conversation with a user are now retained when their concern is escalated to a Live Chat agent in MS Teams.

### 🆕 Token Metrics

<figure><img src=".gitbook/assets/image (6) (1) (1) (1) (1).png" alt="Tokens are now tracked throughout Captivate Chat features. The main Token count is revealed on the left side of the dashboard at all times, giving users an idea how many Tokens they have consumed, when their next Monthly Usage Reset would be, and any Extra Tokens they possess."><figcaption><p>Tokens are now tracked throughout Captivate Chat features. The main Token count is revealed on the left side of the dashboard at all times, giving users an idea how many Tokens they have consumed, when their next Monthly Usage Reset would be, and any Extra Tokens they possess.</p></figcaption></figure>

The Captivate Chat platform will now show **token metrics** to keep track of your Tokens whenever you use them across various parts of the platform. These include:

* Ingesting data that are uploaded into the system.
* Conversations between users and the AI Chatbots they create.
* Testing and deploying AI Chatbots in various platforms.

These token metrics can aid in managing your Captivate Chat plan, as major AI functionalities of the platform rely heavily in Token usage.

In line with this new change, we are also going to **actively track** Token usage across the platform and notify users whenever they have to purchase more Tokens.&#x20;

### 🆕We revamped the Web Widget Preview

<figure><img src=".gitbook/assets/image (8) (1) (1) (1).png" alt="The Web Widget Preview of Setup > Chat Flow > Channels > Web Widget is revamped with a more streamlined look."><figcaption><p>The Web Widget Preview of Setup > Chat Flow > Channels > Web Widget is revamped with a more streamlined look.</p></figcaption></figure>

We've upgraded the look of our **Web Widget Preview**!&#x20;

You can now preview your Web Widget Chat Flow with a completely revamped background.

<figure><img src=".gitbook/assets/image (7) (1) (1) (1).png" alt="The Web Widget Preview of Setup > Chat Flow > Channels > Web Widget now has a more visible &#x22;Page Settings&#x22; button to edit the live preview."><figcaption><p>The Web Widget Preview of Setup > Chat Flow > Channels > Web Widget now has a more visible "Page Settings" button to edit the live preview.</p></figcaption></figure>

The ![](<.gitbook/assets/image (9) (1) (1) (1).png>) button is now more visible and accessible, making it much easier for users to modify their live preview setup.&#x20;

***

## v3.1.1

### 📆 2024-09-19

### ✅ Added

* **Makeover!** We've updated the Captivate Chat website to feature our new logos!
* **Edit AI Chatbots while making Chat Flows!** You can now directly modify your AI Chatbots while creating your Chat Flows.&#x20;

### 🟧 Changed

* **Transcripts** now feature a separate **Date Range** filter instead of the previous **By Date** sorting filter.&#x20;

### ⚠️ Fixed

* Fixed a bug that doesn't load the complete list of ingested content for some Chat Flows.
* **Chat Flow > Channel > Web Widget:** Fixed a typo. There is now an _"Embed Web Widget"_ option instead of the previous _"Embed Live Chat"_ option.

### 🆕 Website Makeover!

<figure><img src=".gitbook/assets/image (4) (1) (1) (1) (1) (1).png" alt="The new Captivate Chat website featuring its updated logo with a blue color palette. "><figcaption><p>The new Captivate Chat website featuring its updated logo with a blue color palette. </p></figcaption></figure>

We're giving the Captivate Chat website a major makeover!&#x20;

This new update features **new logos** we've prepared for Captivate Chat, now featuring a sleek blue color palette designed to evoke a more professional and relaxing atmosphere.&#x20;

### 🆕 Edit your AI Chatbots while making Chat Flows

<figure><img src=".gitbook/assets/image (5) (1) (1) (1) (1) (1).png" alt="Users can now click the three dots above their AI Chatbot choice in Setup > Chat Flow > My AI Chatbots to directly modify their AI Chatbots during the Chat Flow creation process."><figcaption><p>Users can now click the three dots above their AI Chatbot choice in Setup > Chat Flow > My AI Chatbots to directly modify their AI Chatbots during the Chat Flow creation process.</p></figcaption></figure>

We know that creating an AI Chatbot from scratch is wildly different when compared to connecting them to the rest of your Channels and Live Chats via a Chat Flow, as there are things you would only notice about your AI Chatbot after bringing everything together.

It's for this reason that we added a new feature that lets you **edit your AI Chatbots during the Chat Flow creation process**. After clicking _Setup > Chat Flow_, the list of AI Chatbots present in _My AI Chatbots_ menu now feature a three dots that enable you to edit them straight in the Chat Flow-creation process.

This means you no longer have to go all the way back to _Setup > AI Chatbot_ just to modify an AI Chatbot you'd use for your current Chat Flow - you can do everything in one convenient location.

***

## v3.0.0

### 📆 2024-09-18

### ✅ Added

* **Incident Tracker** now informs users whenever Captivate Chat services are down.
* **Overwrite Warning** will inform users that changing the Channel of an existing Chat Flow will remove their current setup.&#x20;

### 🟧 Changed

* **Transcripts** now feature various options to simplify their use, such as sorting and deletion options.

### ⚠️ Fixed

* AI Chatbots now properly recognizes postal codes of locations.
* AI Chatbots no longer declares in a separate chat message that they are checking for available Live Chat agents upon request, as we already have a preset message prepared when users ask to be escalated to a Live Chat agent.&#x20;
* **AI Chatbots > Select Type:** Removed a bug that triggers the _"Submit & Test"_ function whenever users select a tooltip.&#x20;

### 🆕 Overwrite Warning (Chat Flow)

<figure><img src=".gitbook/assets/image (5) (1) (1) (1) (1).png" alt="Trying to change the Channel of an existing Chat Flow will now provide a warning to users that doing so will overwrite their existing data."><figcaption><p>Trying to change the Channel of an existing Chat Flow will now provide a warning to users that doing so will overwrite their existing data.</p></figcaption></figure>

We have included an **override warning** in Chat Flows that will activate whenever users try to change the Channel of an existing Chat Flow. Undergoing this process will overwrite their data, and any overwritten data can no longer be retrieved.

It's advisable for users to duplicate their existing Chat Flow before switching Channels, as doing so will force them to start creating their Chat Flow from scratch.&#x20;



### Transcript Options

<figure><img src=".gitbook/assets/image (3) (1) (1) (1) (1) (1) (1).png" alt="The Transcript page offers various features such as a Search function, as well as sorting through Filters such as Email, Channel, or Chat Flow. There are options to pick a Date to sort lists of conversations, as well as the option to check multiple conversations for deletion."><figcaption><p>The Transcript page offers various features such as a Search function, as well as sorting through Filters such as Email, Channel, or Chat Flow. There are options to pick a Date to sort lists of conversations, as well as the option to check multiple conversations for deletion.</p></figcaption></figure>

The **Transcript** page now offers different options for users to sort conversations detected by the Captivate Chat platform. These include the following:

* **Checkbox selection of conversations.** You can also mass-delete these conversations by pressing the _**Delete**_ button, although this is irreversible.
* **Sort by various filters**, such as Date the conversation occurred, the Email used, Channel where the conversation took place, and the Chat Flow that managed the conversation.

***

## v2.2.0-2

### 📆2022-02-02

It's now much easier to use the Captivate Hub for your **Livechat** needs!&#x20;

We're introducing new ways to modify your Livechat to automate certain tasks. Thanks to **Manual Assignment**, you can now set pre-determined messages that trigger after specific conditions - such as assigning chats based on an agent's MS Teams status.&#x20;

Agents can also use the new _**`"Reassign"`**_ command to transfer the chat to another available agent.&#x20;

### ✅ Added

* reCaptcha support on registration
  * Added new environmental variable on frontend `REACT_APP_GOOGLE_RECAPTCHA_KEY`
* Implementation of **Manual Assignment**
  * Added `manualAssign (bool)` `manualMessageUsersExist(string)` `manualMessageUsersNotExist (string)` `idleTimeoutBeforeAssign(int) (in minute)` `idleTimeoutAfterAssign(int) (in minute)` `idleMessageBeforeTimeout (string)` `idleMessageAfterTimeout (string)` to Hub properties.
* Implementation of **Agent Status**
  * Added `agentStatus (Array) [Available,Busy,Away,Offline]` to Hub properties.
* Implementation of **Reassign Agents**
* New React frontend
  * Added `GOOGLE_SECRET_KEY` to enviromental variable on chatbot
* **Livechat** configuration editor on frontend
* New Teams app permissions
  * `Site.Read.All` (for accessing files to teams and send it to channels)
  * `Group.ReadWrite.All` (for modifying teams channel permissions)

### 🟧 Changed

* All messages on channels to MS Teams is now tagged to selected agent

### 🟥 Removed

* Removed support for the legacy frontend. preferred the new React frontend

### ⚠️ Fixed

* Emojis and attachment message filter on agents' message
* Messages on direct mode is now properly sent to Teams Desktop and Teams Mobile

### 🆕 Agent Status (Livechat)

You can now **modify agent assignments** based on their **presence status** in MS Teams.&#x20;

Using the Livechat configuration, you can **set chat assignments** based on an agent's **status** or availability in MS Teams. Commands can affect agents who set themselves as `"Available",` `"Busy",` `"Away"` and `"Offline."`&#x20;

This example video demonstrates a Livechat configured to only assign chats to someone set as `"Busy".` Check it out:&#x20;

{% embed url="https://www.youtube.com/watch?v=gG1GO2aHJAs" %}
Agent status demonstration
{% endembed %}

### 🆕 Manual Assignment (Livechats)

You can now **activate&#x20;**_**Manual Assignments**_ when configuring a Livechat.&#x20;

This allows **pre-made messages** to be sent after **meeting certain conditions**. Here are the properties you can modify:

*   `manualMessageUsersExist(string)`&#x20;

    Displays a message **if there is an available agent** to respond to the client.
*   `manualMessageUsersNotExist (string)`&#x20;

    Displays a message **if there are no agents available** to respond to the client.&#x20;
*   `idleTimeoutBeforeAssign(int) (in minute)`&#x20;

    A value **(in minutes)** before a timeout is declared, **should a conversation not be escalated** to an agent.&#x20;
*   `idleTimeoutAfterAssign(int) (in minute)`&#x20;

    A value **(in minutes)** before a timeout is declared, **if there's an agent assigned but neither agent nor client is responding** to each other.
*   `idleMessageBeforeTimeout (string)`&#x20;

    Displays a message when `idleTimeoutBeforeAssign(int)` elapses.
*   `idleMessageAfterTimeout (string)`&#x20;

    Display a message when \`\`idleTimeoutAfterAssign(int)\` elapses.&#x20;

#### ➦ Default Values

Here are the **default Manual Assignment** values:&#x20;

* `manualAssign (bool):` false
* `manualMessageUsersExist(string):` “Our agents know you’re waiting and will chat here as soon as they’re free.”
* `manualMessageUsersNotExist (string):` “Our agents is currently busy at the moment.”
* `idleTimeoutBeforeAssign(int) (in minute):` 5
* `idleTimeoutAfterAssign(int) (in minute):` 10
* `idleMessageBeforeTimeout (string):` “Our agents is currently busy at the moment.”
* `idleMessageAfterTimeout (string):` “Livechat Ended”

#### ➦ Example Scenarios

You might find this manual assignment feature useful if you encounter the following scenarios:&#x20;

*   **There are available users.**\
    Displays: **manualMessageUsersExist(string)**

    \
    Suppose Teams Group A is connected to the Captivate Hub web widget, and the channel is asking if there are any agents available. Agent A (Busy) and Agent B (Available) are currently online.\
    \
    If Manual Assignment exists that assigns a chat to anyone set as "Available" (Agent B), then the channel has to declare that there's at least one agent (Agent B) that might be available to assist them. <br>
* **There are no available users.**\
  Displays: **manualMessageUsersNotExist(string)** \
  \
  Suppose Teams Group A has an active channel asking if there are agents available. However, both Agent A (Busy) and Agent B (Busy) are both occupied. \
  \
  If only "Available" agents are programmed to receive chat assignments, then the channel declares there are no available agents to assist them. <br>
* **Time has elapsed and no users managed to assist them.**\
  Runs: **idleTimeoutBeforeAssign**\
  Displays: **idleMessageBeforeTimeout**\
  \
  Suppose Teams Group A has an active channel asking for agents, and Agent B (Available) is not busy. This will have the channel declare that an agent will assist the client soon. Until such a time that Agent B responds to the client, the chatbot will run the Idle Timeout counter. \
  \
  If the assigned time elapses and Agent B hasn't responded, a message explains that chat will be put on time out due to the lack of agent response. <br>
* **Time has elapsed that the agent and client didn't speak to each other.**\
  Runs: **idleTimeoutAfterAssign**\
  Displays: **idleMessageAfterTimeout**\
  \
  Suppose Teams Group A has an active channel asking for agents, and Agent B (Available) managed to respond to the client's questions. After some time, someone in the conversation hasn't responded. This triggers a background Idle Timeout counter.\
  \
  If the assigned time elapses, a message appears that states one of the parties have yet to respond and the chat will be put on time out.&#x20;

{% embed url="https://www.youtube.com/watch?v=4p1kpHahDmk" %}
Manual Assignment Demo
{% endembed %}

### 🆕 Reassign Agent

You can now use the _**`"Reassign"`**_ command to **reassign agents within the same Teams group.**&#x20;

Normally, a Support Chatbot is assigned to an available Live Support Agent so they can answer client queries on their behalf. However, not all Live Support Agents can answer a client's questions. This is where _**Reassign**_ comes in.&#x20;

Should the need arise to transfer control of the Support Chatbot to another Live Support Agent, do this **in the MS Teams chat:**

1. Type _**`"@TheCaptivateHub"`**_ to tag the Captivate Hub
2. Type _**`"Reassign"`**_ and press _Enter_.
3. An automated message will appear alongside a drop down of available team members.
4. Select the desired team member to transfer the Support Chatbot.

Check out the video below:

{% embed url="https://www.youtube.com/watch?v=l1JoTW5_ZG8" %}
Reassign agent demo
{% endembed %}



***

## v2.2.0-1

### 📆2021-08-26

**Instagram support is now live!**&#x20;

You can now use Captivate Hub to create chatbots for Instagram via the Watson Assistant. Before you create your Instagram chatbots, make sure your Instagram account is a Business Account and that it is connected to your Facebook Page.&#x20;

We made updates to the documentation to reflect these new changes.

### ✅ Added

* **Instagram** support
* Add bot templates support on Watson Assistant
* New enviromental variable for app-ecb-frontend (frontend / legacy)
  * `REACT_APP_FACEBOOK_APPID` - Facebook Application ID
* New enviromental variable for app-chatbot (chatbot)
  * `FACEBOOK_APPID` - Facebook Application ID
  * `FACEBOOK_SECRET` - Facebook Application Secret Key
* New permissions added to Facebook Application
  * `instagram_manage_messages`
  * `instagram_basic`
  * `pages_manage_metadata`
  * `pages_show_list`

### 🟧 Changed

* Using Facebook OAuth to add Facebook / Instagram as channels (same as Twitter now)
* Enabled public registration
* Update Microsoft Teams permissions for AppSource ([https://appsource.microsoft.com/en-us/product/office/WA200003575?tab=DetailsAndSupport](https://appsource.microsoft.com/en-us/product/office/WA200003575?tab=DetailsAndSupport))

### 🆕 Instagram Integrations

Before attempting integrations, please ensure that you're using an **Instagram Business Account**. This account has to be **connected to your Facebook page**. For more information, please click [here](https://www.facebook.com/business/help/898752960195806).

#### ➦ Facebook Developers Advance Access

* public\_profile
* pages\_messaging
* Business Asset User Profile Access
* instagram\_manage\_messages
* instagram\_basic
* pages\_manage\_metadata
* pages\_show\_list

#### ➦ Facebook Developers Valid OAuth Redirect URLs

* Your app-channel-gateway Public URL (ex: [https://hub.captivat.io/gateways/channel](https://hub.captivat.io/gateways/channel))

#### ➦ Facebook Developers Allowed Domains for the JavaScript SDK

* Your frontend Public URL (ex: [https://hub.captivat.io/](https://hub.captivat.io/))

To add Instagram to the Hub, you click the link below:

{% content-ref url="/broken/pages/K3oA79KPLTUTTsJbnstn" %}
[Broken link](/broken/pages/K3oA79KPLTUTTsJbnstn)
{% endcontent-ref %}

### ⚠️ Teams Application Permission

* Channel.Create
* Channel.Delete.All
* Channel.ReadBasic.All
* ChannelMessage.Read.All
* Chat.ReadWrite
* Group.Read.All
* Presence.Read.All
* Team.Create
* Team.ReadBasic.All
* TeamMember.ReadWrite.All
* TeamActivity.Send
* TeamAppInstallation.TeadWrite
* User.ReadBasic.All

***

## v2.2.0

### 📆2021-08-06



This is the Initial release of the **Captivate Hub** to the public.

### ✅ Added

* Bot Template setup
* Registration

### 🟧 Changed

* Changed frontend ([https://hub.captivat.io](https://hub.captivat.io)) to the new design
* Old frontend will be hosted on legacy.
* Moved [https://manual.captivat.io](https://manual.captivat.io) to Gitbook
