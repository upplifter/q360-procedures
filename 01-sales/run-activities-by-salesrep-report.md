---
title: Run the Activities by Sales Rep Report
id: SALES-RPT-008
module: Sales
screen: Activities by Sales Rep - Sales Opp Only Report
menu_path: Live Data > SALES > Activities by Sales Rep - Sales Opp Only
applies_to:
  - Sales Rep
  - Sales Manager
prerequisites:
  - Access to Live Data reports
  - Activities linked to opportunities exist in the system
related_procedures:
  - SALES-ACTIVITY-001
  - SALES-RPT-007
  - SALES-OPP-001
tags: activities by sales rep, opportunity activities, sales opp activities, activity by rep, sales rep activity report, opportunity engagement
version: 1.0
last_updated: 2026-03-25
---

# Run the Activities by Sales Rep Report

## What This Procedure Does

Runs the Activities by Sales Rep - Sales Opp Only report to display activities that are linked to sales opportunities. This focused view shows real-time engagement levels across open deals, helping managers identify which opportunities are receiving attention and which may be stalled.

## Before You Begin

- You have access to Live Data reports.
- Activities linked to sales opportunities exist in the system.

## Steps

### Step 1: Open the Report

Navigate to **Live Data > SALES** and select **Activities by Sales Rep - Sales Opp Only**.

### Step 2: Set Filters

| Field | What to enter |
|---|---|
| Start Date | Set the beginning of the date range (default is today). |
| End Date | Set the end of the date range (default is today). |
| Sales Rep | Select a specific sales rep or ALL. |
| Customer Sub Type | Select a customer sub-type classification or ALL. |

### Step 3: Review the Report

The report returns one row per activity with the following columns:

- **Zoom Drilldown** - clickable icon to open the activity record.
- **Activity No** - unique identifier.
- **Sales Rep** - the sales representative responsible.
- **Contact** - primary customer contact.
- **Customer No** - the customer identifier.
- **Company** - customer company name with drilldown.
- **Date** - the activity date.
- **Title** - brief subject of the activity.
- **Activity Type** - category (Call, Meeting, Email, etc.).
- **Comment** - narrative notes.

The report is sorted by Sales Rep then by Date in ascending order.

### Step 4: Identify Gaps

Compare the activity dates across opportunities to identify deals with no recent touchpoints. Opportunities without recent activities may need immediate follow-up.

## What Happens Next

Use this report for coaching conversations, pipeline review meetings, and compliance tracking for documented customer interactions. For a broader activity view that includes non-opportunity activities, see SALES-RPT-007.

## Common Issues

**The report returns no results.**
Expand the date range - both dates default to today. Also confirm activities exist that are linked to opportunities.

**Activities you expect are missing.**
This report only includes activities linked to sales opportunities or their related customer, invoice, contact, or site records. Activities not connected to an opportunity are excluded.

**You see activities from reps outside your team.**
Adjust the Sales Rep filter to show only your team members. The report respects your access permissions.

**The Customer Sub Type filter has no effect.**
If no sub-types are configured in your system, this filter has no impact. Leave it set to ALL.

**You want to see the opportunity details alongside the activities.**
This report focuses on activities. For opportunity details, drill into the activity and navigate to the linked opportunity, or cross-reference with the Sales Opportunity Review (SALES-RPT-004).
