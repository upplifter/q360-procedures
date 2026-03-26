---
title: Run the View Funnel Quick View
id: SALES-RPT-003
module: Sales
screen: Sales Funnel Quick View
menu_path: Sales > Quick Views > View Funnel
applies_to:
  - Sales Rep
  - Sales Manager
prerequisites:
  - Access to Sales Quick Views
  - Opportunities exist with funnel positions assigned (see SALES-OPP-003)
related_procedures:
  - SALES-OPP-003
  - SALES-RPT-002
tags: view funnel, sales funnel, funnel chart, visual funnel, funnel phases, pipeline visual, funnel drill down
version: 1.0
last_updated: 2026-03-25
---

# Run the View Funnel Quick View

## What This Procedure Does

Displays a visual funnel chart of active sales opportunities across defined funnel phases. Each phase shows the total value and count of opportunities. Clicking on a phase drills down to a detailed grid listing the individual opportunities in that stage.

## Before You Begin

- You have access to Sales Quick Views.
- Opportunities have funnel definitions assigned and steps completed (see SALES-OPP-003).

## Steps

### Step 1: Open the View Funnel Quick View

Navigate to **Sales > Quick Views** and select **View Funnel**.

Alternatively, navigate to **Workflow > Sales Overview** and click the **Sales Funnel** bucket.

### Step 2: Set Filters

| Field | What to enter |
|---|---|
| Funnel Definition | Select one or more funnel definitions or ALL. |
| Sales Rep | Select a specific sales rep or ALL. |
| Company | Select a specific company or leave at default. |
| Branch | Select a branch or leave at default. |

### Step 3: Review the Visual Funnel

The funnel chart displays each phase as a segment. Each segment shows:

- The phase name (e.g., Qualify, Discovery, Proposal, Close).
- The total value of opportunities in that phase.
- The count of opportunities in that phase.

The funnel narrows from top to bottom, visually representing the sales pipeline from early-stage to close-stage opportunities.

### Step 4: Drill Into a Phase

Click on any phase segment in the funnel chart. The view transitions to a detailed grid listing individual opportunities in that phase with the following columns:

- **Opportunity No.** - unique identifier with drilldown to the Opportunity form.
- **Company** - the customer or prospect name.
- **Title** - the opportunity title.
- **Total** - the opportunity value in original currency.
- **Conversion Total** - the value converted to the company's default currency (if foreign exchange is enabled).

Footer rows show the sum of Total and Conversion Total for the selected phase.

### Step 5: Return to the Funnel View

Close or navigate back from the detail grid to return to the visual funnel chart.

## What Happens Next

Use the visual funnel to identify pipeline distribution, spot phases with too few or too many opportunities, and guide sales coaching conversations. For a tabular view of the same data, see the Funnel Forecast quick view (SALES-RPT-002).

## Common Issues

**The funnel chart is empty.**
Verify that opportunities exist with funnel definitions and completed steps. Also check the filters - the Branch and Company defaults may exclude opportunities.

**A funnel phase shows zero opportunities but you expect some there.**
The phase assignment depends on completed funnel steps. Opportunities without any completed steps show under the earliest phase or "No Current Position."

**The Conversion Total column shows zero.**
The FOREIGNEXCHANGE system configuration must be enabled for currency conversion. If it is off, only the original currency Total is populated.

**You cannot click on a phase to drill down.**
Ensure your browser allows interactive elements. Try refreshing the page. If the issue persists, use the Funnel Forecast quick view (SALES-RPT-002) as an alternative tabular view.

**The funnel phases do not match your sales process.**
Funnel phases are defined in the funnel definition configuration. Contact your administrator to review or modify the phase names and sequence.
