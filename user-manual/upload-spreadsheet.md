---
title: Upload Spreadsheet
layout: page
nav_order: 1
parent: User Manual
---

# Upload Spreadsheet

Users can upload their spreadsheet file using the input field on the homepage. Currently, the tool supports two types of input format:
1. Excel spreadsheet (.xlsx)
2. TSV file (.tsv)

## Metadata information

Both input formats require metadata information that provides context for the tool's algorithm. The table below lists required metadata fields:

| Field | Description |
| ----------- | ----------- |
| schema:title | Enter the title of the spreadsheet. |
| pav:version | Enter the version of the spreadsheet. |
| pav:createdOn | Enter the creation date and time (format: YYYY-MM-DD hh:mm). |
| pav:derivedFrom | Enter the CEDAR template IRI that contains the validation rules. |

## How to include the metadata information?

* For Excel file format, add a new sheet called `.metadata` and create a table with the metadata information.

![Screen Shot 2023-04-24 at 4 40 18 PM](https://user-images.githubusercontent.com/5062950/234138426-d0765efa-829b-491f-ad78-413914f9a818.png)

* For TSV file format, add a column called `metadata_schema_id` and include the metadata schema UUID identifier. You can find the identifier in the metadata schema documentation (see screenshot below).

<img width="900" alt="Screen Shot 2023-07-11 at 4 32 15 PM" src="https://github.com/metadatacenter/spreadsheet-validator-docs/assets/5062950/7fe93431-652f-4c39-9444-ca8cbfc99f0c">

## Uploading the file to validate

You can either drag-and-drop the file from your local computer to the input field or use the "Browse" option to select the file from your file system.
