---
title: API Status Code + Fix Merge Issue + Updated Jira
date: 2021-08-14
---

Today, we set response status code `200` for successful `GET` request in the Express app and also applied validation to the middleware to display all the boards only if the status code returned in the response is `200`. If not, then display a meaningful error.

We also fixed most of the issues from merging the branches yesterday. Will continue to finish the rest tomorrow.

Last but not the least, we are keeping Jira udpated.