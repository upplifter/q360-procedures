---
title: Ship Items
id: WH-SHIP-001
module: Warehouse
screen: Shipping Form
menu_path: Workflow > Warehouse > Items to Ship
applies_to:
  - Warehouse Staff
prerequisites:
  - Items are picked and in SHIPQ status (see WH-PICK-001)
  - Order is approved and ready to ship
  - Courier and tracking information is available
  - Shipping address is confirmed on the order
related_procedures:
  - WH-PICK-001
  - WH-PICK-003
  - WH-RPT-004
tags: shipping, order shipment, fulfillment, courier tracking
version: 1.0
last_updated: 2026-03-25
---

# Ship Items

## What This Procedure Does

Ship picked items to the customer by recording courier and tracking information, confirming the shipment, and printing the packing slip. Once shipped, items are removed from on-hand inventory and the order is closed.

## Before You Begin

- Items are picked and in SHIPQ status
- All items on the order have been picked (or partial shipment is approved)
- Order is approved and not on hold
- Courier information is available (name, service type)
- Tracking number is available or can be generated
- Shipping address is confirmed on the order

## Steps

### Step 1: Open the Workflow

Navigate to **Workflow > Warehouse** on the left navigation sidebar.

### Step 2: Select Order from Items to Ship Bucket

In the Warehouse Workflow dashboard, locate the **Items to Ship** bucket, which displays all picked items ready to ship.

The bucket shows orders in SHIPQ status with all items picked and ready.

Scan or search for the order number, or scroll through the list to find the order.

Click the order number to open the Shipping Form.

### Step 3: Verify Shipping Address

On the Shipping Form, verify the shipping address is correct and complete.

| Field | What to verify |
|-------|----------------|
| Ship To Address | Confirm name, street, city, state, zip match order |
| Shipping Method | Confirm matches what customer requested |
| Special Instructions | Confirm any special delivery instructions are noted |

Contact Sales or Order Management if the shipping address is incorrect before proceeding.

### Step 4: Enter Courier Information

In the Courier section of the form, enter the shipping carrier details:

| Field | What to enter |
|-------|---------------|
| Carrier | Select the courier (FedEx, UPS, USPS, DHL, other) |
| Service Type | Select the shipping service (Ground, Express, etc.) |
| Tracking Number | Enter the tracking number assigned by courier |
| Estimated Delivery Date | Enter the expected delivery date if available |

Verify the tracking number is correct before proceeding.

### Step 5: Confirm Items to Ship

Review all line items on the Shipping Form to confirm all picked items are listed.

Verify quantities and serial numbers (for A-type items) match the pick information.

If any items should not ship with this shipment, unpick them first (see WH-PICK-002).

### Step 6: Save Shipment

Click the **Save** button (floppy disk icon) on the form action bar.

The system records the shipment with courier, tracking number, and timestamp.

Item status changes to SHIPPED and asset status changes to SHIPPED for A-type items.

### Step 7: Print Packing Slip

After saving the shipment, the system is ready to print the packing slip.

Click the **Print Report** icon (printer) on the form action bar.

The packing slip prints with order number, customer name, shipping address, items shipped, serial numbers (for A-type), quantities, and tracking number.

Affix the packing slip to the outside of the shipping container.

### Step 8: Hand Off to Shipping

Place the completed shipment container with the packing slip in the outbound shipping area for courier pickup.

Verify the courier collects the package and scans the tracking number to confirm pickup.

Document any delivery issues or special handling notes if applicable.

## What Happens Next

The order is marked as SHIPPED in the system and removed from the Items to Ship bucket. Inventory is reduced by the shipped quantities and asset status is updated to SHIPPED. Customer receives tracking information via email if configured. The order appears in shipping reports (see WH-RPT-004) for fulfillment tracking and analysis. Shipped items are no longer available for picking or allocation.

## Common Issues

**Courier tracking number is not available yet**
If the tracking number will not be available until the courier picks up the shipment, save the shipment with a placeholder or estimated tracking number. The tracking number can be updated after courier pickup by editing the shipment record. Do not delay shipment if the carrier will provide tracking at pickup.

**Partial shipment with items not yet picked**
If only some items on the order are picked and ready to ship, you can ship the available items and leave the order partially fulfilled. Other items can ship in a follow-up shipment once picked. Confirm with customer that partial shipment is acceptable and update the order notes.

**Shipping address is incorrect**
Do not ship to an incorrect address. Contact Sales or Order Management to confirm the correct address and update the order before proceeding. If the order was already shipped to the wrong address, contact Warehouse Manager about reverse logistics options.

**Packing slip does not print after saving**
Verify the warehouse printer is online and has paper loaded. Check printer settings in system administration. If the printer is offline, manually reprint the packing slip by opening the shipped order and clicking Print Report. Contact IT if the printer remains unavailable.

**Shipment saved but order still shows in Items to Ship bucket**
Refresh the Warehouse Workflow dashboard by clicking the Refresh icon (circular arrow). The bucket updates to remove shipped orders within a few seconds. If the order remains after refresh, verify the Save operation completed without errors by opening the order to check the SHIPPED status.
