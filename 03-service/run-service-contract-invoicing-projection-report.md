---
title: Run the Service Contract Invoicing Projection Report
id: SVC-RPT-014
module: Service
screen: Service Contract Invoicing Projection Report
menu_path: Service > Reports > Service Contract Invoicing Projection
applies_to: Service Managers, Accounting Managers, Sales Managers
prerequisites:
  - Access to Service Reports
  - Permission to view service contract data
  - Contracts must have billing frequency and terms defined
related_procedures:
  - SVC-RPT-013
  - SVC-RPT-015
tags:
  - Reports
  - Contract Invoicing
  - Projections
  - Revenue Forecasting
version: 1.0
last_updated: 2026-03-25
---

# Run the Service Contract Invoicing Projection Report

## What This Procedure Does

The Service Contract Invoicing Projection Report forecasts upcoming invoicing across up to 24 billing intervals based on contract terms, billing frequency, and renewal type. Use this report for revenue forecasting, cash flow planning, and contract management.

## Before You Begin

- Have permission to access Service Reports
- Understand your contract billing frequencies (monthly, quarterly, annual, etc.)
- Identify the contract status and scope
- Have access to billing and renewal information

## Steps

### Step 1: Open Service Contract Invoicing Projection Report

Go to Service > Reports > Service Contract Invoicing Projection. The Print Report dialog opens with filter options.

### Step 2: Set Filter Criteria

Configure filters to define the analysis:

| Field | What to select |
|-------|----------------|
| Company | Select the company |
| Branch | Select the branch (optional) |
| Department | Select the department (optional) |
| Contract Status | Select contract status (Active, Auto-Renewing, etc.) |

### Step 3: Run the Report

Click Run Report. The report generates and displays in Print Report dialog or Live Data grid.

### Step 4: Review Invoicing Forecast

The report displays per contract across up to 24 monthly or quarterly billing intervals:

- Contract No
- Customer Name
- Contract Amount
- Billing Frequency (Monthly, Quarterly, Annual)
- Renewal Type (Auto-Renew, Manual Renewal, One-Time)
- Next Invoice Date
- Projected Invoice amounts for each interval
- Cumulative Revenue projection
- Renewal Date (if applicable)

Columns represent future billing periods (e.g., Month 1-24 or Quarter 1-8).

### Step 5: Analyze Revenue Projections

Review contract status and renewal dates to identify contracts ending soon. Examine invoicing pattern stability. Compare projections to actual historical performance. Identify contracts with declining or increasing amounts.

## What Happens Next

Results support sales, finance, and operations planning. Use projections for revenue forecasting, cash flow modeling, and customer retention planning. Identify contracts nearing renewal for proactive renewal outreach. Track actual invoicing against projections to refine forecasting accuracy.

## Common Issues

**No Contracts Displayed**
Verify contracts are active and have billing frequencies defined. Check that the contract status filter includes the contracts you need. Ensure the company and branch filters are correct.

**Projection Does Not Match Contract Terms**
Verify billing frequency and amount are correctly configured on the contract. Check renewal type settings. Review any special terms affecting billing pattern.

**Cannot Identify Renewal Dates**
Look for the Renewal Date column in the report. If not visible, contract renewal information may not be configured. Consult the contract record for renewal terms.
