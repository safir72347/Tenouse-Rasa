# Tenouse-Rasa

Tenouse-Rasa is the rasa chatbot project of The Tenouse Project - https://github.com/safir72347/The-Tenouse-Project

### Project Screenshots
<img src="https://github.com/safir72347/The-Tenouse-Project/blob/main/assets/screenshots/chatbot/Screenshot_2021-08-01-20-17-57-09.png" width="400" height="700" />
<img src="https://github.com/safir72347/The-Tenouse-Project/blob/main/assets/screenshots/chatbot/Screenshot_2021-08-01-20-18-03-12.png" width="400" height="700" />
<img src="https://github.com/safir72347/The-Tenouse-Project/blob/main/assets/screenshots/chatbot/Screenshot_2021-08-01-20-18-09-84.png" width="400" height="700" />
<img src="https://github.com/safir72347/The-Tenouse-Project/blob/main/assets/screenshots/chatbot/Screenshot_2021-08-01-20-18-16-81.png" width="400" height="700" />
<img src="https://github.com/safir72347/The-Tenouse-Project/blob/main/assets/screenshots/chatbot/Screenshot_2021-08-01-20-18-24-03.png" width="400" height="700" />
<img src="https://github.com/safir72347/The-Tenouse-Project/blob/main/assets/screenshots/chatbot/Screenshot_2021-08-01-20-18-30-39.png" width="400" height="700" />

### Features
1. Post a property
2. View Properties
3. View Roommates
4. Start/Stop Alerts
5. Subscribe/Unsubscribe to newsletters
6. Buy Premium
7. House of the day

### Steps to run

1. Train the model
```
rasa train
```

2. Start the REST API

```
> rasa run -m models --enable-api --cors “*” --debug
> Endpoint: http://localhost:5005/webhooks/rest/webhook
```

Docker References:

https://elements.heroku.com/buttons/just-ai/rasa-heroku-template
https://github.com/samik-saha/rasa-chatbot
