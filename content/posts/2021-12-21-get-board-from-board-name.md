---
title: "Get Board from BoardName"
date: 2021-12-21
---

Today, we started off by checking the unique board name functionality that we recently implemented in the frontend. This worked as expected, displaying an error message when the user attempts to enter a `boardName` that already exists.

After ensuring this works, we moved on to the backend API code where we began to implement the get board from `boardName` functionality. Essentially, we need this functionality to populate the board in the frontend with its respective notes and attributes.

We got about halfway with functionality, implementing the request and string validation. In the upcoming stream, we will implement the other half, which involves actually retrieving the board from the DB. 