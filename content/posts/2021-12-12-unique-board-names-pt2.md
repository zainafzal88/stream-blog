---
title: "Unique Board Names - Pt.2"
date: 2021-12-12
---

Today, we continued working to ensure we maintained uniqueness of board names. In our previous stream, we realised that DAX is out of our budget, costing approx. 45USD p/m. Due to this, we decided that the way forward would be to scan the DB, retrieve all the board names and check against them in the frontend.

We've made this change to the backend code, but have yet to deploy it. In the upcoming episodes, we plan to merge our changes with the existing backend code, migrate our existing functionality from the old to new AWS account and continue implementing the logic behind board name uniqueness.
