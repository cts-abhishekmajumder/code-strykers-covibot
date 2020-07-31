# CoviBot - An Intelligent COVID-19 Chatbot

A basic GitHub repository example for Call for Code submissions and those projects that join the Code and Response initiative. Not all sections or files are required. You can make this as simple or as in-depth as you need.


## Contents

1. [Description](#description)
1. [Demo video](#demo-video)
1. [The architecture](#the-architecture)
1. [Long description](#long-description)
1. [Built with](#built-with)
1. [Web Preview](#web-preview)
1. [Contributors](#contributors)
1. [Versioning](#versioning)
1. [Authors](#authors)
1. [License](#license)
1. [Acknowledgments](#acknowledgments)

## Description

### What's the problem?

Current COVID 19 pandemic is continuously raising questions on its symptoms, nearby medical facilities as well as the current status of schools, transportation, and other public services.
But, in times of crisis, most of the call centers or helpline numbers are often overloaded with high volume of incoming calls, thus raising the wait time, quality of service and panic. Any other communication service is also rarely available especially in the urban and rural areas. Thus creating an anxiety in the people during this pandemic situation. But, what if people have a chat bot available and accessible easily, which will be able to provide response to the different queries frequently asked by them.

### Our Solution?

CoviBot is an efficient chatbot solution with the below properties which will help communities to understand the latest on the COVID-19 situations along with possible symptoms and probability of having infection - 
- The input will be in text form for now. Voice input can also be incorporated in later releases. 
- Chat bot will provide some basic but important information about current pandemic situation COVID 19 that users requests for.
- It would be able to identify if user might be affected by COVID 19 based on the input symptoms given.
- It would help user about real time COVID 19 statistics for different countries and states worldwide.
- It would be able to help the user about nearest COVID 19 hospital or isolation centers or test center based on specific location mentioned by user.

## Demo video

[![Watch the video](https://github.com/cts-abhishekmajumder/code-strykers-covibot/blob/master/covibot-demo-thumbnail.PNG)](https://player.vimeo.com/video/442740990)

## The architecture

![Video transcription/translation app](https://github.com/cts-abhishekmajumder/code-strykers-covibot/blob/master/covibot-architecture-diagram.png)

1. The user visits a website with the COVID-19 chatbot and asks a question.
2. The Node.js web server calls Watson Assistant hosted in IBM Cloud.
3. Watson Assistant uses natural language understanding and machine learning to extract entities and intents of the user question.
4. The COVID-19 FAQ presents commonly asked questions about the pandemic for the user to select
5. There is another option for users to self-assess their current health status by answering a set of questions.
6. Watson Assistant invokes an OpenWhisk open source-powered IBM Cloud Function.
7. IBM Cloud Function calls Watson Discovery running in IBM Cloud.
8. Watson Discovery presents an external URL for detailed information
9. Watson Assistant invokes an OpenWhisk open source powered IBM Cloud Function.
10. IBM Cloud Function calls a series of COVID-19 APIs to get statistics.
11. Watson Assistant replies to the user inquiry.
12. The Node.js web server displays the chat answer to the user.

## Business Benefits

- It would help communities quickly to understand crucial information about the COVID-19 pandemic situation and free up customer service resources to focus on higher-level issues. 
- The solution will be available 24x7 to cater to variety of requests from end users
- The solution can be accessed by a wide range of users in parallel without any performance delay
- Providing basic information to users, the Chatbot will be able to dispel a lot of myth surrounding the pandemic and build mass awareness
- By helping users in self-detection of probable symptoms of the disease, it can help in early detection and thus minimize community spread
- By providing real-time information and news items, it will make the user more cautious towards the spread of the disease
- By providing information like nearest hospital and Containment or RED Zones it helps the end user get proper assistance during the time of crisis


## Built with

* [IBM Cloudant](https://cloud.ibm.com/catalog?search=cloudant#search_results) - The NoSQL database used
* [IBM Cloud Functions](https://cloud.ibm.com/catalog?search=cloud%20functions#search_results) - The compute platform for handing logic
* [IBM Watson](https://cloud.ibm.com/catalog?search=watson#search_results) - The chatbot framework
* [IBM Watson Discovery](https://cloud.ibm.com/catalog?search=discovery#search_results) - The cognitive search engine

## Web Preview

[CoviBot Web Preview](https://web-chat.global.assistant.watson.cloud.ibm.com/preview.html?region=eu-gb&integrationID=e222ce6d-7923-4330-abd6-b9a223d12358&serviceInstanceID=fd10a9da-d1f9-4fae-abb7-01a04cc81d83)

## Contributors

* Rajat Banerjee
* Sinchan Saha Bhowmick
* Somenath Kundu
* Prasun Ghosh
* Abhishek Majumder

## License

This project is licensed under the Apache 2 License - see the [LICENSE](LICENSE) file for details

## Acknowledgments

* Based on [Billie Thompson's README template](https://gist.github.com/PurpleBooth/109311bb0361f32d87a2).
