---
title: Create Products from Shipped Materials
id: PROJ-PRODUCT-001
module: Projects
screen: Project Form > Materials Tab
menu_path: Main Menu > Projects > Projects
applies_to:
  - Project Manager
prerequisites:
  - PROJECT (Edit) permission
  - PRODUCT (Create) permission
  - Project has SHIPPED line items on the Materials tab
related_procedures:
  - PROJ-CLOSE-002
  - PROJ-MAT-002
tags:
  - create product
  - shipped materials
  - product record
  - system record
  - service tracking
  - asset
  - installed product
version: 1.0
last_updated: 2026-03-25
---

# Create Products from Shipped Materials

## What This Procedure Does

This procedure enables you to create product records from shipped materials on a project. Creating product records establishes system records for installed equipment, systems, or deliverables that require tracking as company assets or for ongoing service and support.

## Before You Begin

- Verify you have PROJECT (Edit) and PRODUCT (Create) permissions assigned to your role
- Ensure the project has SHIPPED line items on the Materials tab
- Have substantial completion date information available for product creation
- Identify which shipped materials should be grouped together as a single product or system

## Steps

### Step 1: Navigate to the Materials Tab
Look up the project in the Projects module. Click on the Materials tab to access the project materials list.

### Step 2: Select Shipped Line Items
Select one or more SHIPPED line items that collectively belong to a single product or system. Multiple materials can be combined into one product record if they form a cohesive system or asset.

### Step 3: Verify Edit Mode Status
Ensure the project is NOT currently in Edit mode. The Create Product function operates in view mode only.

### Step 4: Access the Create Product Function
Click the Extended Menu (3 vertical dots) and select Create Product For Selected Items.

### Step 5: Name the Product and Specify Completion Date
In the product creation dialog:
- Enter a descriptive name for the product
- Specify the date of substantial completion

### Step 6: Submit and Confirm Creation
Click Submit. Q360 creates the product record and automatically opens the product form to confirm successful creation.

### Step 7: Verify Product Details
The product form displays the product created under the project ship site with the selected materials listed as product details. Review the information to ensure accuracy.

### Step 8: Create Additional Products
Repeat steps 2 through 7 for each additional product or system on the project.

## What Happens Next

Product records are now established for installed systems and equipment. These records track the company's service and support obligations and can be used for ongoing maintenance, warranty tracking, and asset management. You can now proceed with project substantial completion (see PROJ-CLOSE-002).

## Common Issues

**The Create Product For Selected Items option does not appear in the Extended Menu.**
Verify that you have selected one or more SHIPPED line items on the Materials tab before accessing the Extended Menu. The option appears only when appropriate items are selected. Additionally, ensure the project is not in Edit mode.

**I cannot create a product because I do not have PRODUCT (Create) permission.**
Contact your system administrator to request PRODUCT (Create) permission. This permission must be assigned to your user role to create new product records. You cannot create products without this permission assigned.

**The product form does not open after clicking Submit.**
The product creation may have succeeded even if the form does not open automatically. Navigate to the Products module and search for the product by name to verify it was created. If the product does not exist, retry the creation process and ensure all required information is entered in the creation dialog.

**Selected materials are not transferred to the product record.**
Verify that the materials you selected in step 2 remained selected before submitting the product creation. The selection may be cleared if you navigate away from the Materials tab. Re-select the desired items and immediately proceed with product creation.

**I need to create a product from a partial shipment of materials.**
You can select any combination of SHIPPED line items to create a product record. If a shipment includes multiple distinct products or systems, create separate product records for each by selecting only the relevant items in each creation process.
