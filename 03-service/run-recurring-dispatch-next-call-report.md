---
title: Run the Recurring Dispatch - Next Call Date Report
id: SVC-RPT-020
module: Service
screen: Recurring Dispatch - Next Call Date Report
menu_path: Service > Reports > Recurring Dispatch - Next Call Date
applies_to: Service Managers, Dispatchers, Scheduling Staff
prerequisites:
  - Access to Service Reports
  - Permission to view recurring dispatch data
  - Recurring dispatch schedules must be configured
related_procedures:
  - SVC-ADMIN-001
tags:
  - Reports
  - Recurring Dispatch
  - Scheduling
  - Upcoming Calls
version: 1.0
last_updated: 2026-03-25
---

# Run the Recurring Dispatch - Next Call Date Report

## What This Procedure Does

The Recurring Dispatch - Next Call Date Report shows recurring dispatch records with calculated next call dates. This report integrates dispatch, billing, and scheduling information to help track and plan upcoming service engagements.

## Before You Begin

- Have permission to access Service Reports
- Identify the company and branch scope
- Determine the bill date or scheduling period
- Understand your recurring dispatch frequency patterns

## Steps

### Step 1: Open Recurring Dispatch - Next Call Date Report

Go to Service > Reports > Recurring Dispatch - Next Call Date. The Print Report dialog opens with filter options.

### Step 2: Set Filter Criteria

Configure filters to define the report scope:

| Field | What to select |
|-------|----------------|
| Company | Select the company |
| Branch | Select the branch (optional) |
| Department | Select the department (optional) |
| Bill Date | Enter the billing or scheduling period date |

### Step 3: Run the Report

Click Run Report. The report generates and displays in Print Report dialog or Live Data grid.

### Step 4: Review Recurring Dispatch and Next Call Dates

The report displays:

- Recurring Dispatch Record No
- Service Contract No
- Customer Name
- Site Location
- Dispatch Frequency (weekly, monthly, quarterly, etc.)
- Last Call Date
- Next Scheduled Call Date
- Billing Information
- Status (Active, Paused, Completed)

Rows are sorted by next call date to highlight upcoming engagements.

### Step 5: Plan and Coordinate Upcoming Calls

Review the next call dates to plan field schedules and resource allocation. Identify calls coming due in the next week or month. Coordinate with technicians to ensure availability. Track completion of recurring calls against this schedule.

## What Happens Next

Results guide scheduling and resource planning for recurring service. Use the report to ensure recurring commitments are met on schedule. Track actual call dates against planned dates. Use variances to identify scheduling issues or customer problems.

## Common Issues

**No Recurring Dispatches Displayed**
Verify recurring dispatch schedules are configured in the system. Check that the bill date or period is appropriate. Ensure the company and branch filters are correct.

**Next Call Date Appears Incorrect**
Verify the last call date is accurate. Check the dispatch frequency configuration. Confirm no pauses or cancellations are in effect for the dispatch.

**Cannot Identify Overdue Calls**
Compare the next call date to today's date. Calls with next call dates in the past are overdue. Contact the relevant technician or dispatcher to schedule the overdue call.
