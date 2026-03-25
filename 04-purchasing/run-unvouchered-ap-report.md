---
title: Run the Unvouchered AP Report
id: PO-RPT-009
module: Purchasing
screen: Unvouchered AP Report
menu_path: Accounting > Accounts Payable > Unvouchered AP
applies_to:
  - Purchasing Manager
  - Accounts Payable Clerk
  - Controller
prerequisites:
  - User has permission to access Accounts Payable reports
  - Received POs exist in the system
related_procedures:
  - PO-CREATE-001
  - PO-SEND-001
tags: unvouchered AP, accrued liability, received not invoiced, PO received, voucher, accounts payable, month end, Q0057
version: 1.0
last_updated: 2026-03-25
---

# Run the Unvouchered AP Report

## What This Procedure Does

Run a report that identifies PO items recorded as received in the warehouse but not yet matched to a corresponding posted vendor invoice (vouchered) as of a specific date. This report tracks accrued liabilities and is essential for month-end close, helping ensure all received goods are accounted for in accounts payable.

## Before You Begin

- You need permission to access Accounts Payable reports.
- PO items must have been received in the system.
- Know the end date for the report period. This is typically the last day of the month for month-end close.

## Steps

### Step 1: Open the Report

Navigate to **Accounting > Accounts Payable > Unvouchered AP** from the Main Navigation Sidebar (vertical panel, left edge). The report filter screen opens.

### Step 2: Set Report Filters

| Field | What to enter |
| --- | --- |
| End Date | The cutoff date for the report. Defaults to today. For month-end reporting, enter the last day of the month. |
| Report Type | Select the type of report: STANDARD (default) for regular POs, RECURRING for recurring POs, or SUSPENSE for suspense items. |

### Step 3: Run the Report

Click **Run Report** or **Search**. The report grid populates with PO items that were received on or before the End Date but have not been fully vouchered as of that date.

### Step 4: Review the Results

The report displays the following columns:

| Field | What to enter |
| --- | --- |
| Vendor | Vendor name associated with the PO. |
| Currency | The currency of the PO. |
| PO No | The purchase order number. |
| Master No | The master inventory number of the received item. |
| Asset No | The asset/serial number for A-type items. |
| Description | Item description. |
| Received Date | Date the item was received in the warehouse. |
| Qty Received | Quantity that was received. |
| Total | Extended price (quantity multiplied by unit cost). |

The report includes a Grand Total summation row at the bottom representing the total unvouchered liability.

### Step 5: Investigate Outstanding Items

For each item on the report, determine why the vendor invoice has not been processed:

1. The vendor invoice may not have arrived yet - follow up with the vendor.
2. The invoice may have arrived but not been entered as a voucher - work with AP to process it.
3. There may be a discrepancy between the PO and invoice that is holding up vouchering.

### Step 6: Export or Print (If Needed)

Right-click the grid to access the **Grid Context Menu** and select **Export** to download the data. Use the **Print Report** button (printer icon) for a printable version for month-end close documentation.

## What Happens Next

Work with the Accounts Payable team to process outstanding vendor invoices and create vouchers for the received items. The Grand Total represents the accrued liability that should be recorded in the financial statements during month-end close. As vouchers are posted, items drop off this report. Run the report again after processing to verify the unvouchered balance has decreased. The Vendor Deposit subledger report in month-end reconciliation complements this report by showing deposit balances.

## Common Issues

**Report shows items that were already vouchered.** Verify the voucher was posted (not just saved in draft). Only posted vouchers clear items from this report. Also check that the voucher date is on or before the report's End Date.

**Grand Total does not match the accrual journal entry.** The report may include items from different currencies. Review the Currency column and ensure your accrual entry accounts for each currency's total separately. Also verify the End Date matches the period being closed.

**An item appears with zero quantity received.** This may occur if the PO item is linked to a vendor invoice item even though the PO item status has not been updated. Review the PO receiving status in the Warehouse module.

**Cancelled POs still appear on the report.** POs with CANCELLED status are excluded by default. If a cancelled PO item appears, the cancellation may not have been fully processed. Verify the PO status and line item status.

**Report takes a long time to run.** The report scans all received PO items across the company. For large organizations with high purchasing volume, this can take time. Avoid running during peak system usage. Consider filtering by Report Type to narrow the scope.
