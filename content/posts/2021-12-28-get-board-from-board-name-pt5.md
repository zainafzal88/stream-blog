---
title: "Get Board from BoardName Pt.5"
date: 2021-12-28
---

Today, we manage to bring all the properties in the board's object. 

We were missing `NonKeyAttributes` which includes any non-HASH or GSI column of the table. We included the `board_notes` and set the `ProjectionType` to `INCLUDE` in the `template.yaml` Once we added that it worked like a charm.

Next task is to integrate websocket in the application as we want multiple users to interact with the board simultaneously. For this we will be using WebSocket API from AWS APIGateway. 

As we haven't used it before, we began to learn about it and found out that it's used for bi-directional communication between the client and the server unlike REST API with handles communication synchronously. We will be continuing to learn more about it tomorrow.