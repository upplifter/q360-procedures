---
title: Log Presales Time Against Opportunity
id: SALES-PRESALES-003
module: Sales
screen: My Tasks / Opportunity Form
menu_path: Main Menu > View > My Tasks
applies_to:
  - Engineering
  - Sales Rep
prerequisites:
  - TIME BILL (Create) permission assigned to your user or group
  - An opportunity exists (see SALES-OPP-001)
  - For task-based time logging, a presales assignment exists in your task list (see SALES-PRESALES-002)
related_procedures:
  - SALES-PRESALES-001
  - SALES-PRESALES-002
  - SALES-PRESALES-004
tags: presales time, time bill, log time, opportunity time, timer, my tasks, presales hours, engineering time
version: 1.0
last_updated: 2026-03-25
---

# Log Presales Time Against Opportunity

## What This Procedure Does

Logs time spent on presales work against a sales opportunity. Time can be logged from the My Tasks list (if you have an assigned funnel task) or directly from the Opportunity form. Logged time feeds into presales cost tracking and the Sales Opportunity Labor Conversion report.

## Before You Begin

- You have TIME BILL (Create) permission.
- The opportunity exists in Q360.
- If logging from My Tasks, you have been assigned a presales funnel task (see SALES-PRESALES-002).

## Steps

### Step 1: Option A - Log Time from My Tasks

1. Navigate to **Main Menu > View > My Tasks**.
2. Locate the opportunity task in your task list.
3. Click the **Timer** button (clock icon) next to the opportunity task to start the time bill. The time bill begins recording and displays in yellow at the top of your task list.
4. When you finish working, click the **Timer** button next to the yellow-highlighted active time bill to stop it.

### Step 1: Option B - Log Time from the Opportunity Form

1. Look up the opportunity from **Main Menu > Sales > Opportunities**.
2. Click the **Time Bill** button (clock/play icon) on the Opportunity form action bar to start a time bill.

### Step 2: Adjust Time (If Needed)

1. Drill into the time bill record by clicking on it in My Tasks or from the opportunity.
2. Click the **Edit Record** button (pencil icon).
3. Adjust the start or end date and time as needed. The Billed Time and Log Time fields update automatically to reflect the duration. You can also type a value directly into the Billed Time field.
4. Click the **Save Record** button (floppy disk icon).

## What Happens Next

The time bill is created in an unposted state and accumulates against the opportunity. The engineering manager or department manager can review and post the time bills (see SALES-PRESALES-004).

Logged presales hours appear in the Sales Opportunity Labor Conversion report (see SALES-RPT-009), which compares presales effort against project labor after the deal is won.

## Common Issues

**The Timer button is not visible on the Opportunity form.**
The Time Bill button may not be enabled for your form configuration. Use the My Tasks method instead, or contact your administrator.

**The opportunity task does not appear in My Tasks.**
Verify that you have been assigned as the Assignee on the presales funnel step (see SALES-PRESALES-002). Also check your My Tasks filters - the date range may need to be adjusted.

**The time bill records against the wrong opportunity.**
Confirm you started the timer from the correct task or opportunity. If the time bill is linked to the wrong record, edit the time bill and update the linked opportunity.

**You cannot stop the active time bill.**
Navigate to My Tasks. The active time bill appears in yellow at the top. Click the Timer button next to it to stop recording.

**Billed Time shows zero after stopping the timer.**
The start and stop times may be identical if the timer was started and stopped too quickly. Edit the time bill and manually enter the correct Billed Time value.
