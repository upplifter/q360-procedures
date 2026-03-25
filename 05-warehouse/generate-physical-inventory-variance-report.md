---
title: Generate a Physical Inventory Variance Report
id: WH-COUNT-002
module: Warehouse
screen: Physical Inventory Variance Report (Q0166)
menu_path: Live Data > INVENTORY > Physical Inventory Variance
applies_to:
  - Warehouse Manager
prerequisites:
  - Physical inventory counts have been entered or imported (see WH-COUNT-001b or WH-COUNT-001c-alt)
related_procedures:
  - WH-COUNT-001b
  - WH-COUNT-001c-alt
  - WH-COUNT-003
tags: physical inventory, variance, report, Q0166
version: 1.0
last_updated: 2026-03-25
---

# Generate a Physical Inventory Variance Report

## What This Procedure Does

Run the Physical Inventory Variance Report (Q0166) to compare counted quantities from the physical inventory against system on-hand quantities. This report identifies discrepancies and items found in the system but not counted, which must be reviewed and resolved before posting variances.

## Before You Begin

- Physical inventory counts have been entered or imported for the count session (see WH-COUNT-001b or WH-COUNT-001c-alt)
- You have Warehouse Manager role to view and act on the report
- You have access to the Live Data reporting module

## Steps

### Step 1: Open the Variance Report

Navigate to **Live Data > INVENTORY > Physical Inventory Variance**. The Physical Inventory Variance Report (Q0166) opens.

The report defaults to show all counts and variances. Apply a filter to focus on a specific count session if multiple counts are in progress.

### Step 2: Apply Filter by Count Number

Click the **Filter** button and select or enter the Count No. for the physical inventory count session you want to review. This filters the report to show only items from that count.

Click **Apply** to display the variance data for the selected count.

### Step 3: Review Variance Report Columns

The report displays the following columns for each item:

| Column | Description |
|--------|-------------|
| Master No. | The inventory master number |
| Asset No. | Serial number (A-type items only) |
| Description | Item description from the master |
| Item Status | Current status (NOTINCOUNT if found in system but not counted) |
| Location | Warehouse location |
| Qty Counted | Physical count quantity entered |
| Variance | Difference between counted and system on-hand (Counted - On Hand) |
| Var. Used | Indicator if variance has been used/posted |
| Qty on Hand | Current system on-hand quantity |
| Qty Received | Received quantity in current period |
| Qty Shipped | Shipped quantity in current period |
| Avg Cost | Average cost per unit |
| Avg Value | Total value (Qty on Hand × Avg Cost) |

### Step 4: Identify Items with Status "NOTINCOUNT"

Scan the report for items with status **NOTINCOUNT**. These items exist in the system but were not physically found or counted. Qty Counted will show 0 for these items.

Investigate these items:

- Were they present but missed during the physical count?
- Have they been shipped or used since the count began?
- Do they need to be physically located and counted?

Items with NOTINCOUNT status must be resolved before variances can be posted.

### Step 5: Review Variance Amounts

For items that were counted, the Variance column shows the difference between physical count and system on-hand:

- **Positive variance**: More items were counted than the system shows (count > on-hand)
- **Negative variance**: Fewer items were counted than the system shows (count < on-hand)
- **Zero variance**: Count matches system exactly; no adjustment needed

Items with significant variances should be investigated. Verify that:

- Count quantities were entered correctly
- System on-hand was accurate before the count
- No transactions occurred during the count period that are unrecorded

### Step 6: Export Report for Review

Click the **Export** button to download the variance report to Excel. This allows you to:

- Share the report with management for approval
- Manually verify variances against count sheets
- Document variance reasons before posting
- Archive the report for audit purposes

## What Happens Next

After reviewing the variance report, the Warehouse Manager must obtain management approval for posting variances. Once approved, variances are posted (see WH-COUNT-003), which adjusts system on-hand quantities and records corresponding GL journal entries to reconcile inventory accounts.

## Common Issues

**Report shows no data after filtering by count number**

Verify that the Count No. you entered exists and that counts have been entered or imported for that count session. Refresh the report or clear the filter and re-enter the count number exactly as it appears in the system. Check that the count session status is active and not archived.

**Items showing NOTINCOUNT status but should have been counted**

These items were in the system but not physically found during the count. They may have been:

- Shipped or issued after the count session was created but before the warehouse was locked
- Located in a different warehouse section or location that was not counted
- Scrap or damaged items that should be addressed

Coordinate with the counting team to determine if a recount is needed or if the items can be physically located and verified.

**Variance amounts seem incorrect or unrealistic**

Verify that counts were entered correctly by cross-referencing against count sheets. Check the system on-hand quantity before the count to ensure it was accurate. Confirm that no transactions (receipts, shipments, adjustments) occurred during the count period that might explain the variance. Review the count session to ensure no double-entries or data entry errors occurred.

**Cannot export report to Excel**

Verify that your system has the necessary export permissions and that the Excel export feature is enabled. Try exporting with a more limited filter (fewer records) to see if a large dataset is causing the issue. Contact your system administrator if export functionality is unavailable.

**Report is very large and difficult to review**

Apply filters to focus on specific criteria such as:

- Items with variance > 0 or < 0 (exclude zero-variance items)
- Specific locations or master types
- High-value items using the Avg Value column

This narrows the report to focus on items requiring investigation.
