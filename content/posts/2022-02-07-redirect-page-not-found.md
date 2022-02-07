---
title: 'Redirecting Page Not Found to index.html'
date: 2022-02-07
---

At the moment, when someone attempts to access a board via a link (e.g. https://scrumblr.roarcoder.dev/example), a `404` page will appear.

This makes sense as they are attempting to access a file that isn't there.

So in today's episode, we attempted to find a solution to fix this issue. Firstly, we added a condition in AWS that re-directs errors to `index.html`. This is a straightforward solution that works as expected.

However, this only loads the `index.html` page without any of the contents associated with the board. To make this into a complete solution, we need to some frontend logic that retrieves board details upon loading the page.

We started writing up a solution that involves determining which page the user has come from by using `window.location.pathname`. Right now, if the user comes from `home.html` it will retrieve the `boardName` from `localstorage`, otherwise it will refer to `location.pathname`.

We will continue expanding on this logic in the upcoming episodes.