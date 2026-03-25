---
title: Create or Edit a Project Template
id: PROJ-TEMPLATE-001
module: Projects
screen: Project Template Form / Project Form
menu_path: Main Menu > Projects > Project Templates
applies_to: Operations Manager, Project Manager, System Administrator
prerequisites:
  - PROJECT (Create/Edit) permission
  - PROJTEMPLATE permission
related_procedures:
  - PROJ-TASK-001a
  - PROJ-TASK-001b
  - PROJ-TASK-001c
tags:
  - project template
  - WBS template
  - task template
  - create template
  - edit template
  - reusable template
  - project planning
  - Gantt template
version: 1.0
last_updated: 2026-03-25
---

# Create or Edit a Project Template

## What This Procedure Does

This procedure shows you how to create a new project template or edit an existing one. Project templates contain reusable task structures, work breakdown schedules, and Gantt charts that you can apply to new projects to standardize planning and accelerate project setup.

## Before You Begin

Ensure you have PROJECT (Create/Edit) and PROJTEMPLATE permissions. You should understand your organization's project structure, standard task categories, and typical project phases. Have your template information prepared before you start, including task names, durations, and dependencies.

## Steps

### Step 1: Navigate to Project Templates

From the Main Menu, click **Projects**. In the Projects menu, click **Project Templates**.

### Step 2: Create a New Template or Open an Existing One

To create a new template, click **Add New Record** (the plus icon) at the top of the template list. To edit an existing template, use the search box to find the template you want to modify, then click its name to open it.

### Step 3: Edit the Template Header

Click the **Edit** button (pencil icon) to enter edit mode. Fill in the template header fields with the following information:

- **Template Name**: Enter a descriptive name for your template (for example, "Standard Software Development Project" or "Client Implementation")
- **Project Type**: Select the project type this template applies to
- **Category**: Choose a category to organize your templates
- **Description**: Enter a brief description explaining when and how this template should be used

### Step 4: Add Tasks to the Template

Click the **Tasks** tab to access the task grid. Click the **Add** button (plus icon) in the Tasks grid to add a new task. For each task, enter the following information:

- **WBS Code**: Enter the work breakdown structure code for the task
- **Task Title**: Enter the name of the task
- **Time Bill Category**: Select the category for time tracking and billing
- **Sub-Category**: Choose the appropriate sub-category
- **Duration**: Enter the number of days or hours for the task
- **Predecessor Dependencies**: If the task depends on another task, specify which task must be completed first

Repeat this process for all tasks you want to include in your template. Tasks will be inserted in the order you add them.

### Step 5: Organize and Group Tasks

To organize your tasks into a work breakdown structure, click the **grouping (folder) button** and drag tasks to nest them under parent tasks or reorder them. Group related tasks together to create a logical project structure. Indented tasks appear as subtasks under their parent task.

### Step 6: Save the Template Header

Click **Save** (floppy disk icon) to save the template header and task list.

### Step 7: Set Up the Gantt Chart (Optional)

To create a visual timeline and set up task durations and dependencies graphically, click the **Extended Menu** (three vertical dots) and select **Open Gantt Chart**. In the Gantt chart view, you can:

- Adjust task durations by dragging the right edge of task bars
- Create dependencies by dragging a line from one task to another
- Adjust start and end dates for your project phases
- Visualize the overall project timeline

After making adjustments in the Gantt chart, click **Save** and close the Gantt view to return to the template form.

### Step 8: Verify and Complete

Review all template information to ensure it is complete and correct. Confirm that all tasks are organized properly and that dependencies are accurately set. Click **Save** to finalize the template.

## What Happens Next

Your project template is now available for use when creating new projects. Project managers can insert this template into new projects to automatically populate the task structure, work breakdown schedule, and Gantt chart (see PROJ-TASK-001a for inserting templates into projects). Templates can be used multiple times and can be edited at any time to reflect process improvements or changes in your project methodology.

## Common Issues

**Cannot add tasks to the template**
Ensure you are in edit mode by clicking the **Edit** button. Templates in view mode do not allow task additions. Click **Edit** and try adding tasks again.

**Tasks are not appearing in the correct order**
Use the grouping button to reorganize tasks. Click and drag tasks to reorder them. If tasks still appear out of order, delete and re-add them in the correct sequence.

**Dependencies between tasks are not saving**
Verify that you are selecting valid predecessor tasks. A task cannot depend on itself, and circular dependencies are not allowed. Check the predecessor field to ensure you have selected a different task that comes before the current task in the sequence.

**Gantt chart will not open or save changes**
Ensure the template has been saved before opening the Gantt chart. If the Gantt chart still will not open, close the template and reopen it. If changes to the Gantt chart are not saving, click **Save** in the Gantt view before closing it.

**Template appears to be incomplete or partially saved**
Refresh the template by closing it and reopening it to see the current saved state. If information is still missing, edit the template again and ensure you click **Save** after making changes. Check that your user session has not timed out.
