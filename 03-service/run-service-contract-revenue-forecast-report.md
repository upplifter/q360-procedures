---
title: Run the Service Contract Revenue Forecast Report
id: SVC-RPT-015
module: Service
screen: Service Contract Revenue Forecast Report
menu_path: Service > Reports > Service Contract Revenue Forecast
applies_to: Service Managers, Finance Managers, Sales Leadership
prerequisites:
  - Access to Service Reports
  - Permission to view service contract data
  - Active or auto-renewing contracts must exist
related_procedures:
  - SVC-RPT-014
  - SVC-RPT-016
tags:
  - Reports
  - Revenue Forecast
  - Contract Revenue
  - Financial Planning
version: 1.0
last_updated: 2026-03-25
---

# Run the Service Contract Revenue Forecast Report

## What This Procedure Does

The Service Contract Revenue Forecast Report projects monthly revenue recognition for active and auto-renewing contracts. Use this report for financial planning, revenue forecasting, and contract value analysis.

## Before You Begin

- Have permission to access Service Reports
- Determine the date range for forecasting
- Identify company and branch scope
- Understand your revenue recognition policies

## Steps

### Step 1: Open Service Contract Revenue Forecast Report

Go to Service > Reports > Service Contract Revenue Forecast. The Print Report dialog opens with filter options.

### Step 2: Set Filter Criteria

Configure filters to define the forecast:

| Field | What to select |
|-------|----------------|
| Company | Select the company |
| Branch | Select the branch (optional) |
| Department | Select the department (optional) |
| Date Range | Enter start and end dates |

### Step 3: Run the Report

Click Run Report. The report generates and displays in Print Report dialog or Live Data grid.

### Step 4: Review Revenue Forecast by Customer

The report displays per customer:

- Customer Name
- Contract No
- Contract Type
- Contract Value
- Monthly Revenue Projection (months across the report)
- Cumulative Revenue projection
- Renewal Information (if applicable)

Summary rows show total revenue by month and department.

### Step 5: Drill Down for Detail

Click a customer row to drill down to the Service Contract Revenue Forecast Detail report (SVC-RPT-016) for line-by-line revenue recognition by contract.

## What Happens Next

Results support financial planning and forecasting. Use projections to set revenue targets, plan cash flow, and monitor contract value. Track actual revenue against forecast to improve prediction accuracy. Review quarterly to adjust forecasts based on contract changes.

## Common Issues

**No Data Displayed**
Verify active or auto-renewing contracts exist in the system. Check that the date range is appropriate for your contracts. Ensure the company and branch filters are correct.

**Forecast Amount Seems Incorrect**
Verify contract amount and billing frequency are correctly configured. Check if contract start/end dates are accurate. Review revenue recognition rules in your system configuration.

**Cannot Drill Down to Detail**
Use the Service Contract Revenue Forecast Detail Report (SVC-RPT-016) directly to see line-by-line revenue per contract. Filter by specific customer or contract if needed.
