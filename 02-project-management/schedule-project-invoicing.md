---
title: Schedule or Update Project Invoicing
id: PROJ-INV-001
module: Projects
screen: Project Form > Tasks Tab
menu_path: Main Menu > Projects > Projects
applies_to: Project Manager, Accounts Receivable
prerequisites: PROJECT (Edit) permission, Project exists with approved order
related_procedures:
  - PROJ-TASK-001a
  - PROJ-TASK-001b
  - PROJ-SOV-001
  - PROJ-CLOSE-003
tags:
  - invoicing
  - project invoicing
  - invoice task
  - fixed invoice
  - percent invoice
  - billing schedule
  - project billing
  - AR
  - accounts receivable
version: 1.0
last_updated: 2026-03-25
---

# Schedule or Update Project Invoicing

## What This Procedure Does

This procedure adds or adjusts invoicing tasks with invoice type (Fixed, Percent, Retention), dates, and amounts on the Tasks tab. Invoicing tasks define the billing schedule and amounts that will be issued to the customer throughout the project lifecycle.

## Before You Begin

Ensure you have PROJECT (Edit) permission. The project must exist and have an approved order. You will be working on the Tasks tab to configure invoicing billing schedules and amounts.

## Steps to Add Invoicing Tasks Manually

### Step 1: Open the Project

Navigate to Main Menu > Projects > Projects. Search for and open the desired project.

### Step 2: Navigate to Tasks Tab

Click the Tasks tab on the project form. The grid displays existing project tasks.

### Step 3: Add an Invoicing Task

Click the Tasks grid Add button (plus icon). A new task row appears ready for data entry.

### Step 4: Enter Task Identification

Fill in the following task information:

| Field | What to enter |
|-------|---------------|
| WBS Code | A hierarchical code such as 2 or 2.1 identifying this invoicing task in the work breakdown structure |
| Title | A descriptive name such as "Progress Billing 1" or "Final Invoice" |
| Estimated Date | The date on which this invoice is expected to be issued to the customer |
| Time Bill Category | The invoicing category if applicable to your project type |

### Step 5: Leave Assignee Blank

Do not assign a team member to an invoicing task. Leave the Assignee field empty as invoicing tasks represent billing milestones, not work assignments.

### Step 6: Set Status to DATAENTRY

Confirm the task status is set to DATAENTRY. Keep invoicing tasks in DATAENTRY status until you are ready to release them for Accounts Receivable processing.

### Step 7: Select Task Control Type

Click the Task Control dropdown and select INVOICE. This designates the task as an invoicing milestone rather than a labor task.

### Step 8: Choose Invoice Type

Click the Invoice Type dropdown and select either FIXED or PERCENT:
- FIXED: Use this for a specific dollar amount invoice
- PERCENT: Use this for a percentage-of-contract invoice

### Step 9: Enter Invoice Amount or Percentage

If you selected FIXED invoice type, enter the estimated invoice amount in the Amount field. If you selected PERCENT, enter the percentage of the total contract value (use cumulative percentages, e.g., 10%, 50%, 100%).

### Step 10: Save Invoicing Tasks

Click Save (floppy disk icon) on the project form. All invoicing tasks are saved to the project.

## Steps to Adjust Existing Invoicing Tasks

### Step 1: Display All Tasks

Navigate to the Tasks tab on the project. Check the Show All checkbox on the Tasks grid to display DATAENTRY status invoicing tasks, which may otherwise be hidden.

### Step 2: Drill into Invoicing Task

Click on the invoicing task you wish to adjust. The task form opens showing current invoice settings.

### Step 3: Edit Invoice Details

Click Edit (pencil icon) if not already in edit mode. Adjust the following as needed:

| Field | What to enter |
|-------|---------------|
| Estimated Date | Update the invoicing date if the customer's billing timeline has changed |
| Amount | For FIXED invoices, update the dollar amount if the billing terms have been revised |
| Percentage | For PERCENT invoices, update the percentage if the billing formula has changed |

### Step 4: Monitor Status Field

The invoicing task status controls visibility to Accounts Receivable. Keep status as DATAENTRY while still planning. Only change status to OPEN when the invoice is ready for AR to see and process for actual issuance to the customer.

### Step 5: Save Changes

Click Save (floppy disk icon). The updated invoicing task is saved.

## What Happens Next

Your invoicing schedule is now configured on the project. When you change the status of invoicing tasks to OPEN, Accounts Receivable will be able to view and process these invoices for issuance to the customer. Monitor actual project progress against your invoicing milestones throughout the project lifecycle.

## Common Issues

**Invoicing Tasks Do Not Appear in Tasks Tab Grid**
Check the Show All checkbox on the Tasks tab to display DATAENTRY invoicing tasks. By default, some systems may hide DATAENTRY tasks until status is changed to OPEN.

**Cannot Change Invoice Type After Task Creation**
In some systems, invoice type is locked once a task is created. If you need to change from FIXED to PERCENT or vice versa, delete the current invoicing task and create a new one with the correct invoice type.

**Percent Invoices Do Not Sum to 100 Percent**
Ensure your cumulative percentages total 100% across all PERCENT invoicing tasks. For example, use 20%, 50%, 100% (not 20%, 50%, 80%). The final invoice should represent 100% of the contract value.

**Invoicing Task Shows Status DATAENTRY But AR Cannot See It**
Accounts Receivable staff can only see invoicing tasks with status OPEN. Change the task status to OPEN only when you are ready for AR to process the invoice. Verify AR sees the task after status change.

**Cannot Save Invoicing Task Without Assignee**
Leave the Assignee field completely blank for invoicing tasks. If the system requires an assignee, contact your administrator as your system may have different invoicing task configuration rules than documented here.
