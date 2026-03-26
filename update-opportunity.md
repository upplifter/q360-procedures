---
title: Update a Sales Opportunity
id: SALES-OPP-002
module: Sales
screen: Opportunity Form
menu_path: Main Menu > Sales > Opportunities
applies_to:
  - Sales Rep
  - Sales Manager
prerequisites:
  - OPPORTUNITY (Edit) permission assigned to your user or group
  - An opportunity record exists (see SALES-OPP-001)
related_procedures:
  - SALES-OPP-001
  - SALES-OPP-003
  - SALES-QUOTE-001
  - SALES-RPT-001
tags: update opportunity, edit opportunity, opportunity value, close date, probability, forecast probability, RMR, sales pipeline, forecast date
version: 1.0
last_updated: 2026-03-25
---

# Update a Sales Opportunity

## What This Procedure Does

Updates key fields on an existing sales opportunity such as project value, RMR value, close date, probability, and forecast probability. Keeping these fields current ensures accurate sales pipeline and management forecasting reports.

## Before You Begin

- You have OPPORTUNITY (Edit) permission.
- The opportunity record exists in Q360 (see SALES-OPP-001).
- You have the updated deal information - estimated value, close date, and probability.

## Steps

### Step 1: Look Up the Opportunity

Navigate to **Main Menu > Sales > Opportunities**. Type part of the opportunity title or number in the **Form Quick Search** field and press **Enter**. Select the correct opportunity from the results.

### Step 2: Enter Edit Mode

Click the **Edit Record** button (pencil icon) on the form action bar. The form switches to edit mode.

### Step 3: Update the Opportunity Fields

Update one or more of the following fields as needed.

| Field | What to enter |
|---|---|
| Value | The updated estimated total revenue value for the deal. |
| RMR Value | The estimated recurring monthly revenue, if applicable. |
| RMR Term | The number of months for the recurring revenue. |
| Close Date | The updated expected close date. |
| Target Install Finish | The target date for project installation completion, if known. |
| Probability | The likelihood of winning the deal as a percentage. This can also update automatically when funnel steps are completed (see SALES-OPP-003). |
| Forecast Probability | The management forecasting probability percentage, which can differ from the funnel-driven probability. |
| Forecast Date | The date used for management forecasting reports, which can differ from the close date. |
| Status | Update the opportunity status as needed (e.g., Active, On Hold, Quoting). |

### Step 4: Save the Record

Click the **Save Record** button (floppy disk icon) on the form action bar.

## What Happens Next

The updated values immediately reflect in the following:

- The **Sales Forecast** quick view uses Value, Probability, and Close Date to calculate weighted pipeline totals and period buckets (see SALES-RPT-001).
- The **Funnel Forecast** quick view uses the opportunity's funnel position and value (see SALES-RPT-002).
- Management forecasting reports use Forecast Probability and Forecast Date independently from the pipeline probability.

Continue to update these fields as the deal progresses through the sales cycle to maintain accurate reporting.

## Common Issues

**The Probability field does not update after completing funnel steps.**
Probability updates from funnel steps depend on the funnel definition configuration. If your funnel definition assigns probability values to each phase, completing a step updates probability automatically. If FUNNELPHASEPROBABILITY is set to EDITABLE, you can also edit probability directly.

**The forecast reports show stale data.**
Verify you clicked Save after making changes. Also confirm the Close Date has not passed - opportunities with a close date in the past appear in the Overdue column of the Sales Forecast.

**The RMR Value field is not visible.**
The RMR fields may be hidden in your form layout. Contact your administrator to confirm the field is enabled on your Opportunity form configuration.

**You cannot enter edit mode.**
Verify you have OPPORTUNITY (Edit) permission. If another user has the record open in edit mode, Q360 may prevent concurrent editing.

**Changes to Value or Close Date are not tracked historically.**
The Sales Forecast quick view tracks historical changes and color-codes cells (green for favorable changes, red for unfavorable). This comparison uses the Days Out history period setting on the report filters.
