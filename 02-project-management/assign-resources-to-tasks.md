---
title: Assign Resources to Tasks
id: PROJ-RESOURCE-001
module: Projects
screen: Project Form > Tasks Tab, Team Tab, Resource Console
menu_path: Main Menu > Projects > Projects
applies_to: Project Manager
prerequisites: PROJECT (Edit) permission, Project tasks exist (see PROJ-TASK-001a or PROJ-TASK-001b), Team members are set up as Q360 users
related_procedures:
  - PROJ-TASK-001a
  - PROJ-TASK-001b
  - PROJ-TB-001
tags:
  - assign resources
  - team
  - resource console
  - availability
  - effort hours
  - task assignment
  - project team
  - scheduling
  - resource allocation
version: 1.0
last_updated: 2026-03-25
---

# Assign Resources to Tasks

## What This Procedure Does

This procedure adds team members to a project, checks resource availability using the Resource Console, and assigns effort hours to project tasks. Resource assignment allocates specific team members to specific project work with defined hour commitments.

## Before You Begin

Ensure you have PROJECT (Edit) permission. The project must have tasks created (refer to PROJ-TASK-001a or PROJ-TASK-001b). All team members you plan to assign must already be set up as Q360 users in your system.

## Steps to Add Resources to Project Team

### Step 1: Open the Project

Navigate to Main Menu > Projects > Projects. Search for and open the desired project.

### Step 2: Navigate to Team Tab

Click the Team tab on the project form. The tab displays team members currently assigned to the project.

### Step 3: Add Team Members

Click the link (chain) button on the Team tab. A dialog opens for adding team members to the project.

### Step 4: Select Team Members

In the dialog, select one or more team members from the available Q360 users list. You can use search or filtering to locate specific individuals.

### Step 5: Confirm Selection

Click the Select button. The selected team members are added to the project team. They now appear on the Team tab.

## Steps to Check Resource Availability

### Step 1: Access Resource Console

From the project form, click the project Extended Menu (3 vertical dots). A menu appears with action options.

### Step 2: Open Resource Console

Click Resource Console from the menu. The console opens in a new view showing timeline availability for all team members on the project.

### Step 3: Set Resource Filters

On the left side of the console, locate the Filters panel. Set or update Resource Filters to focus on specific team members, date ranges, or availability criteria. Click Run to apply the filters.

### Step 4: Interpret Availability

Review the timeline display:
- Green marks indicate a resource is available and has capacity during that time period
- Other colors indicate varying levels of availability or unavailability

Green availability means the resource can take on additional project work during that period.

### Step 5: Expand Timeline View

Collapse the lower section by clicking on any tab caption at the bottom of the console. This expands the timeline display for a larger, clearer view of resource availability.

### Step 6: Adjust Timeline View

Use timeline action buttons to zoom in/out for more or less detail. You can also change the start date of the displayed timeline to focus on different project periods.

## Steps to Assign a Task to Resources

### Step 1: Return to Project Tasks Tab

Navigate back to the project and click the Tasks tab. The tab displays all project tasks.

### Step 2: Select a Task

Click on the task to which you want to assign resources. The task row highlights indicating selection.

### Step 3: Access Assignment Options

Click the Tasks grid Extended Menu (3 vertical dots). A menu appears with task action options.

### Step 4: Select Assign by Team Member

Click Assign by team member from the menu. An assignment dialog opens for the selected task.

### Step 5: Enter Effort Hours

For each resource you plan to assign to the task, enter the estimated effort in hours (Est Effort field). This represents how many hours that person will spend on this task.

### Step 6: Check Sync Flag

Note the Sync flag is on by default. This setting keeps the assignment duration matched to the main task duration. If you need to override the duration synchronization, uncheck the Sync flag.

### Step 7: Filter and Select Resources

Click in the resource selection area. You can right-click to access filtering options. Select "Filter Exclude resources with zero effort" to hide resources where you did not enter effort hours, leaving only the resources you want to assign visible.

Select the filtered resources from the list. Only resources with effort hours greater than zero remain in the list.

### Step 8: Confirm Assignment

Click the Select button. Q360 assigns the selected resources to the task. The assigned resource names now appear in the Assigned column of the Tasks grid.

## Steps to Set Scheduled Effort

### Step 1: Ensure Edit Mode

Navigate to the project Tasks tab. Confirm the project is in Edit mode by clicking Edit (pencil icon) if needed.

### Step 2: Select Parent Task

Select a parent task of one or more tasks that have assigned resources. Parent tasks show the aggregated effort of their child tasks.

### Step 3: Update Scheduled Effort

In the Scheduled Effort column, enter or update the value representing total hours allocated for the parent task. Scheduled hours fund the resource assignments underneath this task. Click on the Scheduled Effort cell and type the new value.

### Step 4: Save Changes

Click Save (floppy disk icon) on the project form. The scheduled effort is saved for forecasting and resource planning purposes.

### Step 5: Monitor Effort Relationships

Ideally, maintain the relationship: **Assigned hours ≤ Scheduled hours ≤ Target hours**

This ensures you do not over-allocate resources and that you have budget capacity for the project work.

## Key Column Definitions for Tasks Grid

Understand these effort-related columns when managing resource assignments:

| Column | Definition |
|--------|-----------|
| Target | Project manager's estimated hours needed to complete the task (set during task creation) |
| Scheduled Effort | Hours carved from Target to fund resource assignments; your capacity for work on this task |
| Assigned Effort | Hours carved from Scheduled for specific resources in a period; what you have committed resources to work |
| Remaining Scheduled Effort | Calculated as Scheduled - Assigned; available capacity before exceeding Scheduled |
| Actual Effort | Total hours booked via time bills; actual work completed (tracked from PROJ-TB-001) |
| Remaining Assigned Effort | Calculated as Assigned - Actual; hours yet to be worked against current assignments |

## What Happens Next

Your project team is now established with clear task assignments and effort commitments. Team members can begin logging time against their assigned tasks using PROJ-TB-001. Continue to monitor resource availability and adjust assignments as the project progresses.

## Common Issues

**Resource Does Not Appear in Team Member Selection Dialog**
The person must be set up as a Q360 user in your system. Contact your administrator if a needed team member does not appear in the user list. New users must be created in the system before they can be assigned to projects.

**Assigned Effort Exceeds Scheduled Effort**
This indicates an overallocation. You have committed more hours to resources than you have budgeted in Scheduled Effort. Reduce Assigned hours or increase Scheduled Effort to resolve the imbalance.

**Resource Shows Red (Unavailable) in Resource Console**
Red indicates the resource is unavailable or already fully allocated during the displayed time period. Hover over the red indication to see details about what is blocking availability. Consider assigning the task to a different resource or adjusting the task dates to avoid the resource's busy period.

**Sync Flag Causes Assignment Duration to Be Longer Than Task**
If you uncheck the Sync flag, assignment duration can diverge from the main task duration. Ensure the assignment period (start and end dates) falls within the task period. If assignment dates extend beyond task dates, adjust one of them for consistency.

**Assigning by Team Member Dialog Does Not Appear**
Ensure you have selected a task before accessing the Extended Menu. Also verify the project has team members added on the Team tab. You cannot assign a task without team members on the project.
