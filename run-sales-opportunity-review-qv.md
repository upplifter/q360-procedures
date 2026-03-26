---
title: Run the Sales Opportunity Review Quick View
id: SALES-RPT-004
module: Sales
screen: Sales Opportunity Review Quick View
menu_path: Sales > Quick Views > Opportunity Review
applies_to:
  - Sales Rep
  - Sales Manager
prerequisites:
  - Access to Sales Quick Views
  - Opportunities exist in the system (see SALES-OPP-001)
related_procedures:
  - SALES-OPP-001
  - SALES-OPP-002
  - SALES-RPT-001
tags: opportunity review, sales opportunity review, won lost analysis, opportunity list, pipeline review, opportunity status, opportunity report
version: 1.0
last_updated: 2026-03-25
---

# Run the Sales Opportunity Review Quick View

## What This Procedure Does

Runs the Sales Opportunity Review quick view to display a detailed list of opportunities with key metrics including status, funnel phase, probability, value, and won/lost analysis. This report is used to analyze opportunity outcomes, compare won versus lost deals, and review pipeline health across sales reps and time periods.

## Before You Begin

- You have access to Sales Quick Views.
- Opportunities exist with status, value, and dates populated.

## Steps

### Step 1: Open the Opportunity Review Quick View

Navigate to **Sales > Quick Views** and select **Opportunity Review**.

### Step 2: Set Filters

| Field | What to enter |
|---|---|
| Company No | Select a company or ALL. |
| Branch | Select a branch or ALL. |
| Department | Select a department or ALL. |
| Status | Select a specific opportunity status or ALL. |
| Won/Lost Code | Select a specific won/lost reason or ALL. |
| Win Status | Select WON, LOST, ACTIVE, or a comma-separated combination (default is WON,LOST). |
| Interest | Select an interest level or ALL. |
| Sales Rep | Select a specific sales rep or ALL. |
| Start Date | Set the beginning of the date range (default is first day of current month). |
| End Date | Set the end of the date range (default is last day of current month). |
| Date Filter | Choose which date the range applies to: CLOSE Date, START Date, or WON/LOST Date. |

### Step 3: Review the Report Grid

The grid displays one row per opportunity with columns including:

- **Oppor. No.** - drilldown link to the Opportunity form.
- **Company**, **Title**, **Contact** - opportunity identification.
- **Status** and **Funnel Phase** - current pipeline position.
- **Probability %** - likelihood of winning.
- **Close Date** and **Won/Lost Date** - timing details.
- **W/L Status** and **Won/Lost** - outcome and reason code.
- **Opp Value** - estimated total value.
- **Conv. Quote Val** - value of quotes converted to orders.
- **Active Quote Value** - value of active (unconverted) quotes.
- **Aging** - days since the opportunity was created.
- **Duration** - days from creation to won/lost date (or today if still active).

Subtotal rows appear in light green (by reason code), light yellow (by win status), and light blue (by sales rep).

### Step 4: Analyze the Data

- Sort by any column header to reorder the data.
- Use the grid filter toggle (funnel icon) to add inline column filters.
- Click the zoom drilldown on any row to open the full Opportunity form.

## What Happens Next

Use the review data for win/loss analysis meetings, identifying patterns in lost deals, and tracking pipeline aging. Export the grid for offline analysis if needed by right-clicking and selecting an Export option.

## Common Issues

**The report returns no results.**
Adjust the Win Status filter - the default is WON,LOST, which excludes active opportunities. Change to ALL or add ACTIVE to see open deals.

**The Date Filter does not seem to work.**
Verify the Start Date and End Date are set and that the Date Filter dropdown matches the date field you intend to filter by (CLOSE Date, START Date, or WON/LOST Date).

**Subtotal rows are missing.**
Subtotal rows appear when the report is sorted by the default sort order (Sales Rep). If you re-sort by another column, subtotals may not display.

**The Active Quote Value shows zero for an opportunity with quotes.**
Only quotes in Data Entry, Confirmed, Approved, Awaiting Customer Approval, or Authorized status are counted. Converted or cancelled quotes are excluded.

**You cannot access opportunities from other branches.**
The report respects your company and branch access permissions. Contact your administrator if you need broader access.
