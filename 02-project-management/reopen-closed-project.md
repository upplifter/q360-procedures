---
title: Reopen a Closed Project
id: PROJ-CLOSE-004
module: Projects
screen: Project Form
menu_path: Main Menu > Projects > Projects
applies_to:
  - Accounts Receivable
  - Finance
  - Operations Manager
prerequisites:
  - PROJREOPEN permission
  - Project is in COMPLETED (POST) status
related_procedures:
  - PROJ-CLOSE-003
  - PROJ-CLOSE-001
  - PROJ-TB-002
tags:
  - reopen project
  - closed project
  - reverse close
  - POST to PRE
  - late costs
  - final billing
  - project reopen
version: 1.0
last_updated: 2026-03-25
---

# Reopen a Closed Project

## What This Procedure Does

This procedure allows you to reopen a closed project to process late costs, additional time bills, billing corrections, or other adjustments that were not completed before the original closing. Reopening a project reverses the COMPLETED status and returns the project to an ACTIVE state for additional processing.

## Before You Begin

- Verify you have PROJREOPEN permission assigned to your role
- Ensure the project is in COMPLETED (POST) status
- Have information ready about the late costs or adjustments that need to be processed
- Plan to follow the standard close procedure again after making adjustments (see PROJ-CLOSE-003)

## Steps

### Step 1: Look Up the Closed Project
Navigate to the Projects module and locate the closed project. The project status displays as COMPLETED or POST.

### Step 2: Enter Edit Mode
Click Edit (pencil icon) to enable editing of the project form.

### Step 3: Change the Project Status
Locate the project status field and change it from POST back to PRE (ACTIVE). This reverses the closed status and allows the project to accept additional transactions.

### Step 4: Save Your Changes
Click Save (floppy disk icon) to record the status change and reopen the project.

### Step 5: Process Additional Work
The project is now reopened and available for additional processing. Process any late costs, additional time bills, or billing corrections as needed using the appropriate procedures in your system.

### Step 6: Close the Project Again
When you have finished processing all additional work, follow the standard project close procedure (see PROJ-CLOSE-003) to create a final closing entry with the updated activity.

## What Happens Next

The project remains in ACTIVE status and is available for continued operational updates. All new transactions are recorded against the reopened project. Once all additional work has been completed, close the project again following the standard procedures to ensure final financial reconciliation and revenue recognition.

## Common Issues

**The PROJREOPEN permission is not assigned to my user role.**
Contact your system administrator to request PROJREOPEN permission. This permission must be explicitly assigned to allow project reopening. Without this permission, you cannot change the project status from COMPLETED back to ACTIVE.

**The project status field does not appear on the form.**
Verify that you are in Edit mode by clicking the Edit (pencil icon). The status field may not be visible in view mode. If the status field remains unavailable after entering Edit mode, contact your system administrator to verify field visibility settings.

**I cannot change the status from POST to PRE.**
Verify that you have PROJREOPEN permission assigned to your role. Additionally, ensure you are in Edit mode before attempting to change the status. If you have the required permission and are in Edit mode but still cannot change the status, contact your system administrator.

**Changes made after reopening the project are not saved.**
Ensure you click Save (floppy disk icon) after changing the project status. The status change must be explicitly saved before the project reopens. If the save appears to fail, check for any validation errors and retry the save operation.

**I need to reverse a closing entry that was created in error.**
If a closing entry was created in error, reopen the project using this procedure and then review the accounting entries. Consult with your Finance or Accounting team to determine if the closing entry needs to be reversed in the general ledger. The project reopening restores operational status but may require separate accounting adjustments.
