# Outgoing Action

* It is stored in the context variable $outgoing\_action.&#x20;
* Aside from messages, actions can also be sent by the chatbot.
* Actions can be used for triggering certain events within Conversational Hub

## **Types of outgoing action**

1. **Normal** - sending specific actions to Conversational Hub.
   * **type** - set type property to “normal”
   * **action** - set action property to any value.

![](https://lh5.googleusercontent.com/8PiVreDVEbeMUPMdSY7UJ2GtiwCAvcfEbk95HCpLCmuZuRiX3e2xGUhkyezqQVsPNylSOdhjWo1Vsm0L6xu-6qqjREhYGFFXfOL79ZJ0V5WhAXjLNUlAm0Ofrvfh6gb3\_kMsVEg)

Developers are free to define their own list of outgoing\_action. These are ways for chatbot developers to send signals with frontend developers. In e.g. web widgets , channels and custom channels.

### **Example use cases**

1. You want to popup a google maps modal in the parent website whenever the user says. I want a map

![](https://lh3.googleusercontent.com/kUUOoMekL3CYnltwxYf9P-7jki3Wh9own4UCNF3GIpiTu5\_SXuf7gy9PBouxpi591zrCiYqnkGV0OHof0-VxlmP6N2bbgXCR1sZ2C4xkKk6gM21sLsHRskcv3XqN-A)

While on the frontend You ask the developer to implement this.

![](https://lh5.googleusercontent.com/5XF\_6ZhA8xi1tL\_I56Aioq1qx9aaybXT63P3VxhoJM4cQhXN8bP07TxtEv1\_jCJU\_o0ttX9tbjSF8PJp4ztWnkHrjgFP1uLaPMsuiXUVkEEHUaTctNNTI2V-4HpRrg)

&#x20;2\. Redirect user to another page

![](https://lh5.googleusercontent.com/scqMM6URuxM7n-RUYeziZuQn4bbId18Jit1WIAMtkRnkr1XLNKhFWZ\_mNxE0iIMeZ05SxRjDPb6seB-5FMgRkM9IAY-twLG8OaEH\_TCRyW9hLpXrrS1zLS1mEKOj\_Q)

While on the frontend you ask the developer to implement this

![](https://lh3.googleusercontent.com/4PQVk0VuRnHzJHgHPxDE63-MwBHC2uk4OGRq1Q\_9ddtNVGR7K-fUIsFvxHFu99VtREPSzcXpuWP98CqTZ8FnjrslgbaNsCHSnK7FAmJs-sMVq1u9\_VVoD3nqjXqeug)

There are many use cases and it is up to the developers to maximize and use this feature that was made possible through Captivate Hub

_It is to be noted that we will be migrating outgoing\_action format to be in parity with incoming\_action format. This means that instead of just having action as property. We will replace it with id and data. Next update will have this kind of format._

![](https://lh5.googleusercontent.com/e92cWbJFWIXm8AKc8EWtBHaZ4A49LWUEtqZvZimnxOJZoNUE2OvWRbpoZs19qvo0kmZsjqiL91BCQRFrsDxpfTvCF9jDFW587JHcbe\_p2pkf1sCHGCcrEBnt7zVAuA)

![](https://lh3.googleusercontent.com/9QCktIZKh2YV8Zf9QZby0CM1q6ZT6oIqztZLaCOBa7LOeWJIMxb7segot858yiwg9lg9yBuEl1QFQdGu1-bccaq1Theq5u7UtrVTwjmHEDM-GSBGEzbqLfGbplntkg)

This will allow more flexibility in sending actions outside the bot. Allowing to send object data throughout the backend of CH and frontend

### **Reserved actions**

1.  **Escalate to Human** - This action triggers the escalation of the conversation between the user and agent.&#x20;

    * set action to “escalateToHuman”



![](https://lh5.googleusercontent.com/8PiVreDVEbeMUPMdSY7UJ2GtiwCAvcfEbk95HCpLCmuZuRiX3e2xGUhkyezqQVsPNylSOdhjWo1Vsm0L6xu-6qqjREhYGFFXfOL79ZJ0V5WhAXjLNUlAm0Ofrvfh6gb3\_kMsVEg)

&#x20;2\. **Get Location** - This action gets the current location of the user.

![](https://lh6.googleusercontent.com/cA3N8FS4e1Py6N68OADbCIlU62c2L0yITZ4JSkeTTl16MDsvBDlSqoMrABWENCLWItEomdEssKNb5RnXE26h77dLvI\_ZvULGN6tk5wy3V0Rj7Y7uENdAjivlZ9MlYCjX43ynQVo)

* Initialize $getLocation context variable in Watson Assistant.&#x20;
* In $getLocation variable, field, storeTo and done properties are required.
  * field - property where the location will be stored.&#x20;
  * storeTo - object where the location will be stored.
  * done - value to be set to $incoming\_action.id to check if get location action is completed.
  * Trigger get location by setting $outgoing\_action context variable to {“type”:”normal”,”action”:”getLocation”}
  * Once location is received, access the location in $formdata context variable. Location variable will be stored on $formdata.userInfoForm.location for this example. ($formdata..)

2\. **API Call** – action for sending API calls.

![](https://lh6.googleusercontent.com/py4kcsyAcKfTbRX8qFS4zFKD9Y2\_Xxtys\_YKHQVjSkgKKNQpoqXtUNr-qUpJ8gizeRqYFDIGiFmDNLIz5zOcmYlBP4oqosNbvvEEz9stD5IzHELxI9M-xGb4wJ4HS-rm2PRm1I8)

* type - set type property to “apiCall”&#x20;
* url - set url property to the link you will send the request to&#x20;
* authentication - set authentication property for any authentication needed.&#x20;
* cookies - set cookies property to add cookies as part of the request.&#x20;
* method - set method property for the request type such as “GET” and “POST”&#x20;
* data - set data property to be sent as part of the body of a POST request, only applicable when the method is set to “POST”.&#x20;
* result - set result property to be the variable name which contains the response.&#x20;
* done - set done property to be the value set to $incoming\_action.id when the API call is successful. If the done property is set to “callDone”, after the API call, $incoming\_action.id will be set to “callDone”.

![](https://lh4.googleusercontent.com/ZJKA5-NzcJZLwLSYP5DBhftK0Wh3Nk\_116BWibya8i-OSOigaBuLmo9qs4WEHh4tmY87dfaF5MeI5XRiE-HBFC2stboW6eJ9QKFhPeSFaK3kN6JrIreivWYKsJfbDg)

_This should not be confused with Watson's own action invoke which calls cloud functions in IBM cloud. While both achieve the same feat. Captivate's own webhook is more diverse as you can freely use it directly and you will not be just limited to IBM Cloud functions. It is also a consistent format across all future NLP integrations in our roadmap. So it will have the same format as using LUIS or any other chatbot vendor_

**File Upload** _-_ uploading files or images on Conversational Hub

* Set your $getFileUpload context variable.&#x20;
* field and storeTo properties are required.
  * &#x20;field - property where the file/s are stored.&#x20;
  * storeTo - object where the file/s are stored.&#x20;
* Upon upload of files, the files will be accessible at $formdata..\[index].&#x20;
* For this example, files are accessible on $formdata.form1.file\[0], Index 0 for the first file. Index 1 for the second file if available.

![](https://lh4.googleusercontent.com/AIFko6M43xlufMThXIDZoSZH-QyRk8jiweZA-jAj6TlpFW2WDAA6sbUDq30XwPtrdNEoeb8PPZP475ahqA0WkWTBpz3DulBQkGXQHU8XNGBuLXmaQ7Sba0nYsbY0X1gkEZhhtDg)
