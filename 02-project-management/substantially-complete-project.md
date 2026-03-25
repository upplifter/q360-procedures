---
title: Substantially Complete a Project
id: PROJ-CLOSE-002
module: Projects
screen: Project Form
menu_path: Main Menu > Projects > Projects
applies_to:
  - Project Manager
prerequisites:
  - PROJECT (Edit) permission
  - Project is in ACTIVE status
  - Products have been created from shipped materials (see PROJ-PRODUCT-001)
related_procedures:
  - PROJ-CLOSE-001
  - PROJ-CLOSE-003
  - PROJ-PRODUCT-001
tags:
  - substantially complete
  - substantial completion
  - project milestone
  - install finish
  - project status
  - SUBSTCOMPL
version: 1.0
last_updated: 2026-03-25
---

# Substantially Complete a Project

## What This Procedure Does

This procedure marks a project as substantially complete, which establishes a key project milestone and initiates the transition toward final project closing. Substantial completion triggers the recording of the actual Install Finish date and changes the project status to reflect this milestone.

## Before You Begin

- Verify you have PROJECT (Edit) permission assigned to your role
- Ensure the project is in ACTIVE status
- Confirm that products have been created from shipped materials (see PROJ-PRODUCT-001)
- Have the date of substantial completion available (typically the date when work is materially complete and ready for customer use)

## Steps

### Step 1: Look Up the Project
Navigate to the Projects module and locate the project you wish to mark as substantially complete.

### Step 2: Access the Substantial Completion Function
Click the Extended Menu (3 vertical dots) and select Mark as Substantially Complete.

### Step 3: Select the Completion Date
In the dialog that appears, select the date of substantial completion. This is typically the date when the project work is materially complete and the deliverables are ready for customer use.

### Step 4: Confirm the Action
Click Ok to execute the substantial completion action.

### Step 5: Verify Status Change
Q360 updates the project status to SUBSTCOMPL (Substantially Complete) and sets the actual Install Finish date to the date you selected.

## What Happens Next

The project is now marked as substantially complete. This milestone records the essential project completion date for financial and operational purposes. Once substantially complete, you can proceed with final project closing after resolving any remaining close issues (see PROJ-CLOSE-001 and PROJ-CLOSE-003).

## Common Issues

**The Mark as Substantially Complete option does not appear in the Extended Menu.**
Verify that the project is in ACTIVE status. The substantial completion function is available only for projects in an active state. If the project has already been substantially completed or closed, this option will not be available.

**I cannot change the project status back to ACTIVE after marking it substantially complete.**
Once a project is marked as substantially complete, you must use the standard reopen procedure if you need to reverse the status. See PROJ-CLOSE-004 for instructions on reopening a closed or substantially complete project.

**The Install Finish date is not set correctly after substantial completion.**
Verify that the completion date you selected in step 3 is the correct date. The system records the Install Finish date based on the date you specify in the substantial completion dialog. If the date is incorrect, you may need to reopen the project and re-mark it substantially complete with the correct date.

**The project cannot be marked substantially complete because products have not been created.**
This may indicate a configuration requirement in your system. Verify that all shipped materials have been properly converted to product records (see PROJ-PRODUCT-001) before attempting substantial completion. Contact your system administrator if this requirement appears to be preventing substantial completion.

**I need to undo substantial completion before closing the project.**
Use the reopen project procedure to change the project status back to ACTIVE if you need to reverse substantial completion (see PROJ-CLOSE-004). This allows you to make any necessary adjustments before proceeding with final closing.
