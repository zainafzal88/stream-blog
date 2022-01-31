---
title: 'Re-routing CloudFront distribution to Subdomain Pt.2'
date: 2022-01-31
---

Today, Zain couldn't make it to the stream as he had something come up. So, Torey jumped on in-place of him.

We started off the episode by looking through the Route53 configuration to see if we had any other approaches to solving our problem from last time. However, after reviewing the config across multiple services (ACM, Route53 and CloudFront), we concluded that the issue is with the domain provider itself. Hence, we decided that we'll have to talk with Zain about this offline.

After this, we moved on to discussing our websocket integration. We realised that we will need to extend our original implementation to include the connection and propagation of messages across multiple users.

We started to think about how we could implement this but didn't get too far due to time. We shall come back to this and more in the upcoming streams.