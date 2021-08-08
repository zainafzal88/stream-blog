---
title: Unexpected Turn To The Session
date: 2021-08-08
---

Today, my co-host Kartik wasn't able to join me as he had an exam and was busy in that. So I continued myself.

The plan was to start implementing `getBoardName` method in the middleware. So I created a new branch in the repository to work on this functionality. When I was testing the posting of the board name just to be sure, I realised that it wasn't posting to the database and was given `CORS` related error again. However, when I posted using Postman, it was working. That clearly indicated that there is something wrong in the `POST` request of Fetch API.

Seeing that, I had to backtrack and spend the entire session in fixing the `CORS` issue again.