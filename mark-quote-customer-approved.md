---
title: Mark Quote as Customer Approved
id: SALES-QUOTE-006
module: Sales
screen: Quote Form
menu_path: Workflow > Sales Overview > Submitted Quotes bucket
applies_to:
  - Sales Rep
  - Sales Manager
prerequisites:
  - QUOTE (Execute) permission assigned to your user or group
  - The quote is in SUBMITTED status (see SALES-QUOTE-004)
  - The Bill To company is of type CUSTOMER (not PROSPECT) - coordinate with Accounting if a type change is needed (see SALES-CUSTOMER-001)
  - The quote is not marked as Optional in the Header tab
  - All optional line items have been removed or had their Optional flag cleared
related_procedures:
  - SALES-QUOTE-004
  - SALES-CUSTOMER-001
  - SALES-ORDER-001
tags: customer approved, approve quote, convert quote to order, won deal, close deal, quote to order, order creation, customer acceptance
version: 1.0
last_updated: 2026-03-25
---

# Mark Quote as Customer Approved

## What This Procedure Does

Processes a submitted quote as customer-approved, converting it to a confirmed order. This is the step that transitions a deal from the quoting phase to an active order. The resulting order must then be internally approved to trigger project, service call, or service contract creation.

## Before You Begin

- You have QUOTE (Execute) permission.
- The quote is in SUBMITTED status.
- The Bill To company type is CUSTOMER or CUSTVEND (not PROSPECT). If the company is still a prospect, coordinate with Accounting to convert it first (see SALES-CUSTOMER-001).
- The quote itself is not marked as Optional in the Header tab.
- All line items with the Optional flag have been removed or had the flag cleared.

## Steps

### Step 1: Open the Submitted Quote

Navigate to **Workflow > Sales Overview** (or **Workflow > My Sales**). Click the **Submitted Quotes** bucket. Drill into the quote to approve.

### Step 2: Verify Prerequisites

Before approving, confirm:

1. The **Bill To** company on the Header tab is of type CUSTOMER or CUSTVEND. If it shows PROSPECT, contact Accounting to change the type (see SALES-CUSTOMER-001).
2. The quote is **not** marked as Optional in the Header tab.
3. No remaining line items have the **Optional** checkbox checked, or remove/clear those items first.

### Step 3: Approve the Quote

Click the **Process Actions** button (gear icon) on the form action bar. Click **Approve**.

### Step 4: Update the Order

Q360 changes the quote status to CONVERTED and creates a matching order.

1. Open the newly created order (Q360 may navigate to it automatically or you can find it from the customer's Orders tab).
2. Click the **Edit Record** button (pencil icon).
3. Enter the customer's **PO #** in the PO field, or attach supporting documentation (email approval, signed quote) in the **Documents** tab.
4. Click the **Save Record** button (floppy disk icon).
5. Close the order form.

## What Happens Next

The order now appears in the **Quotes Converted to Confirmed Orders** bucket in the Sales Overview workflow. The next step is internal order approval (see SALES-ORDER-001), which triggers creation of the associated project, service call, or service contract depending on the order's sale type.

The opportunity's Won/Lost status may update automatically based on your system configuration.

## Common Issues

**The Approve action fails with a message about Bill To type.**
The Bill To company must be of type CUSTOMER or CUSTVEND. Contact Accounting to convert the prospect to a customer before approving (see SALES-CUSTOMER-001).

**The Approve action fails due to optional items.**
Remove any remaining optional line items or uncheck their Optional flag before approving. The system prevents conversion when optional items are present.

**The order was created but you forgot to enter the PO number.**
Open the order, enter edit mode, add the PO number or documentation, and save. This can be done at any time before order approval.

**You approved the wrong quote.**
Contact your administrator. Depending on system configuration, the order may need to be cancelled and the quote status reverted.

**The opportunity still shows as Active after quote approval.**
Some systems require the Won/Lost status to be updated manually on the opportunity. Open the opportunity, edit it, set the Won/Lost Code to WON, and save.
