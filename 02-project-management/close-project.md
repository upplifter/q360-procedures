---
title: Close a Project
id: PROJ-CLOSE-003
module: Projects
screen: Project Form
menu_path: Main Menu > Projects > Projects
applies_to:
  - Accounts Receivable
  - Finance
prerequisites:
  - PROJECT (Edit) permission
  - All close issues resolved (see PROJ-CLOSE-001)
  - Project is substantially complete (see PROJ-CLOSE-002)
related_procedures:
  - PROJ-CLOSE-001
  - PROJ-CLOSE-002
  - PROJ-CLOSE-004
  - PROJ-PROFIT-001
tags:
  - close project
  - closing entry
  - project completed
  - revenue recognition
  - financial closing
  - project closeout
  - COMPLETED
version: 1.0
last_updated: 2026-03-25
---

# Close a Project

## What This Procedure Does

This procedure finalizes a project by creating a closing entry that completes financial recognition and updates the project status to COMPLETED. Project closing reconciles all project activity, recognizes any remaining revenue, and generates the final closing entry for accounting purposes.

## Before You Begin

- Verify you have PROJECT (Edit) permission assigned to your role
- Confirm all project close issues have been resolved (see PROJ-CLOSE-001)
- Ensure the project is substantially complete (see PROJ-CLOSE-002)
- Have the financial closing date available (typically the project substantial completion date or end of the fiscal period)

## Steps

### Step 1: Look Up the Project
Navigate to the Projects module and locate the project you wish to close.

### Step 2: Access the Create Closing Entry Function
Click the Extended Menu (3 vertical dots) and select Create Closing Entry.

### Step 3: Select the Closing Date
In the dialog that appears, select the date of financial closing. This is typically the project substantial completion date or end of the applicable fiscal period.

### Step 4: Confirm the Action
Click Okay to execute the closing entry creation.

### Step 5: Review the Result
Q360 processes the closing entry. If no closing issues are detected, the system updates the project status to COMPLETED and recognizes any remaining revenue in the accounting records.

### Step 6: Resolve Any Detected Issues
If closing issues are detected during the process, resolve them first by following the procedures in PROJ-CLOSE-001, then retry the closing entry.

## What Happens Next

The project is now closed with all financial transactions recorded and final revenue recognition completed. The project status displays as COMPLETED, and the project is no longer available for routine operational updates. If additional costs or billing corrections are needed, you must reopen the project (see PROJ-CLOSE-004) before making changes.

## Common Issues

**The Create Closing Entry option does not appear in the Extended Menu.**
Verify that the project is in a status eligible for closing. The closing entry function is available only for substantially complete projects. Ensure the project has been marked as substantially complete (see PROJ-CLOSE-002) before attempting to close.

**The closing entry fails with detected issues.**
The system has identified unresolved transactions or pending items that must be addressed before closing. Follow the procedures in PROJ-CLOSE-001 to identify and resolve all detected close issues. Retry the closing entry after all issues have been resolved.

**The project status does not change to COMPLETED after I click Okay.**
Verify that the closing entry process completed successfully. If issues were detected, the status change does not occur until all issues are resolved. Review the system messages to identify any warnings or errors that may indicate incomplete processing.

**I need to make adjustments to the project after closing.**
Once a project is closed, you must reopen it before making any changes. Use the reopen project procedure (see PROJ-CLOSE-004) to change the project status back to ACTIVE. After making necessary adjustments, close the project again.

**The remaining revenue recognition does not appear correct.**
Verify that all SOV progress has been recorded through the current period and that all project transactions have been posted. Remaining revenue is calculated based on the difference between total contract revenue and previously recognized revenue. Review the project profitability tab (see PROJ-PROFIT-001) to confirm revenue calculations before closing.
