---
title: Creating Field Library
layout: page
nav_order: 2
parent: CEDAR Manual
---

# Creating Field Library

Creating data fields before building the templates offers the advantage of reusability. This approach is particularly useful when you need to create multiple metadata templates and many of the fields are shared. It ensures that data fields are standardized and consistent across different templates.

At CEDAR, creating field library is straightforward. Begin by creating a new folder to organize all the common data fields. Select "New > Folder" and enter a name for the folder, such as "My Field Library".

### General Steps to Create a New Fields

1. Select "New > Field" to add a new field to your library folder.
2. A new text field is created by default. To change the field type, use the field palette on the right. CEDAR currently supports 14 field types, including number, date, image, and video.
3. Rename the field from "Untitled" to your desired name. Refer to the [naming conventions](best-practices.md) for guidance.
4. Although it is not mandatory, provide a preferred label and description for the field to enhance clarity and usability.


## Creating a Field with Controlled Terms

Often times, you need to create a field with controlled terms to guide and restrict user inputs to specific values. Depending on your requirements, there are three ways to achieve this when creating a new field:

### When controlled terms are plain strings

1. Change the field type to "Multiple Choice" from the field palette.
2. Add the controlled terms as option value strings.

### When controlled terms must come from ontologies

1. Select the "VALUES" setting and click "Add".
2. Type the controlled term label in the "Search in BioPortal" field. If you know the ontology name in advance, enter it in the "Narrow your search to specific ontologies" field.
3. Select the resulting term and click "Add". Ensure the "TERM" option is selected, not "BRANCH" or "ONTOLOGY".
4. Repeat this process until you have added all the controlled term labels.

### When controlled terms must come from an ontology branch or a custom value set

1. Select the "VALUES" setting and click "Add".
2. Type the controlled term label in the "Search in BioPortal" field. If you know the ontology or value set name in advance, enter it in the "Narrow your search to specific ontologies" field.
3. Select the resulting term and click "Add". Ensure the "BRANCH" option is selected, not "TERM" or "ONTOLOGY". For example, to include all medical occupations from the NCI Thesaurus (NCIT), select the term "Medical Occupation" in the result panel and add it as a branch. This will automatically include all known medical occupations in NCIT, such as "Cardiologist", "Clinical Pathologist", "Coroner", "Dermatologist", and so on, as the controlled terms for your field.

## Developing Custom Value Set









