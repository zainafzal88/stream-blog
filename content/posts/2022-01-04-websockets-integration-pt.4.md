---
title: 'Integrating AWS WebSockets Part 4'
date: 2022-01-04
---

Today we, the very determined Roar Coders, continued working on the AWS API Gateway and the Websockets APIs. 

We were able to successfully establish the connection to the WebSocket with the `wscat` terminal app and trigger the `onconnect` lambda successfully. 

Victory! Or did we speak too soon? 

Confidence high, we moved on and attempted to send a test message back to our `wscat` terminal client. 

Sending a message in our connected `wscat` terminal we posted `{"action": "default"}` to trigger our `default` lambda that would use the `AWS.ApiGatewayManagementApi` constructor and `postToConnection` method to send back a generic message to our terminal. 

Victory not!! 

We encountered a dreadful `403` forbidden error: 😱! Upon investigation, we surmised that the error must lie somewhere in the bowels of the `template.yaml`. 

To be continued...
