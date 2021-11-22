---
title: "Displaying Confirmation only when status is 200"
date: 2021-11-22
---

Today was our first stream after a one week break. Due to personal reasons, Zain won't be joining us for one month, and as such Kartik and I will be progressing the stream in spite of his presence. We plan to continue streaming on Monday, Tuesday and Thursday for the time being.

In today's stream, we worked on returning the status from `postNotes` and checking this before displaying the confirmation message. To do this, we simply created a function called `openAlert` which we called inside `updateArray` everytime a `200` status is received. This worked successfully, so we applied the same logic to ensure that the notes are tagged with the approriate status message as well.
