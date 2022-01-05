---
title: "Integrating AWS WebSockets part 1"
date: 2021-12-30
---

Today, we tested if we can connect to the websocket using `npm` package `WebSocket cat` aka `wscat`. It's a tool that lets you connect and communicate with the websocket server.

After the testing 1st time. it gave us `500` error which basically means `Internal Server error`. We enabled cloudwatch logs for the api and tracked the error down and fixed it by ticking the option of enabling Lambda Proxy Integration. It worked but now it was giving `502`. I believe we are very close of getting it working.