---
title: "Merge Day"
date: 2021-10-03
---

Today, we merged `stable-backend` to `dev` branch.

We faced few conflicts that had to be manually resolved. After resolving, we tried to deploy the SAM application to Cloud Formation. It failed as VPC resources were failing to be created.

We researched and found out that we shouldn't create VPC resources every time we deploy the application (it was alrady created before). Knowing that, we commented out the VPC resources in `template.yaml`. This time it deployed successfully.

We still need to connect the existing VPC to Lambda through AWS Console.