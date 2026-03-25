---
title: Run the Dispatcher Performance Summary Report
id: SVC-RPT-009
module: Service
screen: Dispatcher Performance Summary Report
menu_path: Service > Reports > Dispatcher Performance Summary
applies_to: Service Managers, Operations Managers, Executive Leadership
prerequisites:
  - Access to Service Reports
  - Permission to view dispatcher performance data
  - Service calls must be assigned to dispatchers
related_procedures:
  - SVC-RPT-008
tags:
  - Reports
  - Performance
  - Dispatcher Management
  - Summary
version: 1.0
last_updated: 2026-03-25
---

# Run the Dispatcher Performance Summary Report

## What This Procedure Does

The Dispatcher Performance Summary Report aggregates Key Performance Indicators (KPIs) for all dispatchers including total calls, daily averages for new/dispatched/closed calls, and response time metrics. Use this report for overall operations evaluation and comparative performance analysis.

## Before You Begin

- Have permission to access Service Reports
- Determine the date range for evaluation
- Identify performance benchmarks or targets
- Prepare to compare multiple periods if needed

## Steps

### Step 1: Open Dispatcher Performance Summary Report

Go to Service > Reports > Dispatcher Performance Summary. The Print Report dialog opens with filter options.

### Step 2: Set Filter Criteria

Configure filters to define the analysis:

| Field | What to select |
|-------|----------------|
| Company | Select the company |
| Branch | Select the branch (optional) |
| Department | Select the department (optional) |
| Date Range | Enter start and end dates |

### Step 3: Run the Report

Click Run Report. The report generates and displays in Print Report dialog or Live Data grid.

### Step 4: Review Summary KPIs

The report displays aggregated metrics per dispatcher:

- Dispatcher Name
- Total Calls (new calls received)
- Total Dispatched (calls assigned to technicians)
- Total Closed (calls completed)
- Daily Average New Calls
- Daily Average Dispatched Calls
- Daily Average Closed Calls
- Average Response Time
- Efficiency Rating

### Step 5: Compare Performance Across Dispatchers

Identify top and bottom performers. Look for consistency in metrics. Compare current period to previous periods to track trends. Share results with dispatcher team for recognition or coaching.

## What Happens Next

Results provide a high-level view of dispatch operations. Use summary metrics to identify if volume is evenly distributed across dispatchers, if response times meet targets, and if closing rate matches expectations. Plan workload rebalancing or staffing changes based on results.

## Common Issues

**Dispatcher With Missing Data**
Verify the dispatcher has calls assigned in the system during the date range. Check that all calls are properly recorded. Contact dispatcher if individual records appear missing.

**Metrics Do Not Match Expected Values**
Confirm the date range is correct. Check if calls are properly assigned to dispatchers. Verify no calls were incorrectly excluded from the report.

**Cannot Understand Efficiency Rating Calculation**
Efficiency rating is typically calculated from a combination of response time and call closure rate. Consult your system administrator for the specific formula used in your environment.
