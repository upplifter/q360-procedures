---
title: Check Project Close Issues
id: PROJ-CLOSE-001
module: Projects
screen: Project Form
menu_path: Main Menu > Projects > Projects
applies_to:
  - Project Manager
  - Accounts Receivable
prerequisites:
  - PROJECT (View) permission
related_procedures:
  - PROJ-CLOSE-002
  - PROJ-CLOSE-003
  - PROJ-TB-002
tags:
  - project close
  - close issues
  - check close
  - close validation
  - project closeout
  - unresolved issues
version: 1.0
last_updated: 2026-03-25
---

# Check Project Close Issues

## What This Procedure Does

This procedure allows you to validate project readiness for closing by detecting unresolved issues that must be addressed before financial closing. The check identifies pending transactions such as unposted time bills, open purchase orders, unreceived materials, unbilled invoicing tasks, and unposted journal entries.

## Before You Begin

- Verify you have PROJECT (View) permission assigned to your role
- Have the project number or name available for lookup
- Prepare to address any detected issues before closing the project

## Steps

### Step 1: Look Up the Project
Navigate to the Projects module and locate the project you wish to check for close issues.

### Step 2: Access the Check Project Close Function
Click the Extended Menu (3 vertical dots) and select Check Project Close.

### Step 3: Specify the Date
Leave the date blank to indicate "as of today." Alternatively, enter a specific date to check project status as of that date.

### Step 4: Review the List of Detected Issues
Q360 displays a list of any detected issues. Issues may include:
- Unposted time bills
- Open purchase orders
- Unreceived materials
- Unbilled invoicing tasks
- Unposted journal entries

### Step 5: Resolve Detected Issues
Review each listed issue carefully. For each issue identified, take appropriate action to resolve it before proceeding with project closing. You may zoom into any listed issue to navigate directly to the record for resolution.

### Step 6: Reference Additional Information
For more information on the various issues that may be listed, search for "Check Project Close" in Q360 > Help > Contents.

## What Happens Next

Once all detected issues are resolved, you can proceed with the substantial completion and closing procedures. Projects with unresolved close issues cannot be officially closed. Repeat the Check Project Close process after resolving each issue to confirm all items have been addressed.

## Common Issues

**The Check Project Close function does not appear in the Extended Menu.**
Verify that you have PROJECT (View) permission assigned to your user role. If permission is assigned but the function is not visible, refresh your browser to reload the project form. The function should be available for projects in appropriate statuses.

**No issues are detected, but I know there are pending transactions.**
The close check may not detect issues in certain scenarios depending on system configuration. Manually verify that all time entries, purchase orders, material receipts, and invoicing tasks are posted before closing. If issues remain undetected, contact your system administrator to review close validation settings.

**I cannot zoom into or resolve a detected issue.**
Some issues may require specific permissions to resolve. Verify that you have the appropriate permissions to edit time bills, purchase orders, or other affected records. Contact your system administrator or the record owner if you cannot access a detected issue.

**The same issue appears repeatedly in the list.**
If an issue is listed multiple times, resolve all instances of that issue type. For example, if multiple unposted time bills are listed, post each one individually. Re-run the Check Project Close function after posting to confirm all instances have been addressed.

**The Help content for Check Project Close is not accessible.**
Navigate to Q360 > Help > Contents and search for "Check Project Close." If the Help content is unavailable or not installed, contact your system administrator. Additional guidance may be available from your organization's Q360 training resources.
