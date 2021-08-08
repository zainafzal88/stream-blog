---
title: Get a specific board from DynamoDB using Express Application
date: 2021-08-08
---

Today, we worked on next functionality which was to get a specific board from DynamoDB by board name.

For this to work, Express app's `GET` request for getting a specific board had to be updated from taking a `boardId` to `BoardName`. We updated the code. When we tested it first time by deploying it to Cloud Formation, it didn't work and neither Lambda showed us any error in CloudWatch logs. We then decided to to test it locally by using DynamoDB locally and found out the Key Condition didn't have any condition applied on it. 

Then, we changed from using `get` method of `DocumentClient` to `query` method to get a specific board and updated from Key to use `KeyConditionExpression`. That seemed to have worked locally. Subsequently, we decided that we will deploy on Cloud Formation and test it. This time it worked.