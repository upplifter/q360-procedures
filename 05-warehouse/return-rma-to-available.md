---
title: Return an RMA Item to Available Stock
id: WH-RMA-002a
module: Warehouse
screen: RMA Test Queue
menu_path: Workflow > Warehouse > RMA to Test
applies_to:
  - Warehouse Manager
  - Warehouse Staff
prerequisites:
  - RMA item has been received (see WH-RMA-001)
  - Item passes inspection
related_procedures:
  - WH-RMA-001
  - WH-RMA-002b
  - WH-RMA-002c
tags: rma, disposition, returns, inventory
version: 1.0
last_updated: 2026-03-25
---

# Return an RMA Item to Available Stock

## What This Procedure Does

This procedure returns a received RMA item to available inventory after inspection and testing have been completed. The item is restored to usable stock at its original cost.

## Before You Begin

- Verify the RMA item has been received and is in the RMA Test Queue
- Physically inspect and test the item
- Confirm the item passes all quality checks
- Have the RMA number available

## Steps

### Step 1: Navigate to the RMA Test Queue

Go to Workflow > Warehouse > RMA to Test. The system displays all received RMA items awaiting disposition.

### Step 2: Select the RMA Item

Click the RMA item you want to return to available stock. The system opens the item details.

### Step 3: Select Disposition

Locate the disposition dropdown and select **Return to Available**. This action restores the item to the active inventory pool.

### Step 4: Confirm the Disposition

Click the Process Actions gear icon and select **Confirm**. The system updates the item status and returns it to available inventory at the original cost.

## What Happens Next

The item is moved from the RMA Test Queue back to available stock. Quantity on hand increases, and the item is now available for allocation to new orders. The RMA disposition is recorded in the audit trail.

## Common Issues

**Item does not appear in RMA Test Queue**
The item may still be in transit or not yet received. Check the receiving log to confirm the RMA was delivered. If received, contact warehouse management to verify the item was properly checked in.

**Cannot select Return to Available option**
The disposition may be locked if another user is processing the same RMA. Refresh the screen and try again. If the issue persists, check that you have the correct permissions to disposition RMA items.

**Item status shows as Scrapped instead of returning to stock**
If the wrong disposition was selected in error, contact warehouse management immediately. The scrap disposition cannot be reversed without a manual GL adjustment.
