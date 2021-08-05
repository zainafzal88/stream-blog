---
title: Get BoardName from frontend as JSON object to backend
date: 2021-08-03
---

Today we worked on sending the board name as JSON object from frontend using Fetch API as middleware to the backend securely and following the development standards.

**Things we tried**:

Used `Postman` to test if the problem was in the `Express API` or the Middleware FETCH API

**What worked** <br>
We realised that the Express API was functional in an ideal state and the actual problem lied behind how we handled the data parsing through the FETCH APIs
**What didn't work:** <br>
The `FETCH API` was throwing an error in the sense that the data revcieved was still not in a JSON format so that the `BoardName` could be fetched out of the object easily

**Things we tried**:

Changing the reponse type in the FETCH API to return the `response.json()` function. What this ideally meant was this should return the object.
**What happened** : This resolved all the previous errors but the data recieved was still not parsed properly when sent

**What didn't work** : 
This approach really opened some incites on how `FETCH APIs` work when returning a respone object. We still got a garbage data value for our object when recieved in the `API` and inserted in the `Dynamodb` Database
