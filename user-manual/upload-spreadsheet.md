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

* For TSV file format, add a new column called `metadata_schema_id` and include the metadata schema UUID identifier. You can find the identifier in the CEDAR OpenView documentation page. As an example, this [page](https://openview.metadatacenter.org/templates/https:%2F%2Frepo.metadatacenter.org%2Ftemplates%2F329f8a62-a468-4ba9-863d-fc0e328f896a) shows the ATACseq documentation page. Navigate to the bottom of the page to locate the 'Metadata schema ID' field. Hover your mouse cursor over the information (i) icon (as depicted in the screenshot below), and then copy and paste the provided string from the popup message into your TSV file.

<img width="1512" alt="find-metadata-schema-id" src="https://github.com/metadatacenter/spreadsheet-validator-docs/assets/5062950/009a08fd-650c-46b0-ac82-bc1b0d2e58bd">



## Uploading the file to validate

You can either drag-and-drop the file from your local computer to the input field or use the "Browse" option to select the file from your file system.
