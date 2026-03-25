---
title: Unreceive PO Items
id: WH-RECEIVE-002
module: Warehouse
screen: Purchase Order Form
menu_path: Purchasing > Purchase Orders > [select PO]
applies_to:
  - Warehouse Manager
  - Warehouse Staff
prerequisites:
  - Items have been received (status RECEIVED)
  - Items have not been shipped or allocated to orders
  - User has Warehouse Manager or Staff privileges
related_procedures:
  - WH-RECEIVE-001
  - WH-PICK-001
tags: purchase orders, unreceive, receipt reversal, inventory adjustment
version: 1.0
last_updated: 2026-03-25
---

# Unreceive PO Items

## What This Procedure Does

Reverse a PO receipt by removing one or more received line items from inventory. This returns the items to a pre-receipt status and is used when items must be returned to the supplier or when a receipt was recorded in error.

## Before You Begin

- PO line items are in RECEIVED status
- Items have not been shipped or allocated to customer orders
- Items are physically available for return
- User has Warehouse Manager or Staff privileges

## Steps

### Step 1: Open the Purchase Order

Navigate to **Purchasing > Purchase Orders** from the left navigation sidebar.

Search for the PO by number or filter by status to locate it.

Click the PO number to open the Purchase Order Form.

### Step 2: Navigate to Line Items Tab

On the PO form, click the **Line Items** tab to display all line items on the PO.

Scroll to locate the line item(s) you want to unreceive. The line item status should show as RECEIVED.

### Step 3: Select Items to Unreceive

Click the checkbox next to each line item you want to unreceive.

You can select one or multiple line items on the same PO.

Verify the items you have selected are the correct ones before proceeding.

### Step 4: Access Unreceive Option

Click the **Extended Menu** (three vertical dots) on the form action bar.

From the dropdown menu, select **Unreceive** or **Reverse Receipt**.

Alternatively, you can click the **Process Actions** (gear icon) button and select the unreceive option.

### Step 5: Confirm Unreceive Action

A confirmation dialog will appear asking you to verify the unreceive action.

Review the line items listed in the confirmation to ensure you are removing the correct items.

Click **Confirm** or **OK** to proceed with the unreceive operation.

### Step 6: Verify Status Change

The line item status should change from RECEIVED back to DATAENTRY or a pre-receipt status.

The receipt is reversed in the audit trail with timestamp and user name recorded.

Physical items should be prepared for return to the supplier.

## What Happens Next

Unreceived items are removed from on-hand inventory and are no longer available for picking or fulfillment. If items were allocated to customer orders during receipt, those allocations are also reversed and orders return to an available-to-pick status. The PO line item can be received again once corrected or replaced items arrive.

## Common Issues

**Cannot find the unreceive option in menus**
Verify your user account has Warehouse Manager or Staff privileges. Check that you are looking at the Line Items tab on the PO form. The unreceive action may be labeled as "Reverse Receipt" or "Undo Receipt" depending on system configuration. Contact your system administrator if the option does not appear.

**Unreceive operation fails due to allocated inventory**
If items were received and immediately allocated to customer orders, you must unpick those items first (see WH-PICK-002) before unreceiving the PO. Alternatively, contact Warehouse Manager to clear the allocation. This prevents inventory discrepancies.

**Multiple line items show as partially received**
If a PO line item was received in multiple transactions, you may need to unreceive each receipt separately or unreceive all receipts at once. Verify the total on-hand quantity matches what you want to reverse. Partial receipts should be handled carefully to avoid creating discrepancies.

**Item status does not change after clicking unreceive**
Confirm the unreceive action completed by checking the audit trail or refreshing the PO form. If the status remains RECEIVED, the operation may not have saved. Click Save (floppy disk icon) on the form action bar to ensure changes are persisted.

**Physical items are missing but system shows received**
Investigate the discrepancy by checking receiving logs and audit trail. If items cannot be located, mark them as Missing in the physical inventory count (see WH-COUNT-002) and unreceive the PO to reflect actual stock. This synchronizes system records with physical inventory.
