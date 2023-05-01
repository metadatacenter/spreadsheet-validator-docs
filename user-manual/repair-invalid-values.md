---
title: Repair Invalid Values
layout: page
nav_order: 4
parent: User Manual
---

# Repair Invalid Values

When a spreadsheet cell contains a value which doesn't follow the input schema rules, this produces an "invalid value" error. This type of error falls under the broader category of adherence errors, which includes 3 sub-types:
1. Value is not a standard term. In other words, it doesn't match the permissible values.
2. Value is not a number (e.g., `12oz`, `5"`, `$12,000`: value includes a symbol, unit, or abbreviation as well as the numerical value.)
3. Value is not a string.

Selecting one of the error type options on the "App Bar" takes you to the worksheet page where you can perform the needed fix.

<img width="500" alt="Repair Adherence Errors Menu" src="https://user-images.githubusercontent.com/5062950/227059149-6d235034-d049-4fdc-b91e-3bae1a748c88.png">


## Repair Worksheet

The repair worksheet includes the following key features:

<img width="1560" alt="Repair Adherence Error Worksheet" src="https://user-images.githubusercontent.com/5062950/227059545-ca99808d-0ced-43ff-8053-42424091bbe0.png">

- (A) "Original Value" = Displays the original value of a particular column in the spreadsheet. Next to the value string, in parentheses, is the number of cells that contain the same string.
- (B) "New Value Field" = Enter the correct value in this field to replace the original value. This field usually contains a value that was entered automatically by the tool as part of its recommendation feature.
- (C) "Accept Checkbox" = Select the checkbox if you agree with the recommended value. If you agree to **all** the recommended values then select the checkbox in the column header.
- (D) "Save" and "Save and Repair Next" = The first button saves changes without leaving the page. The second button saves the changes and advances you to the next error problem.
- (E) "Page Limit" = Select a number of rows to display per worksheet page.
