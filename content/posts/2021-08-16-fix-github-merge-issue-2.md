---
title: GitHub Merge Issue Part 2
date: 2021-08-16
---

**Issue:** 

A commit was done on 29 July 2021 in the `main` branch directly instead of the `dev` branch. When committing new changes on `dev`, we forgot to make sure that `dev` is in sync with `main` and kept on merging to the `main` every day which override the changes in the commit 29 July 2021. After a few commits we realised that the change from the 29 July 2021 wasn't working which is when we found that the code for the fix wasn't in our latest repository

**Solution Progress**: 

We finally manage to sync the content of `main` and `dev`. We thought everything is working fine now and ready to merge to `main`. Then, we thought we haven't tested one functionality, posting board name to insert in DyanmoDB. When we started to test that functionality, we discovered that board name wasn't being inserted in DynamoDB. We tried to debug it as we thought it might be the `CORS` error again however it didn't show us any error in the frontend. We decided to continue tomorrow on this issue.



