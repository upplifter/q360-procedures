---
title: Monitor Call Events
id: SVC-CALL-010
module: Service
screen: Events Queue
menu_path: Service > Work Queues > Events Q
applies_to: Customer Service Representatives, Service Managers
prerequisites:
  - Events exist in the service call system
  - User has access to the Service > Work Queues menu
related_procedures:
  - SVC-CALL-009
tags:
  - event-monitoring
  - workflow-management
  - audit-trail
version: 1.0
last_updated: 2026-03-25
---

# Monitor Call Events

## What This Procedure Does

This procedure provides centralized monitoring of all service call events across the system. The Events Q displays unreviewed events that require attention, such as status changes, customer contacts, or system-generated alerts. You review events, investigate related calls, and mark events as reviewed to maintain call audit trails.

## Before You Begin

- Events exist in the system (created manually or generated automatically)
- You have access to the Service > Work Queues menu
- You want to review unreviewed events or investigate call-related activities

## Steps

### Step 1: Access the Events Queue

Navigate to Service > Work Queues > Events Q. Alternatively, open the Service Overview workflow and click the Events Q bucket. The Events Q grid displays all unreviewed events across all service calls.

### Step 2: Review Event Listing

The grid shows each event with the following information: event type, related call number, customer name, event description, date/time created, and review status. Review the list to identify events requiring action or investigation.

### Step 3: Filter Events (Optional)

Use filter options to narrow the event list by date range, event type, customer, or branch:

| Filter | What to select |
|--------|----------------|
| Date Range | Select start and end date for events |
| Event Type | Select specific event types (Status Change, Note, Alert, etc.) |
| Customer | Select a customer to view their events only |
| Branch | Select a branch to view events for that location |

Click Filter or Apply to refresh the grid.

### Step 4: Click on Event to Zoom to Call

Click an event row in the grid to navigate to the related service call. The Service Call form opens with the Events tab displayed, showing the selected event in context with all other call events.

### Step 5: Review Call and Event Context

Review the call details and the complete event history on the Events tab. Determine if action is needed based on the event type and description (e.g., customer communication required, technician assignment, status update, etc.).

### Step 6: Mark Event as Reviewed

Return to the Events Q grid (or use Extended Menu from the call) and locate the event. Click Extended Menu (three vertical dots) on the event row. Select Mark as Reviewed or Clear Event. The system removes the event from the unreviewed list and archives it.

## What Happens Next

Reviewed events remain in the call's Events tab for audit purposes but are removed from the Events Q active list. You can continue monitoring remaining events in the queue. Events that require follow-up actions (e.g., customer contact, technician assignment) are documented in the call and may generate follow-on tasks or reminders.

## Common Issues

**Event Shows Incorrect Call Reference**
If an event displays the wrong call number or customer name, verify the event details on the call's Events tab. If the event is truly linked to the wrong call, contact your system administrator as event linking errors may indicate a data issue.

**Cannot Mark Event as Reviewed**
Verify you have permission to manage events in the Events Q. If you lack permission, contact your service manager or system administrator. Alternative approach: navigate to the related call and delete or update the event from the Events tab.

**Events Q Shows No Events**
If the Events Q is empty, all events have been reviewed and archived. This is normal operation. To view historical events, navigate directly to individual service calls and review their Events tabs. Create new events manually using SVC-CALL-009 if needed.
