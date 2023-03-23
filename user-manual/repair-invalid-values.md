---
title: Repair Invalid Values
layout: page
nav_order: 4
parent: User Manual
---

# Repair Invalid Values

When a cell contains a value in the spreadsheet but it doesn't according to the input schema rules then this type of mistake leads to the "invalid value" error. This error is under a broader adherence error category and it has 3 sub-types:
1. Value is not a standard term. In other words, it doesn't match up to the permissible values.
2. Value is not a number (e.g., `12oz`, `5"`, `$12,000`)
3. Value is not a string.

Selecting one of the error type on the "App Bar" will direct you to the worksheet page where you can perform the fix.

<img width="500" alt="Repair Adherence Errors Menu" src="https://user-images.githubusercontent.com/5062950/227059149-6d235034-d049-4fdc-b91e-3bae1a748c88.png">


## Repair Worksheet

The UI components for the repair worksheet are as follow:

<img width="1560" alt="Repair Adherence Error Worksheet" src="https://user-images.githubusercontent.com/5062950/227059545-ca99808d-0ced-43ff-8053-42424091bbe0.png">

- (A) "Original Value" = It displays the original value of a particular column in the spreadsheet. Next to the value string, in parantheses, is the number of cells that contain the same string.
- (B) "New Value Field" = Enter the correct value in this field to replace the original value. This field will usually contain a value that was entered automatically by the tool as part of its recommendation feature.
- (C) "Accept Checkbox" = Select the checkbox if you agree with the recommended value. If you agree to **all** the recommended values then select the checkbox at the column header.
- (D) "Save" and "Save and Repair Next" = The first button is to save changes without leaving the page. The second button serves as a shortcut button where it will save the changes and go to the next error problem.
- (E) "Page Limit" = Select a number of rows to display per worksheet page.
