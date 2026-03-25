---
title: Run the Expense by Vendor Report
id: PO-RPT-003
module: Purchasing
screen: Expense by Vendor Quick View
menu_path: Accounting > Accounts Payable > Quick Views
applies_to:
  - Purchasing Manager
  - Accounts Payable Clerk
  - Controller
prerequisites:
  - User has permission to access Accounts Payable quick views
  - Vendor invoices (vouchers) exist for the selected date range
related_procedures:
  - PO-VENDOR-001
  - PO-RPT-001
tags: expense by vendor, vendor expense, vendor spending, AP report, accounts payable, vendor costs, spending analysis, Q0005
version: 1.0
last_updated: 2026-03-25
---

# Run the Expense by Vendor Report

## What This Procedure Does

Run a quick view report that provides a detailed view of expenses incurred from vendors over a specified date range. The report groups spending by vendor and shows each vendor's total expense and percentage of overall spend. This aids in budgeting, cost management, and vendor relationship management.

## Before You Begin

- You need permission to access Accounts Payable quick views.
- Vendor invoices (vouchers) must be posted in the system for the date range you want to analyze.
- Know the company, branch, and date range for the report.

## Steps

### Step 1: Open the Report

Navigate to **Accounting > Accounts Payable > Quick Views** from the Main Navigation Sidebar (vertical panel, left edge). Select the **Expense by Vendor** quick view.

### Step 2: Set Report Filters

| Field | What to enter |
| --- | --- |
| Company | Select the company to report on. Defaults to your current company. |
| Branch | Select a branch or leave as ALL to include all branches. |
| Start Date | Enter the beginning date of the reporting period. Defaults to today. |
| End Date | Enter the ending date of the reporting period. Defaults to today. |

### Step 3: Run the Report

Click **Run Report** or **Search**. The report grid populates with vendor expense data.

### Step 4: Review the Results

The report displays one row per vendor with the following columns:

| Field | What to enter |
| --- | --- |
| Customer No | The vendor's identifier in Q360. |
| Company | The vendor's company name. |
| Total | Total expense amount for the vendor in the selected period. |
| % | The vendor's percentage of total spend across all vendors in the report. |

Click the **Zoom Drilldown** on any row to view the individual voucher details behind the vendor's total.

### Step 5: Export or Print (If Needed)

Right-click the grid to access the **Grid Context Menu** and select **Export** to download the data. Alternatively, use the **Print Report** button (printer icon) to generate a printable version.

## What Happens Next

Use the report to identify your highest-spend vendors for potential volume discount negotiations, track vendor spending trends over time by running the report for different date ranges, and support budget forecasting. The report excludes vendor deposit (DEPOSIT type) invoices, showing only actual expense transactions. The default sort is by Total descending so the highest-spend vendors appear first.

## Common Issues

**Report returns no data.** Verify the date range includes periods with posted vendor invoices. The Start Date defaults to today, so expand the range to cover the desired period. Confirm the correct company is selected.

**A known vendor is missing from the report.** The vendor must have posted vouchers (not just POs) in the selected date range. Vouchers in draft or unposted status are not included. Verify the voucher posting dates fall within the report period.

**Totals do not match AP aging report.** The Expense by Vendor report shows spending volume for a date range, not outstanding balances. It excludes DEPOSIT type invoices. The AP aging report shows what is currently owed. These are different views of vendor financial data.

**Percentage column does not add to 100%.** Rounding on individual vendor percentages may cause a slight discrepancy. This is normal for percentage calculations across many vendors.

**Need to see expense detail by GL account.** This report summarizes at the vendor level. For GL account-level detail, use the Zoom drilldown on a specific vendor to see individual voucher line items, which include GL account references.
