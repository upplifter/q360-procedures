---
title: Pick Items
id: WH-PICK-001
module: Warehouse
screen: Parts Pick Form
menu_path: Workflow > Warehouse > Items to Pick
applies_to:
  - Warehouse Staff
prerequisites:
  - Order is in APPROVED, PARTSHIP, or PICKQ status
  - Items are on-hand in inventory
  - Items are not marked for drop-ship
  - Pick lines are not locked or frozen
related_procedures:
  - WH-PICK-002
  - WH-PICK-003
  - WH-SHIP-001
tags: picking, order fulfillment, item picking, inventory allocation
version: 1.0
last_updated: 2026-03-25
---

# Pick Items

## What This Procedure Does

Pick order items from inventory by scanning or entering product identifiers and asset serial numbers. Once all items are picked, the order is ready for shipment. The system tracks which items have been picked and their status.

## Before You Begin

- Order is in APPROVED, PARTSHIP, or PICKQ status (visible in Items to Pick bucket)
- All items are on-hand and available in inventory
- Items are not marked for drop-ship or service work
- Order is not RECURRING (recurring orders use separate fulfillment process)
- Pick lines have not been locked or frozen by management

## Steps

### Step 1: Open the Workflow

Navigate to **Workflow > Warehouse** on the left navigation sidebar.

### Step 2: Select Order from Items to Pick Bucket

In the Warehouse Workflow dashboard, locate the **Items to Pick** bucket, which displays all order items ready for picking.

The bucket shows orders in APPROVED, PARTSHIP, or PICKQ status and excludes drop-ship orders.

Scan or search for the order number, or scroll through the list to find the order.

Click the order number to open the Parts Pick Form.

### Step 3: Review Pick Screen Color Codes

The pick screen uses color codes to indicate pickability:

- **Green** = Item is fully approved and ready to pick
- **White** = Item is approved but not yet approved for shipment (can pick but cannot ship)
- **Yellow** = Item is partially pickable (some quantity available, but not all)
- **Red** = Item has no available inventory to pick
- **Yellow (non-inventory)** = Item is non-inventory and auto-picked

Verify items show green or yellow status before attempting to pick.

### Step 4: Pick A-Type Items (Serialized Assets)

For each A-type (asset) line item, scan or manually enter the serial number of the physical unit.

| Field | What to enter |
|-------|---------------|
| Serial Number | Scan or type the unique serial/asset number from the unit |
| Quantity | Automatically fills as 1 for A-type items |

Verify the serial number on the screen matches the physical item in your hand.

Click the **Add** button or press Enter to record the pick.

The item status changes from Available to Scanned (picked).

### Step 5: Pick Q-Type Items (Quantity-Tracked)

For each Q-type (quantity-tracked) line item, enter the quantity to pick.

| Field | What to enter |
|-------|---------------|
| Quantity | Enter the number of units to pick |
| Unit of Measure | Confirm matches the order line (each, case, box, etc.) |

Verify the quantity matches the order line item.

Click the **Add** button to record the pick.

The system reduces available inventory and marks the item as picked.

### Step 6: Confirm All Picks

Review all line items on the pick form to ensure all items have been picked and no items remain unpicked.

If any items show red (not available) and must be excluded, confirm with management that partial shipment is acceptable.

Click the **Save** button (floppy disk icon) to finalize all picks.

### Step 7: Proceed to Shipment

Once all picks are saved, the order is ready for verification and shipment. Proceed to WH-PICK-003 to verify serial numbers, then proceed to WH-SHIP-001 to ship the order.

## What Happens Next

Picked items are marked as SHIPQ status and moved into the Items to Ship bucket. Inventory is committed to the order and unavailable for other picks. The packing slip can now be printed when the order ships. Asset status changes to Scanned for A-type items.

## Common Issues

**Item shows red (not available) on pick screen**
This indicates no inventory is available for this item. Check on-hand levels (see WH-INV-001) to verify stock is in the system. If stock exists but is not available, it may be allocated to another order or missing due to unreceived purchases. Contact Warehouse Manager to clear allocations or investigate discrepancy.

**Serial number will not scan or is rejected**
Verify the serial number on the physical unit matches the order documentation. Check for leading or trailing spaces or special characters when entering manually. If the serial does not match any record on the order, verify you have the correct item. Do not force a mismatch; escalate to Warehouse Manager.

**Cannot save pick due to locked or frozen line**
Management may have locked the pick lines to prevent changes. Contact Warehouse Manager to unlock the order before continuing. Do not force modifications to locked picks.

**Pick appears to complete but items still show in Items to Pick bucket**
Refresh the Warehouse Workflow dashboard by clicking the Refresh icon (circular arrow). The bucket updates to remove completed picks within a few seconds. If items remain after refresh, confirm the Save operation completed without errors.

**Partial quantity available for item on order**
If only some of the requested quantity is available, you can pick the available amount and leave the remainder unpicked. This places the order in partial ship status. Confirm with management that partial shipment is acceptable before saving. The unpicked quantity can be picked in a follow-up transaction once additional stock arrives.
