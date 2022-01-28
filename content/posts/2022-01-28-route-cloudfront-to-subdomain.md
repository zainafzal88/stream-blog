---
title: 'Re-routing CloudFront distribution to Subdomain'
date: 2022-01-28
---

In today's episode, we attempted to re-route the CloudFront distribution to our subdomain (scrumblr.roarcoder.dev).

Initially, we tried to do this by creating an `A` record in Route53 and populating it with our CloudFront distribution URL. However, this failed to work.

After some research, we discovered that we needed a SSL certificate for our newly created subdomain. To organise this, we requested multiple certificates via AWS Certificate Manager (ACM) and created CNAME records to reflect this in Route53. However, this failed to work as well.

We came to an understanding that perhaps this is because the domain is already tied up with another AWS account. We're not certain, but this appears to be the case.

We will continue to investigate this offline and work towards a solution in the upcoming streams.

