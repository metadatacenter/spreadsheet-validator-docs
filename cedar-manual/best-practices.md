---
title: Best Practices
layout: page
nav_order: 4
parent: CEDAR Manual
---

# Best Practices

Follow these best practices when building fields and templates in CEDAR:

1. **Naming Fields**
   
   <img width="800" alt="Naming fields" src="https://github.com/user-attachments/assets/49b8af61-f34f-42da-9b0a-bb10e9076ace" />

   - For the "Field name" label, use snake_case format (e.g., `parent_dataset_id` instead of `Parent Dataset ID`).
   - For the "Preferred Label", use title case format (e.g., `Parent Dataset ID`).

3. **Creating Descriptions**
   - Provide clear and concise descriptions for each field.
   - *(Recommended)* Enhance clarity by including an example value after the description. For example, the "Parent Dataset ID" field description could be:
`Unique identifier of the dataset used to generate this derived dataset. Example: HNDF-123-HH.`.

4. **Naming Boolean Fields**

   <img width="800" alt="Naming boolean fields" src="https://github.com/user-attachments/assets/9765b6c5-cf51-4039-bf91-de0bb60202fd" />

   Use a question format for boolean fields (e.g., `is_rehydrated`, `is_cell_type_annotation_included`) to indicate a "Yes" or "No" response.

6. **Using Regular Expressions for Identifier Validation**

   <img width="800" alt="Using regex for identifier validation" src="https://github.com/user-attachments/assets/764d4d13-6ea3-405a-8c5f-70bf89fb9699" />

   - Apply regular expressions to ensure identifier fields match specific patterns. To do this, select the "OPTIONS" setting and enter the desired regex in the "Enter Regex" field.
   - Common regex patterns:
     - ORCID: `(\d{4}-){3}\d{3}(\d|X)`
     - DOI: `10\.\d+/.*`
     - UniProt ID: `([A-N,R-Z][0-9]([A-Z][A-Z, 0-9][A-Z, 0-9][0-9]){1,2})|([O,P,Q][0-9][A-Z, 0-9][A-Z, 0-9][A-Z, 0-9][0-9])(\.\d+)?]`
     - ISBN: `(-13|-10)?[:]?[ ]?(\d{2,3}[ -]?)?\d{1,5}[ -]?\d{1,7}[ -]?\d{1,6}[ -]?(\d|X)`
   - *Tip*: Visit [Identifiers.org](https://identifiers.org) for more regex examples.

8. **Using Value Set vs. Multiple Choice**
   - Decide between value sets and multiple choice based on whether the values are shareable concepts. Use Multiple Choice for non-shareable values, such as a collection of input parameters.
