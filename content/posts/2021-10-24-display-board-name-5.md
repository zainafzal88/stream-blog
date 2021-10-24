---
title: "Displayed Board Name"
date: 2021-10-24
---

Today, Kartik couldn't make it as he was busy in his assignment. Zain and I managed to display the board name by utilizing an async/await function to retrieve the `promise` value returned by the `getBoardById` method.

After we moved this functionality into the `still-frontend.js` file, we attempted to dynamically retrieve the `boardId` so that we can print out board name without relying on local storage. However, we realised that the backend api hasn't been setup to return the `boardId` given a `boardName`. Due to this, we plan to figure out an alternative way on getting this value.
