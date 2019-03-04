# validation-flash-call
Simple Flash-Call application that makes a call to validate a PSTN number

Author: 
Filipe Leitão (contact@fleitao.org)

# Description:
This is a very simple Flash-Call RCML-based application that triggers an automated call to the number provided.
The call will ring for 10s and drop. If the recipient of the call picks up the call an automated message will play.
Validation of the number provided is the main purpose of the application. It can be used together with a mobile
application that will detect the incoming call and automatically validate it.

# Usage:
1) Edit rc-flash-call.html and replace your Restcomm API details and the path to rc-flash-call.xml;
2) Load rc-flash-call.html and provide your number in the screen and then click on ‘Verify’;
3) You will get an incoming call to the number provided: let it ring or pick up to listen;

# Service Architecture:
The service is split into two components: 
- rc-flash-call.html / simple HTML front-end that triggers the Restcomm Voice API;
- rc-flash-call.xml / RCML-based application that simply plays a Text-To-Speech message validating the number;

You can learn more about RCML: 
https://www.restcomm.com/docs/Restcomm-CSP/1.0/programmable.html#_restcomm_markup_language_rcml_for_programmable_voice 

Please note that to execute this application you'll need a Restcomm account and a SMS number associated to the application.
You can get a free Restcomm account using the following link: https://cloud.restcomm.com/#/signup
In Restcomm you'll find instructions to get a number or use an existing number of yours.
