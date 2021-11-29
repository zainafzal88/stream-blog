---
title: "Post Note Id to DB"
date: 2021-11-29
---

In our last episode, we noticed that the `noteID` wasn't being pushed to the DB along with the note value. As such, today, we worked on getting the `noteID` inserted as we will need to reference this when updating, deleting and getting notes from the DB.

To do this, we amended the `postNote` function to post the frontend `cardID` and changed the backend code to accept this request. This worked well, so we moved on with the aim of implementing the update note functionality. However, upon trying this, we noticed that notes are being duplicated in the DB rather than being updated with the changed data. This is something we will have to come back to and resolve in the upcoming episodes.

Finally, in the final few minutes, Torey Littlefield joined us to talk about his interesting practice interview story. He has an interview upcoming and is planning to join us on the stream tomorrow evening to work on a React App which will aid in his preparation.