---
title: Refresh Quote Line Items
id: SALES-QUOTE-007
module: Sales
screen: Quote Form - Line Items Tab
menu_path: Main Menu > Sales > Quotes > Line Items tab > Extended Menu
applies_to:
  - Sales Rep
  - Engineer
prerequisites:
  - QUOTE (Edit) permission assigned to your user or group
  - A quote exists with line items linked to masters (see SALES-QUOTE-001)
related_procedures:
  - SALES-QUOTE-001
  - SALES-QUOTE-002
  - SALES-QUOTE-003
tags: refresh quote, refresh line items, update pricing, update costs, recost, reprice, master pricing, catalog pricing, quote pricing refresh, MSRP
version: 1.0
last_updated: 2026-03-25
---

# Refresh Quote Line Items

## What This Procedure Does

Updates costs and prices on a quote's line items to reflect current master catalog pricing. This is commonly used when a quote was copied from an older quote or when master pricing has changed since the quote was originally built. The refresh also updates MSRP values where available.

## Before You Begin

- You have QUOTE (Edit) permission.
- The quote exists and contains line items linked to master part numbers.
- Consider creating a revision before refreshing to preserve the original pricing (see SALES-QUOTE-002).

## Steps

### Step 1: Open the Quote

Navigate to **Main Menu > Sales > Quotes**. Search for and open the quote whose pricing needs to be refreshed.

### Step 2: Open the Line Items Tab

Click the **Line Items** tab on the Quote form.

### Step 3: Refresh Line Item Pricing

1. Click the Line Items grid **Extended Menu** (three vertical dots).
2. Select **Refresh Line Items** (or **Refresh Line Item Prices and Costs**, depending on your system version).
3. In the refresh modal, select options as needed. If a master profile dropdown appears, you can select a specific price list (e.g., GPO) to apply profile-based pricing.
4. Confirm the refresh.

Q360 updates the unit cost, unit price, and MSRP for all line items that are linked to master records, including items inside nested sections.

### Step 4: Review and Save

Review the updated costs and prices in the Line Items grid to verify they reflect expected values. Click the **Save Record** button (floppy disk icon) on the form action bar.

## What Happens Next

The quote now reflects current master catalog pricing. You can proceed with the normal quote workflow: confirm (see SALES-QUOTE-001, Step 7), authorize (see SALES-QUOTE-003), and submit to the customer (see SALES-QUOTE-004).

If you need to revert to the previous pricing, restore the revision you created before the refresh (see SALES-QUOTE-002).

## Common Issues

**Some line items are not updated after the refresh.**
Items that are not linked to a master part number (manually entered line items) are not affected by the refresh. Only items with a valid master reference receive updated pricing.

**The refreshed prices differ from what you expected.**
The refresh pulls current costs and prices from the master record. If a master profile was selected, the pricing comes from that profile's price list. Verify the correct profile was chosen in the refresh modal.

**The MSRP column does not update.**
MSRP updates are included in the refresh where the master record has an MSRP value defined. If the master lacks an MSRP, the column remains unchanged.

**You want to refresh only specific line items, not the entire quote.**
The refresh command applies to all master-linked line items in the quote. To update only specific items, manually edit those line items and adjust the cost and price fields individually.

**The refresh modal does not appear.**
Ensure the quote is in edit mode before using the Extended Menu command. Some versions require the form to be in edit mode for the refresh option to be available.
