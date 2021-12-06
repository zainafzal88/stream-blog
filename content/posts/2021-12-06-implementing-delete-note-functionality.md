---
title: "Implementing Delete Note Functionality"
date: 2021-12-06
---

Today, we started off the stream by fixing the `patchNote` functionality. To fix this, we commented out some validation code from the backend so that `cardId` can be checked against what's stored in the db. Although this fixed our issue, we have to ensure we add validation in the future.

After we had that working, we moved on to implementing `deleteNote` functionality. This involved creating a new function to remove the note from the hashmap and delete it from the database. However, upon testing the function, we received a `404` response; indicating that the deletion was not successful. We'll have to continue working on this on the next stream.

