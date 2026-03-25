---
title: Adjust Quantity for Q-Type Master
id: WH-ADJUST-001a
module: Warehouse
screen: Master Form (Q-Type)
menu_path: Inventory > Masters > [search Q-type master]
applies_to:
  - Warehouse Manager
prerequisites:
  - Master is Q-type (quantity-based, not serialized)
  - User has inventory adjustment permission
related_procedures:
  - WH-INV-001
  - WH-ADJUST-001b
tags: inventory adjustment, Q-type, quantity, master
version: 1.0
last_updated: 2026-03-25
---

# Adjust Quantity for Q-Type Master

## What This Procedure Does

Adjust on-hand quantities for a Q-type (quantity-based) inventory master using the Adjust Quantities command. This is used for quick corrections when inventory count discrepancies are found outside of a formal physical inventory count, or for ongoing cycle count adjustments.

## Before You Begin

- The master you want to adjust is Q-type (quantity-based), not A-type (serialized/asset)
- You know the current on-hand quantity and the correct quantity to which it should be adjusted
- You have Warehouse Manager role and inventory adjustment permissions
- You have a reason or reference for the adjustment (e.g., cycle count variance, damage found, etc.)

## Steps

### Step 1: Search and Open the Master

Navigate to **Inventory > Masters**. Use the search field to locate the Q-type master you want to adjust. Type the master number, description, or code.

Click on the master in the search results or press **Enter** to open the master form.

### Step 2: Access Extended Menu

On the master form, click the **Extended Menu** button (three vertical dots) in the toolbar. A menu appears with additional options for the master.

### Step 3: Select Adjust Quantities

From the Extended Menu, click **Adjust Quantities**. The Adjust Quantities dialog opens.

The dialog displays:

- Master number and description
- Current on-hand quantity
- Adjustment amount field
- Reason/Reference field

### Step 4: Enter Adjustment Quantity

In the adjustment amount field, enter the quantity change:

- **Positive number** (e.g., +5) to add quantity to on-hand
- **Negative number** (e.g., -3) to reduce quantity from on-hand

For example:

- If on-hand is 100 and physical count is 105, enter +5
- If on-hand is 100 and physical count is 97, enter -3

The system will calculate the new on-hand quantity and display it as a preview.

### Step 5: Enter Reason or Reference

In the Reason or Reference field, enter a brief explanation for the adjustment:

- "Cycle count variance - bin 3C"
- "Damaged units found and scrap"
- "Receiving discrepancy correction"
- "Count sheet recount variance"

This reason is recorded in the audit trail and GL entries for tracking and compliance purposes.

### Step 6: Confirm and Save

Click the **Save** button (floppy disk icon) or **OK** button in the dialog. The system processes the adjustment:

1. On-hand quantity is updated to the new amount
2. A GL journal entry is created to record the adjustment in the inventory account
3. The adjustment reason is logged in the master's transaction history

The Adjust Quantities dialog closes and you return to the master form. The on-hand quantity now reflects the adjustment.

## What Happens Next

The on-hand quantity for the Q-type master is immediately updated in the system. The adjustment is reflected in:

- Inventory availability for sales orders and allocations
- On-hand quantity reports and inquiries
- GL inventory accounts (debit or credit depending on adjustment direction)
- Master transaction history and audit log

## Common Issues

**Adjust Quantities option is not available in the Extended Menu**

The master may be A-type (serialized) rather than Q-type. Asset adjustments use the Asset tab, not the Adjust Quantities command. Verify the master type by checking the master form settings.

Alternatively, your user role may not have inventory adjustment permissions. Contact your system administrator to grant the necessary permissions.

**System prevents negative adjustment (would create negative on-hand)**

The adjustment would result in a negative on-hand quantity, which the system does not allow. Verify the adjustment amount is correct and that the on-hand quantity in the system is accurate before proceeding.

If the on-hand quantity in the system is incorrect, it may need to be corrected through a larger adjustment or a physical inventory count process.

**Adjustment does not save, showing error "GL account not configured"**

The master does not have a variance or adjustment GL account assigned. This account is needed to record the adjustment in the general ledger.

Contact your Accounting or System Administrator to:

- Assign a variance GL account to the master
- Verify the GL chart of accounts is properly configured
- Check master type settings for default GL accounts

Do not attempt the adjustment until the GL account is configured.

**On-hand quantity reverted after adjustment**

A transaction may have been processed simultaneously that affected the quantity. For example, a shipment or receipt processed at the same time may have altered the on-hand.

Verify the adjustment was actually saved by checking the master form refresh. If the quantity reverted, the adjustment may not have been completed. Reapply the adjustment and save again.

**Cannot find the master in search results**

Verify that the master number or description is spelled correctly. If the master has been recently created, it may not yet be indexed in the search. Try a partial search using part of the master number or description.

If the master does not exist, confirm the correct master number and create the master if needed before attempting adjustment.
