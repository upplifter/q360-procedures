---
title: Run the Manufacturer Sales Forecast Report
id: SALES-RPT-014
module: Sales
screen: Manufacturer Sales Forecast Report
menu_path: Live Data > SALES > Manufacturer Sales Forecast
applies_to:
  - Sales Manager
  - Purchasing Manager
prerequisites:
  - Access to Live Data reports
  - Quotes linked to opportunities exist with master-linked line items (see SALES-QUOTE-001, SALES-OPP-001)
related_procedures:
  - SALES-RPT-001
  - SALES-QUOTE-001
  - SALES-OPP-001
tags: manufacturer forecast, manufacturer sales, product forecast, demand planning, vendor forecast, manufacturer demand, sales by manufacturer, procurement forecast
version: 1.0
last_updated: 2026-03-25
---

# Run the Manufacturer Sales Forecast Report

## What This Procedure Does

Runs the Manufacturer Sales Forecast report to project potential sales revenue by manufacturer, based on items from active quotes linked to opportunities. The report distributes forecasted costs across four time-period buckets (0-30, 31-60, 61-90, and greater than 90 days) based on the opportunity's estimated close date. Two output formats are available: DETAILED (itemized) and SUMMARY (aggregated).

## Before You Begin

- You have access to Live Data reports.
- Quotes linked to opportunities exist with master-linked line items.
- Opportunities have close dates and probability values set.

## Steps

### Step 1: Open the Report

Navigate to **Live Data > SALES** and select **Manufacturer Sales Forecast**.

### Step 2: Set Filters

| Field | What to enter |
|---|---|
| As Of Date | The baseline date for period calculations (default is today). |
| Branch | Select a branch or leave blank for all. |
| Manufacturer | Enter a specific manufacturer name to focus on, or leave blank for all. |
| Probability | Set the minimum probability threshold (e.g., 20 for 20%). Only opportunities at or above this threshold are included. |
| Format | Select DETAILED for an itemized view or SUMMARY for an aggregated view. |
| Company No. | Select a company or ALL. |

### Step 3: Review the Report

**DETAILED format** displays one row per quote line item with:

- **Zoom Drilldown** - link to the Opportunity.
- **Manufacturer**, **Master Item No**, **Item Description** - product identification.
- **Quantity** - the quoted quantity.
- **Est. Close Date** and **Probability %** - from the linked opportunity.
- **Forecasted Cost (0-30 Days)**, **(31-60 Days)**, **(61-90 Days)**, **(>90 Days)** - cost distributed by close date relative to the As Of Date. Calculated as Quantity times Unit Cost.
- **Interest**, **Opportunity No**, **Quote No**, **Quote Status**, **Branch**, **Sales Rep**, **Company**, **Quote Title** - contextual details.

**SUMMARY format** displays aggregated rows with:

- **Zoom Drilldown** - link to the Master.
- **Manufacturer**, **Master Item No**, **Item Description** - product identification.
- **Total Quantity** - aggregated across contributing quotes.
- **Est. Close Date**, **Probability %**, **Interest**, **Branch** - grouping criteria.
- **Forecasted Cost** columns for each time period (aggregated).

Both formats are sorted by Manufacturer in ascending order by default.

### Step 4: Analyze Demand

Use the report to anticipate which manufacturers' products will be in demand over the next 90+ days. Share data with procurement for inventory planning and with manufacturer reps for relationship discussions.

## What Happens Next

Use the forecast data for demand planning, procurement scheduling, and manufacturer relationship management. For a rep-based sales forecast view, see SALES-RPT-001.

## Common Issues

**The report shows no data.**
Verify that quotes linked to opportunities exist with master-linked line items. Only active quotes (not Converted, Cancelled, or Closed) are included. Also check that opportunity close dates are on or after the As Of Date.

**Forecasted costs are all in the >90 Days column.**
This means all included opportunity close dates are more than 90 days from the As Of Date. Adjust the As Of Date to an earlier date to redistribute the data across the period buckets.

**A manufacturer you expect is missing.**
The manufacturer name is pulled from the master record. Verify the master's manufacturer field is populated. Items without masters are excluded.

**The SUMMARY and DETAILED totals differ.**
Both formats should produce the same aggregate totals. If discrepancies exist, check whether filters were changed between running the two formats.

**You want to focus on a single customer's demand.**
The report does not have a customer-specific filter. Use the DETAILED format and sort or filter the grid by Company to isolate a specific customer's quoted items.
