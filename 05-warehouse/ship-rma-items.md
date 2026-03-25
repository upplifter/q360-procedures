---
title: Ship RMA Items
id: WH-RMA-003
module: Warehouse
screen: Shipping Form
menu_path: Workflow > Warehouse > Items to Ship (filter for RMA/vendor return orders)
applies_to:
  - Warehouse Staff
prerequisites:
  - Vendor RMA PO has been created (see WH-RMA-002b)
  - Items are in Vendor RMA Queue
related_procedures:
  - WH-RMA-002b
  - WH-SHIP-001
tags: rma, shipping, vendor-return, logistics
version: 1.0
last_updated: 2026-03-25
---

# Ship RMA Items

## What This Procedure Does

This procedure ships RMA items back to the vendor. You select the items from the Vendor RMA Queue, record shipping information, and confirm the shipment to the system.

## Before You Begin

- Verify the vendor RMA PO exists and items are in the Vendor RMA Queue with RMAVEND status
- Ensure all items have been packed and are ready for shipment
- Have the courier/carrier information available
- Obtain the tracking number from the shipping carrier

## Steps

### Step 1: Navigate to Items to Ship

Go to Workflow > Warehouse > Items to Ship. Filter the list to show only RMA and vendor return orders, or search for the specific vendor RMA order number.

### Step 2: Open the Vendor RMA Order

Click the vendor RMA order to open the Shipping Form. The system displays all items assigned to this RMA return order.

### Step 3: Select Items to Ship

Review the items listed on the order. Check the box next to each item you are shipping. All items on a vendor RMA order are typically shipped together, but you can select individual items if performing a partial shipment.

### Step 4: Enter Shipping Information

Enter the courier and tracking information in the designated fields:

| Field | What to enter |
|-------|---------------|
| Courier | Name of the shipping carrier (e.g., FedEx, UPS, DHL) |
| Tracking Number | The tracking number issued by the carrier |
| Ship Date | The date the shipment is being picked up |

### Step 5: Confirm the Shipment

Click the Process Actions gear icon and select **Confirm Shipment**. The system records the shipment details and updates the RMA order status.

## What Happens Next

The items are marked as shipped in the Vendor RMA Queue. The shipment tracking information is recorded in the system. The vendor can now track the return using the provided tracking number. Once the vendor receives and processes the return, the system may update inventory or cost records based on the vendor's response.

## Common Issues

**Tracking number is not accepted by the system**
Verify that the tracking number format matches the courier's standard. If formatting is correct, the tracking number may already be in use. Check with the shipping carrier to obtain a unique tracking number.

**Cannot find the vendor RMA order**
The order may not have been created yet or may be in a different status. Go to WH-RMA-002b to confirm the vendor RMA PO was successfully created. Verify the order number matches the one you are searching for.

**Items show as already shipped**
Another user may have already shipped this order. Refresh the screen to see the current status. If items were shipped in error, contact warehouse management.

**System will not allow shipment confirmation**
One or more items may not be physically packed or may have a system lock. Verify all items are ready for shipment and all required fields are completed. Check that no other users are editing this order.
