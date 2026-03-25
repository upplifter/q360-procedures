---
title: Run the Funnel Forecast Quick View
id: SALES-RPT-002
module: Sales
screen: Funnel Forecast Quick View
menu_path: Sales > Quick Views > Funnel Forecast
applies_to:
  - Sales Rep
  - Sales Manager
prerequisites:
  - Access to Sales Quick Views
  - Opportunities exist with funnel positions assigned (see SALES-OPP-003)
related_procedures:
  - SALES-OPP-003
  - SALES-RPT-001
  - SALES-RPT-003
tags: funnel forecast, funnel stages, pipeline forecast, sales funnel report, opportunity stages, funnel phase, funnel quick view
version: 1.0
last_updated: 2026-03-25
---

# Run the Funnel Forecast Quick View

## What This Procedure Does

Runs the Funnel Forecast quick view to display a consolidated overview of active sales opportunities grouped by their current funnel stage. The report shows each opportunity's value, forecast date, and assigned sales representatives, enabling pipeline tracking by funnel phase.

## Before You Begin

- You have access to Sales Quick Views.
- Opportunities have funnel definitions assigned and steps marked as complete (see SALES-OPP-003).

## Steps

### Step 1: Open the Funnel Forecast Quick View

Navigate to **Sales > Quick Views** and select **Funnel Forecast**.

### Step 2: Set Filters

| Field | What to enter |
|---|---|
| Funnel Definition | Select a specific funnel definition or ALL. |
| Sales Rep | Select a specific sales rep or ALL. The list respects your sales group access permissions. |

### Step 3: Review the Forecast Grid

The grid displays one row per active opportunity with the following columns:

- **Bal Forecast** - the current funnel phase (e.g., Qualify, Discovery, Proposal).
- **Code** - the interest code for the opportunity.
- **Prospect Name** - the customer or prospect company name.
- **Value** - the estimated monetary value.
- **Forecast Date** - the anticipated close date.
- **Title** - the opportunity title.
- **Sales Rep** and **Sales Rep 2** - primary and secondary sales reps.

A footer row shows **Total Act. Forecast** - the sum of all opportunity values in the current view.

The grid is sorted by funnel position (ascending) then by prospect name.

### Step 4: Drill Into Opportunities

Click on any opportunity row to open the full Opportunity form for detailed review or updates.

## What Happens Next

Use the funnel forecast to monitor how opportunities are distributed across sales stages. Identify phases with high value concentration or potential bottlenecks. Compare this view with the visual funnel chart (see SALES-RPT-003) for a graphical perspective.

## Common Issues

**The report shows "No Current Position" for some opportunities.**
These opportunities have a funnel definition assigned but no steps marked as complete. Advance them through the funnel process (see SALES-OPP-003).

**Won or Lost opportunities appear in the list.**
Only active opportunities are included. If you see won or lost deals, verify their Won/Lost Code is set correctly on the opportunity record.

**The Total Act. Forecast seems too low.**
The total only sums opportunities visible in the current filtered view. Adjust the Funnel Definition and Sales Rep filters to include all desired opportunities.

**You do not see the Funnel Forecast in Quick Views.**
Confirm you have the appropriate permission to access Sales Quick Views. Contact your administrator if the quick view is not available.

**Opportunities are missing from specific funnel phases.**
The funnel phase shown is based on the highest completed step. If a step was skipped, the opportunity may appear in an earlier phase than expected.
