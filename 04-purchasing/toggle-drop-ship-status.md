---
title: Toggle Drop Ship Status
id: PO-DROPSHIP-001
module: Purchasing
screen: Purchasing Workflow
menu_path: Workflow > Purchasing
applies_to:
  - Purchasing Agent
  - Purchasing Manager
prerequisites:
  - User has permission to access the Purchasing workflow
  - Order line items exist in the Items to Purchase queue
  - The vendor can ship directly to the customer site
related_procedures:
  - PO-CREATE-001
  - PO-SEND-001
tags: drop ship, dropship, direct ship, vendor to customer, toggle drop ship, skip warehouse, direct delivery, yellow flag
version: 1.0
last_updated: 2026-03-25
---

# Toggle Drop Ship Status

## What This Procedure Does

Mark or unmark order line items in the Purchasing queue for direct vendor-to-customer delivery (drop ship). Drop ship items bypass the warehouse - the vendor ships directly to the customer site. When received in Q360, drop ship items are automatically shipped on the linked order.

## Before You Begin

- You need permission to access the Purchasing workflow and modify order line items.
- Confirm with the vendor that direct shipment to the customer site is supported.
- Know the customer's delivery address for the drop ship.
- The items must be in the Items to Purchase queue on the Purchasing workflow.

## Steps

### Step 1: Open the Purchasing Workflow

Navigate to **Workflow > Purchasing** from the Main Navigation Sidebar (vertical panel, left edge). The Purchasing workflow canvas opens.

### Step 2: Open the Items to Purchase Queue

Click the **Count of Items to Purchase** bucket on the workflow canvas. The Items to Purchase grid opens listing order line items pending procurement.

### Step 3: Select Items for Drop Ship

Identify the items that should ship directly from the vendor to the customer. Click the **Row Selector** (checkbox in the far-left column) to select one or more line items.

### Step 4: Toggle the Drop Ship Flag

Click the **Grid Extended Menu** (three vertical dots on the Grid Toolbar) and choose **Toggle Drop Ship for Selected Items**. The selected items are now flagged for drop ship. Drop ship items display in **yellow** in the grid to visually distinguish them from standard warehouse-routed items.

To remove the drop ship flag, select the yellow-highlighted items and choose **Toggle Drop Ship for Selected Items** again. The flag toggles off and the items return to normal color.

### Step 5: Continue with PO Creation

Proceed to assign vendors and create purchase orders for the flagged items (see PO-CREATE-001). Drop ship items appear on the PO with a drop ship indicator.

## What Happens Next

Drop ship items appear in the **Count of Drop Ship Items** bucket on the Purchasing workflow for tracking. When the PO is received in Q360, the system automatically processes the linked order item as shipped, skipping the warehouse pick and ship steps. The items are received into a designated drop ship location. In the PO Receive Queue, drop ship items display in yellow, and at least one item marked for drop ship shows as ready to be received. On the Orders Pick Queue and Shipping Queue, drop ship items also display in yellow to indicate they follow a different fulfillment path.

## Common Issues

**Drop ship flag does not appear after toggling.** Verify you selected the correct items before clicking the toggle option. Refresh the grid and check if the items now display in yellow. If the toggle did not take effect, ensure you have the required permission.

**Item was flagged as drop ship by mistake.** Select the item and use **Toggle Drop Ship for Selected Items** again to remove the flag. This must be done before the PO is created and confirmed.

**Drop ship item was received but order did not auto-ship.** Verify the PO line item is properly linked to the order line item (see PO-LINK-001). The auto-ship on receiving only works when the link between the PO item and order item is intact.

**Customer address is not correct on the drop ship PO.** The ship-to address on the PO should reflect the customer's delivery site, not the warehouse. Verify the address on the PO header before confirming and sending to the vendor.

**Inventory shows in a drop ship location instead of main warehouse.** This is expected behavior. Drop ship items are received into a designated drop ship location in Q360. They do not increase the main warehouse On Hand count because they are immediately associated with the customer delivery.
