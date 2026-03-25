---
title: Unpick Order Items
id: WH-PICK-002
module: Warehouse
screen: Parts Pick Form / Order Form
menu_path: Workflow > Warehouse > Items to Pick > [select order]
applies_to:
  - Warehouse Staff
  - Warehouse Manager
prerequisites:
  - Items are in PICKED or SHIPQ status
  - Items have not been shipped
  - Order is still in warehouse fulfillment process
related_procedures:
  - WH-PICK-001
  - WH-PICK-003
  - WH-SHIP-001
tags: unpicking, pick reversal, inventory allocation, order modification
version: 1.0
last_updated: 2026-03-25
---

# Unpick Order Items

## What This Procedure Does

Reverse a pick operation by removing one or more picked line items from an order. This returns items to available inventory and is used when incorrect items were picked, items are damaged, or picking must be undone for order modifications.

## Before You Begin

- Items are in PICKED or SHIPQ status
- Items have not been shipped (shipment reversal requires different process)
- Order is still in active warehouse fulfillment
- User has Warehouse Staff or Manager privileges

## Steps

### Step 1: Open the Order

Navigate to **Workflow > Warehouse** and locate the order in the **Items to Pick** bucket or **Items to Ship** bucket.

Click the order number to open the Parts Pick Form or Order Form.

Alternatively, navigate to **Orders > Sales Orders**, search for the order, and open it directly.

### Step 2: Identify Items to Unpick

On the form, locate the line items that are in PICKED or SHIPQ status.

Review which items need to be unpicked. This may be all items on the order or just specific line items.

Verify you are removing the correct items before proceeding.

### Step 3: Select Items for Unpicking

Click the checkbox next to each line item you want to unpick.

You can select one or multiple line items on the same order.

Verify the selection includes only the items you intend to unpick.

### Step 4: Access Unpick Option

Click the **Extended Menu** (three vertical dots) on the form action bar.

From the dropdown menu, select **Unpick**, **Remove Pick**, or **Reverse Pick**.

Alternatively, click the **Process Actions** (gear icon) button and select the unpick option from the dropdown menu.

### Step 5: Confirm Unpick Action

A confirmation dialog will appear asking you to verify the unpick action.

Review the line items listed in the confirmation to ensure you are unpicking the correct items.

Click **Confirm** or **OK** to proceed with the unpick operation.

### Step 6: Verify Status Change

The line item status should change from PICKED or SHIPQ back to APPROVED or an available-to-pick status.

The unpick is recorded in the audit trail with timestamp and user name.

Items return to available inventory and can be picked again if needed.

### Step 7: Save Changes

Click the **Save** button (floppy disk icon) on the form action bar to ensure all changes are persisted.

The order moves back to the Items to Pick bucket if not all items have been picked.

## What Happens Next

Unpicked items are returned to available inventory and are no longer committed to this order. The order remains in an active fulfillment status but with fewer items ready to ship. If items were damaged during picking, you can inspect them for damage disposition. The order can be picked again once items are located or issues are resolved.

## Common Issues

**Cannot find the unpick option in menus**
Verify your user account has Warehouse Staff or Manager privileges. Confirm you are looking at the correct form (Parts Pick Form or Order Form). The unpick action may be labeled as "Remove Pick" or "Reverse Pick" depending on system configuration. Contact system administrator if the option does not appear.

**Unpick operation fails due to shipped status**
Items that have already been shipped cannot be unpicked. If you need to reverse a shipment, contact Warehouse Manager for return processing (see WH-RMA process). Do not attempt to force unpick of shipped items.

**Multiple line items were picked from same product master**
If the order includes multiple line items for the same product (different serial numbers for A-type, or separate quantities for Q-type), verify you are unpicking the correct line item. Check the pick sequence or line item numbers to ensure you are removing the intended item.

**Item status does not change after clicking unpick**
Confirm the unpick action completed by checking the order status and refreshing the screen. If the status remains PICKED or SHIPQ, the operation may not have saved. Click Save (floppy disk icon) to persist changes.

**Order was partially picked and now needs complete unpick**
You can unpick all items on the order at once by selecting all checkboxes, or unpick items individually. Confirm management approval if the order requires complete fulfillment reset. This may indicate a process issue that should be documented.
