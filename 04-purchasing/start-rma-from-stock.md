---
title: Start RMA from Stock
id: PO-RMA-001
module: Purchasing
screen: Return to Vendor
menu_path: Inventory > Return to Vendor
applies_to:
  - Purchasing Agent
  - Warehouse Manager
prerequisites:
  - User has permission to process vendor RMAs
  - The item to be returned exists in inventory (on hand)
  - A vendor record exists for the supplier receiving the return (see PO-VENDOR-001)
  - An RMA authorization number has been obtained from the vendor (if required)
related_procedures:
  - PO-VENDOR-001
  - PO-MASTER-001
  - PO-SEND-001
tags: RMA, return to vendor, vendor RMA, return merchandise, stock return, defective item, vendor return, return authorization
version: 1.0
last_updated: 2026-03-25
---

# Start RMA from Stock

## What This Procedure Does

Initiate a return-to-vendor process for stock items via the Return to Vendor function. This creates an RMA purchase order that tracks the return shipment and, optionally, replacement items expected from the vendor.

## Before You Begin

- You need permission to process vendor RMAs in the Inventory module.
- The item to be returned must currently exist in inventory with available on-hand quantity.
- Obtain an RMA authorization number from the vendor if their process requires one.
- Know the vendor number, master number (for Q-type items) or serial/asset number (for A-type items), and the quantity to return.
- If a restocking fee is anticipated, have a miscellaneous master number for the fee (e.g., Restocking Fee or Misc Expense master).

## Steps

### Step 1: Open the Return to Vendor Form

Navigate to **Inventory > Return to Vendor** from the Main Navigation Sidebar (vertical panel, left edge). The Return to Vendor form opens.

### Step 2: Select Company and Branch

| Field | What to enter |
| --- | --- |
| Company | Select the company that holds the inventory. |
| Branch | Select the branch location where the item is stocked. |

### Step 3: Select the Vendor

| Field | What to enter |
| --- | --- |
| Vendor | Select the vendor to whom the item is being returned. |

### Step 4: Enter the Item to Return

| Field | What to enter |
| --- | --- |
| Master No | For Q-type (quantity) items, enter or search for the master number. |
| Serial No / Asset No | For A-type (serialized) items, enter the serial number or asset number. |

Press **Tab** after entering the item identifier. Q360 displays the item details including description and available quantity.

### Step 5: Adjust Quantity (If Partial Return)

If you are returning only a portion of the on-hand quantity for a Q-type item, click the **Change Qty** button and enter the quantity to return.

### Step 6: Add Additional Return Items (If Needed)

Repeat Steps 4 and 5 for each additional item to include in this vendor return.

### Step 7: Save the Return

Click the **Save** button. Q360 prompts you to indicate whether replacement items are expected from the vendor.

1. Click **Yes** if the vendor will send replacement items. Q360 creates an RMA PO with the return items and adds placeholder lines for expected replacements.
2. Click **No** if this is a return for credit only with no replacements expected. Q360 creates an RMA PO for the return shipment only.

### Step 8: Edit the RMA PO

The RMA PO opens automatically. Click the **Edit Record** button (pencil icon on the Form Action Bar) to update the PO.

| Field | What to enter |
| --- | --- |
| Vendor Order Ref | Enter the vendor's RMA authorization number if available. |

### Step 9: Add Restocking Fee (If Applicable)

Navigate to the **Line Items** tab. If the vendor charges a restocking fee:

1. Click the grid **Add** button (plus icon on the Grid Toolbar).
2. Search for your organization's miscellaneous master number for restocking fees (e.g., "Restocking Fee" or "Misc Expense").
3. Add the master and enter the fee amount in the cost field.
4. Click **Save**.

### Step 10: Confirm the RMA PO

Click the **Process Actions** button (gear icon on the Form Action Bar) and select **Confirm PO**. The RMA PO status changes to CONFIRMED and appears in the shipment queue for the warehouse team to physically ship the return.

## What Happens Next

The returned items are deducted from on-hand inventory and reflected in the Vend RMA quantity on the master record. The RMA PO appears in the shipment queue for the warehouse to prepare the physical return. If replacement items were indicated, the RMA PO also appears in the PO Receive Queue so the warehouse can receive the replacements when they arrive. Once the vendor processes the return, they issue a credit memo or ship replacements. For replacements, receive them against the RMA PO in the warehouse (see WH-RECEIVE-001). The PO line item status changes to RETURNED for returned items and RECEIVED for replacement items.

## Common Issues

**Item does not appear when entering the master or serial number.** Verify the item has available on-hand quantity at the selected company and branch. Items with zero on-hand or that are fully allocated cannot be returned. Check inventory levels (see PO-MASTER-001).

**RMA PO was created but vendor requires a specific RMA number.** Edit the RMA PO and enter the vendor's RMA authorization number in the Vendor Order Ref field. Communicate this number to the warehouse team for inclusion on the shipping label.

**Restocking fee master does not exist.** Create a miscellaneous (M-type) master for restocking fees or other miscellaneous charges (see PO-MASTER-004). Use this master whenever you need to add non-inventory charges to a PO.

**Replacement items arrived but cannot be received.** Verify the RMA PO was confirmed and is visible in the PO Receive Queue. The replacement line items must be in a receivable status. If the RMA PO was created without replacement items (No was selected in Step 7), you may need to add replacement lines manually.

**Returned item still shows in inventory.** The inventory adjustment occurs when the RMA PO is confirmed and the item is physically shipped from the warehouse. If the return has not been processed through the shipment queue, the on-hand quantity has not yet been decremented.
