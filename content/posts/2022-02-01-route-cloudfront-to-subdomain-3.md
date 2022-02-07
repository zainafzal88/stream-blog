---
title: 'Re-routing CloudFront distribution to Subdomain Pt.3'
date: 2022-02-01
---

Today, we kept on working on generating `SSL` certificate through AWS Certificate Manager in order to make scrumblr live on `HTTPS` protocol.

We tried to change `NS` record to be the same as in the NameCheap, however, that didn't work. We then made sure the `SOA` record was a proper one. It wasn't so, we changed that too. We ran out of time to test it. 

We'll see if it's worked tomorrow and are one step closer to our outcome.

