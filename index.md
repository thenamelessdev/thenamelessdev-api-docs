---
permalink: /
title: API docs
---
# [thenamelessdev.com](https://thenamelessdev.com) API docs
**Welcome to the API docs! You will find everything you need to know about thenamelessdev.com api endpoints**
### Basics
To make your API key you have to go to https://thenamelessdev.com/users/dashboard/api after logging it with either Discord or GitHub.
**Fun Fact:** the letters before the . is your username in Base64. It can help you identify leaked API keys.
### API reference
Main URL: https://thenamelessdev.com/api/VERSION
Versions:
- v1
### Authing
For the "authed" endpoints you will need a auth in your header or a logged in session
**Example auth header:** {"auth":"YOUR_API_KEY"}
For "unauthed endpoints you will not need any headers.
### Errors:
- 401: missing or invalid api key
### Endpoints:
- [authed](/authed)
- unauthed (docs coming soon)
