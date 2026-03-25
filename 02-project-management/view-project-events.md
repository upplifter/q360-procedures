---
title: View Unreviewed Project Events
id: PROJ-EVENT-002
module: Projects
screen: Projects Overview Workflow / My Projects Workflow
menu_path: Workflow > Projects Overview
applies_to: Project Manager
prerequisites: Access to Projects Overview or My Projects workflow
related_procedures:
  - PROJ-EVENT-001
tags:
  - unreviewed events
  - project events
  - event review
  - mark reviewed
  - projects overview
  - workflow
  - event management
version: "1.0"
last_updated: 2026-03-25
---

# View Unreviewed Project Events

## What This Procedure Does

This procedure displays all unreviewed project events in a centralized workflow view, allowing project managers to review events and mark them as reviewed. Events are created at the project or task level and accumulate in the unreviewed queue until explicitly marked as reviewed.

## Before You Begin

- Verify you have access to the Projects Overview or My Projects workflow
- Confirm that project events have been created and require review

## Steps

### Step 1: Open the Projects Overview Workflow

Navigate to Workflow > Projects Overview (or My Projects if you prefer a personalized view). The workflow dashboard displays several buckets including project status, tasks, and events.

### Step 2: Click the Unreviewed Events Bucket

Locate the Unreviewed Events bucket in the workflow. Click on it to display a list of all unreviewed project and task-level events. Q360 shows event title, creation date, project or task name, and event type.

### Step 3: View Event Details

To read the full details of an event, click the drilldown link on the event row. The event details display including the event title, description, dates, and any notes. Review the content to understand what action or acknowledgment is required.

### Step 4: Mark Events as Reviewed

Select one or more events in the grid that you have reviewed and want to mark as reviewed. Use the checkbox next to each event.

### Step 5: Apply the Mark Reviewed Action

Click the Extended Menu (3 vertical dots) and select the option to mark selected events as reviewed. Q360 updates the event status from unreviewed to reviewed and removes them from the Unreviewed Events bucket.

## What Happens Next

Marked events are removed from the unreviewed queue and archived in the event history. The project header tab displays a count of remaining unreviewed events. To view all events on a single project, including reviewed and unreviewed events, access the project's Events tab. Events remain in the system as a permanent record of project activities and decisions.

## Common Issues

**Unreviewed Events bucket is empty but events still exist**
Some events may already be marked as reviewed. To see all events including reviewed ones, navigate directly to the project or task and view the Events tab. Use the filter settings in the Events tab to show both reviewed and unreviewed events.

**Cannot find an event that was just created**
New events may take a moment to appear in the workflow. Refresh the page using the Refresh button (circular arrow icon) to reload the event list. Confirm the event is actually unreviewed; if it was marked reviewed during creation, it won't appear in this bucket.

**Extended Menu doesn't show Mark Reviewed option**
Ensure at least one event is selected. Verify you have edit permissions for the event. Refresh the form to reload the menu options.

**Selected events don't get marked as reviewed after clicking OK**
Verify the system saved the action. Refresh the page to see the updated status. If events remain unreviewed, check that the action completed without errors.

**Need to reopen a reviewed event to make changes**
Navigate to the project or task's Events tab to locate reviewed events. You can edit event details by clicking Edit (pencil icon) on the event record. To mark a reviewed event back to unreviewed status, access the event record and look for an option to change the reviewed status in the Extended Menu.
