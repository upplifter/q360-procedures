---
title: Run the Physical Inventory Variance Report
id: WH-RPT-006
module: Warehouse
screen: Physical Inventory Variance Report (Q0166)
menu_path: Live Data > INVENTORY > Physical Inventory Variance
applies_to:
  - Warehouse Manager
  - Controller
prerequisites:
  - Access to Live Data reports
  - Physical inventory count has been recorded
related_procedures:
  - WH-COUNT-002
  - WH-COUNT-003
  - WH-RPT-005
tags: reporting, physical-inventory, variance-analysis, inventory-reconciliation
version: 1.0
last_updated: 2026-03-25
---

# Run the Physical Inventory Variance Report

## What This Procedure Does

This report displays physical inventory count results with variances between counted quantities and system quantities. Use this to identify inventory discrepancies, investigate loss or overage, and support inventory adjustments and reconciliation.

## Before You Begin

- Have access to the Live Data > INVENTORY section
- Know the count number you want to analyze
- Be prepared to investigate variances and determine root causes
- Have access to approval authority for inventory adjustments if needed

## Steps

### Step 1: Navigate to the Report

Go to Live Data > INVENTORY > Physical Inventory Variance. The system opens the report filter screen.

### Step 2: Select the Count

In the Count No filter field, enter the count number:

| Field | What to enter |
|-------|---------------|
| Count No | The physical inventory count number to analyze (text field) |

### Step 3: Run the Report

Click the appropriate button to generate or view the report. The system compiles variance data for the specified count.

### Step 4: Review the Variance Data

The report displays the following columns for each item:

| Column | Description |
|--------|-------------|
| Master No | Master inventory number |
| Asset No | Individual asset number |
| Description | Item description |
| Item Status | COUNTED, RECOUNTED, or NOTINCOUNT |
| Location | Warehouse location of the item |
| Qty Counted | Physical quantity counted during inventory |
| Variance | Difference between Qty Counted and system Qty On Hand |
| Var. Used | Variance amount used in prior adjustments |
| Qty on Hand | System quantity before adjustment |
| Qty Received | Total quantity received in the current period |
| Qty Shipped | Total quantity shipped in the current period |
| Avg Cost | Average cost per unit |
| Avg Value | Total inventory value at average cost |

### Step 5: Interpret Item Status Codes

The Item Status column indicates the count status for each item:

- **COUNTED** = Item was physically counted and recorded
- **RECOUNTED** = Item was counted multiple times (may indicate discrepancy investigation)
- **NOTINCOUNT** = Item exists in the system but was not found during the physical count

Items with NOTINCOUNT status show Qty Counted = 0 and may indicate missing inventory.

### Step 6: Analyze Variances

Review the Variance column to identify discrepancies. Positive variances indicate physical count exceeded system records. Negative variances indicate system records exceeded physical count. Large variances require investigation and explanation.

### Step 7: Export for Analysis and Approval

Use the Extended Menu (three vertical dots) to export the report to Excel. Distribute the variance report to warehouse management and accounting for investigation and approval of adjustments.

## What Happens Next

Review all variances with warehouse staff to identify causes (damage, theft, counting error, system error, etc.). Once causes are identified and approved, record inventory adjustments to bring the system quantities in line with the physical count. See WH-COUNT-002 and WH-COUNT-003 for procedures on recording adjustments.

## Common Issues

**Report shows items with NOTINCOUNT status**
These items exist in the system but were not found during the count. Verify the items are still in the warehouse. If items are missing, they may have been damaged, lost, or incorrectly recorded. Investigate and mark as scrapped if appropriate. See WH-RMA-002c for scrap procedures.

**Large negative variance**
The physical count is less than the system quantity. This may indicate items were damaged, lost, or sold without updating the system. Investigate with warehouse staff to determine what happened to the items. Record a scrap adjustment if items are no longer recoverable.

**Large positive variance**
The physical count is more than the system quantity. This is unusual and may indicate a data entry error, receiving error, or duplicate counts. Verify the count and check receiving records to explain the overage.

**Variance report differs from Physical Inventory Report**
Both reports show the same count data. Any differences may be due to different filtering or timing. Verify the count number and date are the same on both reports.

**Cannot locate count by count number**
Verify the count number is correct and has been completed. If the count is still in progress, it may not appear in the report. Check with warehouse management to confirm the count status.

**Avg Value column shows unexpected values**
Avg Value = Qty Counted × Avg Cost. If the cost seems incorrect, verify the average cost was properly calculated for the item. Consult with accounting if cost data appears inaccurate.
