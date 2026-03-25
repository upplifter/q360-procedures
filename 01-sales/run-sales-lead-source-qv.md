---
title: Run the Sales Lead Source Report Quick View
id: SALES-RPT-012
module: Sales
screen: Sales Lead Source Report Quick View
menu_path: Sales > Quick Views > Sales Lead Source Report
applies_to:
  - Sales Manager
  - Marketing Manager
prerequisites:
  - Access to Sales Quick Views
  - Opportunities, quotes, orders, and customers have lead source values populated
related_procedures:
  - SALES-RPT-013
  - SALES-OPP-001
  - SALES-LEAD-001
tags: lead source, lead source report, marketing ROI, source effectiveness, lead generation, channel performance, campaign tracking, lead attribution
version: 1.0
last_updated: 2026-03-25
---

# Run the Sales Lead Source Report Quick View

## What This Procedure Does

Runs the Sales Lead Source Report quick view to display a quantitative summary of lead source effectiveness. The report counts opportunities, quotes, orders, invoices, and new customers grouped by their original lead source, enabling analysis of which marketing channels and acquisition methods generate the most business.

## Before You Begin

- You have access to Sales Quick Views.
- Opportunities, quotes, orders, and customer records have Source values populated.

## Steps

### Step 1: Open the Report

Navigate to **Sales > Quick Views** and select **Sales Lead Source Report**.

### Step 2: Set Filters

| Field | What to enter |
|---|---|
| Start Date | Set the beginning of the analysis period (default is start of current month). |
| End Date | Set the end of the analysis period (default is today). |
| Source | Select one or more lead sources to focus on, or ALL for all sources. |

### Step 3: Review the Summary

The report displays one row per lead source with the following columns:

- **Source** - the lead source (e.g., Referral, Trade Show, Website, Marketing Campaign).
- **Opportunity Count** - new opportunities attributed to this source in the period.
- **Quote Count** - quotes generated from this source.
- **Order Count** - orders created from this source.
- **Invoice Count** - invoices linked to orders from this source.
- **Customer Count** - new customers acquired from this source.

Each count is clickable, drilling down to the Sales Lead Source Report Detail (see SALES-RPT-013) showing the individual records.

### Step 4: Drill Into Details

Click any count value to open the detailed view showing the specific opportunities, quotes, orders, invoices, or customers that make up that count.

## What Happens Next

Use the data to evaluate marketing ROI, identify top-performing lead sources, and reallocate marketing spend to the most effective channels. For granular record-level detail, see SALES-RPT-013.

## Common Issues

**The report shows no data.**
Records without a Source value are excluded. Verify that opportunities and other records have their Source field populated.

**A lead source you expect is missing.**
The source list is derived from actual data entered across opportunities, quotes, customers, orders, and invoices. If no records have a specific source value, it does not appear.

**Counts seem lower than expected.**
The report filters by Add Date of the record. Only records created within the selected date range are counted.

**You want to compare sources across a longer period.**
Expand the Start Date and End Date range to cover the desired period (e.g., full year).

**The drilldown shows records you do not recognize.**
The detail report includes all record types (opportunities, quotes, orders, invoices, customers) attributed to the source. Filter by Source Type in the detail view to focus on a specific record type.
