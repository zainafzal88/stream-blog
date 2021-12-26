---
title: "Get Board from BoardName Pt.3"
date: 2021-12-26
---

Today, we continued working on the `getBoardByName` functionality.

However, while the implementation of this method is complete, it isn't functional. This is because, by default dynamodb only accepts `boardId` as the primary index when fetching data, meaning that it doesn't accept the `boardName` being passed by our function.

To resolve this, we began implementing a Global Secondary Index (GSI) to be used on dynamodb which would allow us to retrieve data using the `boardName` instead. In order to do this, we amended the `template.yaml` file, adding the required components to the configuration as outlined in the AWS documentation. 

However, whenever we attempted to deploy the code, it would result in an error. Despite this, we are really close to having this working and will come back to it in the upcoming stream.