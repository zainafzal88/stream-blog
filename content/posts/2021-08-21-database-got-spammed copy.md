---
title: "Database Got Spammed"
date: 2021-08-21
---

Today while we were trying to insert the boardName in the database from the frontend after making changes according the new backend design, we found out someone was spamming our database.

This happened because in our API Gateway, we added `Access-Control-Allow-Origin: '*'` which basically means that allow request from any origin endpoint.

We found out that one of our friend played with us for fun.

To prevent this, we changed the `Access-Control-Allow-Origin: '*'` to `Access-Control-Allow-Origin: '[localhost-address]'`, saved the changes
however, it didn't make sense because any user can still spam us using their `localhost`. We stopped our friend from doing that, logged this problem in Jira to come back to it.
When we changed back to `Access-Control-Allow-Origin: '*'`, we started to get CORS issue.