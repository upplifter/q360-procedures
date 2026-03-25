---
title: Time Bill a Project Task
id: PROJ-TB-001
module: Projects
screen: My Tasks / Task Form
menu_path: View > My Tasks
applies_to: Project Team Member, Project Manager, Technician
prerequisites: TIMEBILL (Create) permission, Task is assigned to the user or user has permission to bill against the task
related_procedures:
  - PROJ-TB-002
  - PROJ-RESOURCE-001
tags:
  - time bill
  - timebill
  - log time
  - clock
  - project task
  - my tasks
  - labor
  - hours
  - time tracking
  - time entry
version: 1.0
last_updated: 2026-03-25
---

# Time Bill a Project Task

## What This Procedure Does

This procedure starts and stops a time bill against a project task from My Tasks or drills into a task to log time manually. Time bills track actual labor hours worked on project tasks and feed into project costing, payroll, and revenue recognition.

## Before You Begin

Ensure you have TIMEBILL (Create) permission. The task must be assigned to you, or you must have permission to bill time against the task. You will be starting and stopping a time bill to track your work hours.

## Steps Using My Tasks

### Step 1: Access My Tasks

Click View > My Tasks in the Q360 web client. The My Tasks view opens displaying all tasks assigned to you.

### Step 2: Locate the Project Task

Find the task you want to time bill in the task list. The list shows task titles, projects, and status information.

### Step 3: Start a Time Bill

Click the clock icon (Time Bill button) associated with the task. A time bill is created and begins recording elapsed time immediately.

### Step 4: Confirm Time Bill Started

A currently running time bill displays in yellow at the top of the task list, highlighting which task's time is being recorded. The yellow highlighting indicates an active, running time bill.

### Step 5: Continue Your Work

Proceed with the work on the project task. The time bill runs in the background tracking elapsed time. You can navigate away from My Tasks to work on the project or access other Q360 features while the time bill runs.

### Step 6: Stop the Time Bill

When you have completed work on the task, return to My Tasks. Locate the yellow-highlighted task representing your active time bill.

Click the clock icon next to the yellow-highlighted task to stop the time bill. The time bill closes and stops recording elapsed time.

## To Adjust Time After Stopping

### Step 1: Navigate to the Time Bill Record

After stopping a time bill, click into the task record to access the time bill details. The time bill record displays with your recorded time.

### Step 2: Edit the Time Bill

Click Edit (pencil icon) on the time bill record. The time bill enters edit mode allowing modifications.

### Step 3: Adjust Start or End Date/Time

Modify the start date/time or end date/time fields if needed. Use these fields if you need to correct the times recorded by the system, or if you need to adjust for breaks or other corrections.

### Step 4: Observe Calculated Fields

As you adjust start and end times, notice:
- **Billed Time**: The duration that will be used for project costing and billing purposes
- **Log Time**: The total elapsed time recorded on the time bill

These fields update automatically as you modify the time fields.

### Step 5: Enter Billed Time Directly

You can also bypass adjusting start/end times by directly entering a value in the Billed Time field. Billed Time is the value actually used for costing, billing, and potentially payroll calculations. Enter the actual number of hours you worked on the task.

For example, if you worked 4 hours on the task but took a 1-hour lunch break, enter 4 in the Billed Time field rather than stopping/starting the time bill.

### Step 6: Save Changes

Click Save (floppy disk icon). The time bill is saved with your adjusted time entries.

## What Happens Next

Your time bill hours are now recorded against the project task. The hours feed into:
- Project cost tracking and profitability analysis
- Resource utilization and availability calculations
- Payroll processing for labor-based compensation
- Revenue recognition for labor-hour billing models

Continue to time bill all work on project tasks to maintain accurate project records.

## Common Issues

**Clock Icon Does Not Appear Next to My Task**
You may not have TIMEBILL (Create) permission or the task may not be assigned to you. Verify your user permissions include time bill creation. If the task is not assigned to you, contact your project manager to add you to the task assignment.

**Time Bill Started But I Cannot Find the Yellow Highlighted Task**
The yellow highlighted task appears at the top of the My Tasks list. Scroll to the top of the task list to locate your active time bill. If you navigated away from My Tasks, return to View > My Tasks to see the running time bill.

**Billed Time and Log Time Show Different Values**
Log Time is the actual elapsed time the system recorded. Billed Time is what you manually entered or the duration the system calculated. You can intentionally set Billed Time to differ from Log Time (e.g., to account for breaks). Verify the Billed Time value represents the actual billable hours you worked.

**Cannot Stop a Running Time Bill**
Click the clock icon again on the active task in My Tasks. If the icon does not respond, click into the time bill record directly and look for a Stop Time button. You can also edit the end time directly in the time bill record to close it.

**Need to Split Time Across Multiple Tasks**
Create separate time bills for each task. Stop the first time bill, then start a new time bill on the second task. Each task will have its own time bill record with the hours worked on that specific task.

**Time Bill Created on Wrong Task**
If you accidentally started a time bill on the wrong task, stop it immediately and create a correct time bill on the right task. You can then edit the incorrect time bill to set Billed Time to zero, or delete it if your system allows. Contact your administrator if you need help correcting an erroneous time bill.
