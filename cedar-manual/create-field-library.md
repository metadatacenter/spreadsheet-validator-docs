---
title: Creating Field Library
layout: page
nav_order: 2
parent: CEDAR Manual
---

# Creating Field Library

Creating data fields before building the templates offers the advantage of reusability. This approach is particularly useful when you need to create multiple metadata templates and many of the fields are shared. It ensures that data fields are standardized and consistent across different templates.

<img width="800" alt="Data field library" src="https://github.com/user-attachments/assets/7488e7b1-199a-4978-ae69-21e891ad9cf0" />

At CEDAR, creating field library is straightforward. Begin by creating a new folder to organize all the common data fields. Select "New > Folder" and enter a name for the folder, such as "My Field Library".

### General Steps to Create a New Fields

1. Select "New > Field" to add a new field to your library folder.
2. A new text field is created by default. To change the field type, use the field palette on the right. CEDAR currently supports 14 field types, including number, date, image, and video.
3. Rename the field from "Untitled" to your desired name. Refer to the [naming conventions](best-practices.md) for guidance.
4. Next, provide the preferred label and description for the field. You can use ChatGPT or other LLM tool to refine your description for better readability. *__Tip__: Enhance clarity by including an example value after the description. For example, the "Parent Dataset ID" field description could be:
`Unique identifier of the dataset used to generate this derived dataset. Example: HNDF-123-HH.`*.

## Creating a Field with Controlled Terms

Often times, you need to create a field with controlled terms to guide and restrict user inputs to specific values. Depending on your requirements, there are three ways to achieve this when creating a new field:

### When controlled terms are plain strings

1. Change the field type to "Multiple Choice" from the field palette.
2. Add the controlled terms as option value strings. The figure below illustrates an example of using a multiple-choice field to enumerate all possible barcode sizes.
   
   <img width="700" alt="Controlled terms source from multiple choices" src="https://github.com/user-attachments/assets/f4af4e11-b1c4-48fe-9067-5ccc44b943f7" />

### When controlled terms must come from ontologies

1. Select the "VALUES" setting and click "Add".
2. Type the controlled term label in the "Search in BioPortal" field. If you know the ontology name in advance, enter it in the "Narrow your search to specific ontologies" field.
3. Select the resulting term and click "Add". Ensure the "TERM" option is selected, not "BRANCH" or "ONTOLOGY".
4. Repeat this process until you have added all the controlled term labels. The figure below illustrates an example of using controlled values from ontologies to enumerate all possible processing time units.
   
   <img width="700" alt="Controlled terms sourced from individual ontology terms" src="https://github.com/user-attachments/assets/70d36136-03f4-4988-952d-856c7f0852f0" />

### When controlled terms must come from an ontology branch or a custom value set

1. Select the "VALUES" setting and click "Add".
2. Type the controlled term label in the "Search in BioPortal" field. If you know the ontology or value set name in advance, enter it in the "Narrow your search to specific ontologies" field.
3. Select the resulting term and click "Add". Ensure the "BRANCH" option is selected, not "TERM" or "ONTOLOGY". The figure below illustrates an example of using a branch from the NCI Thesaurus (NCIT) to include all medical occupations. Clicking the "Arrange" button displays the list of the occupations, such as "Cardiologist", "Clinical Pathologist", "Coroner", "Dermatologist".

   <img width="700" alt="Controlled terms sourced from ontology branches" src="https://github.com/user-attachments/assets/92244ddc-bc97-448d-8043-9468b377cbd9" />








