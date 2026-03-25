---
title: Import or Update Master Vendors
id: PO-MASTER-003
module: Purchasing
screen: Update Master Vendors
menu_path: Inventory > Update Master Vendors
applies_to:
  - Purchasing Agent
  - Warehouse Manager
  - System Administrator
prerequisites:
  - User has permission to access the Inventory module and import functions
  - Master records already exist for the items being associated with vendors (see PO-MASTER-002)
  - Vendor records already exist in Q360 (see PO-VENDOR-001)
  - A properly formatted Excel import file is prepared
related_procedures:
  - PO-MASTER-001
  - PO-MASTER-002
  - PO-VENDOR-001
tags: import master vendors, update master vendors, bulk vendor import, vendor association, master vendor link, vendor pricing, Excel import vendors
version: 1.0
last_updated: 2026-03-25
---

# Import or Update Master Vendors

## What This Procedure Does

Bulk import or update the associations between master inventory items and their vendors from an Excel spreadsheet. This links vendor part numbers, costs, and lead times to master records, enabling the purchasing workflow to automatically select vendors when creating purchase orders.

## Before You Begin

- You need permission to access the Update Master Vendors function in the Inventory module.
- Master records must already exist for every item in your import file (see PO-MASTER-002).
- Vendor records must already exist for every vendor referenced in the file (see PO-VENDOR-001).
- Download the master vendor import template from Q360.
- Populate the template with master-vendor association data and save in Excel (.xlsx) format.

## Steps

### Step 1: Download the Master Vendor Template

If you do not already have the template, navigate to the import screen and download it. The template includes columns for the master number, vendor number, vendor part number, cost, and other association fields.

### Step 2: Populate the Template

Fill in the template with the master-vendor data.

| Field | What to enter |
| --- | --- |
| Master No | The Q360 master number for the inventory item. Must match an existing master record. |
| Vendor No | The Q360 vendor number. Must match an existing vendor record. |
| Vendor Part No | The vendor's own part number or SKU for this item. |
| Cost | The vendor's unit cost for this item. |
| Lead Time | Expected number of days from order to delivery. |
| Primary | Indicate whether this is the primary (default) vendor for the item. |

Save the file in Excel (.xlsx) format.

### Step 3: Open the Update Master Vendors Screen

Navigate to **Inventory > Update Master Vendors** from the Main Navigation Sidebar (vertical panel, left edge).

### Step 4: Select the Import File

Click the file selection button, navigate to your prepared Excel file, and select it. Click **OK** to upload.

### Step 5: Save the Import

Click **Save**. Q360 processes each row and creates or updates the master-vendor associations. A summary displays showing successful records and any errors.

### Step 6: Verify the Associations

Open a master record via Find Product (see PO-MASTER-001) and check the Vendors tab to confirm the vendor associations imported correctly with the expected costs and lead times.

## What Happens Next

The vendor associations are immediately available in the purchasing workflow. When items are queued for purchase, Q360 can auto-assign the primary vendor and use the imported cost for PO creation (see PO-CREATE-001). The AUTOMASTERVENDOR configuration option controls whether master-vendor records are auto-created when vendor lines are selected in the Purchase Queue - if set to ON, the system creates the association automatically.

## Common Issues

**Import fails with "Master not found" errors.** The Master No values in your file do not match existing records. Verify spelling, spacing, and case. Import or create the missing master records first (see PO-MASTER-002).

**Import fails with "Vendor not found" errors.** The Vendor No values do not match existing vendor records. Create the missing vendors first (see PO-VENDOR-001), then re-import.

**Vendor cost shows as zero after import.** Verify the cost column in the source file contains numeric values without currency symbols. Blank cells default to zero.

**Primary vendor flag did not set correctly.** Each master can have only one primary vendor. If the import file marks multiple vendors as primary for the same master, only the last one processed takes effect. Review and correct in the Master Inventory form if needed.

**Duplicate master-vendor associations.** If the combination of Master No and Vendor No already exists, the import updates the existing record rather than creating a duplicate. Verify the updated values are correct on the Vendors tab of the master record.
