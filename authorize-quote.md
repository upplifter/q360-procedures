---
title: Authorize a Quote
id: SALES-QUOTE-003
module: Sales
screen: Quote Form
menu_path: Workflow > Sales Overview > Confirmed Quotes bucket
applies_to:
  - Sales Rep
  - Sales Manager
prerequisites:
  - QUOTE (Execute) permission assigned to your user or group
  - The quote is in CONFIRMED status (see SALES-QUOTE-001)
related_procedures:
  - SALES-QUOTE-001
  - SALES-QUOTE-004
  - SALES-QUOTE-005
tags: authorize quote, approve quote internally, confirmed quote, sales overview, quote authorization, review quote, quote workflow
version: 1.0
last_updated: 2026-03-25
---

# Authorize a Quote

## What This Procedure Does

Reviews and authorizes a confirmed quote from the Sales Overview or My Sales workflow. Authorization is an internal approval step that makes the quote ready for customer submission. Once authorized, the quote can be printed and emailed to the customer.

## Before You Begin

- You have QUOTE (Execute) permission.
- The quote is in CONFIRMED status.
- You have reviewed the quote for completeness and accuracy of costs and prices.

## Steps

### Step 1: Open the Sales Overview Workflow

Navigate to **Workflow > Sales Overview** (or **Workflow > My Sales**). Locate the **Confirmed Quotes** bucket and click on it. A grid opens listing all confirmed quotes matching the workflow filters.

### Step 2: Drill Into the Quote

Click on the quote you want to authorize to open the Quote form.

### Step 3: Review the Quote

Review the following before authorizing:

- Header tab: Verify the customer, site, contact, sale type, and sales rep are correct.
- Line Items tab: Confirm line item quantities, costs, prices, and margins are accurate.
- Optionally, preview the quote by clicking the **Print Report** button (printer icon) on the form action bar. Select the desired template, choose **Screen** as the Print Destination, and click **Print** to generate a preview.

### Step 4: Authorize the Quote

Click the **Process Actions** button (gear icon) on the form action bar. Click **Authorize**.

## What Happens Next

The quote status changes to AUTHORIZED. It moves from the Confirmed Quotes bucket to the **Authorized Quotes** bucket in the Sales Overview workflow. The quote is now ready to be submitted to the customer (see SALES-QUOTE-004).

If multiple quotes need to be submitted together as one combined document, see SALES-QUOTE-005.

## Common Issues

**The Authorize action is not available in the Process menu.**
Verify the quote is in CONFIRMED status. The Authorize action is only available for confirmed quotes. Also confirm you have QUOTE (Execute) permission.

**You authorized the quote but need to make changes.**
Depending on your system configuration, you may be able to return the quote to a previous status. Check the Process Actions menu for a revert or recall option. Otherwise, contact your administrator.

**The quote preview shows incorrect information.**
Return to the quote, enter edit mode, make the needed corrections, and save. Refresh the preview browser tab to see the updated output without regenerating from the Print dialog.

**You want to authorize multiple quotes at once.**
The authorization process is performed one quote at a time through the Process Actions menu. Each quote must be opened and authorized individually.

**The Confirmed Quotes bucket shows no quotes.**
Adjust the Sales Overview workflow filters (Company No, Branch, Sales Rep, Sale Type, Department) to match the quotes you expect to see.
