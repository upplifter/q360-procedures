---
title: Run the Inventory Value By Location Report
id: WH-RPT-003
module: Warehouse
screen: Inventory Value By Location Report
menu_path: Live Data > INVENTORY > Inventory Value By Location
applies_to:
  - Warehouse Manager
  - Controller
prerequisites:
  - Access to Live Data reports
related_procedures:
  - WH-RPT-001
  - WH-RPT-002
tags: reporting, inventory-valuation, location-analysis, live-data
version: 1.0
last_updated: 2026-03-25
---

# Run the Inventory Value By Location Report

## What This Procedure Does

This report displays inventory values broken down by location type and branch. Use this to analyze how inventory is distributed across different warehouse areas (such as main warehouse stock, tech stock, and other location types) and to support warehouse planning and optimization.

## Before You Begin

- Determine the company and branch you want to analyze, or leave blank for all
- Identify the specific as-of date if you want a valuation snapshot, or use today's date
- Have access to the Live Data reports section

## Steps

### Step 1: Navigate to the Report

Go to Live Data > INVENTORY > Inventory Value By Location. The system opens the report filter screen.

### Step 2: Set the Report Parameters

Enter or select the desired filters:

| Field | What to enter |
|-------|---------------|
| Company | Select the company to include, or leave blank for all companies |
| Branch | Select the branch to include, or leave blank for all branches |
| As Of Date | The date for the valuation snapshot (defaults to today) |

### Step 3: Run the Report

Click the appropriate button to generate or view the report. The system compiles the inventory value data grouped by location type.

### Step 4: Review the Report Data

The report groups inventory values by location type such as:

- Main warehouse stock
- Tech stock
- Reserve stock
- Other configured location types

Each section shows the total inventory value stored in that location type within the selected branch(es).

### Step 5: Analyze by Branch

The report breaks down values by branch, showing how inventory is distributed across your warehouse locations. This helps identify inventory concentration and optimize warehouse space utilization.

### Step 6: Export or Further Analysis

Use the Extended Menu (three vertical dots) to export the report to Excel or PDF for more detailed analysis, trend comparisons, or archival.

## What Happens Next

Use the location-based inventory values to plan warehouse layouts, evaluate storage requirements, and support inventory management decisions. The data can inform decisions about stock rotation, cycle counting priorities, and warehouse optimization initiatives.

## Common Issues

**Report shows zero values for some locations**
If a location type has no inventory, it may display with a zero value or may not appear in the report at all. This is expected. Verify the location type exists in the system and has had inventory transactions.

**Inventory values do not match other reports**
Compare with WH-RPT-001 (Master Valuation By Date) and WH-RPT-002 (Inventory Master Valuation) to reconcile. All three reports should total to approximately the same value if run on the same date with the same filters.

**Cannot filter by specific location**
This report groups by location type, not individual locations. For details on specific locations, use WH-RPT-002 (Inventory Master Valuation) which shows the Location column.

**Report takes a long time to run**
Filter to a specific company and branch to improve performance. If performance issues continue, contact the system administrator.
