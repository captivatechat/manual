# CH Response Formats

CH Responses are sent in JSON format, below is an example CH Response.

```javascript
{
    "confidence": 1,
    "actions": [],
    "metadata": {
        "internal": {}
    },
    "messages": [
        {
            "text": "Hi. I'm the Captivate Bot.",
            "type": "text"
        },
        {
            "text": "You can leave us your contact details or you can chat to us directly now!",
            "type": "text"
        },
        {
            "type": "button",
            "buttons": {
                "title": "Please choose from one of the following:",
                "options": [
                    {
                        "label": "Leave Contact Details",
                        "value": "Leave Contact Details"
                    },
                    {
                        "label": "Chat to Agent",
                        "value": "Chat to Agent"
                    }
                ]
            }
        }
    ],
    "intents": [
        {
            "intent": "welcome",
            "confidence": 1
        },
        {
            "intent": "cancel",
            "confidence": 0.54
        },
        {
            "intent": "askFeedback",
            "confidence": 0.53
        },
        {
            "intent": "generalPositiveFeedback",
            "confidence": 0.49
        },
        {
            "intent": "support",
            "confidence": 0.48
        }
    ],
    "responseLanguage": "en_US",
    "chMessage": "62bd352ad4cc30008ecf713c"
}
```
