---
title: Receive RMA Items
id: WH-RMA-001
module: Warehouse
screen: RMA Receiving
menu_path: Workflow > Warehouse > RMA to Receive
applies_to:
  - Warehouse Staff
prerequisites:
  - RMA order exists and items are expected from customer
  - Physical items are in hand in the warehouse
related_procedures:
  - WH-RMA-002a
  - WH-RMA-002b
  - WH-RMA-002c
tags: RMA, receive, return, workflow, A-type, Q-type
version: 1.0
last_updated: 2026-03-25
---

# Receive RMA Items

## What This Procedure Does

Receive customer RMA (Return Merchandise Authorization) items from the Warehouse workflow RMA to Receive bucket. This records the physical receipt of returned items from customers and prepares them for testing or disposition decisions.

## Before You Begin

- An RMA order has been created and issued to the customer
- The customer has returned the items with an RMA number reference
- The physical returned items are in hand in the warehouse receiving area
- The RMA is available in the Warehouse workflow RMA to Receive bucket
- You have Warehouse Staff role

## Steps

### Step 1: Access Warehouse Workflow

Navigate to **Workflow > Warehouse**. The Warehouse workflow buckets appear, including the **RMA to Receive** bucket.

Click the **RMA to Receive** bucket to view open RMA orders awaiting receipt.

### Step 2: Select RMA Order

The RMA to Receive bucket displays a list of RMA orders expecting item returns. Search for and click on the RMA order you are receiving. The RMA form opens, displaying:

- RMA number
- Customer name
- RMA reason/description
- Line items with descriptions and quantities expected
- Item types (A-type serialized or Q-type quantity)

### Step 3: Verify Items Match RMA

Compare the physical items in hand to the RMA line items on the form. Verify:

- Item descriptions match the RMA
- Quantity of items received matches the RMA quantity (or note any discrepancies)
- All expected items are present
- Items are in the condition expected for the RMA reason

If items do not match or quantities are different, note the discrepancies before proceeding.

### Step 4: Enter A-Type Serial Numbers (Serialized Items)

For any A-type (serialized asset) items on the RMA:

Click on the item line to open the serial number entry field. Either:

- **Scan the barcode** using a barcode scanner to automatically populate the serial number field, or
- **Manually enter the serial number** from the physical item

The serial number must match the serial number recorded on the original shipment or RMA order. Press **Enter** or click to confirm the entry.

Repeat for each serialized item being returned.

### Step 5: Enter Q-Type Quantities (Quantity Items)

For any Q-type (quantity-based) items on the RMA:

Click on the item line to open the quantity field. Enter the actual quantity received. This should match the quantity listed on the RMA.

If the received quantity differs from the RMA quantity, enter the actual count and note the discrepancy. The RMA will reflect the received quantity.

Press **Enter** or click to confirm the entry. Repeat for each Q-type item.

### Step 6: Review Receipt Summary

Before saving, review the receipt summary:

- All A-type items have serial numbers entered
- All Q-type items have quantities entered
- Quantity and item descriptions match the RMA
- Any discrepancies between RMA and received quantities are noted

If corrections are needed, click on the item line to edit the entry.

### Step 7: Save Receipt

Click the **Save** button (floppy disk icon) to record the RMA receipt. The system:

1. Records the receipt of returned items
2. Moves the RMA from "RMA to Receive" bucket to the next workflow queue (typically RMA Test queue)
3. Creates receipt transactions for the returned items
4. Makes items available for testing or evaluation

A confirmation message appears indicating the RMA receipt has been processed successfully.

## What Happens Next

The received RMA items move to the RMA Test queue for evaluation and disposition decisions. The items will be:

- Inspected and tested to determine if they can be resold, reworked, or must be scrapped
- Tracked through the RMA workflow until disposition is final
- Potentially restocked if tests show they are usable
- Credited back to the customer if approved for credit

Subsequent RMA steps (testing, disposition decisions, and credit/return shipment) are handled in the RMA Test and RMA Return workflows (see WH-RMA-002a, WH-RMA-002b, WH-RMA-002c).

## Common Issues

**RMA is not visible in the RMA to Receive bucket**

The RMA may not be in the correct workflow status. Verify that:

- The RMA has been issued to the customer and expects items to be returned
- The RMA has not already been received or moved to another workflow step
- You are viewing the correct Warehouse workflow (not a different module workflow)

Contact your RMA coordinator if the RMA is not appearing in the queue.

**Serial number is not found when scanning or entering**

The scanned or entered serial number does not exist on the original shipment or in the system. Verify:

- The serial number on the physical item matches the RMA order exactly
- The serial number was correctly recorded when the item was originally shipped
- No typos were introduced when scanning or manually entering

If the serial number is genuinely different from the RMA, document the discrepancy and contact your RMA coordinator or Sales team.

**Received quantity does not match RMA quantity**

If you receive fewer items than the RMA quantity:

- Enter the actual received quantity on the form
- The RMA will reflect the partial receipt
- Contact your customer service team to follow up on missing items

If you receive more items than expected:

- Verify you are receiving the correct RMA
- Enter the actual count received
- Document the overage for your RMA coordinator to investigate

**Cannot find the correct item line on the RMA**

Verify you have the correct RMA selected. If the RMA does not contain the item you are receiving:

- Check the RMA number on the returned items against the RMA you have open
- Search for a different RMA that matches the items
- Contact your RMA coordinator if the items do not match any open RMA

**System shows error when saving the receipt**

The receipt may not save due to:

- Missing required fields (serial numbers or quantities not entered)
- Invalid serial numbers that do not exist in the system
- RMA status changes that prevent receipt

Verify all required fields are complete. If errors persist, contact your system administrator.

**Items are received but do not move to next workflow step**

Verify the receipt was actually saved by checking the RMA status. The RMA should move from "RMA to Receive" to the next queue (typically RMA Test).

If the RMA remains in RMA to Receive:

- The save may not have completed successfully
- Try saving the receipt again
- Contact your system administrator if the workflow does not advance

**Need to receive partial quantity or partial items**

You can receive a different quantity than the RMA quantity:

- Enter the actual received quantity on the form
- The RMA will reflect the partial receipt
- The RMA remains open for receipt of additional items if more are expected later

Document any shortages with your RMA coordinator.
