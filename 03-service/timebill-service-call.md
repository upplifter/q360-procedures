---
title: Time Bill a Service Call
id: SVC-CALL-007
module: Service
screen: Service Call Form / Time Bills Tab
menu_path: Service > Service Calls
applies_to: Technicians, Service Managers
prerequisites:
  - Service call exists in DISPATCHED or TECHDONE status
  - Technician has completed or is completing work on the call
  - Service work time is known
related_procedures:
  - SVC-CALL-006
  - SVC-CALL-008
tags:
  - time-tracking
  - labor-cost
version: 1.0
last_updated: 2026-03-25
---

# Time Bill a Service Call

## What This Procedure Does

This procedure records the time spent by a technician performing service work on a call. You can start a live timer from the task list, or manually enter time entries directly on the Time Bills tab. Time bills track labor costs against the call and are posted later to generate cost entries and billing records.

## Before You Begin

- Service call is assigned to a technician and in DISPATCHED or TECHDONE status
- Technician has completed service work or is actively working on the call
- Start and end times are known, or a live timer will be used
- Work type is identified (e.g., Labor, Travel, Diagnostics)

## Steps

### Method 1: Use Live Timer from Task List

#### Step 1: Access the Task List

Navigate to My Tasks or open the Dispatch Q (Service > Work Queues > Dispatch Q). The list displays all assigned service calls for the current user.

#### Step 2: Start the Timer

Locate the service call in the list. Click the Start Timebill clock or play icon on the call row. A timer begins tracking elapsed time, and the icon changes to indicate timing is active.

#### Step 3: Stop the Timer

When the service work is complete, click the Stop Timebill icon (stop/square icon) on the same call row. The timer stops and the elapsed time is recorded. A time bill entry is automatically created with the calculated duration.

#### Step 4: Time Bill Created

The time bill appears on the Time Bills tab of the service call with the calculated start time, end time, and duration. The entry remains unposted until posted via SVC-CALL-008.

### Method 2: Manually Enter Time on Time Bills Tab

#### Step 1: Open the Service Call

Navigate to Service > Service Calls. Click the call number to open the Service Call form.

#### Step 2: Access Time Bills Tab

Click the Time Bills tab. The grid displays any existing time entries for this call. Click Add (plus icon) to create a new time bill entry.

#### Step 3: Enter Time Information

Fill in the following fields:

| Field | What to enter |
|-------|---------------|
| Employee | Select the technician or employee who performed the work |
| Start Time | Enter the date and time when work began |
| End Time | Enter the date and time when work ended |
| Work Type | Select the work type (Labor, Travel, Diagnostics, etc.) |
| Description | Enter a brief description of work performed |

#### Step 4: Save the Time Entry

Click Save (floppy disk icon). The system calculates the duration and saves the time bill entry. The entry remains unposted.

## What Happens Next

Time bill entries are created but not yet posted to the accounting system. Multiple time entries can be added to a single call (e.g., separate entries for travel, diagnostics, and labor). Proceed with SVC-CALL-008 to post all unposted time bills and generate cost entries. Posted time bills become part of the call's labor cost and can be billed to the customer through AR Journal entries.

## Common Issues

**Timer Started But Not Stopped on Completion**
If you forget to stop the timer, the elapsed time will continue accumulating. Return to the task list and click Stop Timebill immediately to end the timing session. You can then manually adjust the end time on the Time Bills tab if the recorded duration is inaccurate.

**Duplicate Time Bill Entries Created**
Avoid using both the live timer and manual entry methods for the same work session, as this may create duplicate time entries. Use one method per work session. If duplicates exist, delete the extra entry using the Delete action on the Time Bills tab.

**Time Entry Missing Employee or Work Type**
The system requires Employee and Work Type to be populated. If you skipped these fields during entry, click Edit (pencil icon) on the time bill row and complete the missing information before posting.
