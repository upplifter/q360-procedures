---
title: Merge a Project
id: PROJ-MERGE-001
module: Projects
screen: Project Form
menu_path: Main Menu > Projects > Projects
applies_to:
  - Operations Manager
  - Project Manager
prerequisites:
  - PROJECT (Edit) permission
  - PROJMERGE permission
  - Both source and target projects exist
related_procedures:
  - PROJ-CLOSE-003
  - PROJ-PM-001
tags:
  - merge project
  - consolidate projects
  - combine projects
  - duplicate project
  - project merge
version: 1.0
last_updated: 2026-03-25
---

# Merge a Project

## What This Procedure Does

This procedure consolidates two projects by merging all records and data from a source project into a target project. Merging projects combines related work, materials, tasks, time bills, and other associated records under a single project, eliminating duplicate project records while preserving all historical data.

## Before You Begin

- Verify you have PROJECT (Edit) and PROJMERGE permissions assigned to your role
- Identify the source project (the project to be merged into another) and the target project (the project that will receive the merged data)
- Confirm both projects exist and are accessible in the system
- Review the records that will be transferred to ensure the merge is appropriate

## Steps

### Step 1: Look Up the Source Project
Navigate to the Projects module and locate the source project (the project that will be merged into another).

### Step 2: Access the Merge Project Function
Click the Extended Menu (3 vertical dots) and select Merge Project.

### Step 3: Select the Target Project
In the merge dialog, search for and select the target project (the project that will receive the merged data from the source project).

### Step 4: Review the Merge Summary
Q360 displays a summary of the merge showing which records will be transferred, including:
- Orders
- Line items
- Tasks
- Time bills
- Events
- Documents

Review this summary carefully to ensure all relevant records are identified for transfer.

### Step 5: Execute the Merge
Click Confirm or Merge to execute the project merge operation.

### Step 6: Verify the Merge Results
Q360 transfers all associated records from the source project to the target project. The source project status is updated to indicate it has been merged. All records are now consolidated under the target project.

## What Happens Next

The source project is now merged into the target project. All project data has been consolidated, and the source project is marked to indicate the merge. The target project now contains all consolidated records and history from both projects. The source project is no longer actively used, and future work should be recorded against the target project.

## Common Issues

**The Merge Project option does not appear in the Extended Menu.**
Verify that you have PROJECT (Edit) and PROJMERGE permissions assigned to your role. Both permissions must be assigned to access the merge function. If permissions are assigned but the option is not visible, refresh your browser to reload the project form.

**I cannot select the target project in the merge dialog.**
Verify that the target project exists and is accessible to your user role. The target project must be a valid existing project that you can view. If you cannot locate the target project in the search results, verify the project name or number and retry the search.

**The merge summary does not show all the records I expect to transfer.**
Verify that the records exist in the source project before attempting the merge. Only records currently associated with the source project are shown in the merge summary. If certain records are missing, they may already be associated with the target project or may not be attached to the source project.

**The merge cannot be completed because of validation errors.**
Certain records or data configurations may prevent the merge from proceeding. Review any validation errors displayed in the merge dialog. Resolve data issues in the source or target project as indicated, and retry the merge operation. Contact your system administrator if validation errors persist.

**I cannot undo a merge after it has been completed.**
Verify the merge details carefully before confirming the operation, as merges cannot be automatically reversed. If a merge was executed in error, contact your system administrator for assistance with data recovery or reversal procedures.
