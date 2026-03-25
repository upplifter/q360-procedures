---
title: Create a Call Event
id: SVC-CALL-009
module: Service
screen: Service Call Form - Events Tab
menu_path: Service > Service Calls
applies_to: Customer Service Representatives, Service Managers, Technicians
prerequisites:
  - Service call exists in the system
  - Event type is selected from the EVENTTYPE general code
related_procedures:
  - SVC-CALL-010
tags:
  - audit-trail
  - event-tracking
  - documentation
version: 1.0
last_updated: 2026-03-25
---

# Create a Call Event

## What This Procedure Does

This procedure creates an event entry on a service call to document status changes, notes, system actions, or communication milestones. Events provide an audit trail of all significant actions taken on a call. Events can be triggered manually or automatically by the system, and can generate email alerts if configured.

## Before You Begin

- Service call exists in the system
- Event type is identified (e.g., Status Change, Note, Customer Contact, Technician Assignment)
- Event date and time are known
- Event description details are available

## Steps

### Step 1: Open the Service Call

Navigate to Service > Service Calls or the Service Calls tab on the customer record. Click the call number to open the Service Call form.

### Step 2: Access the Events Tab

Click the Events tab. The grid displays all existing events for this call in chronological order, including system-generated events (e.g., call created, status changes) and manually created events.

### Step 3: Create New Event

Click Add (plus icon) in the Events grid. A new row appears for data entry.

### Step 4: Enter Event Information

Fill in the following fields:

| Field | What to enter |
|-------|---------------|
| Event Type | Select the event type from the dropdown (Status Change, Note, Customer Contact, Technician Assignment, etc.) |
| Description | Enter a detailed description of the event, notes, or action taken |
| Date/Time | Enter the date and time when the event occurred |

### Step 5: Save the Event

Click Save (floppy disk icon). The system records the event and displays it in the Events grid. The event becomes part of the call's permanent audit trail.

## What Happens Next

The newly created event appears in the Events tab and is visible to all users who access the call. The event is timestamped with the creation date and user ID. If the event type is configured to trigger email alerts, the system sends notifications to relevant stakeholders (customer, technician, manager). System-generated events (e.g., status changes) are created automatically and cannot be edited.

Proceed with SVC-CALL-010 to monitor and review all call events across the system in the Events Q.

## Common Issues

**Event Type Not Available in Dropdown**
If the expected event type is missing from the dropdown, the EVENTTYPE general code may not be configured with that type. Contact your system administrator to add the missing event type to the general code. In the interim, use a similar event type or add a note event with the relevant information.

**Event Not Appearing in Events Grid**
After saving, click Refresh (circular arrow icon) on the Events tab to refresh the grid view. The newly created event should appear at the bottom of the chronological list. If it still does not appear, verify that Save was clicked and no error messages were displayed.

**Email Alert Not Sent for Event Creation**
Email alert configuration is controlled at the event type level in the system configuration. If alerts are not being sent, verify that the event type is configured to trigger notifications. Contact your system administrator to enable alerts for specific event types if needed.
