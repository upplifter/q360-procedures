---
title: Create Stock PO
id: PO-CREATE-002
module: Purchasing
screen: Purchase Order Form
menu_path: Inventory > Purchase Orders
applies_to:
  - Purchasing Agent
  - Warehouse Manager
prerequisites:
  - User has permission to create purchase orders
  - A vendor record exists for the supplier (see PO-VENDOR-001)
  - Master records exist for the stock items to order (see PO-MASTER-001)
related_procedures:
  - PO-MASTER-001
  - PO-VENDOR-001
  - PO-SEND-001
  - PO-UPDATE-001
tags: stock PO, stock purchase order, replenishment, reorder, inventory replenishment, stock reorder, warehouse stock, vendor PO
version: 1.0
last_updated: 2026-03-25
---

# Create Stock PO

## What This Procedure Does

Create a purchase order for stock replenishment that is not tied to a specific project or service call. This is used to maintain warehouse inventory levels based on minimum quantity thresholds or anticipated demand.

## Before You Begin

- You need permission to create purchase orders.
- A vendor record must exist for the supplier (see PO-VENDOR-001).
- Master records must exist for the items you plan to order (see PO-MASTER-001).
- Review current inventory levels to confirm which items need replenishment. The Purchasing workflow's **Count of Stock Items Needing Reorder** bucket identifies items below their minimum quantity threshold.

## Steps

### Step 1: Review Stock Items Needing Reorder

Navigate to **Workflow > Purchasing** from the Main Navigation Sidebar (vertical panel, left edge). Click the **Count of Stock Items Needing Reorder** bucket on the workflow canvas to see items whose current inventory has fallen below the Min Qty threshold. The grid displays quantity levels including Qty Min, Qty Max, Description, Vendor No, Manufacturer, and Vendor Name.

### Step 2: Open the Purchase Order Form

Navigate to **Inventory > Purchase Orders** from the Main Navigation Sidebar. Click the **Add New Record** button (plus icon on the Form Action Bar) to create a new PO.

### Step 3: Enter PO Header Information

| Field | What to enter |
| --- | --- |
| Vendor | Select the vendor from the lookup. The vendor's address and payment terms auto-populate. |
| Company | Select or confirm the company number. |
| Branch | Select the branch receiving the stock. |
| PO Date | Defaults to today. Adjust if needed. |
| Ship To | Select the warehouse or branch location where the stock will be received. |

### Step 4: Add Line Items

Click the **Line Items** tab. Click the grid **Add** button (plus icon on the Grid Toolbar) to add items to the PO.

| Field | What to enter |
| --- | --- |
| Master No | Search for and select the master item to order. |
| Description | Auto-populates from the master record. Edit if needed for this specific order. |
| Quantity | Enter the quantity to order. Reference the reorder quantity and max quantity from the master record. |
| Unit Cost | Auto-populates from the master-vendor association. Override if a different price was negotiated. |

Repeat for each item to be ordered. Multiple items from the same vendor can be added to a single PO.

### Step 5: Save the PO

Click the **Save Record** button (floppy disk icon on the Form Action Bar). The PO is saved in DATAENTRY status.

### Step 6: Review and Verify

Review all line items for correct quantities and costs. Make any necessary edits while the PO is in DATAENTRY status.

## What Happens Next

The PO appears in the **Count of POs to Confirm** bucket on the Purchasing workflow. Proceed to confirm and send the PO to the vendor (see PO-SEND-001). Once confirmed and received, the stock items increase the On Hand inventory at the specified branch. Stock PO items are not linked to any specific customer order.

## Common Issues

**Stock items do not appear in the reorder bucket.** The Min Qty field on the master record must be set for the item to trigger reorder alerts. Open the master record and configure the Min Qty and Reorder Qty fields.

**Vendor not available in the PO vendor lookup.** The vendor record must be of type CUSTVEND. Verify the vendor exists and has the correct type (see PO-VENDOR-001).

**Unit cost is zero on the PO line item.** The master-vendor association may not have a cost entered. Update the vendor cost on the master record's Vendors tab, or manually enter the cost on the PO line item.

**PO was saved but cannot be edited.** If the PO has been confirmed (moved past DATAENTRY status), it cannot be edited directly. Contact your purchasing manager or use the appropriate process to revert the PO status if changes are needed.

**Ship To location is incorrect.** Verify the Ship To field on the PO header matches the warehouse branch where the stock should be received. Changing this after line items are added may require re-saving the PO.
