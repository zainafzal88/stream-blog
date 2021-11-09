---
title: "Insert All Notes in Database Done"
date: 2021-11-08
---

Today, we had to insert multiple notes created in the database on a click of a `save` button.

We managed to do that by storing the created notes as objects in an array called `textForNotes` and then when the `save` button is clicked, we used a `forEach()` to loop through each of the note `textForNotes` array and inserted only the text value in each note to the database.

That worked! However, it was inserting the notes as many times as we clicked the save button. This wasn't good because we didn't want to insert the notes that were already inserted in the database.

We implemented a solution to this by creating a property in the notes object called `status` and gave a value of `Not Inserted` or `Inserted`. If the note hasn't been inserted in the database, it will have the status, `Not Inserted`, otherwise, `Inserted`. This solution seems to have worked