---
title: Run the Order Bookings by Master No Report
id: PO-RPT-002
module: Purchasing
screen: Order Bookings by Master No Report
menu_path: Reports > Order Bookings by Master No
applies_to:
  - Purchasing Agent
  - Purchasing Manager
  - Sales Manager
prerequisites:
  - User has permission to access the Reports module
  - Order data exists for the selected date range
related_procedures:
  - PO-MASTER-001
  - PO-RPT-001
tags: order bookings by master, bookings report, master number bookings, revenue by item, order analysis, Q0040
version: 1.0
last_updated: 2026-03-25
---

# Run the Order Bookings by Master No Report

## What This Procedure Does

Run a report that summarizes booked order revenue grouped by master item number. The report shows the quantity, sales amount, cost, gross profit, and gross margin percentage for each item ordered within a specified date range. This helps identify which products drive the most revenue and profit.

## Before You Begin

- You need permission to access the Reports module.
- Customer orders must exist in the system for the date range you want to analyze.
- Know the company and date range you want to report on.

## Steps

### Step 1: Open the Report

Navigate to **Reports > Order Bookings by Master No** from the Main Navigation Sidebar (vertical panel, left edge). The report filter screen opens.

### Step 2: Set Report Filters

| Field | What to enter |
| --- | --- |
| Company | Select the company to report on. |
| Start Date | Enter the beginning date of the reporting period. |
| End Date | Enter the ending date of the reporting period. |

### Step 3: Run the Report

Click **Run Report** or **Search**. The report grid populates with order booking data grouped by master number.

### Step 4: Review the Results

The report displays one row per master number with the following columns:

| Field | What to enter |
| --- | --- |
| Master No | The inventory master number. |
| Description | Item description. |
| Qty | Total quantity ordered during the period. |
| Amount | Total sales amount for the item. |
| Cost | Total cost for the item. |
| GP | Gross profit (Amount minus Cost). |
| GM% | Gross margin percentage (GP divided by Amount, multiplied by 100). |

Click the **Zoom Drilldown** on any row to view the individual order details behind the summary.

### Step 5: Export or Print (If Needed)

Right-click the grid to access the **Grid Context Menu** and select **Export** to download the data. Alternatively, click the **Print Report** button (printer icon) to generate a printable version.

## What Happens Next

Use the report data to identify top-selling items, evaluate product profitability, and compare bookings against purchasing costs (see PO-RPT-001). The Zoom drilldown provides access to individual order details. The report is sorted by Master No ascending and Amount descending by default. Cross-reference with the Purchases by Master No report to analyze the relationship between what you buy and what you sell for each item.

## Common Issues

**Report returns no data.** Verify the date range includes periods with order activity. Expand the date range or check that the correct company is selected.

**Gross margin is negative for some items.** The cost on the order line item exceeds the sales amount. This may indicate pricing errors on the order or cost increases that were not reflected in the selling price. Review the individual orders via the Zoom drilldown.

**A known item is missing from the report.** The item may not have any booked order activity in the selected date range. Verify the order date falls within the report period and that the order is in an included status (not CANCELLED or DATAENTRY).

**Quantities do not match purchase quantities.** This report shows order bookings (what was sold), not purchasing (what was bought). Differences are expected. Compare with the Purchases by Master No report (see PO-RPT-001) to analyze buy vs. sell discrepancies.

**Report includes cancelled orders.** By default, the report excludes cancelled orders. If unexpected items appear, check the order status via the drilldown to confirm the order is active.
