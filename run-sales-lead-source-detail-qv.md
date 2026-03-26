---
title: Run the Sales Lead Source Report Detail Quick View
id: SALES-RPT-013
module: Sales
screen: Sales Lead Source Report Detail
menu_path: Live Data > Sales Lead Source Report Detail
applies_to:
  - Sales Manager
  - Marketing Manager
prerequisites:
  - Access to Live Data reports
  - Records with lead source values exist
related_procedures:
  - SALES-RPT-012
  - SALES-OPP-001
  - SALES-LEAD-001
tags: lead source detail, lead source granular, source attribution detail, lead tracking detail, lead source drill down, marketing detail report
version: 1.0
last_updated: 2026-03-25
---

# Run the Sales Lead Source Report Detail Quick View

## What This Procedure Does

Runs the Sales Lead Source Report Detail to display an itemized list of all business records - opportunities, quotes, orders, invoices, and new customers - attributed to specific lead sources. This report provides the granular detail behind the summary counts shown in the Sales Lead Source Report (SALES-RPT-012).

## Before You Begin

- You have access to Live Data reports.
- Records with lead source values exist in the system.

## Steps

### Step 1: Open the Report

Navigate to **Live Data** and select **Sales Lead Source Report Detail**.

This report is also accessible by clicking a drilldown count in the Sales Lead Source Report summary (see SALES-RPT-012).

### Step 2: Set Filters

| Field | What to enter |
|---|---|
| Source Type | Select a specific record type (OPPORTUNITY, QUOTE, ORDER, CUSTOMER, INVOICE) or ALL. |
| Source | Select a specific lead source or ALL. |
| Time Period | Set the date range (default is Month to Date). |
| Sales Rep | Select a specific sales rep or ALL. |

### Step 3: Review the Detail Grid

The report displays one row per record with the following columns:

- **Zoom Drilldown** - link to open the specific record.
- **Source Type** - the type of record (Opportunity, Quote, Order, Invoice, Customer).
- **Source** - the attributed lead source.
- **Key Text** - the unique identifier (e.g., Opportunity No., Quote No., Order No., Invoice No., Customer No.).
- **Title** - the record's title. For customers, this is the company name.
- **Add Date** - when the record was created.
- **Sales Rep 1** - primary sales representative.
- **Sales Rep 2** - secondary sales representative.

### Step 4: Drill Into Individual Records

Click the Zoom Drilldown link on any row to open the full record for detailed review.

## What Happens Next

Use the detail data to trace specific deals back to their lead source, validate attribution accuracy, and support detailed marketing ROI analysis. Cross-reference with the summary report (SALES-RPT-012) for high-level insights.

## Common Issues

**The report returns no records.**
Records without a lead source are excluded. Adjust the Source and Time Period filters. Also verify records exist with Source values in the selected period.

**You see duplicate entries for the same deal.**
A single deal may generate multiple records (opportunity, quote, order, invoice). Each record type appears as a separate row if it has the same source attribution.

**The Sales Rep filter has no effect.**
Verify the selected sales rep has records in the filtered period. If no records match, the report returns empty results.

**You want to see only opportunities, not all record types.**
Set the Source Type filter to OPPORTUNITY to focus exclusively on opportunity records.

**The Time Period filter does not match the summary report.**
Ensure the Time Period in this detail report matches the Start Date and End Date used in the summary report (SALES-RPT-012) for consistent results.
