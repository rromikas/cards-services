# What is it?

It is node js app that has netlify functions. It provides api endpoints:

| Endpoint       | Method   | Body parameters                                              |
| -------------- | -------- | ------------------------------------------------------------ |
| /api/sendCards | **POST** | name, numberOnFront, provider, email, logoText, logoTextSize |
| /api/sendEmail | **POST** | message, email                                               |

# How to launch?

You need to set 2 env variables:  
EMAIL  
EMAIL_PASSWORD  
Variables must be from your **gmail** account since api uses gmail service
For this to work complete 2 steps:

1. "allow less secure apps to access gmail" must be turned on.
2. enable 2-step verification and create new password for app category "other". Use this password as EMAIL_PASSWORD env variable.

### Locally

npm install netlify-cli -g  
npm install  
netlify dev  
\*Now you can access endpoints at localhost:8888/api/\*\*

### On Netlify

Just deploy site from github repository
