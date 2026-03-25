---
title: Import or Update Masters
id: PO-MASTER-002
module: Purchasing
screen: Import/Update Masters
menu_path: Inventory > Import/Update Masters
applies_to:
  - Purchasing Agent
  - Warehouse Manager
  - System Administrator
prerequisites:
  - User has permission to access the Inventory module and import functions
  - A properly formatted Excel import file is prepared
related_procedures:
  - PO-MASTER-001
  - PO-MASTER-003
  - PO-MASTER-004
tags: import masters, update masters, bulk import, master inventory, Excel import, master upload, inventory import, mass update masters
version: 1.0
last_updated: 2026-03-25
---

# Import or Update Masters

## What This Procedure Does

Bulk import new master inventory records or update existing master records from an Excel spreadsheet. This is used when onboarding a large catalog of parts, updating pricing across multiple items, or synchronizing master data from an external source.

## Before You Begin

- You need permission to access the Import/Update Masters function in the Inventory module.
- Download the master import template from Q360 to ensure correct column formatting.
- Populate the template with the master data you want to import or update. Each row represents one master record.
- For updates to existing masters, the Master No column must match existing records exactly.
- Save the file in Excel (.xlsx) format.

## Steps

### Step 1: Open the Import/Update Masters Screen

Navigate to **Inventory > Import/Update Masters** from the Main Navigation Sidebar (vertical panel, left edge). The import form opens in a new tab.

### Step 2: Download the Import Template (If Needed)

If you do not already have the template, click the **Download Template** button. Save the Excel file locally, populate it with your master data, and save.

### Step 3: Select the Import File

Click the **Browse** or **Select File** button. Navigate to your prepared Excel file and select it. The file name displays in the file path field.

### Step 4: Upload and Preview

Click **OK** or **Upload**. Q360 reads the file and displays a preview of the records to be imported or updated. Review the preview grid to verify that data mapped correctly to the expected columns.

| Field | What to enter |
| --- | --- |
| Master No | Unique identifier for the master item. For new records, this must not already exist. For updates, it must match exactly. |
| Description | Item description text. |
| Master Type | A (Asset/serialized), Q (Quantitative), M (Miscellaneous), L (Labor), F (Freight), K (Kit), S (Service), or B (Budget). |
| Manufacturer | Manufacturer or brand name. |
| Category | Item category classification. |
| Standard Cost | Default cost used for inventory valuation. |
| Standard Price | Default selling price or use a pricing factor. |
| Taxable | Whether the item is subject to sales tax. |

### Step 5: Save the Import

Click **Save**. Q360 processes each row and creates new master records or updates existing ones. A summary displays showing the number of records successfully imported and any errors encountered.

### Step 6: Review Results

Check the results summary for any failed rows. Common failures include duplicate master numbers for new imports, missing fields, or invalid master types. Correct errors in the source file and re-import only the failed rows.

## What Happens Next

New master records are immediately available in the Master Inventory form and searchable via Find Product (see PO-MASTER-001). Updated records reflect the new values across all modules that reference the master number. If you also need to associate vendors with the imported masters, proceed to Import or Update Master Vendors (see PO-MASTER-003).

## Common Issues

**Import fails with duplicate master number errors.** The Master No values in your file already exist in Q360. If you intend to update existing records, ensure the import mode is set to update rather than insert. If creating new records, assign unique master numbers.

**Columns do not map correctly.** The column headers in your file must match the template exactly. Download a fresh template and copy your data into it, preserving the header row. Do not rename or reorder columns.

**Standard Cost or Price shows as zero after import.** Verify the source file has numeric values in the cost and price columns without currency symbols or special characters. Blank cells default to zero.

**Master Type is rejected.** Only valid type codes are accepted: A, Q, M, L, F, K, S, B. Check for extra spaces or lowercase letters in the Master Type column.

**Large file takes a long time to process.** Files with thousands of rows may take several minutes. Do not close the browser tab or navigate away during processing. For very large imports, consider splitting the file into smaller batches.
