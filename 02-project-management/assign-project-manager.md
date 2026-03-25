---
title: Assign Project Manager
id: PROJ-PM-001
module: Projects
screen: Project Form
menu_path: Workflow > Projects Overview > Projects with No PM
applies_to: Operations Manager, Project Manager
prerequisites: PROJECT (Edit) permission, Access to Projects Overview workflow
related_procedures:
  - PROJ-TASK-001a
  - PROJ-TASK-001b
  - PROJ-INV-001
tags:
  - assign PM
  - project manager
  - projects with no PM
  - project assignment
  - project leader
  - workflow
version: 1.0
last_updated: 2026-03-25
---

# Assign Project Manager

## What This Procedure Does

This procedure assigns a project manager to a DATAENTRY status project from the Projects Overview workflow. When you assign a PM, the project is removed from the "Projects with No PM" bucket and transitions to active management.

## Before You Begin

Ensure you have PROJECT (Edit) permission and access to the Projects Overview workflow. The project must be in DATAENTRY status and currently appear in the "Projects with No PM" bucket.

## Steps

### Step 1: Open Projects Overview Workflow

Go to Workflow > Projects Overview. The workflow display shows all active project buckets and filters.

### Step 2: Select the Projects with No PM Bucket

Click the "Projects with No PM" bucket. The grid updates to show all DATAENTRY projects without an assigned project manager.

### Step 3: Zoom into the Project

Click on the desired project in the grid. The project record zooms into focus, displaying project details and the edit interface.

### Step 4: Edit the Project

Click Edit (pencil icon). The project form opens in edit mode, enabling field modifications.

### Step 5: Select Project Leader

In the Project Leader field, click the dropdown and select the project manager from the available list. The selection displays the manager's name in the field.

### Step 6: Save the Assignment

Click Save (floppy disk icon). The system saves the project manager assignment and closes edit mode.

## What Happens Next

The project now has an assigned PM and will no longer appear in the "Projects with No PM" bucket. The project manager can now proceed with task planning and resource allocation using procedures PROJ-TASK-001a and PROJ-TASK-001b.

## Common Issues

**Project Still Appears in Projects with No PM Bucket**
If the project continues to appear in the bucket after saving, refresh the workflow view by clicking the Circular arrow (Refresh Form) icon. The bucket updates to reflect the new PM assignment.

**Cannot Find Project Manager in Dropdown**
Ensure the team member is set up as a Q360 user in your system. Only active Q360 users appear in the project manager dropdown. Contact your system administrator if the intended PM is not listed.

**Missing PROJECT Edit Permission**
You must have PROJECT (Edit) permission to assign a project manager. Verify your user role includes this permission. Contact your administrator if you need this permission added to your account.

**Project Not in DATAENTRY Status**
Projects in ACTIVE or CLOSED status may not appear in the "Projects with No PM" bucket. Verify the project status before attempting this procedure. Only projects in DATAENTRY status can be managed through this bucket.
