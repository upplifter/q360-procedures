---
title: Create a Project Event
id: PROJ-EVENT-001
module: Projects
screen: Project Form > Events Tab / Task Form > Events Tab
menu_path: Main Menu > Projects > Projects
applies_to: Project Manager, Project Team Member
prerequisites: PROJECT (Edit) permission
related_procedures:
  - PROJ-EVENT-002
tags:
  - project event
  - create event
  - events tab
  - task event
  - project communication
  - event log
  - project notes
version: "1.0"
last_updated: 2026-03-25
---

# Create a Project Event

## What This Procedure Does

This procedure creates an event record at the project level or task level to document project activities, milestones, communications, issues, or notes. Events provide an audit trail and communication log for the project.

## Before You Begin

- Verify you have PROJECT (Edit) permission
- Identify whether the event applies to the entire project or a specific task
- Gather event details including title, description, and relevant dates

## Steps for Project-Level Event

### Step 1: Look Up the Project

Navigate to the project using Main Menu > Projects > Projects. Search for and open the project record where you want to add an event.

### Step 2: Navigate to Events Tab

Click the Events tab on the project form to display the Events grid.

### Step 3: Add a New Event

Click the Add button (plus icon) on the Events grid to create a new event record.

### Step 4: Fill in the Event Form

Complete the following fields in the event form:

| Field | What to enter |
|-------|---------------|
| Title | Event heading (e.g., "Client Approved Scope Change") |
| Description | Detailed explanation of the event and its significance |
| Event Date | Date when the event occurred |
| Event Type | Category of event (milestone, issue, communication, change, etc.) |
| Notes | Additional context or follow-up actions |

### Step 5: Save the Event

Click Save (floppy disk icon) to create the event record. The event is added to the Events grid and becomes part of the project history.

## Steps for Task-Level Event

### Step 1: Look Up and Drill Into the Task

Access the task from My Tasks or from the project's Tasks tab. Open the task record to display task details.

### Step 2: Navigate to Events Tab

Click the Events tab on the task form to display the Events grid for that task.

### Step 3: Add a New Event

Click the Add button (plus icon) on the Events grid to create a new event record.

### Step 4: Fill in the Event Form

Complete the following fields in the event form:

| Field | What to enter |
|-------|---------------|
| Title | Event heading (e.g., "Task Delayed Due to Weather") |
| Description | Detailed explanation of the event and its impact on the task |
| Event Date | Date when the event occurred |
| Event Type | Category of event (milestone, issue, communication, delay, etc.) |
| Notes | Additional context or remediation steps |

### Step 5: Save the Event

Click Save (floppy disk icon) to create the task event record. The event is added to the task's Events grid and can be reviewed in the project's overall event log.

## What Happens Next

The event is recorded in the system and becomes part of the project or task history. Events are visible to all project team members with access to the project or task. Events can be marked as reviewed using the Projects Overview workflow. Events help track project status, communication, and decision-making throughout the project lifecycle.

## Common Issues

**Events Tab is not visible on the project or task form**
Verify you have PROJECT (Edit) permission. The Events tab may be hidden if disabled in system configuration. Contact your system administrator to confirm that the Events feature is enabled.

**Add button (plus icon) is inactive or doesn't respond**
Ensure you have PROJECT (Edit) permission and are viewing an existing project or task record. You cannot add events to an unsaved draft. Verify the project or task has been saved to the system.

**Event form displays validation errors when saving**
Confirm that all required fields are completed. The Title field is typically required. Check that any date fields are in the correct format. Verify that any dropdown selections have valid values.

**Need to edit an event that's already been created**
Open the event record from the Events grid. If you have edit permission, click Edit (pencil icon) to modify the event. Save changes using the Save button (floppy disk icon).

**Event appears in task but not visible in project-level event list**
Task-level events are separate from project-level events. To see all events across the project, use the Projects Overview workflow (see PROJ-EVENT-002) which consolidates events from all tasks and the project level.
