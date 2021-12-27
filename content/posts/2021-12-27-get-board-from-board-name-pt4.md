---
title: "Get Board from BoardName Pt.4"
date: 2021-12-27
---

Today, we completed the implementation of Global Secondary Index (GSI). 

The problem was that we weren't including the `AttributeName` of `BoardName` in the main table and setting the `KeyType` as `S` whereas it should've been `HASH`. After those minor changes, we managed to get the GSI working deloyed successfully.

Then, we referenced the index in the `params` of `getBoardByName()` to work with the board name without needing to boardId. Consequently, it worked and we were getting the board object. However `board_notes` column wasn't coming. We think we are one step closer to the actual solution and will be coming back for it tomorrow.