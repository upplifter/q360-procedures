---
title: View Service Contract Reports
id: SVC-CONTRACT-007
module: Service
screen: Service Contract
menu_path: Service Contract > Print Report (printer icon) OR Service > Reports
applies_to: Service Managers, Finance Managers, Business Analysts, Report Users
prerequisites:
  - Service contract must be created
  - Service calls or billing data must be recorded against the contract
related_procedures:
  - SVC-CONTRACT-006
  - SVC-RPT-013
  - SVC-RPT-014
  - SVC-RPT-015
tags:
  - reporting
  - profitability
  - analysis
version: 1.0
last_updated: 2026-03-25
---

# View Service Contract Reports

## What This Procedure Does

Generates and views standard service contract reports including profitability analysis, invoicing projections, and revenue forecasts. Reports can be run from the Service Contract form or from the Service Reports menu.

## Before You Begin

- Service contract must exist with line items and billing configuration
- Service calls or invoice data must be recorded against the contract (for profitability and invoicing reports)
- You must have access to the Service module and Reports menu
- Report templates must be configured in your Q360 system

## Steps

### Method 1: Generate Report from Service Contract Form

### Step 1A: Open the Service Contract

Navigate to Service > Service Contracts and open the contract for which you want to generate a report.

### Step 2A: Access the Print Report Option

Click the Print Report button (printer icon) in the contract form toolbar.

### Step 3A: Select Report Template

A dialog appears with available report templates. Choose one of the following:

| Report | Purpose |
|--------|---------|
| Service Contract Profitability | Shows revenue, cost, and gross profit/margin for the contract (see SVC-RPT-013) |
| Invoicing Projection | Displays forecasted invoices based on billing frequency and contract dates (see SVC-RPT-014) |
| Revenue Projection | Shows forecasted revenue recognition over the contract period (see SVC-RPT-015) |

### Step 4A: Configure Report Filters and Options

The report dialog displays options:

| Field | What to set |
|-------|------------|
| Date Range | Select start and end dates for the report period |
| Contract | Pre-populated with the current contract (can change if multi-contract reports are supported) |
| Group By | Choose report grouping (by line item, by date, by revenue source, etc.) |
| Include | Select what data to include (invoices, costs, forecasts, etc.) |

### Step 5A: Set Output Destination

Choose where to send the report:

| Option | Result |
|--------|--------|
| View | Display report in web browser |
| PDF | Export report as PDF file |
| Excel | Export report as Excel spreadsheet |
| Email | Send report via email to specified recipients |

### Step 6A: Generate and View Report

Click Generate or Run Report. The system creates the report and displays or exports it according to your selected destination.

---

### Method 2: Generate Report from Service Reports Menu

### Step 1B: Navigate to Service Reports

Go to Service menu > Reports. A Reports submenu or page displays all available service reports.

### Step 2B: Select Report Type

From the Reports list, select one of the service contract reports:

- Service Contract Profitability (SVC-RPT-013)
- Invoicing Projection (SVC-RPT-014)
- Revenue Projection (SVC-RPT-015)

### Step 3B: Select Specific Contracts

The report dialog displays a list of all service contracts. Select one or multiple contracts to include in the report using checkboxes or a multi-select field.

### Step 4B: Set Report Parameters

Configure report options:

| Parameter | What to set |
|-----------|------------|
| Date Range | Specify report period start and end dates |
| Filter by Contract Type | Optionally filter to warranty, recurring, block amount, or T&M contracts |
| Filter by Status | Optionally filter to ACTIVE, EXPIRED, or CANCELLED contracts |
| Show Comparisons | Enable side-by-side comparison of multiple contracts if generating multi-contract reports |

### Step 5B: Set Output Format

Choose report output:

| Option | Result |
|--------|--------|
| Screen | Display in web browser |
| PDF | Download as PDF file |
| Excel | Download as Excel spreadsheet |
| Email | Send via email |
| Print | Send to configured printer |

### Step 6B: Run the Report

Click Run Report or Execute. The system generates the report and delivers it to your chosen destination.

## What Happens Next

Reports are generated on demand and displayed, downloaded, or emailed based on your selection. For Profitability reports, revenue and cost data from service calls and invoices are aggregated and analyzed. For Invoicing Projection reports, forecasted invoice amounts are calculated based on contract billing frequency and dates. For Revenue Projection reports, revenue recognition is modeled based on deferred revenue accounting settings. Reports can be scheduled for recurring generation if your system supports subscribed reports.

## Common Issues

**Report returns no data even though the contract has calls and invoices**

Verify that:

- Service calls have been invoiced (not just created)
- Invoice status is POSTED or APPROVED
- The date range in the report includes the invoice dates
- Cost data has been posted to the contract

If service calls exist but no data appears in reports, check that cost posting is enabled and that calls are properly linked to the contract.

**Invoicing Projection shows different amounts than the contract Billing tab**

Invoicing Projection forecasts future invoices based on contract dates and billing frequency. The projection may differ from the contract Bill Amount if:

- Proration is applied (contract start/end dates do not align with billing cycle)
- Line items have different dates than the header
- Billing Method is T&M (projected on estimated hours, not fixed amount)

Verify that the projection date range matches your expected billing period.

**Revenue Projection does not match Deferred Revenue on the balance sheet**

Revenue Projection reports show how service revenue will be recognized over the contract period. If the projection does not match your accounting records:

- Check that the Deferred Revenue Account is correctly populated on the Billing tab
- Verify that the Recognition Method (straight-line, other) matches your accounting policy
- Ensure invoices have been posted to the revenue account

Reconcile the projection with your general ledger to identify discrepancies.

**Cannot export report to Excel or PDF**

Export functionality requires that your system has report generation engines configured. If export options are unavailable:

- Confirm that your user role has export permissions
- Check that the necessary report output modules are installed
- Contact your system administrator to enable export functionality

You can always view reports in the browser and manually copy data to external formats if export is not available.
