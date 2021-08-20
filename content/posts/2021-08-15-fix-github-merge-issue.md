---
title: GitHub Merge Issue
date: 2021-08-15
---

**Issue:** 

A commit was done on 29 July 2021 in the `main` branch directly instead of the `dev` branch. When committing new changes on `dev`, we forgot to make sure that `dev` is in sync with `main` and kept on merging to the `main` every day which override the changes in the commit 29 July 2021. After a few commits we realised that the change from the 29 July 2021 wasn't working which is when we found that the code for the fix wasn't in our latest repository

**Solution**: 

In order to fix the above, we decided that we will compare the 29 July 2021 commit from the `master` branch to the `dev` branch's latest commit and merge the differences.

We learnt of a new tool got **GitLens** to help us search and compare commits. However, we didn't know how to actually merge the differences. That's something we need to learn. To just check if what we are trying to do will even work, we copied and pasted the code from the that commited file from `main` branch to our file in `dev` and found that the functionality still didn't work.

I thought it would be to do with the cache and tried clearing that out too but it didn't give us any joy.

So, the journey of fixing continue tomorrow



