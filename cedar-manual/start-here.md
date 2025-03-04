---
title: Start Here
layout: page
nav_order: 1
parent: Building CEDAR Templates for Community Standards
---

# Start Here

This guide provides a step-by-step process for building metadata templates that adhere to community standards using the [CEDAR platform](https://cedar.metadatacenter.org/).

## Workflow Overview

1. Pre-requisite
2. Planning Phase
3. Building the Template
4. Version Management
5. Sharing to Public
6. Disseminate the Template

## 1. Pre-requisite

* Ensure you have an active CEDAR user account. Follow the steps in this [guide to create a CEDAR account](https://metadatacenter.readthedocs.io/en/latest/user-guide/sections/a1/creating_a_cedar_account/).

* Start by gathering the source metadata specification documents:
  - Spreadsheets (.xlsx, .csv)
  - Text documents (.doc, .pdf)
  - Existing metadata schemas

  These documents outline the required metadata fields according to the established community standards. The figure below illustrates an example of metadata specification document, curated by a community and structured in a spreadsheet format.

  <img width="1000" alt="Typical metadata schema document" style="margin:0 0 10px 0;" src="../img/metadata-schema-document.png" />

## 2. Planning Phase

Before building templates, plan your approach:

* Identify the data fields that will be reused across templates, if you're building more than one.
* Review the [best practices](best-practices.html) for naming the fields and other tips.
* [Begin by building the common data field library](create-reusable-fields.html) first. 
* Construct the template using the data field library as the foundation.
  
Think of data fields as reusable building blocks--like Lego pieces that can be assembled into different structures.

## 3. Building the Template

### Steps to Create a New Template

Login to your CEDAR account first before following these steps below:

1. Select the "New > Template" button in the top-left corner to create a new template.
2. Replace "Untitled" with the desired template name.
3. In the "Field Type Selector" bar on the right, click the magnifier icon at the bottom to open the field search dialog.
4. Browse the directory structure to find the common data field folder that contains the fields you previously created. Image below illustrates an example of HuBMAP common data fields, the content of your folder may be different. <img width="700" alt="Common data field folder" style="margin:10px 0 10px 0;" src="../img/common-data-field-folder.png" />
6. Accumulate the required fields for the metadata template by clicking the plus icon, then and click the "Select" button to finish.

### Customization Options

On the Template Designer editor page, you can customize the selected fields, including updating the field descriptions to align with the template's context. Below are two common customizations you may encounter.

* **Set Requirement Level**: 
  - On the field panel, click the "REQUIRED" tab.
  - Select "YES" to make the field required, or "NO" to make it optional (default is "NO").
    <img width="700" alt="Modify the requirement level" style="margin:10px 0 10px 0;" src="../img/modify-requirement-level.png" />

* **Add Default Value**: 
  - On the field panel, click the "OPTIONS" tab.
  - Enter the default value in the "Enter Default Value" field.
    <img width="700" alt="Modify the default value" style="margin:10px 0 10px 0;" src="../img/modify-default-value.png" />


## 4. Version Management 

### Steps to Set a Version

* A newly created CEDAR template always starts with version 0.0.1. To set a version to your template, go to the Workspace View and open the Resource Menu by clicking the vertical dots (the 'kebab menu', ⋮) on the right-hand side of the template.

* Select "Publish Version" and set the version number.
  <img width="800" alt="Publish version" style="margin:10px 0 10px 0;" src="../img/publish-version.png" />

Each version of a CEDAR template is assigned a unique UUID and a distinct URL is generated for accessing each one of them.

*Tip*: If you prefer to work in draft mode but want to start with version 1.0.0, first publish the template to get version 0.0.1. Then, select "Create Version" and set it to 1.0.0. Use version 1.0.0 for any future development of the template.

## 5. Sharing to Public

To increase the visibility of your template, follow these steps:

1. Open the Resource Menu and select "Share".
2. In the "Enter group name" field, type the keyword "Everybody" and set the permission to "can read".
   <img width="680" alt="Share permission" style="margin:10px 0 10px 0;" src="../img/share-permission.png" />
 
4. Next, select "Enable Open View" from the Resource Menu.
   <img width="800" alt="Share permission" style="margin:10px 0 10px 0;" src="../img/enable-openview.png" />

5. To share the template, select "Visit Open View" and copy the URL provided.

By enabling these features, your template will be accessible to a broader audience.

## 6. Disemminate the Template

### As an Excel Spreadsheet

*COMMENT: The menu option is still under development by CEDAR Team*

It is possible to produce an Excel spreadsheet out of a CEDAR template for collecting metadata records from users. However, this method is only feasible if the template has a simple, flat structure without nested elements. 

Spreadsheets offer several advantages: 1) they are widely used, and their user-friendly interface makes data entry intuitive; 2) they are highly versatile, allowing easy copying and distribution; 3) they support bulk editing, making them ideal for adding large metadata records efficiently.

To convert a CEDAR template into an Excel spreadsheet, use the "Download Excel" option in the menu. If this option is unavailable, it means your template does not meet the criteria of having a simple, flat structure. You may need to restructure the template to enable this functionality. Once selected, the action will immediately generate an Excel file that is automatically downloaded.

### As a Shareable Web Form

Another way to distribute CEDAR templates is through its native Web form user interface. Follow [this link](publish-web-form.html) to learn how to share CEDAR templates as Web forms.

## Related Topics

- Review the guide on [creating reusable fields](create-reusable-fields.html).
- Learn about [naming conventions](best-practices.html).
- See [examples of completed templates](https://github.com/hubmapconsortium/dataset-metadata-spreadsheet).
