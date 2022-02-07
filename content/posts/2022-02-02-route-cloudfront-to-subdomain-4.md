---
title: 'Re-routing CloudFront distribution to Subdomain Pt.4'
date: 2022-02-02
---

In today's episode, we finally managed to route our CloudFront distribution to our Subdomain (scrumblr.roarcoder.dev).

Thanks to a member in DevCop, who explained that we needed to create a new Hosted Zone in our Roarcoders AWS account and add the generated Nameservers in Zain's personal account.

After we did this, the rest flowed smoothly.

To get this completely working, we actioned the following:
1. Request an SSL certificate for the subdomain in ACM.
2. Add the subdomain under the 'Alternate domain names' setting in CloudFront.
3. Create an `A` record in Route53 pointing to the CloudFront distribution.

Once we did this, we visited the subdomain, and our project appeared! We can finally move on...