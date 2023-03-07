# Enviromental Variables

### Frontend

```
REACT_APP_MSTEAMS_URL - MS Teams Bot Public URL
REACT_APP_CHATBOT_URL - Chatbot Public URL
REACT_APP_CHANNEL_URL - Channel Public URL
```

Sample .env:

```
REACT_APP_MSTEAMS_URL=https://msteams.server.local
REACT_APP_CHATBOT_URL=https://chatbot.server.local
REACT_APP_CHANNEL_URL=https://channel.server.local
```

### Chatbot

```
MONGODB_URL - MongoDB url
REDIS_URL - Redis url

DEV_HUB_URL - Public URL of frontend container

JWT_SECRET_KEY - secret key being used to generate JSON Web Tokens for all authenticated routes. A long and random string is recommended for this. 
JWT_EXPIRY - JWT expiry in hours.

GOOGLE_SEARCH_URL - url for the google search microservice that can be enabled to produce backup responses in case of low confidence chatbot responses.
GOOGLE_CLIENT_ID - google client id used for google sign-in.

LANG_TRANS_URL - url for IBM Watson’s Language Translator API. 
LANG_TRANS_KEY - key generated upon signing up to IBM Watson’s Language Translator API

MAILER_SERVICE - email service used to send notifications such as welcome messages for signing-up, low confidence, etc. 
MAILER_USER - email address that sends all mails.
MAILER_PW - password of the email that sends all mails.
MAILER_ADMINS - comma-separated email addresses of the administrators, these emails will receive notifications such as requests for account activation.
MAILER_BCC - bcc email addresses for the same emails the administrators receive. 

LOW_CONF_EMAILS -  comma-separated email addresses to be notified in case of low confidence chatbot responses.
USER_SEED_MONGOID - random mongodb ObjectId. 
USER_SEED_FIRSTNAME - seed first name
USER_SEED_LASTNAME- seed last name
USER_SEED_EMAIL - seed email
USER_SEED_PASSWORD - seed password
USER_SEED_COMPANY - seed company
```

If you will deploy TrialHub feature for use case when you need new users have automatically trial accounts for Watson, Facebook, WhatsApp (Twilio) and Twitter you need to fill up these enviromental variable, if not applicable to your setup you can just the value `none`.

```
TRIALHUB_FACEBOOK_PAGEID -  Facebook Page ID of the Trial Hub
TRIALHUB_FACEBOOK_PAGETOKEN -  Facebook Page Token of the Trial Hub
TRIALHUB_TWITTER_ACCESSTOKEN -  Twitter Access Token of the Trial Hub
TRIALHUB_TWITTER_ACCESSTOKEN_SECRET -  Twitter Secret of the Trial Hub
TRIALHUB_TWITTER_USERID -  Twitter UserID (numbers) of the Trial Hub
TRIALHUB_WATSON_WORKSPACE - Watson Skill ID of the Trial Hub
TRIALHUB_WATSOSN_APIKEY  -  Watson API Key of the Trial Hub
TRIALHUB_WHATSAPP_ACCOUNTSID -  Twilio Account SID of the Trial Hub
TRIALHUB_WHATSAPP_AUTHTOKEN  - Twilio Auth Token of the Trial Hub
```

Sample .env:

