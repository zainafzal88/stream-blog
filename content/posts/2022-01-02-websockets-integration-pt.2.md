---
title: "Integrating AWS WebSockets"
date: 2022-01-02
---

Today we continued to research the `502` error and found out the error was coming from lambda and the actual error was `410`. Turns out that the reason was we were sending response to the client while connecting to the websocket. We commented out the sending response part and it connected succesfully.

