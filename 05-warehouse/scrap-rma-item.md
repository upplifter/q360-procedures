---
title: Scrap an RMA Item
id: WH-RMA-002c
module: Warehouse
screen: RMA Test Queue
menu_path: Workflow > Warehouse > RMA to Test
applies_to:
  - Warehouse Manager
prerequisites:
  - RMA item has been received (see WH-RMA-001)
  - Scrap GL account is configured on master
related_procedures:
  - WH-RMA-001
  - WH-RMA-002a
  - WH-ADJUST-001c
tags: rma, scrap, disposition, inventory-writeoff
version: 1.0
last_updated: 2026-03-25
---

# Scrap an RMA Item

## What This Procedure Does

This procedure dispositions a received RMA item as scrap and records the inventory write-off to the general ledger. The asset status is changed to Scrapped and the inventory value is removed from the system.

## Before You Begin

- Verify the RMA item has been received and is in the RMA Test Queue
- Confirm the item is determined to be non-repairable or non-returnable
- Verify the scrap GL account is configured on the master record
- Have the RMA number available

## Steps

### Step 1: Navigate to the RMA Test Queue

Go to Workflow > Warehouse > RMA to Test. The system displays all received RMA items awaiting disposition.

### Step 2: Select the RMA Item

Click the RMA item you want to scrap. The system opens the item details.

### Step 3: Select Disposition

Locate the disposition dropdown and select **Scrap**. This action marks the item for scrapping and inventory write-off.

### Step 4: Confirm the Disposition

Click the Process Actions gear icon and select **Confirm**. The system records the scrap disposition, writes off the inventory value to the configured scrap GL account, and changes the asset status to Scrapped.

## What Happens Next

The item is removed from available inventory. The inventory value is written off to the scrap GL account in Accounting. Quantity on hand decreases and the asset record is marked as Scrapped. The transaction is recorded in the audit trail for future reference. The scrapped item should be physically disposed of according to company policy.

## Common Issues

**Scrap GL account is not configured**
The asset master record must have a scrap GL account assigned before the scrap disposition can be confirmed. Contact accounting to configure the scrap account on the master record.

**Cannot select Scrap option**
Verify that you have warehouse manager permissions. If permissions are correct, the system may be preventing scrap disposition if the item is still allocated to an active order. Check for any pending allocations.

**Item status shows Scrapped but inventory was not written off**
If the GL write-off did not post, contact accounting to verify the scrap GL account is active and reconcile the transaction manually. Check the audit trail to confirm the scrap disposition was recorded.

**Scrap disposition was selected in error**
Scrap dispositions cannot be reversed through the RMA interface. Contact warehouse management and accounting immediately to request a manual reversal journal entry if the item was scrapped in error.
