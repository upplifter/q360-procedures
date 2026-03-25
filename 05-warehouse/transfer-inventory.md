---
title: Transfer Inventory
id: WH-TRANSFER-001
module: Warehouse
screen: Inventory Transfer
menu_path: Workflow > Warehouse > Transfer Inventory OR Inventory > Inventory Transfer
applies_to:
  - Warehouse Staff
  - Warehouse Manager
prerequisites:
  - Inventory is available at source branch
  - User has transfer permission in both branches
  - Receiving branch has capacity for transferred inventory
  - Both source and destination branches are active
related_procedures:
  - WH-INV-001
  - WH-TECH-001
tags: inventory transfer, branch transfer, stock rebalancing, inter-branch transfer
version: 1.0
last_updated: 2026-03-25
---

# Transfer Inventory

## What This Procedure Does

Transfer A-type (serialized) or Q-type (quantity-tracked) inventory between warehouse branches. Use this procedure to rebalance stock, move items to meet customer demand, or consolidate inventory across locations.

## Before You Begin

- Inventory is available and on-hand at the source branch
- User has transfer permission in both source and destination branches
- Receiving branch has space and capacity for the transfer
- Both branches are active and operational
- For A-type items, serial numbers are known and accessible

## Steps

### Step 1: Open Inventory Transfer Screen

Navigate to **Workflow > Warehouse** and click **Transfer Inventory** to open the Inventory Transfer screen.

Alternatively, navigate to **Inventory > Inventory Transfer** from the left navigation sidebar.

### Step 2: Select Source Branch

On the Inventory Transfer form, select the **Source Branch** from the dropdown menu.

| Field | What to enter |
|-------|---------------|
| Source Branch | Select the branch where inventory currently resides |
| Company | Automatically populated based on source branch selection |

Verify the correct branch is selected before proceeding.

### Step 3: Select Destination Branch

Select the **Destination Branch** from the dropdown menu.

| Field | What to enter |
|-------|---------------|
| Destination Branch | Select the branch that will receive the inventory |

The destination branch must be different from the source branch.

### Step 4: Add Master Items to Transfer

Click the **Add** button (plus icon) to add a master item to the transfer list.

A dialog or form appears to select the master product to transfer.

| Field | What to enter |
|-------|---------------|
| Master Product | Search for and select the product to transfer |
| Product Code | Confirm the code matches the intended product |

Select the master and confirm the selection.

### Step 5: Specify A-Type Items (Serialized Assets)

For A-type (serialized) items, you must select the specific asset serial numbers to transfer.

The form displays a list of available assets at the source branch.

Check the checkbox next to each serial number you want to transfer.

| Field | What to check |
|--------|---------------|
| Serial Number | Confirm the asset serial to be transferred |
| Asset Status | Verify status is Available (not Picked, Shipped, or Missing) |

You can transfer one or multiple assets of the same master in a single transfer.

### Step 6: Specify Q-Type Items (Quantity-Tracked)

For Q-type (quantity-tracked) items, enter the quantity to transfer.

| Field | What to enter |
|-------|---------------|
| Quantity | Enter the number of units to transfer from source to destination |
| Unit of Measure | Confirm matches the master (each, case, box, etc.) |

Verify the quantity does not exceed on-hand availability at the source branch.

### Step 7: Review Transfer Details

Review the complete transfer list with all masters, serial numbers (for A-type), and quantities (for Q-type).

Verify source and destination branches are correct.

Confirm the total quantity being transferred is accurate.

### Step 8: Save and Submit Transfer

Click the **Save** button (floppy disk icon) to record the transfer.

The transfer is created with status IN TRANSIT or PENDING, depending on system configuration.

The audit trail records the transfer with timestamp, user name, and transfer details.

### Step 9: Receiving Branch Confirms Receipt

At the destination branch, the transfer appears as an inbound receipt.

Warehouse staff at the destination branch must receive the transfer to complete it (process varies by configuration).

Physical inventory arrives at destination branch and is received into inventory.

Transfer status changes to COMPLETED once received.

## What Happens Next

Inventory is removed from the source branch on-hand count and added to the destination branch on-hand count. Asset status remains Available. Items can now be picked for orders at the destination branch. The transfer history is recorded in the audit trail for both branches. Stock levels are updated on inventory reports for both locations.

## Common Issues

**Cannot select destination branch**
Verify the destination branch is active and operational in the system. The branch may be closed, archived, or restricted. Contact system administrator if the branch does not appear in the dropdown menu.

**Source branch does not have sufficient quantity**
Verify on-hand inventory at the source branch using the Find Product screen (see WH-INV-001). If on-hand is lower than expected, committed or picked inventory may not be available for transfer. Transfer only the available quantity, or unpick items to free up inventory (see WH-PICK-002).

**A-type asset serial number not available for selection**
The asset may be in Picked, Shipped, or Missing status. Only assets with Available status can be transferred. Verify the asset is not allocated to an order or shipment. Contact Warehouse Manager if the asset status is incorrect.

**Transfer created but inventory not updated at destination**
The transfer may be pending receipt at the destination branch. Contact Warehouse Manager at the destination location to complete the receipt. The transfer remains IN TRANSIT until received and confirmed.

**Cannot save transfer due to permission error**
Verify your user account has Warehouse Staff or Manager privileges in both the source and destination branches. Contact system administrator if permissions are insufficient. Transfer permission may be restricted by branch or user role.
