---
title: Schedule a Service Call
id: SVC-CALL-005
module: Service
screen: Service Call Form / Resource Console
menu_path: Service > Service Calls or Service > Resource Console
applies_to: Customer Service Representatives, Service Managers, Dispatch Coordinators
prerequisites:
  - Service call exists in OPEN status
  - Technician is available on requested date
  - Scheduling window is known
related_procedures:
  - SVC-CALL-001
  - SVC-CALL-004
  - SVC-CALL-006
tags:
  - scheduling
  - resource-management
version: 1.0
last_updated: 2026-03-25
---

# Schedule a Service Call

## What This Procedure Does

This procedure assigns a service call to a technician and creates a scheduled dispatch. You can schedule using the call form directly or by dragging the call onto a technician's timeline in the Resource Console. After scheduling, the call status changes to SCHEDULED and is ready for dispatch.

## Before You Begin

- Service call exists in OPEN status
- Technician availability information is known
- Customer preferred dates and times are confirmed
- Estimated call duration is available

## Steps

### Method 1: Schedule from the Service Call Form

#### Step 1: Open the Service Call

Navigate to Service > Service Calls or open the Service Calls tab on the customer record. Click the call number to open the Service Call form. Verify the call status is OPEN.

#### Step 2: Access the Dispatch Tab

Click the Dispatch tab on the Service Call form. The Dispatch grid displays any existing schedule entries for this call.

#### Step 3: Add Schedule Entry

Click Add (plus icon) in the schedule grid. A new row appears for data entry.

#### Step 4: Enter Scheduling Information

Fill in the following fields:

| Field | What to enter |
|-------|---------------|
| Technician | Select the technician assigned to the call |
| Scheduled Start Date/Time | Enter the date and time when service begins |
| Scheduled End Date/Time | Enter the date and time when service ends |

#### Step 5: Save the Schedule

Click Save (floppy disk icon). The system saves the schedule entry and automatically changes the call status to SCHEDULED. The technician is now assigned to the call.

### Method 2: Schedule Using Resource Console

#### Step 1: Open Resource Console

Navigate to Service > Resource Console. The Resource Console displays a timeline view with technicians listed on the left and their scheduled work on the right.

#### Step 2: Locate the Unscheduled Call

Find the service call in the unassigned calls list (typically shown at the top or in a left sidebar). The call appears with its customer name and call number.

#### Step 3: Drag Call to Technician Timeline

Click and drag the call from the unassigned list onto the technician's timeline at the desired date and time. The call snaps to the technician's schedule slot. A dialog may appear to confirm the scheduled start and end times.

#### Step 4: Confirm the Schedule

Review the schedule slot on the technician's timeline. Click Save or confirm the dialog. The system immediately changes the call status to SCHEDULED and creates the dispatch record.

## What Happens Next

The call now appears in SCHEDULED status. The assigned technician can view the call in their task list. You can proceed with SVC-CALL-006 to dispatch the call and send notification to the technician. The call remains in SCHEDULED status until it is dispatched.

## Common Issues

**Technician Not Available on Requested Date**
Review the Resource Console to identify available technicians on the requested date. If no technician is available, extend the search to adjacent dates or request alternative scheduling options from the customer using SVC-CALL-004.

**Schedule Overlap with Another Call**
The system may prevent scheduling if the technician already has a call scheduled at the same time. Review the technician's timeline in the Resource Console to identify available gaps. Adjust the scheduled start/end times to avoid conflicts.

**Schedule Not Saved After Drag-and-Drop**
If the Resource Console drag-and-drop does not save the schedule, verify the technician's calendar is not locked for editing. Return to the Service Call form and use Method 1 to manually enter the schedule details instead.
