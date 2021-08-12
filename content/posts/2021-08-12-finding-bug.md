---
title: Finding a bug + Updating Jira + Update Delete Controller
date: 2021-08-12
---
Today we started with updating the delete board controller in the backend.
This meant that the middleware would be able to delete a board from the database just by passing the name to the delete board controller.

This was a design alteration which we made to our current API delete controller.

Next we moved on to check if everything was working fine in the middleware FETCH API.
After uncommenting all the important bits and integrating bits of the middlware, we found that we need to implement a validation for the API.

The API needs to respond with a response code about successful or unsuccessful completion of the request to the middlware.

This turned out to be concernning as the request was terminated as the next page was being displayed before the request could be penetrated.

We also updated our Jira board with the bug and the new feature we implemented

Tune in tomorrow to find out how we resolved this.

Thanks,
RoarCoders