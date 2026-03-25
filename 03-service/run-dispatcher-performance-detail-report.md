---
title: Run the Dispatcher Performance Detail Report
id: SVC-RPT-008
module: Service
screen: Dispatcher Performance Detail Report
menu_path: Service > Reports > Dispatcher Performance Detail
applies_to: Service Managers, Operations Managers, Human Resources
prerequisites:
  - Access to Service Reports
  - Permission to view dispatcher performance data
  - Service calls must be assigned to dispatchers
related_procedures:
  - SVC-RPT-009
tags:
  - Reports
  - Performance
  - Dispatcher Management
  - KPIs
version: 1.0
last_updated: 2026-03-25
---

# Run the Dispatcher Performance Detail Report

## What This Procedure Does

The Dispatcher Performance Detail Report shows individual call records for each dispatcher with response times and outcomes. Use this report to evaluate dispatcher performance, identify training needs, and ensure consistent service delivery.

## Before You Begin

- Have permission to access Service Reports
- Determine the date range for evaluation
- Identify which dispatcher(s) to analyze
- Have performance standards for comparison

## Steps

### Step 1: Open Dispatcher Performance Detail Report

Go to Service > Reports > Dispatcher Performance Detail. The Print Report dialog opens with filter options.

### Step 2: Set Filter Criteria

Configure filters to define the analysis:

| Field | What to select |
|-------|----------------|
| Company | Select the company |
| Branch | Select the branch (optional) |
| Department | Select the department (optional) |
| Date Range | Enter start and end dates |
| Dispatcher | Select specific dispatcher (optional) |

Leave Dispatcher blank to include all dispatchers, or select one for focused analysis.

### Step 3: Run the Report

Click Run Report. The report generates and displays in Print Report dialog or Live Data grid.

### Step 4: Review Dispatcher Performance Data

The report displays line items for each call showing:

- Dispatcher Name
- Call No
- Customer
- Call Created Date/Time
- Call Dispatched Date/Time
- Response Time (minutes to dispatch)
- Technician Assigned
- Call Status
- Call Outcome
- Priority Level

### Step 5: Analyze Performance Metrics

Review response times against organizational standards. Identify calls with extended response times. Evaluate dispatch efficiency, call complexity, and outcome quality. Compare performance across dispatchers over the same period.

## What Happens Next

Results support performance reviews, training planning, and process improvement. High performers can be recognized or promoted. Slower response times may indicate workload issues, training needs, or system bottlenecks. Use the report to set targets and track improvement over subsequent periods.

## Common Issues

**No Data Displayed**
Verify the date range includes dispatched calls. Ensure dispatchers are assigned to calls in the system. Check that the dispatcher filter is not too restrictive.

**Cannot Identify Root Cause of Slow Response**
Review individual calls to understand context (e.g., call volume spike, complex dispatch). Check system logs for any dispatch delays. Interview the dispatcher about workload or challenges.

**Report Does Not Match Manual Records**
Verify the date range in the report filter. Confirm all calls have dispatcher assignments. Check if any calls were reassigned multiple times.
