---
title: 'Connect to WebSocket via Client Part 2'
date: 2022-01-23
---

Today we deployed the `default` lambda again to AWS by adding that `handler` to our SAM `template.yaml` so that we could receive a message back to our connected `Websocket` client on the frontend of our application.

On the frontend we added the `onmessage` event handler for the websocket and we wrote the logic for the client to `send` the object `{action: "default"}` to invoke the `$default` route and our `default` lambda handler and receive back a message to the client.