```
MONGODB_URL=mongodb://mongodb0.example.com:27017
REDIS_URL=redis://localhost:6379

DEV_HUB_URL=https://hub.server.local

JWT_SECRET_KEY=9xMVIzqABvAMp4QYutPsXxE0hli8lcot05ykZQrS3uDp51MgrevE0JvhMmzSV6C
JWT_EXPIRY=3h

GOOGLE_SEARCH_URL=https://googlesearch.yourdomain.com/search
LOW_CONF_EMAILS=hi@example.com,hello@example.com
GOOGLE_CLIENT_ID=somerandom-id.apps.googleusercontent.com

LANG_TRANS_URL=https://gateway-lon.watsonplatform.net/language-translator/api
LANG_TRANS_KEY=langtranskeystring

MAILER_SERVICE=gmail
MAILER_USER=hello@gmail.com
MAILER_PW=somepassword
MAILER_ADMINS=hi@example.com,hello@example.com
MAILER_BCC=no@example.com

TRIALHUB_FACEBOOK_PAGEID: none
TRIALHUB_FACEBOOK_PAGETOKEN: none
TRIALHUB_TWITTER_ACCESSTOKEN: none
TRIALHUB_TWITTER_ACCESSTOKEN_SECRET: none
TRIALHUB_TWITTER_USERID: none
TRIALHUB_WATSON_WORKSPACE: none
TRIALHUB_WATSOSN_APIKEY: none
TRIALHUB_WHATSAPP_ACCOUNTSID: none
TRIALHUB_WHATSAPP_AUTHTOKEN: none

USER_SEED_MONGOID=5bde800ac324c3005bc216f4
USER_SEED_FIRSTNAME=John
USER_SEED_LASTNAME=Doe
USER_SEED_EMAIL=hi@email.com
USER_SEED_PASSWORD=testpassword
USER_SEED_COMPANY=testcompany
```

### Channel

```
MONGODB_URL - MongoDB url
REDIS_URL - Redis url
RABBIT_URL - RabbitMQ url

DEV_HUB_URL - Frontend Public URL
DEV_CHANNEL_URL - Channel Public URL
DEV_CHATBOT_URL - Chatbot Private URL
DEV_WIDGET_URL - Widget Server Private URL

DEV_CHATBOT_URL - base url for The Captivate Hub back-end.
FACEBOOK_VERIFY_TOKEN - random string to be used in the facebook developer page when required such as changing webhook urls. 

Twitter keys: Apps keys for twitter app owner. Follow this [guide](channel#twitter).
`TWITTER_CONSUMER_KEY`,`TWITTER_CONSUMER_SECRET`,`TWITTER_ACCESS_TOKEN`,`TWITTER_ACCESS_TOKEN_SECRET`,`TWITTER_WEBHOOK_ENV`
```

Sample .env:

```
MONGODB_URL

DEV_HUB_URL=https://hub.server.local
DEV_CHANNEL_URL=https://channel.server.local
DEV_CHATBOT_URL=https://chatbot.server.local
DEV_WIDGET_URL=https://widget-server.server.local

FACEBOOK_VERIFY_TOKEN=RANDOM_TOKEN_HERE

SESSION_SECRET=XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX

TWITTER_ACCESS_TOKEN=XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX
TWITTER_ACCESS_TOKEN_SECRET=XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX
TWITTER_CONSUMER_KEY=XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX
TWITTER_CONSUMER_SECRET=XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX
TWITTER_WEBHOOK_ENV=dev
```

### Livechat

```
OPENSHIFT_LIVECHAT_URL - Livechat Public URL
DEV_CHANNEL_URL - Channel Public URL
DEV_CHATBOT_URL - Chatbot Private URL
MSTEAMS_BOT_URL - MSTeams Bot Private URL

MONGODB_URL - MongoDB url
REDIS_URL - Redis url
RABBIT_URL - RabbitMQ url

MS_APP_NAME - Name of the MS Teams Application installed on your tenant
```

Sample .env:

```
OPENSHIFT_LIVECHAT_URL=https://livechat.server.local
DEV_CHANNEL_URL=https://channel.server.local
DEV_CHATBOT_URL=https://chatbot.server.local

MONGODB_URL=mongodb://mongodb0.example.com:27017
REDIS_URL=redis://localhost:6379
RABBIT_URL=amqp://user:pass@host:10000/vhost

MS_APP_NAME='Captivate Hub'
```

### Teams Bot

