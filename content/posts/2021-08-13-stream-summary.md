---
title: Github Bug + Post Note + Updated Jira
date: 2021-08-13
---

Today, while testing the functionality of notes being create when "+" is clicked, we found out that Github "working" commit was overriden by a "non-working" code due to merging branches.

We, applied a quick fix for it and continued however, proper fix will be applied. Then, we started to implement posting the note text to the backend from the middleware.

Whilst doing that, we found out that another snipped of code has been overriden as well. We will fix this overriden issues by limiting who has access to `main` branch.

During all these times, we made sure we updated Jira with all the issues we noticed so that we don't forget they exists.