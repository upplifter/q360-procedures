---
title: Update PO Items ETA and Inbound Shipping
id: PO-UPDATE-001
module: Purchasing
screen: Purchase Order Form
menu_path: Inventory > Purchase Orders
applies_to:
  - Purchasing Agent
  - Purchasing Manager
  - Warehouse Manager
prerequisites:
  - User has permission to edit purchase order line items
  - A PO exists in CONFIRMED or APPROVED status with outstanding items
  - The vendor has provided ETA dates or shipping/tracking information
related_procedures:
  - PO-SEND-001
  - PO-CREATE-001
  - PO-CREATE-002
tags: PO ETA, estimated arrival, shipping update, tracking number, waybill, inbound shipping, PO update, delivery date, courier, ETA overdue
version: 1.0
last_updated: 2026-03-25
---

# Update PO Items ETA and Inbound Shipping

## What This Procedure Does

Set or update the estimated time of arrival (ETA) and inbound courier or waybill tracking information on PO line items. This keeps the purchasing team and project managers informed about expected delivery dates and enables the Purchasing workflow to flag overdue or at-risk items.

## Before You Begin

- You need edit permission on purchase order line items.
- The PO must be in CONFIRMED or APPROVED status.
- Have the vendor's ETA date and any courier or waybill tracking numbers available.

## Steps

### Step 1: Open the Purchase Order

Navigate to **Inventory > Purchase Orders** from the Main Navigation Sidebar (vertical panel, left edge) and search for the PO.

Alternatively, use the Purchasing workflow to find POs needing ETA updates:

- **Count of POs No ETA (Past 48 Hrs)** - PO items created more than 48 hours ago that still have no ETA date entered.
- **Count of ETA Overdue** - PO items whose ETA date has passed and the item status is still DATAENTRY.
- **Count of ETA Past Req. Date** - PO items where the vendor's ETA is later than the original requested delivery date.

Click any of these buckets to open the relevant grid, then double-click a PO to open it.

### Step 2: Navigate to the Line Items Tab

Click the **Line Items** tab on the PO form to view all ordered items.

### Step 3: Enter Edit Mode

Click the **Edit Record** button (pencil icon on the Form Action Bar) to enable editing on the PO line items.

### Step 4: Update ETA and Shipping Fields

Select each line item and update the tracking fields.

| Field | What to enter |
| --- | --- |
| ETA Date | The vendor's estimated delivery date for this item. |
| Courier | The name of the shipping carrier (e.g., UPS, FedEx, freight carrier). |
| Waybill / Tracking No | The tracking number or waybill number provided by the vendor or carrier. |

Repeat for each line item on the PO. If all items share the same ETA and shipping details, some organizations use a batch update function from the extended menu.

### Step 5: Save the Changes

Click the **Save Record** button (floppy disk icon on the Form Action Bar) to save the updated ETA and shipping information.

## What Happens Next

The ETA date drives several workflow indicators. Items with an ETA in the past that have not been received appear in the **Count of ETA Overdue** bucket, alerting the purchasing team to follow up with the vendor. Items where the ETA exceeds the original requested date appear in **Count of ETA Past Req. Date**, flagging potential project schedule impacts. Project managers can view the ETA on the project's material status to plan accordingly (see PROJ-MAT-002). When the items arrive at the warehouse, they are received against this PO (see WH-RECEIVE-001).

## Common Issues

**ETA fields are not editable.** Verify you are in Edit mode (pencil icon clicked) and the PO is not in a locked status such as RECEIVED or CANCELLED.

**PO still appears in the "No ETA" bucket after updating.** Ensure you saved the changes. If the ETA was entered only on some line items, the remaining items without an ETA still trigger the bucket count. Update all outstanding line items.

**ETA Overdue bucket shows items that were already received.** The line item status may not have been updated during receiving. Verify the item was properly received in the Warehouse module (see WH-RECEIVE-001).

**Vendor changed the delivery date after initial ETA entry.** Update the ETA Date field with the new date and save. The workflow automatically recalculates whether the item is overdue or past the requested date based on the updated ETA.

**Tracking number is invalid or not working.** Verify the tracking number with the vendor. Carrier websites sometimes have a delay before a newly created tracking number becomes active. Re-enter the number if there was a transcription error.
