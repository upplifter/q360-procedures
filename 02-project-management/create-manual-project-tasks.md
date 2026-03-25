---
title: Create Manual Project Tasks
id: PROJ-TASK-001b
module: Projects
screen: Project Form > Tasks Tab
menu_path: Main Menu > Projects > Projects
applies_to: Project Manager
prerequisites: PROJECT (Edit) permission, Project exists
related_procedures:
  - PROJ-TASK-001a
  - PROJ-TASK-001c
  - PROJ-RESOURCE-001
  - PROJ-INV-001
tags:
  - manual tasks
  - add task
  - WBS
  - project task
  - task creation
  - work breakdown structure
  - project planning
  - task dependencies
version: 1.0
last_updated: 2026-03-25
---

# Create Manual Project Tasks

## What This Procedure Does

This procedure adds individual tasks to a project, setting WBS codes, durations, dates, and predecessor dependencies on the Tasks tab. Manual task creation gives you complete control over task structure, timing, and relationships.

## Before You Begin

Ensure you have PROJECT (Edit) permission and the project exists. You can add tasks to projects in any status, though DATAENTRY status is typical for new projects during planning.

## Steps

### Step 1: Open the Project

Navigate to Main Menu > Projects > Projects. Search for and open the desired project.

### Step 2: Navigate to Tasks Tab

Click the Tasks tab on the project form. The tab displays the current task grid (initially empty if this is a new project).

### Step 3: Enter Edit Mode

Click Edit (pencil icon) on the project form. Edit mode activates, enabling task grid modifications.

### Step 4: Select an Insert Position

Select a row in the Tasks grid under which the new task will be inserted. If adding a top-level task, select the last task in the grid or leave no selection for end insertion.

### Step 5: Add a New Task

Click the Tasks grid Add button (plus icon). A new task row appears in the grid ready for data entry.

### Step 6: Fill Task Information

Enter the following task information:

| Field | What to enter |
|-------|---------------|
| WBS Code | A hierarchical code such as 1, 1.1, 1.1.1 identifying the task position in the work breakdown structure |
| Title | A clear, descriptive name for the task |
| Time Bill Category | The labor category that will bill time to this task (e.g., Engineering, Installation, Management) |
| Sub-category | A refinement of the time bill category if applicable |

### Step 7: Set Task Dates

Enter the start date and end date for the task. The system calculates duration from these dates. Dates establish the project timeline and drive resource scheduling.

### Step 8: Set Duration

Enter or confirm the task duration in days. Duration represents the elapsed time from start to end date. The system auto-calculates this from dates but you may override it.

### Step 9: Add Additional Tasks

Repeat Steps 4 through 8 for each task in your work breakdown structure. Add as many tasks as needed to fully decompose your project scope.

### Step 10: Save All Tasks

When all tasks are entered, click Save (floppy disk icon) on the project form. All tasks are saved to the project simultaneously.

## Reorder or Group Tasks

### Step 1: Enter Edit Mode

Click Edit (pencil icon) on the project form if not already in edit mode.

### Step 2: Activate Reorder/Grouping Mode

Click the grouping (folder) button in the Tasks grid toolbar. Reorder/grouping mode activates, highlighting tasks with drag handles.

### Step 3: Reorder Tasks

Highlight and drag one or more tasks up or down in the grid. As you drag, a bold line shows the drop position. Release to reorder tasks at that location.

### Step 4: Group Tasks (Create Hierarchy)

To create a hierarchical parent-child relationship, highlight and drag a task on top of another task. The dragged task becomes a child of the target task, indenting one level.

### Step 5: Exit Reorder/Grouping Mode

Click the grouping (folder) button again to exit reorder/grouping mode and apply all changes.

## Set Target Effort Hours

### Step 1: Enter Edit Mode

Click Edit (pencil icon) on the project form if not already in edit mode.

### Step 2: Update Target Column

On the Tasks tab grid, locate the Target column. Enter the estimated number of hours needed to complete each task. Target represents the project manager's labor hour estimate for scope execution.

### Step 3: Save Changes

Click Save (floppy disk icon) on the project form. Target effort hours are saved for each task.

## What Happens Next

Your tasks are now created and structured. Proceed to assign resources to tasks using PROJ-RESOURCE-001, adjust the Gantt chart timeline using PROJ-TASK-001c, or schedule project invoicing using PROJ-INV-001.

## Common Issues

**Tasks Not Saving After Click of Save Button**
Verify all required fields are filled in each task row. Check that WBS codes are unique and properly formatted. If errors exist, the system prevents save and displays a validation message. Correct errors and try saving again.

**Duration Appears Zero After Entering Start and End Dates**
Ensure the start date is before or equal to the end date. If end date is before start date, the system may not calculate a valid duration. Correct the date range and re-enter duration if needed.

**Cannot Add Tasks to CLOSED Project**
Projects in CLOSED status are typically locked from modifications. Contact your project manager or administrator if task additions are needed on a closed project. Reopening the project may be required.

**Inserted Tasks Not Appearing in Correct Hierarchical Position**
WBS codes control task hierarchy. Verify codes follow proper numbering (1, 1.1, 1.1.1). If codes are not sequential or properly formatted, reorder using the grouping (folder) mode to establish correct relationships.

**Target Hours Not Calculating Correctly in Resource Assignments**
Target effort is a PM estimate independent of actual resource assignments. Check that you are entering target hours in the Target column during task creation. Assigned hours (actual resource allocations) are set separately when assigning resources via PROJ-RESOURCE-001.
