---
title: Receive a PO
id: WH-RECEIVE-001
module: Warehouse
screen: PO Receiving
menu_path: Workflow > Warehouse > POs to Receive
applies_to:
  - Warehouse Staff
prerequisites:
  - PO is in CONFIRMED or APPROVED status
  - Items are physically in hand
  - Packing slip or receipt documentation is available
related_procedures:
  - PO-CREATE-001
  - WH-RECEIVE-002
  - WH-LABEL-001
tags: purchase orders, receiving, PO receipt, inventory receipt
version: 1.0
last_updated: 2026-03-25
---

# Receive a PO

## What This Procedure Does

Receive items from a purchase order by entering serial numbers for A-type assets or quantities for Q-type items. Once received, inventory moves into on-hand stock and receipt labels print automatically.

## Before You Begin

- PO is in CONFIRMED or APPROVED status (visible in POs to Receive bucket)
- Physical items have arrived and are ready to stock
- Packing slip or receipt documentation is available for reference
- For A-type items, serial numbers are visible on the physical units

## Steps

### Step 1: Open the Workflow

Navigate to **Workflow > Warehouse** on the left navigation sidebar to open the Warehouse Workflow dashboard.

### Step 2: Select PO from POs to Receive Bucket

In the dashboard, locate the **POs to Receive** bucket, which displays all POs in CONFIRMED or APPROVED status ready for receipt.

Scan or search for the PO number, or scroll through the list to find the PO you want to receive.

Click the PO number to open the PO Receiving screen.

### Step 3: Receive A-Type Items (Serialized Assets)

For each line item on the PO that is an A-type asset, scan or manually enter the serial number of the physical unit.

Verify the serial number matches the item description and PO line item.

| Field | What to enter |
|-------|---------------|
| Serial Number | Scan or type the unique serial/asset number |
| Quantity | Automatically fills as 1 for A-type items |

Click the **Add** button or press Enter to register the serial number.

Repeat for each unit of the A-type item on this PO line.

### Step 4: Receive Q-Type Items (Quantity-Tracked)

For each line item on the PO that is a Q-type item, enter the quantity received.

| Field | What to enter |
|-------|---------------|
| Quantity Received | Enter the number of units counted |
| Unit of Measure | Confirm matches PO line (case, each, box, etc.) |

Verify the quantity matches the packing slip.

Click the **Add** button to record the quantity.

### Step 5: Confirm and Save Receipt

Review all line items on the receipt form to ensure quantities and serial numbers are correct.

Click the **Save** button (floppy disk icon) on the form action bar.

### Step 6: Print Receipt Labels

After saving, the system automatically prints receipt labels for all received items. Labels will include item description, serial numbers (for A-type), quantities (for Q-type), and receipt date.

Affix labels to the physical items and move them to their designated warehouse locations.

## What Happens Next

Once received, items move from the incoming dock to on-hand inventory in the branch. The PO line item status changes to RECEIVED. On-hand inventory becomes available for picking and fulfillment. Receipt is recorded in the audit trail with timestamp and receiving user name.

## Common Issues

**PO does not appear in POs to Receive bucket**
Verify the PO status is CONFIRMED or APPROVED in Purchasing. POs in RECURRING status are excluded from the bucket and must be received through a different process. Check the Branch and Company filters on the Warehouse Workflow to ensure the correct PO is displayed.

**Serial number will not scan or is rejected by system**
Verify the serial number matches exactly what is recorded on the PO line item. Check for leading or trailing spaces when entering manually. If the serial has special characters, confirm those are being entered correctly. Contact Purchasing if the serial number on the physical unit does not match the PO documentation.

**Quantity received does not match PO line quantity**
This is acceptable during partial receipt. Document the actual quantity received. If the remainder is expected later, the PO line remains in RECEIVED status and you can receive additional quantities in a follow-up receipt. If the discrepancy indicates damaged or missing items, contact the supplier and create a return (see WH-RECEIVE-002).

**Receipt labels do not print after saving**
Verify the warehouse printer is online and has paper loaded. Check printer settings in system administration. If the printer is offline, manually reprint labels by opening the received PO and using the Print Report icon. Contact IT if the printer remains unavailable.

**Unable to receive due to system message about missing information**
Ensure all required fields on the PO line item are completed (description, unit of measure, etc.). If receiving A-type items, verify serial numbers are being entered in the Serial Number field, not the Quantity field. Confirm your user account has Warehouse Staff or Manager privileges.
