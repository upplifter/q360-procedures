---
title: Run the Service Contract Revenue Forecast Detail Report
id: SVC-RPT-016
module: Service
screen: Service Contract Revenue Forecast Detail Report
menu_path: Service > Reports > Service Contract Revenue Forecast Detail
applies_to: Service Managers, Finance Managers, Accounting Staff
prerequisites:
  - Access to Service Reports
  - Permission to view detailed service contract data
  - Contracts must have line items and revenue recognition configured
related_procedures:
  - SVC-RPT-015
tags:
  - Reports
  - Revenue Forecast
  - Contract Detail
  - Line Items
version: 1.0
last_updated: 2026-03-25
---

# Run the Service Contract Revenue Forecast Detail Report

## What This Procedure Does

The Service Contract Revenue Forecast Detail Report shows line-by-line revenue recognition per contract with monthly forecast columns distinguishing between invoiced revenue and future unbilled (TBD) items. Use this report for detailed contract financial analysis and revenue planning.

## Before You Begin

- Have permission to access Service Reports
- Determine the customer, contract, and date range
- Understand the difference between invoiced and TBD revenue
- Prepare to analyze contract-level revenue detail

## Steps

### Step 1: Open Service Contract Revenue Forecast Detail Report

Go to Service > Reports > Service Contract Revenue Forecast Detail. The Print Report dialog opens with filter options.

### Step 2: Set Filter Criteria

Configure filters to define the analysis:

| Field | What to select |
|-------|----------------|
| Company | Select the company |
| Customer No | Select customer (optional) |
| Date Range | Enter start and end dates |

### Step 3: Run the Report

Click Run Report. The report generates and displays in Print Report dialog or Live Data grid.

### Step 4: Review Contract Line Item Revenue

The report displays per contract and line item:

- Contract No
- Customer Name
- Line Item Description
- Item Amount
- Monthly Revenue Columns for the forecast period
- Each month shows: Invoiced amount + TBD (To Be Determined/future unbilled) amount
- Cumulative invoiced and TBD totals
- Status (Active, Completed, Pending, etc.)

### Step 5: Analyze Invoiced vs. TBD Revenue

Review the split between revenue already invoiced and future unbilled revenue. Identify line items with significant TBD amounts indicating future billing. Compare projections to actual contract performance to identify variances.

## What Happens Next

Results provide detailed insight into contract revenue streams. Use the information for customer discussions about upcoming invoicing, contract adjustments, or renewal planning. Track TBD revenue aging to identify contracts with delayed invoicing. Monitor actual invoicing against TBD projections.

## Common Issues

**Missing Line Items**
Verify all contract line items are configured in the contract detail section. Check that the date range includes the line items. Ensure the customer filter is correct.

**Invoiced and TBD Amounts Do Not Match Contract Total**
Confirm all line items are included in the report. Check if any items are marked as inactive or pending. Review contract header amount versus sum of line items.

**Cannot Understand TBD Column**
TBD represents revenue that will be invoiced in future periods per the contract terms. Invoiced columns show already-billed amounts. The combination shows total revenue recognition over time.
