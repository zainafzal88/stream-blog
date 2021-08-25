---
title: "Implement New Design For Backend"
date: 2021-08-20
---

Today we changed our backend `POST` request to return the created board's Id. 

We did this as all our methods in Express app are taking in the Id's, we wanted to hit the database once only and fully utilize the connection.

As Sam Nolan suggested us to create the board and return the `Id` in the response so that we can use the `Id` from the response in other methods
in other methods.

Then we tested the Express App with Postman and it worked as intended.
