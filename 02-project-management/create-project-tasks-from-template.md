---
title: Create Project Tasks from Template
id: PROJ-TASK-001a
module: Projects
screen: Project Form > Tasks Tab
menu_path: Main Menu > Projects > Projects
applies_to: Project Manager
prerequisites: PROJECT (Edit) permission, Project exists in DATAENTRY or ACTIVE status, Project template exists (see PROJ-TEMPLATE-001)
related_procedures:
  - PROJ-TASK-001b
  - PROJ-TASK-001c
  - PROJ-RESOURCE-001
  - PROJ-TEMPLATE-001
tags:
  - project template
  - tasks
  - WBS
  - work breakdown structure
  - insert template
  - task structure
  - project planning
version: 1.0
last_updated: 2026-03-25
---

# Create Project Tasks from Template

## What This Procedure Does

This procedure applies a project template to generate a complete work breakdown structure (WBS) with pre-defined task codes, durations, and dependencies. Templates accelerate project setup by providing standardized task hierarchies and timelines for common project types.

## Before You Begin

Ensure you have PROJECT (Edit) permission. The project must exist in DATAENTRY or ACTIVE status. A project template must already exist in your system (refer to PROJ-TEMPLATE-001 to create one if needed). The project should not currently be in edit mode.

## Steps

### Step 1: Look Up the Project

Navigate to Main Menu > Projects > Projects. Search for and open the desired project.

### Step 2: Verify Edit Mode is Off

Confirm the project is not currently in edit mode. If the project displays an active Edit button, do not click it at this step.

### Step 3: Access the Insert Template Option

Click the Extended Menu (3 vertical dots) at the top of the project form. A menu appears with action options.

### Step 4: Select Insert Project Template

Click Insert Project Template from the menu. A template selection dialog opens displaying all available project templates in your system.

### Step 5: Choose the Template

Locate and select the desired project template from the dialog. The template name and description display to help you select the correct template for your project type.

### Step 6: Confirm Template Selection

Click the Select button. Q360 validates the template and inserts all template tasks into the project's Tasks tab.

### Step 7: Review Inserted Tasks

Navigate to the Tasks tab to review the newly inserted tasks. The system has automatically created:
- WBS codes structured hierarchically
- Task titles and descriptions
- Pre-defined durations for each task
- Predecessor dependencies linking tasks together

### Step 8: Adjust as Needed

Modify task dates, durations, or assignments if your project timeline differs from the template defaults. Refer to PROJ-TASK-001b and PROJ-TASK-001c for detailed task adjustment procedures.

## What Happens Next

Your project now has a complete task structure based on the template. Proceed to assign resources to tasks using PROJ-RESOURCE-001, schedule invoicing using PROJ-INV-001, or adjust the Gantt chart timeline using PROJ-TASK-001c.

## Common Issues

**Template Does Not Appear in Selection Dialog**
Verify the template exists in your system. Contact your administrator if the intended template is not visible. Ensure you have permission to view and use project templates.

**Inserted Tasks Have Incorrect Dates**
Template tasks use baseline dates that may not align with your project start date. Adjust task start and end dates on the Tasks tab after insertion. You can adjust multiple tasks at once using the Tasks grid Extended Menu options.

**Unable to Insert Template into ACTIVE Project**
Most systems restrict template insertion to DATAENTRY status projects to prevent workflow disruption. If you need to modify an ACTIVE project, contact your project manager or administrator for guidance on the appropriate procedure.

**Duplicate Tasks Appear After Template Insertion**
If the project already contained tasks, template insertion may add tasks without removing existing ones. Review the Tasks tab carefully and delete any unintended duplicate tasks by selecting them and using the Trash can icon.

**Dependencies Not Created Between Inserted Tasks**
Verify the template was configured with predecessor relationships. Check task dependency settings in the template itself. If dependencies are missing, manually create them using the Gantt chart view (PROJ-TASK-001c) or by editing individual task predecessor fields.
