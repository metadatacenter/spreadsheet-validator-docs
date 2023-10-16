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
3. Value is not a URL (e.g., google*com, google.co)
4. Value is not in a valid format.

Selecting one of the error type options on the navigation bar takes you to the worksheet page where you can perform the needed fix.

<img width="500" alt="repair-adherence-errors-menu" src="https://github.com/metadatacenter/spreadsheet-validator-docs/assets/5062950/e7edab87-b9eb-402a-9282-2b5a207a0233">



## Repair Worksheet

The repair worksheet includes the following key features:

<img width="1552" alt="repair-adherence-errors-worksheet" src="https://github.com/metadatacenter/spreadsheet-validator-docs/assets/5062950/dc4f8f75-9146-4f0b-817b-c402da658ecf">

- (A) "Original Value" = Displays the original value of a particular column in the spreadsheet. At the bottom of the value string, in parentheses, is the number of cells that contain the same string. Next to the value is a "down arrow" button that can show the original spreadsheet to provide some context.
- (B) "New Value Field" = Enter the correct value in this field to replace the original value. This field usually contains a value that was entered automatically by the tool as part of its recommendation feature.
- (C) "Accept Checkbox" = Select the checkbox if you agree with the recommended value. If you agree to **all** the recommended values then select the checkbox in the column header.
- (D) "Save" and "Save and Repair Next" = The first button saves changes without leaving the page. The second button saves the changes and advances you to the next error problem.
- (E) "Page Limit" = Select a number of rows to display per worksheet page.

### Repair invalid URL

Follow these steps to repair invalid URL:

<img width="1450" alt="repair-invalid-url" src="https://github.com/metadatacenter/spreadsheet-validator-docs/assets/5062950/81dba857-f2e9-4667-851c-237cf5047bd9">

1. Fill out the "New Value Field" with the correct URL, or copy the previous value by clicking the "Original Value" and paste it onto the "New Value Field" for further correction. A URL string must start with either "http://" or "https://" prefix.
2. The validator will automatically check the validity of the input string.
3. If it is a valid URL string, the validator will show a checkmark icon that you can click to check the webpage.

### Repair invalid format

Follow these steps to repair invalid format:

<img width="1410" alt="repair-invalid-format" src="https://github.com/metadatacenter/spreadsheet-validator-docs/assets/5062950/0ecab1da-5d0d-48af-9e99-ef13dd4f5608">

1. Fill out the "New Value Field" with the correct string, or copy the previous value by clicking the "Original Value" and paste it onto the "New Value Field" for further correction. Use the field description (by hovering on the question mark (?) icon), or use the example value (by hovering on the information (i) icon) to get some hints the expected string format.
2. The validator will automatically check the validity of the input string.
3. If it is a valid string, the validator will show a checkmark icon.
