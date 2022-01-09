---
title: 'Integrating AWS WebSockets part 8'
date: 2022-01-07
---

Today more AWS API Gateway Websockets. A few silly "oopsies" live streaming with private credentials were had, and that's the hazard of live streaming and screen sharing. Eventually, we did get down to real business debugging our API Gateway Websockets and our SAM `template.yaml`.

It was frustrating, but thankfully a very helpful viewer pointed out an extremely small detail in the `yaml` on our ` TestRoute:` API Gateway Route. `RouteKey` was set to `default` when it should have been `$default`. So we were simply missing a `$` in our string. This fixed the error and we were finally able to get back a response to our `WebSocket` client after connecting.

Thanks to our special viewer for pointing out that same typo! Kebabs 🥙 were awarded to the viewer for saving us! We could finally move on!
