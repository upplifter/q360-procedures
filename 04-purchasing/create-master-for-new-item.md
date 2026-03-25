---
title: Create Master for New Item to Purchase
id: PO-MASTER-004
module: Purchasing
screen: Master Inventory Form
menu_path: Inventory > Master Inventory
applies_to:
  - Purchasing Agent
  - Warehouse Manager
  - System Administrator
prerequisites:
  - User has permission to create master inventory records
  - Item details including manufacturer, description, and cost are known
  - The item does not already exist as a master record (see PO-MASTER-001)
related_procedures:
  - PO-MASTER-001
  - PO-MASTER-002
  - PO-MASTER-003
  - PO-CREATE-001
tags: create master, new master, new item, master inventory, A-type, Q-type, unverified item, add part number, new part, create part
version: 1.0
last_updated: 2026-03-25
---

# Create Master for New Item to Purchase

## What This Procedure Does

Create a new A-type (asset/serialized) or Q-type (quantitative) master inventory record for an item that needs to be purchased but does not yet exist in Q360. This resolves unverified line items on quotes or orders and enables the item to flow through the purchasing workflow.

## Before You Begin

- You need create permission for the Master Inventory form.
- Search for the item first to confirm it does not already exist (see PO-MASTER-001).
- Have the following information ready: manufacturer name, item description, category, standard cost, and standard price or pricing factor.
- Know whether the item is serialized (A-type) or non-serialized/bulk quantity (Q-type).

## Steps

### Step 1: Open the Master Inventory Form

Navigate to **Inventory > Master Inventory** from the Main Navigation Sidebar (vertical panel, left edge). The Master Inventory form opens in a new tab.

Alternatively, if you are in the Purchasing workflow and an unverified item appears in the Items to Purchase queue, click the grid **Add** button (plus icon on the Grid Toolbar) to create a master directly from the queue.

### Step 2: Add a New Record

Click the **Add New Record** button (plus icon on the Form Action Bar). A blank master record form opens.

### Step 3: Enter Master Header Information

| Field | What to enter |
| --- | --- |
| Master No | A unique identifier for the item. Follow your organization's naming convention. |
| Description | A clear description of the item. |
| Master Type | Select **A** for serialized/asset items or **Q** for quantity-tracked items. |
| Manufacturer | Select or enter the manufacturer name. |
| Category | Select the appropriate item category from the dropdown. |

### Step 4: Enter Cost and Pricing Information

| Field | What to enter |
| --- | --- |
| Standard Cost | The default purchase cost for this item. Used for inventory valuation. |
| Standard Price | The default selling price. Alternatively, enter a pricing factor that calculates the price from cost. |
| Sales Taxable | Check this box if the item is subject to sales tax. |

### Step 5: Configure Inventory Settings

| Field | What to enter |
| --- | --- |
| Auto Pick | Check this box if the item should be automatically picked when orders are processed. |
| Reorder Qty | The quantity to reorder when stock falls below the minimum. |
| Min Qty | The minimum inventory level that triggers a reorder alert. |
| Max Qty | The maximum inventory level to maintain. |

### Step 6: Save the Record

Click the **Save Record** button (floppy disk icon on the Form Action Bar). Q360 assigns the master number and saves the record.

### Step 7: Add Vendor Association (If Known)

Click the **Vendors** tab on the master record. Click the grid **Add** button (plus icon) to add a vendor association.

| Field | What to enter |
| --- | --- |
| Vendor No | Select the vendor who supplies this item. |
| Vendor Part No | The vendor's own part number or SKU. |
| Cost | The vendor's unit cost. |
| Lead Time | Expected days from order to delivery. |
| Primary | Check this box to designate as the default vendor for purchasing. |

Click **Save** to store the vendor association.

## What Happens Next

The new master record is immediately available throughout Q360. Unverified line items on quotes or orders that match this master number are resolved. The item appears in the Purchasing workflow for procurement (see PO-CREATE-001). If you need to set up vendor associations in bulk, use the Import or Update Master Vendors function (see PO-MASTER-003).

## Common Issues

**Master number already exists.** The Master No you entered is already in use. Search for the existing record (see PO-MASTER-001) to verify whether it is the same item. If it is a different item, choose a unique master number.

**Item still shows as unverified on the order.** The master number on the order line item must match the new master record exactly. Edit the order line item and re-select the master number from the lookup, then save.

**Cannot determine whether to use A-type or Q-type.** Use A-type for items that are individually tracked by serial number or asset tag, such as cameras, panels, or controllers. Use Q-type for bulk consumable items tracked only by quantity, such as cable, connectors, or screws.

**Standard cost and price are unknown.** Enter the best available estimate. The cost can be updated later when a vendor quote is received. The master-vendor association cost takes priority over the standard cost during PO creation.

**Vendor tab is empty after save.** Adding a vendor association is a separate step. After saving the master record, navigate to the Vendors tab and add the vendor. Alternatively, import vendor associations in bulk (see PO-MASTER-003).
