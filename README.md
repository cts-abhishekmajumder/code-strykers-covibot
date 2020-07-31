# CoviBot - An Intelligent COVID-19 Chatbot

A basic GitHub repository example for Call for Code submissions and those projects that join the Code and Response initiative. Not all sections or files are required. You can make this as simple or as in-depth as you need.


## Contents

1. [Short description](#short-description)
1. [Demo video](#demo-video)
1. [The architecture](#the-architecture)
1. [Long description](#long-description)
1. [Built with](#built-with)
1. [Web Preview](#web-preview)
1. [Contributing](#contributing)
1. [Versioning](#versioning)
1. [Authors](#authors)
1. [License](#license)
1. [Acknowledgments](#acknowledgments)

## Short description

### What's the problem?

Part of the World Health Organization's guidance on limiting further spread of COVID-19 is to practice social distancing. As a result, schools in most affected areas are taking precautionary measures by closing their facilities. With school-aged children at home for an indeterminate amount of time,  keeping them engaged, entertained, and on top of their education is important.

### How can technology help?

Schools and teachers can continue to engage with their students through virtual classrooms, and even create interactive spaces for classes. As parents face a new situation where they may need to homeschool their children, finding appropriate online resources is important as well.

### The idea

It's imperative that learning and creating can continue when educational institutions have to shift the way they teach in times of crises, such as the COVID-19 pandemic. Providing a set of open source tools, backed by IBM Cloud and Watson Services, will enable educators to more easily make content available for their students.

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

## Long description

[More detail is available here](DESCRIPTION.md)

## Built with

* [IBM Cloudant](https://cloud.ibm.com/catalog?search=cloudant#search_results) - The NoSQL database used
* [IBM Cloud Functions](https://cloud.ibm.com/catalog?search=cloud%20functions#search_results) - The compute platform for handing logic
* [IBM Watson](https://cloud.ibm.com/catalog?search=watson#search_results) - The chatbot framework
* [IBM Watson Discovery](https://cloud.ibm.com/catalog?search=discovery#search_results) - The cognitive search engine

## Web Preview

[CoviBot Web Preview](https://web-chat.global.assistant.watson.cloud.ibm.com/preview.html?region=eu-gb&integrationID=e222ce6d-7923-4330-abd6-b9a223d12358&serviceInstanceID=fd10a9da-d1f9-4fae-abb7-01a04cc81d83)

## Contributing

Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details on our code of conduct, and the process for submitting pull requests to us.

## Versioning

We use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/your/project/tags).

## Authors

* **Billie Thompson** - *Initial work* - [PurpleBooth](https://github.com/PurpleBooth)

See also the list of [contributors](https://github.com/Code-and-Response/Project-Sample/graphs/contributors) who participated in this project.

## License

This project is licensed under the Apache 2 License - see the [LICENSE](LICENSE) file for details

## Acknowledgments

* Based on [Billie Thompson's README template](https://gist.github.com/PurpleBooth/109311bb0361f32d87a2).
