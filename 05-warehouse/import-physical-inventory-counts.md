---
title: Import Physical Inventory Counts via Spreadsheet
id: WH-COUNT-001c-alt
module: Warehouse
screen: Physical Inventory Count / IMPORTMAP
menu_path: Inventory > Physical Inventory Count > [select count] > Import
applies_to:
  - Warehouse Manager
prerequisites:
  - Count session is open (see WH-COUNT-001a)
  - Excel file is formatted per template
related_procedures:
  - WH-COUNT-001a
  - WH-COUNT-001b
  - WH-COUNT-002
tags: physical inventory, count, import, spreadsheet, IMPORTMAP
version: 1.0
last_updated: 2026-03-25
---

# Import Physical Inventory Counts via Spreadsheet

## What This Procedure Does

Import physical inventory counts for Q-type masters from an Excel spreadsheet using the IMPORTMAP utility. This method is efficient when count quantities have been recorded on paper or in a spreadsheet and need to be bulk-loaded into the count session.

## Before You Begin

- A physical inventory count session is open and ready to receive import data
- Count quantities have been collected on count sheets or in a spreadsheet
- An Excel file has been prepared in the format matching the count template
- The file contains only Q-type master counts (not serialized asset serial numbers)
- User has Warehouse Manager role

## Steps

### Step 1: Export the Count Template

Open the count session from **Inventory > Physical Inventory Count**. Select the count session you want to import data into. Click the **Import** button (or locate the import option in the extended menu). The system displays an option to export the count template. Click **Export Template** to download the Excel file structure.

This template file contains the master numbers and expected columns for count quantities. Save this file to your local machine.

### Step 2: Populate the Excel File

Open the exported template in Microsoft Excel. For each Q-type master listed:

| Field | What to enter |
|-------|---------------|
| Master No. | Pre-populated; do not modify |
| Description | Pre-populated; informational only |
| Count Qty | Enter the physical count quantity from your warehouse count sheets |
| Location | Enter the location code where items were counted (if required) |

Complete the Count Qty column with the quantities counted from the warehouse floor. Ensure all quantities are numeric values. Save the file to your computer.

### Step 3: Access IMPORTMAP Utility

From the count session import screen, click **Select File** and choose the populated Excel file. The IMPORTMAP utility opens, displaying the file contents and import mapping.

Verify that the columns are correctly mapped:

- Master No. column maps to the master identifier
- Count Qty column maps to the counted quantity field
- Any location or detail columns are mapped appropriately

### Step 4: Verify and Upload

Review the preview of the data to be imported. Check that quantities appear correct and all required fields are populated. Click the **Validate** button to verify the data format and values.

If validation passes, click **Import** to upload the counts into the count session. The system confirms the number of records imported.

If validation shows errors, correct the Excel file and re-upload. Common errors include blank quantity cells, non-numeric values, or invalid master numbers.

### Step 5: Verify Imported Counts

Return to the count session view and review the counts that were imported. Verify that:

- All Q-type masters show counted quantities
- Quantities match the Excel file values
- No error records were skipped or rejected

Click **Save** (floppy disk icon) to confirm the import and save the count session.

## What Happens Next

The imported counts are now recorded in the count session. The Warehouse Manager can run the Physical Inventory Variance Report (see WH-COUNT-002) to compare imported counts against system on-hand quantities. Variances will be reviewed and approved before posting.

## Common Issues

**File format not recognized**

Ensure the Excel file is in .xlsx or .csv format as required by IMPORTMAP. The file must follow the exported template structure exactly. Check that the template was downloaded from the count session you are importing to; templates may vary by count type.

**Column mapping is incorrect**

Review the column headers in your Excel file and match them to the template exactly. Use copy-paste from the exported template to ensure header names are identical. The IMPORTMAP utility will show the mapping on screen; verify each column is assigned to the correct field.

**Quantities are rejected or show as zero**

Verify that all quantity cells contain numeric values only. Remove any text, currency symbols, or special characters from the Count Qty column. Empty cells may be interpreted as zero; fill in actual counted quantities or leave items blank if not found.

**Master numbers do not match**

The master numbers in the Excel file must exactly match the master numbers in the count session. Verify the master numbers in the template and ensure no typos were introduced. If masters have been added or removed from the session since the template was exported, re-export the template.

**Import completes but some records are missing**

Check the import summary report for rejected or skipped records. Records are typically rejected if the master number is invalid or a duplicate entry exists for the same master in the same import. Review the error log and correct the Excel file before re-importing.
