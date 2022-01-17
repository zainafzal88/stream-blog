---
title: 'Delete User's ConnectionID in DynamoDB - AWS Websocket'
date: 2022-01-17
---

After, inserting the `connectionID` in DynamoDB to indicate when a user connects, the next step is to delete this `connectionID` when the user disconnects. However, the ` WebSocketDisconnectHandlerFunction` isn't functioning as expected.

Today, we attempted to investigate why this is, by looking through the code and AWS console. We even tried a couple of methods that we thought might work, such as: changing the order of the code and re-naming keywords; yet, the functionality refused to work.

We will continue working on this in the upcoming streams.

