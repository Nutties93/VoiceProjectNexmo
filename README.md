# VoiceProjectNexmo

# Overview
This project focuses on the API/Webhooks integration from express server to Nexmo server.

## Usage

Create an application on the Nexmo portal. A private.key will be downloaded. Move this private.key to the root directy.
Take note of the application_id. 

Update the .env file. Insert values for API_KEY, API_SECRET,APPLICATION_ID, PRIVATE_KEY, VIRTUAL_NUMBER,TO_NUMBER.

Install npm modules (from the root of the project)

```
npm install
```

To start the server (from the root of the project)
```
node ivr.js
```

Run ngrok application. Listen to port 3000
```
ngrok http 3000
```

Update the webhook url in your account setting for the above application. it will look like this!
1) EVENT URL
```
https://1fd8a7c3.ngrok.io/webhooks/events
```
2) ANSWER URL
```
https://1fd8a7c3.ngrok.io/webhooks/answer
```


## How this works
We will run the IVR application. I have edited to sample code to meet all the requirements for the certification project.


## After starting the application
--> 1) Dial to your VIRTUAL.NUMBER that you have stored in the .env file.
```
2nd requirement: You will the current date,day and time from the phone call.
```
--> 2) Press 1 to be redirected to the TO_NUMBER that you have stored in the .env file.
```
3rd requirement: Your TO_NUMBER phone should start ringing.
```
--> 1) Dial to your VIRTUAL.NUMBER that you have stored in the .env file.

--> 2) Press 4 to hear a sample mp3 audio file.

```
1st requirement: listening to an audio file.
```





