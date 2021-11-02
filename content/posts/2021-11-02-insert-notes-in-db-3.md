---
title: "Insert Note In Database From Frontend Pt.3"
date: 2021-11-02
---

After fixing the `CORS` issue yesterday, our task today was to insert a single note into the database. 

In the beginning, we attempted to insert the note from the `sendAction` function but this resulted in a `502` error as the database doesn't accept empty strings. From this, we realised that the best step forward was to create a seperate function to handle this functionality.

As such, we created a function called `addTextToArray` which adds a note to a global array containing all the notes on the board. Using the function, we managed to post one note to the backend via the `onCardChange` method. The plan going forward is to have all notes stored in this array and pushed to the database under one operation.