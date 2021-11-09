---
title: "Insert All Notes in Database using Dynamic Board Id"
date: 2021-11-09
---

Today, we began the stream by testing our solution to inserting multiple notes into the DB. It wasn't working initially, but we quickly realised that it was due to a simple mistake being made when referencing the `entry` variable.

Once we fixed that, we began thinking about how we could call our `postNote` function using a dynamic `boardId`. We decided that the most efficient solution forward would be to utilize the `localStorage` functionality. Similar to what we did for `boardName`, we stored `boardId` in `localStorage` and passed this value into `postNote`. This solution worked well in Safari but not in Chrome.

Going forward, we need to investigate why the solution wasn't working in Chrome and implement a `GET` method in the backend so that we can retrieve `boardId` from `boardName`.