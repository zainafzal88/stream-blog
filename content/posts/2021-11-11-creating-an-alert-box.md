---
title: "Created an alert box to confirm when notes have saved"
date: 2021-11-11
---

Today, we started by briefly discussing `toast.js` and how we can go about creating an alert box for when the user clicks 'save'. We determined that the best way forward was to create an alert box from scratch, instead of importing Bootstrap; as we would just be using it for a single component.

As such, we decided to copy the `toast.js` alert box layout from w3schools by using inspect element on Chrome. Although seemingly simple, we ran into some hurdles with `CSS` and utilizing the right `HTML` classes. Once we got the layout in order, we added the `closeAlert` function in `script.js` and assigned this to the close button on the alert box. This worked seamlessly.

Moving forward, we need to ensure that the right messages are displayed on this alert.