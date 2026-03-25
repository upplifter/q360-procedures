---
title: Run the Master Valuation By Date Report
id: WH-RPT-001
module: Warehouse
screen: Master Valuation By Date Report (Q0002)
menu_path: Inventory > Reports > Master Valuation By Date
applies_to:
  - Warehouse Manager
  - Controller
  - Accounting
prerequisites:
  - Access to Inventory reports menu
related_procedures:
  - WH-RPT-002
  - WH-INV-001
tags: reporting, inventory-valuation, inventory-analysis
version: 1.0
last_updated: 2026-03-25
---

# Run the Master Valuation By Date Report

## What This Procedure Does

This report displays the on-hand inventory valuation as of a specific date. Use this to analyze inventory values, track cost changes over time, and support period-end financial reporting.

## Before You Begin

- Determine the date for which you want inventory valuation
- Identify the company, branch, category, and sub-category if you want to filter the results
- Have access to the Inventory reports menu

## Steps

### Step 1: Navigate to the Report

Go to Inventory > Reports > Master Valuation By Date. The system opens the report filter screen.

### Step 2: Set the Report Parameters

Enter or select the desired filters:

| Field | What to enter |
|-------|---------------|
| Master No | (Optional) Specific master number to filter, or leave blank for all |
| End Date | Date for the valuation snapshot (defaults to today) |
| Company No | Select the company to include, or leave blank for all companies |
| Branch | Select the branch to include, or leave blank for all branches |
| Category | Select the inventory category to filter, or leave blank for all |
| Sub-Category | Select the sub-category to filter, or leave blank for all |

### Step 3: Run the Report

Click the appropriate button to generate or preview the report. The system compiles the data and displays the results.

### Step 4: Review the Results

The report displays columns for each master item:

| Column | Description |
|--------|-------------|
| Master No | The master inventory number |
| Item Type | Classification (Q type = finished goods, A type = assets) |
| Description | Item description |
| Qty | Quantity on hand as of the end date |
| Standard Cost | Standard cost per unit |
| Avg Cost | Average cost per unit |
| Avg Value | Total inventory value (Qty × Avg Cost) |
| Manufacturer | Item manufacturer if applicable |
| Branch | The warehouse branch |

The report only includes Q and A type masters that have transaction history. Zero quantity items are excluded by default.

### Step 5: Export or Save the Report

Use the Extended Menu (three vertical dots) to export the report to Excel, PDF, or other formats as needed for analysis or archival.

## What Happens Next

The report data can be used to reconcile inventory records with the general ledger, support period-end closing procedures, or analyze inventory valuation trends. Export the report for further analysis or filing.

## Common Issues

**Report shows no data**
Verify the end date is after the first inventory transaction. If the date is correct, check that you have selected the correct company and branch. The report only includes items with transaction history, so new masters without any activity will not appear.

**Inventory values do not match general ledger**
Reconcile the quantities using this report along with the Physical Inventory Variance Report (WH-RPT-006). Differences may indicate unrecorded transactions or physical inventory discrepancies.

**Report takes a long time to run**
If you included all companies and branches, the data set may be large. Try filtering to a specific company or branch to improve performance. Contact system administrator if performance issues persist.

**Cannot see all columns on screen**
Use the Extended Menu to adjust column visibility or export the report to Excel where all columns can be viewed and formatted.
