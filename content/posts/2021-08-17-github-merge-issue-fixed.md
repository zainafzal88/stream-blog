---
title: GitHub Merge Issue Fixed
date: 2021-08-17
---

**Issue** 

`dev` branch is in sync with the `main` however, board name wasn't being inserted in DynamoDB.

**Solution Progress**

Today, we managed to find out why the board name wasn't posting when `go` button was pressed in Fetch API. The reason was because when the post request was initiated, it wasn't waiting for the request status to come back from backend as `200` (`OK`). It skipped that step and continued to the page where the actual board is.

We added a validation on the `go` button to only go to the next page (where the actual board is) when the response status is recieved as `200`. Consequently, it worked. We also tested if the notes were being created in the UI and they were. 

Then we tried to merge `dev` into `main` and recieved frew conflicts, resolved them, commmited the changes and pushed them. Now `main` and `dev` branch are in sync with expected functionality.