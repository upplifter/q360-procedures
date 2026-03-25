---
title: Run the Call WIP Report
id: SVC-RPT-002
module: Service
screen: Call WIP Report
menu_path: Service > Reports > Call WIP
applies_to: Service Managers, Accounting Managers, Finance Staff
prerequisites:
  - Access to Service Reports
  - Permission to view service call financial data
  - Calls must have time bills, parts, or other charges entered
related_procedures:
  - SVC-RPT-001
  - SVC-RPT-003
tags:
  - Reports
  - WIP
  - Work in Progress
  - Financials
version: 1.0
last_updated: 2026-03-25
---

# Run the Call WIP Report

## What This Procedure Does

The Call WIP (Work in Progress) Report shows financial data for open service calls including recognized revenue, material costs, labor costs, subcontractor costs, and miscellaneous costs. This report is used for financial reporting and accrual accounting.

## Before You Begin

- Service calls must be open with time bills, parts, or charges entered
- Have permission to access Service Reports
- Determine the as-of date and format you need
- Understand the difference between Detail and Summary formats

## Steps

### Step 1: Open Call WIP Report

Go to Service > Reports > Call WIP. The Print Report dialog opens with filter options.

### Step 2: Set Filter Criteria

Configure the filters to define your report scope:

| Field | What to select |
|-------|----------------|
| Company | Select the company to report on |
| Branch | Select the branch (optional) |
| Department | Select the department (optional) |
| As Of Date | Enter the date for WIP snapshot |
| Format | Select Detail (line-by-line) or Summary (totals only) |

### Step 3: Run the Report

Click Run Report. The report generates and opens in either Print Report dialog or Live Data grid depending on your format selection.

### Step 4: Review WIP Financials

The report shows:

- Call No and customer information
- Recognized revenue for completed work
- Material costs incurred
- Labor costs accumulated
- Subcontractor costs
- Miscellaneous costs
- Summary totals by department or branch

Detail format shows individual line items. Summary format shows aggregated totals with subtotals by grouping.

### Step 5: Export or Print Results

If needed, export the report data to Excel or print a hard copy for filing. Use the Print icon (printer icon) or export function in the report toolbar.

## What Happens Next

The WIP report is used for financial statement preparation and accrual accounting entries. Open calls continue to show in WIP until they are closed. Once calls are closed, they roll into historical profit reports. Use this report monthly or quarterly for financial close procedures.

## Common Issues

**Report Shows No Data**
Verify the As Of Date includes open calls. Check that calls have time bills, parts, or charges entered. Ensure the company and branch filters are correct.

**WIP Totals Do Not Match General Ledger**
Confirm the report includes all relevant departments and branches. Check for timing differences between when entries are made and when they are posted. Verify the As Of Date matches your general ledger cutoff date.

**Cannot Export Report Data**
Check that you have permission to export reports. Verify the report generated successfully before attempting export. Try a different export format if one is not working.
