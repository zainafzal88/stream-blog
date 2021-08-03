---
title: Get BoardName from frontend as JSON object to backend
date: 2021-08-03
---

Today we worked on sending the board name as JSON object from frontend using Fetch API as middleware to the backend securely and following the development standards.

**Things we tried**:

`JSON.stringify` the object from the Fetch API while sending it which meant the object was a string while we were passing it to the backend.

**What worked** <br>
We got to know that it won't let us access the `BoardName` in the object as it was being sent as a string

**What didn't work:** <br>
We got a `502 bad gateway` error, which meant that the sent data and received data type didn't match. It made sense as the body expected an object and we sent a `JSON` stringified string

**Things we tried**:

Directly creating the JSON object in the body through FETCH POST request.

This wasn't the breakthrough for us as it pretty much meant the same thing rather than assigning the data into a variable sending it directly in the body.

**What happened** : This caused `502 Bad Gateway` error.

**What didn't work** : The error persisted as it didn't make any difference as to the content which was being sent by the FETCH POST request. It was the same thing sending it using or not using a variable

**Things we tried:**:
Console logging every piece of data we received from the Post request

This was a major turnout for today as it made us realise the body was recieving data as we got an array of numbers which had a type of buffer. This meant that we were on the right track of resolving our data to the `BoardName`. 

**What worked:** <br>
Console.logs were successful in telling us the types and the data received. The error was resolved though the `BoardName` was assigned garbage value

**What didn't work:**  Though the error was resolved and we were able to access the BoardName attribute in the database, we still have some work to do to revolve the object from the POST request