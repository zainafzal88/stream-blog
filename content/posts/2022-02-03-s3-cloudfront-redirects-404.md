---
title: 'S3 and CloudFront Redirects 404'
date: 2022-02-03
---

In today's episode, we recapped the approach to routing our CloudFront distribution to our Subdomain (scrumblr.roarcoder.dev).

Next, we proceeded to testing the functionality of creating a board and having another different client join that board. When we did that, we received a `404` "NoSuchKey" error from `Amazon S3`.

We discussed the potential causes and solutions for why this error occured but it was clear the client was not being directed to the `index.html` where the board should appear so we looked into solutions for `S3` and `CloudFront` redirects.
