---
title: 'Adding CloudFront CDN, Route 53, and S3 for scrumbler client'
date: 2022-01-27
---

In this episode we added and configured AWS `CloudFront`, the CDN, to host the client files from the `S3` bucket we previously set up. Since the website is public facing attached the appropriate readonly `S3` bucket policy holding our files like so:

```JSON
{
    "Version": "2012-10-17",
    "Statement": [
        {
            "Sid": "PublicReadGetObject",
            "Effect": "Allow",
            "Principal": "*",
            "Action": [
                "s3:GetObject"
            ],
            "Resource": [
                "arn:aws:s3:::Bucket-Name/*"
            ]
        }
    ]
}
```

This allows read access so that vistors and CloudFront can view the site.

In `CloudFront` we updated the configuration to allow `anonymous (public) access` and updated the `Origin Domain` in CloudFront to point at our website hosted in `S3` at the `S3 Website Endpoint` and not at the `S3 Rest Endpoint`.

Example of a website endpoint from S3 for the `Origin Domain` in CloudFront:

`DOC-EXAMPLE-BUCKET.s3-website-region.amazonaws.com`
