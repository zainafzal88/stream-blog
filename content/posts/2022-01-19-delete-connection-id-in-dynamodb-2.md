---
title: 'Delete Users ConnectionID in DynamoDB - AWS Websocket Pt.2'
date: 2022-01-19
---

In today's stream, we continued investigating why `WebSocketDisconnectHandlerFunction` wasn't deleting the `connectionID` from dynamoDB once the user disconnects.

We tried to replacing the code in `template.yaml` with example code given by AWS but that didn't work for us either. However, after further investigation, we noticed that we had written the incorrect configuration under the `Depends On` section of `WebsocketDisconnectLambdaPermission:`.

After we corrected this with the correct configuration (replacing `WebsocketDisconnectLambdaPermission` with `WebSocketDisconnectHandlerFunction`), the function began to work as expected; the `connectionID` deletes when the user disconnects.

We can now move on to the next part.
