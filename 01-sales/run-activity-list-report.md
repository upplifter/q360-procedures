---
title: Run the Activity List Report
id: SALES-RPT-007
module: Sales
screen: Activity List Report
menu_path: Sales > Reports > Activity List
applies_to:
  - Sales Rep
  - Sales Manager
prerequisites:
  - Access to Sales Reports
  - Sales activities exist in the system (see SALES-ACTIVITY-001)
related_procedures:
  - SALES-ACTIVITY-001
  - SALES-RPT-008
tags: activity list, activity report, sales activities, call log, meeting log, email log, activity tracking, customer touchpoints
version: 1.0
last_updated: 2026-03-25
---

# Run the Activity List Report

## What This Procedure Does

Runs the Activity List report to display a time-bounded list of all recorded sales activities including calls, emails, meetings, and other customer touchpoints. The report shows activity details alongside customer, opportunity, and sales rep information for monitoring engagement levels and workload distribution.

## Before You Begin

- You have access to Sales Reports.
- Sales activities have been recorded in the system (see SALES-ACTIVITY-001).

## Steps

### Step 1: Open the Activity List Report

Navigate to **Sales > Reports** and select **Activity List**.

### Step 2: Set Filters

| Field | What to enter |
|---|---|
| Type | Select a specific activity type (e.g., Call, Meeting, Email) or ALL. |
| Sales Rep | Select a specific sales rep or ALL. |
| Status | Select a specific activity status or ALL. |
| Start Date | Set the beginning of the date range (default is today). |
| End Date | Set the end of the date range (default is today). |

### Step 3: Review the Report

The report returns one row per activity with the following columns:

- **Activity No** - unique identifier with drilldown to the activity record.
- **Activity Type** - the category (Call, Meeting, Email, etc.).
- **Sales Rep** - the responsible sales representative.
- **Customer No** - drilldown to the customer record.
- **Title** - summary of the activity objective.
- **Date** - when the activity occurred.
- **Comment** - full narrative notes.
- **Contact** - the primary contact associated with the activity.
- **Opportunity No** - the linked opportunity, if applicable.
- **Company** - the customer company name.

The report is sorted by Sales Rep (ascending) then by Date (ascending) by default.

### Step 4: Drill Into Records

Click the Activity No or Customer No links to open the full record for detailed review.

## What Happens Next

Use the report to verify sales engagement consistency, ensure timely follow-up, and review workload distribution across the team. For a report focused specifically on opportunity-linked activities, see SALES-RPT-008.

## Common Issues

**The report returns no results.**
The Start Date and End Date both default to today. Expand the date range to include the period you want to review.

**Activities appear without an Opportunity No.**
Not all activities are linked to opportunities. Activities logged directly against a customer without an opportunity reference leave this column blank.

**You cannot see activities from other reps.**
The Sales Rep filter may be restricted by your access permissions. Contact your administrator if you need broader visibility.

**The report takes a long time to load.**
Narrow the date range or filter by a specific sales rep to reduce the data volume.

**Activity types you expect are not in the Type filter.**
Activity types are controlled by the ACTTYPE general code. Contact your administrator to verify the expected types are configured.
