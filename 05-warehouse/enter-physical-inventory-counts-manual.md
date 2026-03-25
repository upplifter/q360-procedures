---
title: Enter Physical Inventory Counts Manually
id: WH-COUNT-001b
module: Warehouse
screen: Physical Inventory Count
menu_path: Inventory > Physical Inventory Count > [select count]
applies_to:
  - Warehouse Staff
prerequisites:
  - Physical inventory count session is open (see WH-COUNT-001a)
  - Count sheets are distributed
  - Warehouse is locked
related_procedures:
  - WH-COUNT-001a
  - WH-COUNT-001c-alt
  - WH-COUNT-002
tags: physical inventory, count, entry, A-type, Q-type
version: 1.0
last_updated: 2026-03-25
---

# Enter Physical Inventory Counts Manually

## What This Procedure Does

Enter physical inventory counts directly into the count session from the warehouse floor. For serialized assets (A-type), scan or manually enter serial numbers. For quantities (Q-type), enter the counted quantities. This is the primary method for manual count data entry.

## Before You Begin

- Verify that a physical inventory count session is open and assigned to your location
- Confirm count sheets have been distributed to all counting teams
- Ensure the warehouse has been locked to prevent inventory movement during the count
- Have the Physical Inventory Count screen open in Q360

## Steps

### Step 1: Access the Count Session

Navigate to **Inventory > Physical Inventory Count**. Select the count session assigned to your area or warehouse section from the list. The count session opens to the item listing view.

### Step 2: Enter A-Type Serial Numbers (Serialized Assets)

For any A-type (asset/serialized) master items listed in the count:

Click on the item row to open the serial number entry field. Either:

- **Scan the barcode** using a barcode scanner to automatically populate the serial number field, or
- **Manually type the serial number** into the field

The system validates that the serial number matches an asset in the master record. Press **Enter** or click the save icon to confirm the entry. Repeat for each serialized asset found in your count area.

### Step 3: Enter Q-Type Quantities

For any Q-type (quantity-based) master items listed in the count:

Click on the item row to open the quantity field. Type the counted quantity (the number of units physically present). This should match the count quantity listed on your count sheet.

Press **Enter** or click the save icon to confirm the entry. Repeat for each Q-type item in your count area.

### Step 4: Review and Complete

Scan through the count session to verify all items in your section have been counted and entered. Check that:

- All A-type serial numbers have been scanned or entered
- All Q-type quantities have been entered
- Quantities match the count sheets

Once all items are entered, click the **Save** button (floppy disk icon) to save the count session. The count data is now recorded and ready for variance report generation.

## What Happens Next

After counts are entered, the count session data is available for variance report generation. The Warehouse Manager will run the Physical Inventory Variance Report (see WH-COUNT-002) to compare counted quantities against system on-hand quantities. Any discrepancies will be reviewed and variances posted to adjust system quantities.

## Common Issues

**Barcode scanner not working for serial numbers**

Verify that the barcode scanner is connected and configured. Try manually typing the serial number into the field instead. If the scanner is connected, ensure the serial number format in the barcode matches the format stored in the master record exactly.

**Serial number not found in the system**

The entered serial number does not exist on the A-type master. Verify the serial number is correct by checking the physical item or the count sheet. If the serial number is newly received, confirm it has been entered on the master record prior to the count.

**Quantity field shows as read-only or locked**

The count session may be locked or your user role may not have edit permissions. Confirm with your Warehouse Manager that the session is still active and open for entry. Check that your user account has the Warehouse Staff role assigned.

**Duplicate serial number error**

The serial number has already been entered in this count session or exists multiple times in the system. Verify the serial number on the physical item. If a duplicate exists, consult your count sheet to ensure you have the correct item.

**Cannot find count session in the list**

The count session may not have been created or assigned to your location. Contact your Warehouse Manager to verify the session exists and has been routed to your area. Refresh the Inventory > Physical Inventory Count view to see the latest sessions.
