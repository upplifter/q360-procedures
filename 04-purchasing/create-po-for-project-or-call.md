---
title: Create PO for Project or Service Call
id: PO-CREATE-001
module: Purchasing
screen: Purchasing Workflow
menu_path: Workflow > Purchasing
applies_to:
  - Purchasing Agent
  - Purchasing Manager
  - Project Manager
prerequisites:
  - User has permission to access the Purchasing workflow
  - An approved customer order exists with line items requiring procurement
  - Vendor records exist for the items to be purchased (see PO-VENDOR-001)
  - Master records exist for all items (see PO-MASTER-001)
related_procedures:
  - PO-MASTER-001
  - PO-MASTER-004
  - PO-VENDOR-001
  - PO-SEND-001
  - PO-DROPSHIP-001
  - PO-LINK-001
tags: create PO, purchase order, project PO, service call PO, purchasing workflow, items to purchase, procurement, buy materials
version: 1.0
last_updated: 2026-03-25
---

# Create PO for Project or Service Call

## What This Procedure Does

Select items from the Purchasing workflow Items to Purchase bucket and create purchase orders for project materials or service call parts. This is the primary method for procuring items tied to approved customer orders.

## Before You Begin

- You need permission to access the Purchasing workflow and create purchase orders.
- A customer order must be approved with line items that require purchasing.
- Master records must exist for all items. If an item has no master, create one first (see PO-MASTER-004).
- Vendors must be associated with the master items, or you must manually assign vendors during this process.
- Review inventory levels to determine if stock already covers the requirement (see PO-MASTER-001).

## Steps

### Step 1: Open the Purchasing Workflow

Navigate to **Workflow > Purchasing** from the Main Navigation Sidebar (vertical panel, left edge). The Purchasing workflow canvas opens showing colored bucket nodes with counts.

### Step 2: Set Workflow Filters

Use the filters at the top of the workflow to narrow results by Company, Branch, Department, or Project Type as needed.

### Step 3: Open the Items to Purchase Queue

Click the **Count of Items to Purchase** bucket on the workflow canvas. The Items to Purchase grid opens, listing all order line items pending procurement. Items are filtered by PO Release Date of today or earlier.

### Step 4: Verify Inventory Levels

Review each item's quantity against the master inventory On Hand and Available columns. If sufficient stock exists, the item may not need a new PO. For items that need purchasing, proceed to the next step.

### Step 5: Split Quantities (If Needed)

If you need to order only a partial quantity from one vendor and the remainder from another, select the line item and use the **Split** function to divide the quantity into separate rows for independent vendor assignment.

### Step 6: Handle Items Without a Master

If any items appear in the **Count of Unverified Items on Quote/Order** bucket, they lack master records. Click the grid **Add** button (plus icon on the Grid Toolbar) to create an A-type or Q-type master directly from the queue (see PO-MASTER-004).

### Step 7: Mark Drop Ship Items (If Applicable)

For items that should ship directly from the vendor to the customer site, select the items in the grid, then click **Grid Extended Menu** (three vertical dots on the Grid Toolbar) and choose **Toggle Drop Ship for Selected Items**. Drop ship items display in yellow. See PO-DROPSHIP-001 for details.

### Step 8: Assign Vendors

Verify that each line item has a vendor assigned. If a vendor is missing, select the item(s), click the **Grid Extended Menu** (three vertical dots), and choose **Choose a Vendor**. Select the appropriate vendor from the list.

### Step 9: Create Purchase Orders

Select all items ready for ordering by checking the **Row Selector** (checkbox in the far-left column). Click the **Grid Extended Menu** (three vertical dots) and choose **Create Purchase Orders for Selected Items**. A prompt asks whether to use order line item costs. Select your preference.

1. Choose **Yes** to carry the order's negotiated costs onto the PO.
2. Choose **No** to use the standard master-vendor cost.

Q360 groups the selected items by vendor and creates one PO per vendor.

### Step 10: Review the Created POs

The newly created POs open in DATAENTRY status. Review each PO for accuracy, including vendor, line items, quantities, and costs. Make any necessary edits while the PO is in DATAENTRY status.

## What Happens Next

The POs appear in the **Count of POs to Confirm** bucket on the Purchasing workflow. Proceed to confirm and send each PO to the vendor (see PO-SEND-001). Items on the PO are reflected in the master inventory On Order quantity. The PO line items are automatically linked to the originating order line items.

## Common Issues

**Items do not appear in the Items to Purchase queue.** The PO Release Date on the order line item may be in the future. Check the order's material schedule. Also verify the order status is APPROVED and the workflow filters match the order's company, branch, and department.

**Vendor is not assigned to a line item.** The master record may not have a vendor association. Use the extended menu to Choose a Vendor manually, or set up the master-vendor relationship (see PO-MASTER-003) for future orders.

**Cannot create PO - "Unverified item" error.** The line item does not have a valid master number. Create a master record for the item first (see PO-MASTER-004), then return to the Items to Purchase queue.

**PO created with incorrect cost.** If you selected the wrong cost option during PO creation, edit the PO while it is still in DATAENTRY status. Update the unit cost on the line items and save.

**Items split incorrectly.** If the split quantities are wrong, you can re-merge the rows by selecting them and using the appropriate extended menu option, then split again with the correct quantities.
