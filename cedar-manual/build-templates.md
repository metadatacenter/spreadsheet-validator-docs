---
title: Building CEDAR Templates for Community Standards
layout: page
nav_order: 1
parent: CEDAR Manual
---

# Building CEDAR Templates for Community Standards

This guide provides a step-by-step process for building metadata templates that adhere to community standards using the CEDAR platform.

## Workflow Overview

1. Pre-requisite
2. Planning Phase
3. Building the Template
4. Version Management
5. Sharing to Public

## 1. Pre-requisite

* Ensure you have an active CEDAR user account. Follow the steps in this [guide to create a CEDAR account](https://metadatacenter.readthedocs.io/en/latest/user-guide/sections/a1/creating_a_cedar_account/).

* Start by gathering the source metadata specification documents:
  - Spreadsheets (.xlsx, .csv)
  - Text documents (.doc, .pdf)
  - Existing metadata schemas

  These documents outline the required metadata fields according to the established community standards.

## 2. Planning Phase

Before building templates, plan your approach:

* Review the [best practices](best-practices.md) for naming the fields and other best practices.
* Identify the common data fields that will be reused across templates.
* [Begin by building the common data fields](build-common-fields.md) first.
* Construct the template using these common data fields as the foundation.

Think of common data fields as reusable building blocks--like Lego pieces that can be assembled into different structures.

## 3. Building the Template

### Steps to Create a New Template

1. Select "New > Template" to create a new template.
2. Replace "Untitled" with the desired template name.
3. Move the mouse pointer to the right-hand side and click the search magnifier icon (see Fig 1).
4. In the search dialog window, navigate to the common data field folder containing the fields you created earlier (see Fig 2).
5. Select the required fields for the metadata template.
6. Click the "Select" button to close the window.

### Customization Options

* **Requirement Level**: 
  - On the field panel, click the "REQUIRED" tab.
  - Select "YES" to make the field required, or "NO" to make it optional (default is "NO").

* **Default Value**: 
  - On the field panel, click the "OPTIONS" tab.
  - Enter the default value in the "Enter Default Value" field.

## 4. Version Management 

### Steps to Set a Version

* A newly created CEDAR template always starts with version 0.0.1. To set a version to your template, go to the Workspace View and open the Resource Menu by clicking the vertical dots (the 'kebab menu', ⋮) on the right-hand side of the template.

* Select "Publish Version" and set the version number. 

Each version of a CEDAR template is assigned a unique UUID and a distinct URL is generated for accessing each one of them.

*Tip*: If you prefer to work in draft mode but want to start with version 1.0.0, first publish the template to get version 0.0.1. Then, select "Create Version" and set it to 1.0.0. Use version 1.0.0 for any future development of the template.

## 5. Sharing to Public

To increase the visibility of your template, follow these steps:

1. Open the Resource Menu and select "Share".
2. In the "Enter group name" field, type the keyword "Everybody" and set the permission to "can read".
3. Next, select "Enable Open View" from the Resource Menu.
4. To share the template, select "Visit Open View" and copy the URL provided.

By enabling these features, your template will be accessible to a broader audience.

## Related Topics

- Review the [field building guide](build-common-fields.md)
- Learn about [naming conventions](conventions.md)
- See examples of completed templates