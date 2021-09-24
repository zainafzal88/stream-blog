---
title: "Validation for Updating Notes and Update Jira"
date: 2021-09-24
---

Today we implemented validation for updating (`PATCH` method) notes in the backend.

We covered the below scenarios:

1. BoardId and NoteId must be alphanumeric
2. Topic for note must not be empty
3. Topic must be a `string`

We also had a bit of a glitch streaming to Twitch however, we resolved it very efficiently.

We are also keeping Jira udpated every day and it's helping us keep on track.