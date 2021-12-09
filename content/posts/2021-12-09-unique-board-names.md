---
title: "Unique Board Names"
date: 2021-12-09
---

Today I (Zain) came back.

We want to make sure there are no duplicate boards inserted in the database. Therefore, thought of storing all the board names in server cache but that woudn't work as our server is stateless, it would run, do the work and stop (die). Which means when it dies cache is gone as well.

Then we thought of using cache service of DynamoDB known as DAX. It would be faster, easier to use however, it wasn't cheap. We used a Simple Calculater from AWS to calculate the cost and it was costing 45USD montly minimum.

We will come back to this tomorrow.
