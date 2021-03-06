---
slug: opsdroid
title:  Opsdroid
date:   2017-11-20 09:30:00 +0000
categories: Projects
tag: Chat Bot
tag-icon: fas fa-robot
source: https://github.com/opsdroid/opsdroid
tech: Python Asyncio NLU
image: ../../images/opsdroid.jpg
excerpt: An open source chatbot framework written in python. It is designed to be extendable, scalable and simple.
---
While listening to one episode of `Podcast.__init__` I came across Opsdroid. In the end of the show, Jacob Tomlinson says that he would love to have people helping with the project.  

I always wanted to contribute to an Open Source project but wasn't sure how to start. One day I checked Osdroid on GitHub, went through the list of issues, forked the repo and read some of the code to try and understand how everything worked.

Initially, I was unsure how to help. I doubted that I could do much with the knowledge I had. I even had to read about yaml files and what you do with them. In the end, I helped with documentation (mostly changing README and the example configuration file).

Jacob has been a pretty amazing person since the first day I've made my first pull request to Opsdroid and he is always ready to give a hand or a piece of advice. Not only I've grown a lot since I started contributing to the project I've also learned new things and ways to write better code.

# Things I've contributed with

- example_configuration.yaml
  - Added new skills to the file
  - Added database details
  - Added connectors details

- include another yaml file inside main configuration file
  - Added `include constructor` to work with the command `!include` in a yaml file
  - Created test to assert if a yaml file contains all the data from another yaml file
  - Updated documentation file referred to the `!include` function

- Log welcome message with useful info
  - Created text to be logged
  - Created function to be called upon start of opsdroid
  - Added functionality to turn message on/off through the configuration file
  - Created test to assert if the welcome message was called

- [skill-google-it](https://github.com/opsdroid/skill-google-it)
  - Added more search engines
  - Updated regex to accept both `google` and `search` commands
  - Added personalised message to be returned together with the googled link
  - Updated README title

- [skill-devtools](https://github.com/opsdroid/skill-devtools/)
  - Added `help` function - returns quick info and useful links
  - Added `help skills` function - returns active opsdroid skills
  - Added `clear` function - clears terminal text
  - Updated README - added the new functions

- [skill-chat](https://github.com/FabioRosado/skill-chat)
  - Created all the functions
  - Created `customise.yaml` to allow user to customise opsdroid replies
  - Created `vocab` List
  - Modified README from `skill-google-it` to suit the chat skill

- [skill-weather](https://github.com/FabioRosado/skill-weather/)
  - Created function to get weather data from `OpenWeatherMap` API
  - Created `weather` function to get current weather, humidity levels and degrees
  - Created `cold_outside` function to get information if it's cold outside
  - Replaced requests with aiohttp to interact with the OpenWeatherMap API

- Add [wit.ai](https://wit.ai) parser/matcher support
  - Created parser by following the api.ai parser as example
  - Added test cases for the parser and matcher

- Add a test for `aiohttp.ClientOSError` exceptions in parsers
  - Used wit.ai parser to test ways to catch the ClientOSError exception on a test
  - Updated api.ai and luis.ai parser tests to include the ClientOSError test

- Add Issue/PR template 

- Rename Api.ai references with Dialogflow
  - Renamed all Api.ai references to Dialogflow
  - Created new dialogflow matcher and Added tests for it
  - Logged deprecation warning on apiai matcher - tested if logging was called

- Add [Recast.AI](https://recast.ai/) parser/matcher support
  - Created parser and matcher
  - Added test cases for the parser and matcher
  
- Added/Updated Documentation
  - Created tutorials to help beginners get started with opsdroid
  - Updated contributing.md
  - Updated READMe.md
  - Added documentation for wit.ai and Recast.AI parser/matcher
  - Replaced Api.ai reference with new name - Dialogflow

- Added typing/thinking delay functionality
  - Added two functions in `opsdroid.message`: typing, thinking delay
  - Created tests for the functions
  - Updated documentation

# Info

**Official site:** [https://opsdroid.github.io](https://opsdroid.github.io)

**GitHub repo:** [https://github.com/opsdroid/opsdroi](https://github.com/opsdroid/opsdroid)

**Creator:** [Jacob Tomlinson](https://www.jacobtomlinson.co.uk)