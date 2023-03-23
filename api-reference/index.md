---
title: API Reference
layout: home
nav_order: 1
---

Base URL: `https://api.metadatavalidator.metadatacenter.org/`

## Validate Spreadsheet

```
POST /service/validate
```

### Header

| Variable Name | Value |
| ------------- | ----- |
| `Content-Type` | `application\json` |

### Body Schema

```
{
  "spreadsheetData": [
    { Row },
    { Row },
    { Row },
    ...
  ],
  "cedarTemplateIri": "string"
}
```

| Attribute Name | Type | Description |
| -------------- | ---- | ----------- |
| `spreadsheetData` | [ `Row` ] | An array of metadata records. |
| `cedarTemplateIri` | string | The CEDAR Template IRI that provides the metadata specification. |

#### `Row` Schema

```
{
  column1: value1,
  column2: value2,
  column3: value3,
  ...
}
```
| Attribute Name | Type | Description |
| -------------- | ---- | ----------- |
| `column1`, `column2`, ..., `columnN` | Any | The column value. |

#### Example

```
{
  "spreadsheetData": [
    {
      "sample_id": "Visium_9OLC_I4_S2",
      "source_storage_time_value": 208,
      "source_storage_time_unit": "day",
      "preparation_medium": "Methanol (100%)",
      "preparation_condition": "Ice",
      "processing_time_value": 4,
      "processing_time_unit": "minute",
      "storage_medium": "OCT embedded",
      "storage_condition": "-80 celsius freezer",
      "quality_criteria": "",
      "histological_report": "",
      "thickness_value": 10,
      "thickness_unit": "millimeter",
      "section_index_number": 3,
      "area_value": 15.84,
      "area_unit": "square millimeter",
      "notes": ""
    },
    {
      "sample_id": "",
      "source_storage_time_value": "86 days",
      "source_storage_time_unit": "days",
      "preparation_medium": "Formalin",
      "preparation_condition": "",
      "processing_time_value": "10 minutes",
      "processing_time_unit": "minutes",
      "storage_medium": "Paraffin embedded",
      "storage_condition": "Liquid nitrogen",
      "quality_criteria": "",
      "histological_report": 12.05,
      "thickness_value": 10,
      "thickness_unit": "mm",
      "section_index_number": 1,
      "area_value": 12.05,
      "area_unit": "mm^2",
      "notes": ""
    },
    {
      "sample_id": "",
      "source_storage_time_value": "86 days",
      "source_storage_time_unit": "days",
      "preparation_medium": "Formalin",
      "preparation_condition": "",
      "processing_time_value": "10 minutes",
      "processing_time_unit": "minutes",
      "storage_medium": "Paraffin embedded",
      "storage_condition": "Liquid nitrogen",
      "quality_criteria": "",
      "histological_report": 15.84,
      "thickness_value": 10,
      "thickness_unit": "mm",
      "section_index_number": 2,
      "area_value": 15.84,
      "area_unit": "mm^2",
      "notes": ""
    }
  ],
  "cedarTemplateIri": "https://repo.metadatacenter.org/templates/a9efb30e-4e2c-4d66-8890-b66204a4a774"
}
```

### Response Schema

```
{
  "schema": {
    "name": "string",
    "columnDescription": {
      ColumnSchema
    },
    "columnOrder": [
      "string"
    ],
    "generatedFrom": "string"
  },
  "data": [
    { Row },
    { Row },
    { Row },
    ...
  ],
  "reporting": [
    { ErrorReport },
    { ErrorReport },
    { ErrorReport },
    ...
  ]
}
```

| Attribute Name | Description |
| -------------- | ----------- |
| `schema` | The metadata specification object. |
| `schema.name` | The



### Response Code

| Code | Description |
| ---- | ----------- |
| 200 | Success. |
| 400 | The request could not be understood by the server due to malformed syntax in the request body. |
| 500 | The server encountered an unexpected condition that prevented it from fulfilling the request. |
