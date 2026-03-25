---
title: Add Service Contract Line Items
id: SVC-CONTRACT-002b
module: Service
screen: Service Contract > Line Items
menu_path: Service Contract > Line Items Tab
applies_to: Service Managers, Contract Administrators
prerequisites:
  - Service contract header must be created
  - Product master records must exist
  - Master No (for block amount contracts) must be configured
related_procedures:
  - SVC-CONTRACT-002a
  - SVC-CONTRACT-002c
tags:
  - line items
  - products
  - contract setup
version: 1.0
last_updated: 2026-03-25
---

# Add Service Contract Line Items

## What This Procedure Does

Adds products and services to an existing service contract by creating line items that define what will be serviced under the contract. Each line item specifies a product, site, pricing, and coverage dates.

## Before You Begin

- A service contract header must already exist and be saved
- Product master records must be configured in the system
- You must have the contract open in edit mode
- For block amount contracts, you must know the master item number (M-type product)

## Steps

### Step 1: Open the Contract and Navigate to Line Items

Open the service contract from Service > Service Contracts list. Click the Line Items tab to display the line items grid.

### Step 2: Add a New Line Item

In the Line Items grid, click the Add button (plus icon) in the toolbar. A new line item row is created and enters edit mode.

### Step 3: Enter Line Item Details

Fill in the following fields for the line item:

| Field | What to enter |
|-------|---------------|
| Product | Select the product to be serviced under the contract |
| Site | Select the specific site where the product is located |
| Master No | For block amount contracts, enter the M-type master product number; leave blank for other contract types |
| Description | Enter a description of the product or service (auto-populated from product master) |
| Price | Enter the service price or rate |
| Cost | Enter the cost for tracking profitability |
| Start Date | Enter the date service coverage begins for this item |
| End Date | Enter the date service coverage ends for this item |
| Sync Dates | Check this flag to align the line item dates with the header Start Date and End Date |
| Coverage Details | Enter any special coverage terms or limitations |

### Step 4: Configure Additional Coverage Details

Expand the Coverage Details section if additional information is needed. Specify coverage windows, SLA response times, or special service terms applicable to this line item.

### Step 5: Save the Line Item

Click Save to add the line item to the contract. The line item now appears in the grid. Repeat steps 2-5 to add additional products or services.

### Step 6: Review and Finalize

Once all line items are added, review the complete Line Items grid. Verify that products, dates, and pricing are correct. Click the Save button (floppy disk icon) in the contract header to save all changes.

## What Happens Next

Line items are saved and associated with the contract. If the Sync Dates flag is checked, line item dates are synchronized with header dates. When you configure billing on the Billing tab, the system calculates billing amounts based on these line items. For recurring dispatch contracts, you can define call schedules on the Recurring tab of each product line item.

## Common Issues

**Product does not appear in the Product dropdown**

Ensure the product master record exists and is marked as serviceable. If the product does not appear, create the product in the Product Master module first. Products must have valid product codes and be configured with appropriate service attributes.

**Sync Dates flag overrides my manually entered dates**

The Sync Dates flag, when checked, forces line item dates to match the contract header Start Date and End Date. If you need line items with different date ranges than the header, uncheck this flag and enter dates manually for each line item.

**Cannot enter Master No for block amount contracts**

Master No is a specific field for block amount contracts using an M-type product. Ensure the product you selected is configured as a master item with the Warr/Def Rev flag checked. If you are not using a block amount contract type, leave this field blank.