```
LIVECHAT_URL - Livechat Public URL
CHANNEL_URL - Channel Public URL
MSTEAMS_AGENT_URL - MSTeams Agent Private URL

MicrosoftAppId - Microsoft Application ID
MicrosoftAppPassword - Microsoft Application Secret

MONGODB_URL - MongoDB url
REDIS_URL - Redis url
RABBIT_URL - RabbitMQ url

PRESENCE_BOT_EMAIL - Office365 Email of Presence Bot
PRESENCE_BOT_PASSWORD: Office365 Password of Presence Bot
```

Sample .env:

```
MONGODB_URL=mongodb://mongodb0.example.com:27017
REDIS_URL=redis://localhost:6379
RABBIT_URL=amqp://user:pass@host:10000/vhost

LIVECHAT_URL=https://livechat.server.local
CHANNEL_URL=https://channel.server.local
CHATBOT_URL=https://chatbot.server.local
MSTEAMS_AGENT_URL=https://msteamsagent.server.local

MicrosoftAppId=XXXXXXXXXXXXXXXX
MicrosoftAppPassword=XXXXXXXXXXXXXX

PRESENCE_BOT_EMAIL=sample@captivat.io
PRESENCE_BOT_PASSWORD=samplepasswordcaptivat
```

### Teams Agent

```
MONGODB_URL - MongoDB url
REDIS_URL - Redis url
RABBIT_URL - RabbitMQ url

LIVECHAT_URL - Livechat Private URL

MicrosoftAppId - Microsoft Application ID
MicrosoftAppPassword - Microsoft Application Secret
```

Sample .env:

```
MONGODB_URL=mongodb://mongodb0.example.com:27017
REDIS_URL=redis://localhost:6379
RABBIT_URL=amqp://user:pass@host:10000/vhost

LIVECHAT_URL=https://livechat.server.local

MicrosoftAppId=XXXXXXXXXXXXXXXX
MicrosoftAppPassword=XXXXXXXXXXXXXX
```

### Widget Frontend

```
REACT_APP_ASSETS_PATH - Widget Frontend Public URL
REACT_APP_DOMAIN - Widget Server Public URL
```

Sample .env

```
REACT_APP_ASSETS_PATH=https://widget.server.local
REACT_APP_DOMAIN=https://widget-server.server.local
```

### Widget Backend

```
channel_gateway_host - Channel Gateway Public URL
channel_gateway_hub_path: /api/widget/hub
channel_gateway_widget_channel_path: /api/widget/integration
channel_gateway_widget_properties_path: /api/widget/widgetProperties
database_uri: MongoDB url

email_bcc - Email BCC for reporting Bugs on Widget
email_from - Email address of Office365 Bot
email_user: Email address of Office365 Bot
email_password: Password of Office365 Bot


mapbox_reverse_geocode_path - MapBox API Public URL
mapbox_token - MapBox Token
session_secret: Random Text for Secret
socket_encryption_key: Random Text for Secret

# for storage_* configuration, create [IBM Cloud Object Storage](https://www.ibm.com/cloud/storage) and fill up the information below using the service credentials
storage_acl
storage_api_key_id
storage_bucket_name
storage_endpoint
storage_ibm_auth_endpoint
storage_service_instance_id
```

Sample .env

```
channel_gateway_host=https://channel.server.local
channel_gateway_hub_path: /api/widget/hub
channel_gateway_widget_channel_path: /api/widget/integration
channel_gateway_widget_properties_path: /api/widget/widgetProperties

database_uri: mongodb://mongodb0.example.com:27017

email_bcc: admin@captitvat.io,qa@captivat.io
email_from: "no-reply" <noreply@captivat.io>
email_password: XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX
email_user: noreply@captivat.io

mapbox_reverse_geocode_path: api.mapbox.com/geocoding/v5/mapbox.places
mapbox_token: XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX

session_secret: XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX
socket_encryption_key: XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX

storage_acl: 
storage_api_key_id: 
storage_bucket_name: 
storage_endpoint: s3.eu-geo.objectstorage.softlayer.net
storage_ibm_auth_endpoint: 
storage_service_instance_id: 
```
