---
title: '$disconnect route in AWS API Gateway Websockets & Lambda'
date: 2022-01-16
---

Today we worked with the AWS SAM `template.yaml` by adding a `DisconnectRoute` and `WebSocketDisconnectHandlerFunction` with permissions to trigger the lambda when the client disconnects from the websocket. We updated the `ondisconnect` lambda to remove the `connectionId` from the DynamoDB table where we are storing the connected clients.

We deployed the SAM build and changes however CloudWatch logs did not indicate that the `ondisconnect` lambda was being trigger when we tested with PieSocket. We tried to troubleshoot our CloudFormation stack and SAM template but we had to save it for another day.
