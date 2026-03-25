---
title: Run the Purchases by Master No Report
id: PO-RPT-001
module: Purchasing
screen: Purchases by Master No Report
menu_path: Reports > Purchases by Master No
applies_to:
  - Purchasing Agent
  - Purchasing Manager
  - Warehouse Manager
prerequisites:
  - User has permission to access the Reports module
  - Purchase order data exists for the selected date range
related_procedures:
  - PO-MASTER-001
  - PO-CREATE-001
tags: purchases by master, purchase report, master number report, spending by item, purchase history, procurement report, Q0039
version: 1.0
last_updated: 2026-03-25
---

# Run the Purchases by Master No Report

## What This Procedure Does

Run a report that analyzes purchase history grouped by master item number. The report shows how much was spent on specific items over a defined date range, including quantities, total costs, average cost, and last cost. This supports vendor negotiation and procurement planning.

## Before You Begin

- You need permission to access the Reports module.
- Purchase orders with received items must exist in the system for the date range you want to analyze.
- Know the company and date range you want to report on.

## Steps

### Step 1: Open the Report

Navigate to **Reports > Purchases by Master No** from the Main Navigation Sidebar (vertical panel, left edge). The report filter screen opens.

### Step 2: Set Report Filters

| Field | What to enter |
| --- | --- |
| Company | Select the company to report on. |
| Start Date | Enter the beginning date of the reporting period. |
| End Date | Enter the ending date of the reporting period. |

### Step 3: Run the Report

Click **Run Report** or **Search**. The report grid populates with purchase data grouped by master number.

### Step 4: Review the Results

The report displays one row per master number with the following columns:

| Field | What to enter |
| --- | --- |
| Master No | The inventory master number. |
| Description | Item description. |
| Qty | Total quantity purchased during the period. |
| Total | Total purchase cost for the item. |
| Average Cost | Average unit cost across all purchases. |
| Last Cost | The most recent purchase cost for the item. |
| Manufacturer | The item's manufacturer. |

Click the **Zoom Drilldown** on any row to view the individual purchase order details behind the summary.

### Step 5: Export or Print (If Needed)

Right-click the grid to access the **Grid Context Menu** and select **Export** to download the data. Alternatively, click the **Print Report** button (printer icon) to generate a printable version.

## What Happens Next

Use the report data to identify high-spend items for vendor negotiation, spot cost trends, and compare average costs against current pricing. The Zoom drilldown provides access to individual PO details for further investigation. The report is sorted by Master No ascending and Total descending by default.

## Common Issues

**Report returns no data.** Verify the date range includes periods with purchase activity. Expand the date range or check that the correct company is selected.

**Average cost does not match expected values.** The average cost is calculated across all purchases in the selected date range. It may differ from the current standard cost on the master record if prices have fluctuated. Use the Zoom drilldown to see individual transaction costs.

**A known item is missing from the report.** The item may not have any received PO activity in the selected date range. Verify the PO was received and the receiving date falls within the report period.

**Report is too large to review efficiently.** Use the grid's inline filter row (toggle with the funnel icon on the Grid Toolbar) to filter by manufacturer, description keyword, or cost threshold. Export to Excel for further analysis.

**Last Cost shows an old value.** Last Cost reflects the most recent purchase within the report date range, not the most recent purchase overall. Expand the end date to include more recent transactions.
