---
title: Run the Inventory Master Valuation Report
id: WH-RPT-002
module: Warehouse
screen: Inventory Master Valuation Report (Q0030)
menu_path: Live Data > INVENTORY > Inventory Master Valuation
applies_to:
  - Warehouse Manager
  - Controller
  - Accounting
prerequisites:
  - Access to Live Data reports
related_procedures:
  - WH-RPT-001
  - WH-INV-001
tags: reporting, inventory-valuation, live-data, inventory-analysis
version: 1.0
last_updated: 2026-03-25
---

# Run the Inventory Master Valuation Report

## What This Procedure Does

This detailed live data report shows the current inventory master valuation with breakdowns by location, branch, and line item. Use this to analyze inventory values, committed quantities, and available stock in real time.

## Before You Begin

- Determine the date for which you want to view inventory valuation
- Identify the company and branch if you want to filter the results
- Have access to the Live Data reports section

## Steps

### Step 1: Navigate to the Report

Go to Live Data > INVENTORY > Inventory Master Valuation. The system opens the report filter screen.

### Step 2: Set the Report Parameters

Enter or select the desired filters:

| Field | What to enter |
|-------|---------------|
| As Of Date | The date for the valuation snapshot (defaults to today) |
| Company No | Select the company to include, or leave blank for all companies |
| Branch | Select the branch to include, or leave blank for all branches |

### Step 3: Run the Report

Click the appropriate button to generate or view the report. The system compiles the current inventory data and displays the results.

### Step 4: Review the Report Data

The report displays detailed columns for each inventory master:

| Column | Description |
|--------|-------------|
| Branch | Warehouse branch |
| Master No | Master inventory number |
| Item Type | Q (quantity-tracked) or A (serialized asset) |
| Qty On Hand | Total quantity in stock |
| Qty Available | Quantity available for new orders |
| Avg Cost | Average cost per unit |
| Total Value | Qty On Hand × Avg Cost |
| Qty Commit | Quantity committed to pending orders |
| Commit Value | Qty Commit × Avg Cost |
| Description | Item description |
| Part No | Manufacturer part number |
| M/Qty | Total quantity on hand across all branches and companies |
| M/Avg Cost | Overall average cost across all branches and companies |
| Standard Cost | Standard cost per unit |
| Qty Picked | Quantity picked for shipment |
| Qty Allocated | Quantity reserved for specific orders |
| Location | Warehouse location code |
| Manufacturer | Manufacturer name |
| Category | Inventory category |
| Sub Cat | Sub-category |
| Price List | Price list code |
| Journal Bal | GL balance for account 1310 (inventory control account) |
| Total Value (Summary) | Grand total inventory value for all items in the report |
| Diff | Difference between Journal Bal and Total Value for reconciliation |

### Step 5: Interpret Summary Rows

The report uses color-coded summary rows to show subtotals and totals:

- **Light Yellow row** = Branch subtotal
- **Light Blue row** = Company subtotal
- **Light Green row** = Grand total (across all selected companies and branches)

### Step 6: Export or Analyze the Report

Use the Extended Menu (three vertical dots) to export the report to Excel or PDF. The report can be filtered and analyzed further in Excel for detailed inventory management.

## What Happens Next

The report provides live data for inventory decision-making. Use the data to identify slow-moving items, analyze inventory turnover, or support cycle counting and physical inventory procedures.

## Common Issues

**Report shows different quantities than the Master Valuation By Date Report**
This report shows live current data, while the Master Valuation By Date Report shows a snapshot as of a specific date. If running on the same date, the quantities should be similar. If different, verify that transactions were not recorded after the date you specified.

**Qty Available is lower than expected**
Qty Available includes only stock that is not committed to pending orders. Check the Qty Commit column to see how much inventory is reserved. Qty Available = Qty On Hand - Qty Commit.

**Total Value does not match general ledger**
Compare this report with WH-RPT-001 (Master Valuation By Date) and WH-RPT-006 (Physical Inventory Variance) to identify discrepancies. Work with accounting to reconcile any differences.

**Report will not export to Excel**
Verify that you have Excel installed and configured on your computer. If you can view the report on screen, try using your browser's built-in export function to save as CSV, then open in Excel.

**Cannot see all columns**
Scroll horizontally to view additional columns. For easier viewing, export the report to Excel where all columns can be displayed and formatted side-by-side.
