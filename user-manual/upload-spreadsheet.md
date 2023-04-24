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
| schema:title | Enter the title of the spreadsheet. |
| pav:version | Enter the version of the spreadsheet. |
| pav:createdOn | Enter the creation date and time (format: YYYY-MM-DD hh:mm). |
| pav:derivedFrom | Enter the CEDAR template IRI that contains the validation rules. |

## How to include the metadata information?

* For Excel file format, add a new sheet called `.metadata` and create a table with the metadata information.

![Screen Shot 2023-04-24 at 4 40 18 PM](https://user-images.githubusercontent.com/5062950/234138426-d0765efa-829b-491f-ad78-413914f9a818.png)

* For CSV file format, create a new file called `metadata`, create a table with the metadata information and place it in a same directory as the CSV file. You will need pack them together in a zip file.

  ![Screen Shot 2023-03-22 at 1 56 20 PM](https://user-images.githubusercontent.com/5062950/227036180-7106e97b-7ee0-4ee7-bc7d-1f2849087cf7.png)
  
## Uploading the file

You can either drag-and-drop the file from your local computer to the input field or use the "Browse" option to select the file from your file system.
