---
title: "Integrating AWS WebSockets part 6"
date: 2022-01-06
---

Today, we worked on the same problem, checking why is API Gatway erroring out.

We found out that Lambda had to be used as a proxy integration.

So we enabled that option in the `route` name `default`, deployed and tested. It still didn't work. 

We are one step closer to finding out the solution.