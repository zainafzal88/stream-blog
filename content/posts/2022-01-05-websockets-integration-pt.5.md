---
title: "Integrating AWS WebSockets part 5"
date: 2022-01-05
---

Today we continued to work on trying to get response from lambda when it's triggered by API Gateway & WebSocket API. 

We faced `Forbidden` error when triggering lambda however, we found out that the lambda function wasn't even deployed. So, we deleted the stack, re-created it, built, and deployed. To our surprise, we didn't get the same error hwoever, got `Internal Server Error` this time which means we are one step closer to the solution. 

Upon researching, we found out that something is missing in API Gateway. Then we ran out of time.

Join us tomorrow in the journey of solving it.