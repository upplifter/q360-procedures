---
title: Submit Multiple Quotes as One to Customer
id: SALES-QUOTE-005
module: Sales
screen: Opportunity Form - Quotes Tab
menu_path: Main Menu > Sales > Opportunities > Quotes tab
applies_to:
  - Sales Rep
  - Sales Manager
prerequisites:
  - QUOTE (View) permission assigned to your user or group
  - Multiple quotes exist under the same opportunity
  - Quotes are in AUTHORIZED status (see SALES-QUOTE-003)
related_procedures:
  - SALES-OPP-001
  - SALES-QUOTE-001
  - SALES-QUOTE-003
  - SALES-QUOTE-004
  - SALES-QUOTE-006
tags: multiple quotes, combined quote, submit multiple, merge quotes, combined PDF, opportunity quotes, multi-quote submission
version: 1.0
last_updated: 2026-03-25
---

# Submit Multiple Quotes as One to Customer

## What This Procedure Does

Combines and emails multiple quotes linked to the same opportunity as a single document to the customer. This is useful when a deal has been broken into separate quotes (e.g., by system, phase, or trade) but the customer expects to receive one consolidated proposal.

## Before You Begin

- Multiple quotes exist under the same opportunity.
- The quotes to be combined are in AUTHORIZED status (see SALES-QUOTE-003).
- You know the customer contact's email address.

## Steps

### Step 1: Open the Opportunity

Navigate to **Main Menu > Sales > Opportunities**. Search for and open the opportunity that contains the quotes.

### Step 2: Select the Quotes

Click the **Quotes** tab on the Opportunity form. The Quotes grid lists all quotes linked to this opportunity. Select one or more quotes to include in the combined submission by clicking their rows (hold Ctrl for non-adjacent rows, or Shift for adjacent rows).

### Step 3: Print the Combined Quote

Click the grid-level **Print** button and select **Print Selected Quote(s)**. The Print Report dialog opens.

### Step 4: Preview (Recommended)

1. Select the desired template.
2. Set **Print Destination** to **Screen**.
3. Click **Print**. A combined preview opens in a new browser tab showing all selected quotes as one document.
4. Review the output. If changes are needed, return to individual quotes, edit and save, then refresh the preview tab.

### Step 5: Email to Customer

1. Return to the Print Report dialog.
2. Set **Print Destination** to **Email**.
3. Select a recipient or type the email address in the compose window.
4. Click **Print**. Review and send the email.

## What Happens Next

The combined document is sent to the customer as a single PDF. Each individual quote retains its own status in Q360. When the customer approves, mark each quote as customer approved individually (see SALES-QUOTE-006), or work with your team to determine which quotes proceed.

## Common Issues

**The Print Selected Quote(s) option is not available.**
Ensure you have selected at least one quote in the grid before clicking the grid-level print button. The option appears in the print button dropdown.

**The combined output shows quotes in an unexpected order.**
The order of quotes in the combined document typically follows the grid order. Sort the grid as desired before printing to control the output sequence.

**Only some quotes appear in the combined preview.**
Verify all desired quotes were selected (highlighted) in the grid before printing. Quotes that were not selected are excluded.

**You need to remove a quote from the combined submission after sending.**
The combined PDF is a point-in-time output. To send an updated version, deselect the unwanted quote and regenerate the combined print.

**The customer wants to approve only part of the combined submission.**
Each quote is a separate record in Q360. The customer can approve individual quotes while declining others. Mark only the approved quotes as customer approved (see SALES-QUOTE-006).
