---
title: Create a Vendor RMA from a Customer Return
id: WH-RMA-002b
module: Warehouse
screen: RMA Test Queue
menu_path: Workflow > Warehouse > RMA to Test
applies_to:
  - Warehouse Manager
prerequisites:
  - RMA item has been received (see WH-RMA-001)
  - Vendor accepts returns
related_procedures:
  - WH-RMA-001
  - WH-RMA-002a
  - WH-RMA-003
tags: rma, vendor-return, disposition, procurement
version: 1.0
last_updated: 2026-03-25
---

# Create a Vendor RMA from a Customer Return

## What This Procedure Does

This procedure initiates a return to the original vendor for a received RMA item. The system automatically creates a vendor RMA purchase order and moves the item to the Vendor RMA Queue for shipment back to the supplier.

## Before You Begin

- Verify the RMA item has been received and is in the RMA Test Queue
- Confirm the original vendor accepts returns
- Verify you have the vendor contact information if needed
- Have the RMA number available

## Steps

### Step 1: Navigate to the RMA Test Queue

Go to Workflow > Warehouse > RMA to Test. The system displays all received RMA items awaiting disposition.

### Step 2: Select the RMA Item

Click the RMA item you want to return to the vendor. The system opens the item details.

### Step 3: Select Disposition

Locate the disposition dropdown and select **Return to Vendor**. This action initiates the vendor return process.

### Step 4: Confirm the Disposition

Click the Process Actions gear icon and select **Confirm**. The system automatically creates a vendor RMA purchase order and assigns the item a RMAVEND status.

## What Happens Next

The system generates a vendor RMA PO with all relevant details from the original purchase. The item moves to the Vendor RMA Queue with RMAVEND status. The item is now ready to be packaged and shipped back to the vendor. See WH-RMA-003 for instructions on shipping the vendor RMA items.

## Common Issues

**System does not create a vendor RMA PO**
This typically occurs if the vendor master record is not configured to accept returns. Verify the vendor settings and contact procurement to enable vendor returns if needed.

**Item shows RMAVEND status but does not appear in Vendor RMA Queue**
The item may be temporarily locked while the PO is being created. Refresh the screen after 1-2 minutes and check again. If the item still does not appear, verify the PO was created by checking the purchase order list.

**Cannot select Return to Vendor option**
This may indicate the vendor does not accept returns or the vendor master is inactive. Check the vendor record to confirm return authorization status.

**Wrong vendor RMA PO was created**
If the system created a PO for the wrong vendor, contact warehouse management immediately. The PO will need to be manually corrected or canceled before shipping.
