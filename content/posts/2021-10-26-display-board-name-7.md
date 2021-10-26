---
title: "Display Board Name With Dynamic BoardId Pt.2"
date: 2021-10-26
---

Today, we attempted to store and pass the `boardSessionId` from `still-frontend.js` to `index.html`. After several attempts, we noticed that the value wasn't being passed on as it wasn't being stored in the session.

After some discussion, we thought it might be a good idea to have the `boardSessionId` stored in `localStorage` after it is returned from `postBoardName`. However, there were drawbacks to this approach; namely, the case when the user attempts to access the board directly from a link (e.g. scrumblr.ca/demo1).

As such, we determined that the ideal solution, given time constraints, is to amend the backend api and create a method which retrieves the board based on `boardName`. This way we can call the `GET` request in `index.html` and interact with the returned object directly. This is how we plan to move forward, especially to ensure we are working within our timeline.
