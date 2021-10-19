---
title: "Display Board Name - 2"
date: 2021-10-19
---

Today, Kartik couldn't make it as he was busy in his assignment. I and Thanesh managed to get one step closer to our main goal which is to display a board name from the database.

We worked on the error in which the url was getting recognised as the localhost instead of the api endpoint. We noticed that url was declared as a member variable which was the cause of the problem. As soon as we set url to be as a member variable, it worked.

Next step is to get the board name appearing as a heading just above the board.