---
title: Run the Sales Opportunity Labor Conversion Report
id: SALES-RPT-009
module: Sales
screen: Sales Opportunity Labor Conversion Report
menu_path: Live Data > Accounting > Sales Opportunity Labor Conversion
applies_to:
  - Sales Manager
  - Engineering Manager
prerequisites:
  - Access to Live Data reports
  - Presales time has been logged and posted against opportunities (see SALES-PRESALES-003, SALES-PRESALES-004)
related_procedures:
  - SALES-PRESALES-003
  - SALES-PRESALES-004
  - SALES-OPP-001
tags: labor conversion, presales labor, opportunity cost, presales vs project, labor analysis, presales hours, estimation accuracy, cost tracking
version: 1.0
last_updated: 2026-03-25
---

# Run the Sales Opportunity Labor Conversion Report

## What This Procedure Does

Runs the Sales Opportunity Labor Conversion report to analyze the conversion of presales labor hours and costs to project labor. The report compares presales effort (hours and costs logged against opportunities) with actual project outcomes, showing deltas to evaluate estimation accuracy and presales investment efficiency.

## Before You Begin

- You have access to Live Data reports.
- Presales time has been logged and posted against opportunities.
- For the most meaningful analysis, some opportunities should have been converted to projects.

## Steps

### Step 1: Open the Report

Navigate to **Live Data > Accounting** and select **Sales Opportunity Labor Conversion**.

Alternatively, navigate to **Workflow > Sales Overview** and click the **Sales Opportunity Labor Conversion** bucket.

### Step 2: Set Filters

| Field | What to enter |
|---|---|
| Start Date | Set the beginning of the date range (default is today). |
| End Date | Set the end of the date range (default is today). |
| Branch | Select a branch or ALL. |
| Sales Rep | Select a specific sales rep or leave blank for all. |
| Cost Type | Select POSTED (uses actual posted journal amounts) or STANDARD (uses standard labor cost from master). |
| Won/Lost | Select ALL, ACTIVE, WON, or LOST to filter by opportunity outcome. |

### Step 3: Review the Report

The report displays one row per opportunity with the following columns:

- **Zoom Drilldown** - link to the Opportunity form.
- **Branch** and **Sales Rep** - organizational context.
- **Interest** - opportunity classification.
- **Customer No** and **Company** - customer identification.
- **Opportunity No** and **Opportunity Title** - the opportunity details.
- **Probability** and **Won Lost Code** - outcome indicators.
- **Value** - total opportunity value.
- **Total Hours** - total presales labor hours logged across the opportunity's lifecycle.
- **Total Cost** - total presales labor cost (calculated based on the Cost Type filter).
- **Delta Hours** - presales hours logged within the filtered date range.
- **Delta Cost** - presales cost within the filtered date range.
- **Project No**, **Start Date**, **Status**, **Project Title** - the resulting project details (if the opportunity was won and converted).

The report is sorted by Branch then Won Lost Code by default.

### Step 4: Analyze Conversion Efficiency

Compare Total Hours and Total Cost against the opportunity Value to assess presales investment per deal. For won opportunities, compare presales effort against the resulting project to evaluate estimation accuracy.

## What Happens Next

Use the data to identify opportunities where presales investment is disproportionate to deal value, improve estimation accuracy, and guide resource allocation decisions for future presales efforts.

## Common Issues

**The report shows no data.**
Expand the date range and verify that presales time bills have been posted (see SALES-PRESALES-004). Unposted time bills do not appear in the report.

**Total Cost differs between POSTED and STANDARD cost types.**
POSTED uses actual journal amounts from the GL, while STANDARD multiplies billed time by the standard labor cost from the master. These methods produce different results by design.

**The Project columns are blank.**
Project details only appear for opportunities that have been won and converted to projects. Active or lost opportunities without projects show blank project columns.

**Delta Hours and Total Hours show the same value.**
If the entire presales effort falls within the filtered date range, Delta equals Total. Expand the date range to see the full lifecycle versus period-specific activity.

**You want to see the report for lost opportunities only.**
Set the Won/Lost filter to LOST to isolate lost deals and evaluate the presales investment that did not convert.
