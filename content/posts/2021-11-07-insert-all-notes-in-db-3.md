---
title: "Insert All Notes in Database Pt.3"
date: 2021-11-07
---

Today, we began the stream with a `CORS` error (again). However, after a quick re-deployment we were able to get back on the right track.

From here, we successfully managed to insert a hardcoded note into the database (again). Although this works well, we noticed that too many notes were being pushed into the local array. This is because a new note object is being added everytime a change occurred to the card. 

Going forward, we plan to add the note only after the user has clicked outside the card; whilst ensuring that the array holds only a distinct set of notes. This will significantly reduce the number of notes in the array; whilst pushing only the required data to the backend.