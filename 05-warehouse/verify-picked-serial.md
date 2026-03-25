---
title: Verify Picked Item Serial Number
id: WH-PICK-003
module: Warehouse
screen: Parts Pick Form
menu_path: Workflow > Warehouse > Items to Pick > [select order]
applies_to:
  - Warehouse Staff
prerequisites:
  - Item has been picked (see WH-PICK-001)
  - Physical item is accessible for verification
  - Item is A-type (serialized asset)
related_procedures:
  - WH-PICK-001
  - WH-PICK-002
  - WH-SHIP-001
tags: serial verification, quality control, pick verification, asset validation
version: 1.0
last_updated: 2026-03-25
---

# Verify Picked Item Serial Number

## What This Procedure Does

Validate that the serial number of the physical item in hand matches the system record before the packing slip is printed and the order ships. This verification step prevents serial number mismatches and ensures correct assets are shipped to customers.

## Before You Begin

- Item has been picked (see WH-PICK-001)
- Item is A-type (serialized asset), not Q-type (quantity-tracked)
- Physical item is accessible and in the picking area
- Pick form is still open on the Parts Pick Form screen

## Steps

### Step 1: Locate the Physical Item

In the warehouse picking area, locate the physical unit that was just picked for the order.

Have the item in hand or clearly visible for inspection.

### Step 2: Find the Serial Number on the Physical Item

Examine the physical unit and locate the serial number label or marking.

The serial number may be printed on a label, engraved, or marked on the item itself.

Write down or note the serial number visible on the physical unit.

### Step 3: Verify Against System Record

On the Parts Pick Form screen, locate the picked line item for this asset.

Compare the serial number displayed on the pick form screen with the serial number on the physical unit.

| Verification | What to check |
|--------------|---------------|
| Serial Number Match | Confirm the digits/characters match exactly |
| Item Description | Confirm the item description matches what you hold |
| Quantity | Confirm quantity is 1 for A-type items |

The serial numbers must match exactly—no discrepancies are acceptable.

### Step 4: Mismatch Found—Unpick and Re-pick

If the serial number on the physical item does NOT match the system record, unpick the item immediately.

Click the **Extended Menu** (three vertical dots) on the pick form.

Select **Unpick** or **Remove Pick** for the mismatched line item.

Click **Save** (floppy disk icon) to confirm the unpick action.

The item returns to available inventory and is no longer allocated to this order.

### Step 5: Locate and Pick Correct Serial

Return to the warehouse and locate the physical unit with the serial number that matches the system record.

Complete the pick for the correct serial number (see WH-PICK-001, Step 4).

Repeat the verification process (Steps 1-3) to confirm the new pick is correct.

### Step 6: Verification Passed—Proceed to Shipment

If the serial number on the physical item matches the system record, verification is complete.

The order can now proceed to shipment. Proceed to WH-SHIP-001 to ship the order and print the packing slip.

## What Happens Next

Once verification is complete and confirmed correct, the packing slip is printed with the verified serial numbers. The order ships with the correct assets. Asset status changes to Shipped in the system. Customer receives the correct units as documented on the packing slip.

## Common Issues

**Serial number on item is damaged or unreadable**
If the serial label is damaged or unreadable, contact Warehouse Manager to determine whether the item can be relabeled or if it must be returned to the supplier. Do not guess at the serial number. Document the damaged label in the order notes or system.

**Physical item does not match any line item on the order**
You may have picked the wrong item or the item is from a different order. Return the item to inventory, unpick it from this order, and locate the correct item. Verify carefully before repicking.

**Multiple units of the same item on order**
If the order includes multiple units of the same A-type item, verify each unit individually before marking picks complete. Each serial number must match its corresponding line item on the order. Use the line item sequence or location in the pick area to track which unit corresponds to which line.

**System shows pick completed but item not yet picked**
Refresh the Parts Pick Form to ensure the display is current. If the pick status appears out of sync with physical status, verify the Save operation completed successfully. Check the audit trail to confirm when the pick was recorded.

**Customer reports receiving wrong serial number after shipment**
This indicates verification was not performed or a serial mismatch was not caught. Review the audit trail and packing slip for that order. Contact Warehouse Manager to investigate root cause and implement additional verification procedures if needed.
