---
title: Run the Physical Inventory Report
id: WH-RPT-005
module: Warehouse
screen: Physical Inventory Report (Q0202)
menu_path: Inventory > Reports > Physical Inventory
applies_to:
  - Warehouse Manager
prerequisites:
  - Access to Inventory reports menu
  - Physical inventory count has been recorded
related_procedures:
  - WH-COUNT-001a
  - WH-COUNT-001b
  - WH-RPT-006
tags: reporting, physical-inventory, cycle-counting, inventory-records
version: 1.0
last_updated: 2026-03-25
---

# Run the Physical Inventory Report

## What This Procedure Does

This report displays physical inventory count records and results. Use this to view count details, track counting progress, and document physical inventory counts for audit and reconciliation purposes.

## Before You Begin

- Have access to the Inventory reports menu
- Know the count number you want to report on, or be prepared to select from available counts
- Determine if you want to view a specific count or all recent counts

## Steps

### Step 1: Navigate to the Report

Go to Inventory > Reports > Physical Inventory. The system opens the report filter screen.

### Step 2: Select the Count

In the Count No filter field, select from the available physical inventory counts:

| Field | What to enter |
|-------|---------------|
| Count No | Select the specific count number to report on, or leave blank to include all counts |

### Step 3: Run the Report

Click the appropriate button to generate or view the report. The system compiles the count data for the selected count(s).

### Step 4: Review the Count Data

The report displays the following columns for each item counted:

| Column | Description |
|--------|-------------|
| Count No | Physical inventory count identifier |
| Count Date | Date the count was performed |
| Asset | Asset number of the item counted |
| Description | Item description |
| Status | Count status (COUNTED, RECOUNTED, or other status) |
| Master No | Master inventory number |
| Qty Counted | Physical quantity counted during the count |
| Branch | Warehouse branch where the item is located |
| User | Name or ID of the user who performed the count |
| Master Location | Primary warehouse location for the master |
| Count Location | Specific location where the item was physically counted |

### Step 5: Analyze the Results

Review the quantities counted and compare to system records. Identify any items with unusual or unexpected counts. Note the user and location information for follow-up if needed.

### Step 6: Export or Archive

Use the Extended Menu (three vertical dots) to export the report to Excel or PDF. Save the report for audit documentation and reconciliation with the Physical Inventory Variance Report (WH-RPT-006).

## What Happens Next

After the physical count is recorded and documented, run the Physical Inventory Variance Report (WH-RPT-006) to identify discrepancies between counted and system quantities. Work with warehouse staff to investigate variances and record any necessary inventory adjustments.

## Common Issues

**Report shows no count data**
Verify the count number exists and has been completed. If you left Count No blank, the system may only show recent counts. Check that the count date falls within the current fiscal period.

**Count location differs from master location**
This is normal if inventory has been moved or is being stored in a temporary location. The Count Location shows where the item was physically located during the count. Verify with warehouse staff that the location is correct.

**Qty Counted appears to be zero**
If an item shows Qty Counted = 0, verify that it was actually counted. A zero quantity may indicate the item was not found during the physical count. Cross-reference with WH-RPT-006 (Physical Inventory Variance) to see if the system expected inventory.

**Cannot filter to a specific count**
Verify the count number is correct. If you cannot find a specific count, it may not have been completed yet or may be archived. Check with warehouse management to confirm the count exists.

**User or location information is missing**
If user or location fields are blank, the count data may be incomplete. Contact warehouse staff to verify the count was properly recorded with all required information.
