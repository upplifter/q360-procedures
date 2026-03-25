---
title: Approve Project Expenses
id: PROJ-EXPENSE-002
module: Projects
screen: Review Project Expenses Form
menu_path: Main Menu > Projects > Review Project Expenses
applies_to: Project Manager
prerequisites: EXPENSE (Execute) permission, Unposted project expenses exist
related_procedures:
  - PROJ-EXPENSE-001
  - PROJ-TB-002
tags:
  - approve expenses
  - reject expenses
  - project expenses
  - expense review
  - per diem approval
  - expense management
version: "1.0"
last_updated: 2026-03-25
---

# Approve Project Expenses

## What This Procedure Does

This procedure allows project managers to review, approve, or reject project-related expenses including per diem requests, travel expenses, and other project costs. Approving expenses authorizes their posting to the project. Rejecting expenses returns them to the submitter for revision or cancellation.

## Before You Begin

- Verify you have EXPENSE (Execute) permission
- Confirm unposted project expenses exist for review
- Gather any supporting documentation or receipts needed to validate expenses

## Steps

### Step 1: Navigate to Review Project Expenses Form

Go to Main Menu > Projects > Review Project Expenses. The form displays unposted expenses related to projects matching your chosen filters.

### Step 2: Apply Filters

Set desired filters in the Filters panel to display relevant expenses:

| Field | What to enter |
|-------|---------------|
| Project Manager | Name of the project manager to review expenses for their projects |
| Date Range | Start and end dates to filter expenses by submission or travel date |
| Expense Category | Specific type of expense (per diem, mileage, materials, etc.) |
| Project | Specific project to filter expenses |
| Status | Unposted or pending approval status |

### Step 3: Review Displayed Expenses

Examine each expense record for completeness and accuracy:

| Field | What to enter |
|-------|---------------|
| Description | Purpose and details of the expense |
| Category | Type of expense (per diem, travel, etc.) |
| Amount | Dollar amount being claimed |
| Employee | Name of the employee who submitted the expense |
| Dates | Travel or work dates covered by the expense |

### Step 4: Review Document Attachments

Click on any document attachments to review supporting receipts, invoices, or justification. Verify that documentation supports the expense claim and complies with company policy.

### Step 5: Select Expenses for Action

Select one or more expenses that you are ready to approve or reject. Use the checkbox next to each expense to select it.

### Step 6: Approve Expenses

To approve selected expenses, click the Extended Menu (3 vertical dots) and select Approve. Q360 changes the expense status to approved and sends an automatic email notification to the expense submitter confirming approval.

### Step 7: Reject Expenses

To reject selected expenses, click the Extended Menu (3 vertical dots) and select Reject. Q360 returns the expense to the submitter with notification requesting revision or cancellation. Include any comments or feedback for the submitter in the rejection dialog.

## What Happens Next

Approved expenses move into the posting workflow and can be finalized to the project. Rejected expenses are returned to the employee for revision or withdrawal. The employee receives automatic email notification of the approval or rejection decision. Once approved, expenses become available for posting to the project through the post expenses workflow.

## Common Issues

**Extended Menu doesn't display Approve or Reject options**
Verify you have EXPENSE (Execute) permission. Confirm at least one expense is selected. Refresh the form using the Refresh button (circular arrow icon) to reload the menu options.

**Cannot find specific expenses in the list**
Check that the filters are set correctly for the project manager and date range you're looking for. Verify that expenses have been submitted and are in unposted status. If filtering by category, confirm the expense is coded to that category.

**Approval or rejection action doesn't complete**
Verify your EXPENSE (Execute) permission is active. Check that the expense record is still in unposted status; it may have been actioned by another approver. Refresh the form to see the current status of all expenses.

**Email notification not sent to submitter**
The automatic email may take a few moments to send after you approve or reject. Verify that the employee has a valid email address in the system. Check your system's email configuration if notifications consistently fail to send.

**Need to reverse an approval or rejection decision**
Depending on system configuration and the expense status, you may be able to change an approval decision through the Extended Menu on a posted expense. Contact your system administrator if the option to modify approval status is not available.
