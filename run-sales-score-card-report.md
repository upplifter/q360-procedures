---
title: Run the Sales Score Card Report
id: SALES-RPT-010
module: Sales
screen: Sales Score Card Report
menu_path: Live Data > SALES > Sales Score Card
applies_to:
  - Sales Manager
prerequisites:
  - Access to Live Data reports
  - Sales representatives have sales targets configured
  - SALESCORE configuration is set up
related_procedures:
  - SALES-OPP-001
  - SALES-QUOTE-001
  - SALES-ORDER-001
  - SALES-ACTIVITY-001
tags: sales score card, sales performance, sales metrics, rep performance, target vs actual, activity score, opportunity score, quote score, order score, invoice score, funnel score
version: 1.0
last_updated: 2026-03-25
---

# Run the Sales Score Card Report

## What This Procedure Does

Runs the Sales Score Card report to evaluate sales representative performance by aggregating key metrics including activity, opportunity, quote, order, invoice, and funnel scores against configured targets. The report provides a holistic view of each rep's effectiveness over a chosen period for benchmarking and coaching.

## Before You Begin

- You have access to Live Data reports.
- Sales representatives have sales targets assigned.
- The SALESCORE configuration is set up in your system, defining multiplier and target period parameters.

## Steps

### Step 1: Open the Report

Navigate to **Live Data > SALES** and select **Sales Score Card**.

### Step 2: Set Filters

| Field | What to enter |
|---|---|
| Company No. | Select a company or ALL. |
| Branch | Select a branch or ALL. |
| Department | Select a department or ALL. |
| Time Period | Select the period to evaluate (default is Calendar YTD). |

### Step 3: Review the Score Card

The report displays one row per active sales representative who has an assigned sales target. Each row includes:

- **User ID** - the sales rep identifier.
- **Target** - the calculated sales target (base target multiplied by the number of periods in the selected date range).
- **Act. Type** and **Act. Score** - weighted score from sales activity records.
- **Oppor Score** - weighted score from opportunity records adjusted for customer type.
- **Quote Score** - score derived from quote count and value, adjusted by customer type.
- **Order Score** - score from confirmed orders in the period.
- **Invoice Score** - score from posted invoices.
- **FunnelScore** - score from completed funnel steps.

The report is sorted by User ID in ascending order.

### Step 4: Compare and Coach

Compare individual scores against targets and across team members to identify top performers, areas for improvement, and coaching opportunities.

## What Happens Next

Use the score card in performance review meetings, to set improvement goals, and to identify training needs. The scores update as activities, opportunities, quotes, orders, and invoices are recorded throughout the period.

## Common Issues

**A sales rep does not appear in the report.**
The report includes only active sales representatives with the SALES job role who have a sales target set. Verify the rep has a target configured.

**All scores show zero.**
The report may be filtered to a period with no activity. Adjust the Time Period filter. Also verify the SALESCORE configuration is properly set up.

**The Target value seems incorrect.**
Target is calculated as the base target multiplied by the number of periods in the selected date range. Verify the base target and the SALESCORE configuration for period multipliers.

**You see only your own data.**
The report automatically filters to the logged-in user. If you are a manager and need to see all reps, verify your permissions allow broader access.

**Score weights seem unbalanced.**
Score calculations use multipliers defined in the SALESCORE configuration. Contact your administrator to review and adjust the weighting parameters.
