---
title: Adjust Project Gantt Chart
id: PROJ-TASK-001c
module: Projects
screen: Project Form > Gantt Chart
menu_path: Main Menu > Projects > Projects
applies_to: Project Manager
prerequisites: PROJECT (Edit) permission, Project tasks exist (see PROJ-TASK-001a or PROJ-TASK-001b), Tasks have non-zero duration
related_procedures:
  - PROJ-TASK-001a
  - PROJ-TASK-001b
  - PROJ-RESOURCE-001
tags:
  - Gantt chart
  - project schedule
  - task timeline
  - dependencies
  - reschedule
  - project planning
  - task duration
  - predecessor
version: 1.0
last_updated: 2026-03-25
---

# Adjust Project Gantt Chart

## What This Procedure Does

This procedure modifies task timelines, creates dependencies, and visually reschedules project work via the Gantt chart view. The Gantt chart provides a visual timeline representation that makes it easy to drag tasks, adjust durations, and see how changes cascade through dependent tasks.

## Before You Begin

Ensure you have PROJECT (Edit) permission. The project must have tasks created (refer to PROJ-TASK-001a or PROJ-TASK-001b). All non-invoicing tasks must have non-zero duration. Before opening the Gantt chart, check the Tasks tab and adjust any tasks with 0 duration by modifying their start or end dates.

## Steps

### Step 1: Verify Task Durations

Navigate to Main Menu > Projects > Projects and open the desired project. Click the Tasks tab. Review all non-invoicing tasks and confirm each has a duration greater than zero days. If any task shows 0 duration, click Edit (pencil icon), adjust the task's start or end dates to create a valid duration, and click Save (floppy disk icon).

### Step 2: Look Up the Project

Open the project from Main Menu > Projects > Projects. Confirm the project is not currently in edit mode on the main form.

### Step 3: Open the Gantt Chart

Click the Extended Menu (3 vertical dots) at the top of the project form. A menu appears with action options.

### Step 4: Select Open Gantt Chart

Click Open Gantt Chart from the menu. The Gantt chart opens in a new view, displaying all project tasks as horizontal bars along a timeline.

### Step 5: Enter Edit Mode

Click the chart Edit button. The chart interface activates for modifications, enabling task dragging and dependency creation.

### Step 6: Adjust Task Duration

To change how long a task takes, position your cursor at the left or right border of a task bar. The cursor changes to a resize indicator. Click and drag the border horizontally to extend or shorten the task duration. Dependent tasks automatically cascade forward or backward if their predecessors change.

### Step 7: Adjust Task Timing

To move a task to a different start and end date without changing its duration, click on the body of the task bar (not the borders) and drag it horizontally along the timeline. The entire task bar moves maintaining its width. Dependent tasks shift accordingly.

### Step 8: Create Task Dependencies

To establish that one task must complete before another begins, locate the rightmost circle on a task bar (the predecessor task). Click and drag this circle to the leftmost circle of another task bar (the successor task). A line connects the two tasks indicating the dependency. The successor task cannot start before the predecessor task completes.

### Step 9: Review Cascading Changes

As you make adjustments, watch dependent tasks automatically shift to honor their predecessor relationships. This cascade ensures your project plan remains logically consistent.

### Step 10: Save Changes

Click Save (floppy disk icon). The system saves all Gantt chart modifications and updates the project's task dates and dependencies.

### Step 11: Close the Gantt Chart

Close the Gantt chart view to return to the main project form. Changes are reflected on the Tasks tab.

## Alternative: Adjust Multiple Tasks at Once

You can also adjust timing or duration for multiple selected tasks using the Tasks grid Extended Menu. Return to the project Tasks tab, select one or more tasks, click the Extended Menu (3 vertical dots), and choose options to adjust duration or dates in bulk. This approach is useful when multiple tasks need uniform timing adjustments.

## What Happens Next

Your project timeline is now visually refined with proper task sequencing and dependencies. The schedule reflects realistic task durations and relationships. Proceed to assign resources to tasks using PROJ-RESOURCE-001 to allocate team members to the work.

## Common Issues

**Cannot Open Gantt Chart or Chart Displays Empty**
Verify the project has tasks created with non-zero durations. If the Tasks tab is empty or all tasks have 0 duration, the Gantt chart cannot display. Create or adjust tasks on the Tasks tab first using PROJ-TASK-001a or PROJ-TASK-001b.

**Dragging Tasks Does Not Work or Feels Unresponsive**
Ensure you have clicked the Edit button on the Gantt chart. The chart must be in edit mode for drag operations to function. If edit mode is active and dragging still does not work, try refreshing the Gantt chart view or navigating away and reopening it.

**Dependencies Not Creating Between Tasks**
When dragging from one task to another to create a dependency, ensure you are dragging from the rightmost circle of the predecessor task to the leftmost circle of the successor task. Both circles must be clearly visible and you must complete the drag operation by releasing on the target circle. Partial drags that do not land on the target circle do not create dependencies.

**Gantt Chart Changes Not Saving**
Click Save (floppy disk icon) explicitly before closing the chart. If the save fails, check that all tasks still have valid non-zero durations. If a task duration became zero during your adjustments, correct it and retry saving.

**Project Plan Becomes Invalid After Dependency Adjustments**
If you create circular dependencies (where task A depends on B, B depends on C, and C depends on A), the system may behave unexpectedly. Review your dependencies carefully to ensure they flow logically from start to finish without cycles. Delete problematic dependencies and recreate them in the correct direction.
