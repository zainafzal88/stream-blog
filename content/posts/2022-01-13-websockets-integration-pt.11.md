---
title: 'Integrating AWS WebSockets part 11'
date: 2022-01-13
---

The RoadCoders were back today working with AWS API Gateway, Websockets, and DynamoDB.

For today, we first decided to move on from a problem we are currently experiencing with the `$default` route and `lambda`. It's sending back two messages. We'll be circling back to this problem later.

We moved on to configuring our DynamoDB `WSConnection` table by updating our SAM `template.yaml`. We also rewrote the `onconnect` lambda handler to add the clients `connectionId` from the `event.requestContext` object to the `WSConnection` DynamoDB table to keep track of clients that are connected to the API Gateway WebSocket. We'll use those connectionIds so we can broadcast messages/data to connected clients in another lambda function we will write in the near future.
