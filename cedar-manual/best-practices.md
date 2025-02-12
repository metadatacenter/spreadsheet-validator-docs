---
title: Best Practices
layout: page
nav_order: 4
parent: CEDAR Manual
---

# Best Practices

Follow these best practices when building fields and templates in CEDAR:

1. **Naming Fields**
   - For the "Field name" label, use snake_case format (e.g., `parent_dataset_id` instead of `Parent Dataset ID`).
   - For the "Preferred Label", use title case format (e.g., `Parent Dataset ID`).

2. **Creating Descriptions**
   - Provide clear and concise descriptions for each field.
   - *(Optional)* Include an example value after the description. For instance, for "Parent dataset ID": "Unique identifier of the dataset used to generate this derived dataset. Example: HNDF-123-HH".

3. **Naming Boolean Fields**
   - Use a question format for boolean fields (e.g., `is_antibody`, `is_cell_type_annotation_included`) to indicate a "Yes" or "No" response.

4. **Using Regular Expressions for Identifier Validation**
   - Apply regular expressions to ensure identifier fields match specific patterns. To do this, select the "OPTIONS" setting and enter the desired regex in the "Enter Regex" field.
   - Common regex patterns:
     - ORCID: `(\d{4}-){3}\d{3}(\d|X)`
     - DOI: `10\.\d+/.*`
     - UniProt ID: `([A-N,R-Z][0-9]([A-Z][A-Z, 0-9][A-Z, 0-9][0-9]){1,2})|([O,P,Q][0-9][A-Z, 0-9][A-Z, 0-9][A-Z, 0-9][0-9])(\.\d+)?]`
     - ISBN: `(-13|-10)?[:]?[ ]?(\d{2,3}[ -]?)?\d{1,5}[ -]?\d{1,7}[ -]?\d{1,6}[ -]?(\d|X)`
   - *Tip*: Visit [Identifiers.org](https://identifiers.org) for more regex examples.

5. **Using Value Set vs. Multiple Choice**
   - Decide between value sets and multiple choice based on whether the values are shareable concepts. Use Multiple Choice for non-shareable values, such as a collection of input parameters.
