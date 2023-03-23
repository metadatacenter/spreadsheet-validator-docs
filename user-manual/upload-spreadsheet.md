---
title: Upload Spreadsheet
layout: page
nav_order: 1
parent: User Manual
---

# Upload Spreadsheet

Users can upload their spreadsheet file using the input field on the homepage. At the moment, the tool supports two types of input format:
1. Excel spreadsheet (.xlsx)
2. CSV file (.csv)

## Metadata information

Either input format requires a metadata information that will provide the tool's algorithm a context. The table below shows the required metadata fields:

| Field | Description |
| ----------- | ----------- |
| schema:name | Enter the name of the spreadsheet. |
| schema:description | Enter the description of the spreadsheet. |
| schema:description | Enter the description of the spreadsheet. |
| schema:schemaVersion | Enter the version of the spreadsheet. |
| pav:createdOn | Enter the creation date and time (format: YYYY-MM-DD hh:mm). |
| pav:createdBy	| Enter the full name and ORCID (if available) who creates this spreadsheet. |
| pav:derivedFrom | Enter the CEDAR template IRI that contains the validation rules. |

## How to include the metadata information?

* For Excel file format, add a new sheet called `.metadata` and create a table with the metadata fields.

  <img width="862" alt="Metadata information in Excel" src="https://user-images.githubusercontent.com/5062950/227035467-2e137e9a-2360-438d-a1d8-48897b7dd693.png">

* For CSV file format, create a new file called `metadata`, create a table with the metadata fields and place it in a same directory as the CSV file. You will need pack them together in a zip file.

  ![Screen Shot 2023-03-22 at 1 56 20 PM](https://user-images.githubusercontent.com/5062950/227036180-7106e97b-7ee0-4ee7-bc7d-1f2849087cf7.png)
  
## Uploading the file

You can either drag-and-drop the file from your local computer to the input field or use the "Browse" option to select the file from your file system.
