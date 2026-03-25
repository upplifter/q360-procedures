---
title: Link or Unlink PO Item to Order Item
id: PO-LINK-001
module: Purchasing
screen: Purchase Order Form
menu_path: Inventory > Purchase Orders
applies_to:
  - Purchasing Agent
  - Purchasing Manager
prerequisites:
  - User has permission to edit purchase order line items
  - A PO exists with line items that need to be linked or unlinked from order items
  - The target order item exists on an approved customer order
related_procedures:
  - PO-CREATE-001
  - PO-SEND-001
tags: link PO, unlink PO, PO to order, order item link, purchase order link, reassign PO, PO item association, change PO link
version: 1.0
last_updated: 2026-03-25
---

# Link or Unlink PO Item to Order Item

## What This Procedure Does

Link a PO line item to a specific customer order line item, or unlink an existing association. Linking connects the purchased item to the order it fulfills, enabling end-to-end tracking from purchase through receiving, picking, and shipping. Unlinking breaks this association, typically when a PO item needs to be reassigned to a different order or when the original order changes.

## Before You Begin

- You need edit permission on purchase order line items.
- Know the PO number and line item to link or unlink.
- For linking, know the target order number and line item number.
- The PO must be in a status that allows editing (DATAENTRY or as permitted by your configuration).

## Steps

### Step 1: Open the Purchase Order

Navigate to **Inventory > Purchase Orders** from the Main Navigation Sidebar (vertical panel, left edge). Search for the PO using the Form Quick Search (text input at the top-left of the form tab) or browse from the Purchasing workflow.

### Step 2: Navigate to the Line Items Tab

Click the **Line Items** tab to view the PO's line items.

### Step 3: Link a PO Item to an Order Item

1. Select the line item you want to link.
2. Click the **Grid Extended Menu** (three vertical dots on the Grid Toolbar).
3. Choose **Link to Order Item** or the equivalent option.
4. A selection dialog opens showing available order line items that match the master number.
5. Select the target order and line item from the list.
6. Click **OK** or **Save** to confirm the link.

The PO line item now displays the linked order number and line item reference.

### Step 4: Unlink a PO Item from an Order Item

1. Select the linked line item you want to unlink.
2. Click the **Grid Extended Menu** (three vertical dots on the Grid Toolbar).
3. Choose **Unlink from Order Item** or the equivalent option.
4. Confirm the unlink action when prompted.

The PO line item is now disassociated from the order. The item remains on the PO but is no longer tied to a specific customer order.

### Step 5: Save the Changes

Click the **Save Record** button (floppy disk icon on the Form Action Bar) to save the updated link or unlink.

## What Happens Next

When a PO item is linked to an order item, receiving the PO item in the warehouse updates the order's material status. The order line item shows the linked PO and its receiving status, providing visibility into procurement progress (see PROJ-MAT-002). Unlinked PO items return to the general inventory upon receiving and must be separately picked and assigned to fulfill orders. If you need to reassign the PO item to a different order, unlink it first, then link it to the new order item.

## Common Issues

**Link option is not available in the extended menu.** The PO may be in a status that does not allow linking, or you may lack the required permission. Check the PO status and your user permissions.

**No matching order items appear in the link dialog.** The master number on the PO line item must match the master number on the order line item. Verify both records reference the same master. If the order item uses a different master, the link cannot be made directly.

**Unlinked item went to general stock instead of a specific order.** After unlinking, the PO item is no longer associated with any order. When received, it goes to general inventory. To assign it to an order, either re-link it before receiving or pick it from stock after receiving.

**PO item was already received before unlinking.** If the PO item has been received, the inventory is already allocated. Unlinking after receiving does not move the physical inventory. Coordinate with the warehouse team to handle the item allocation.

**Order was cancelled after PO item was linked.** If the customer order is cancelled, the linked PO item should be reviewed. Either cancel the PO line item if the item is no longer needed, or unlink it and reassign to another order or stock replenishment.
