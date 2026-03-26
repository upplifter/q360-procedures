---
title: Post Opportunity Time Bills
id: SALES-PRESALES-004
module: Sales
screen: Post Time Bills Records
menu_path: Main Menu > Projects > Post Time Bills Records
applies_to:
  - Engineering Manager
  - Department Manager
prerequisites:
  - POST TIME BILLS permission assigned to your user or group
  - Unposted presales time bills exist against opportunities (see SALES-PRESALES-003)
related_procedures:
  - SALES-PRESALES-003
  - SALES-RPT-009
tags: post time bills, post presales, time bill posting, opportunity time bills, presales cost, engineering time bills
version: 1.0
last_updated: 2026-03-25
---

# Post Opportunity Time Bills

## What This Procedure Does

Posts unposted presales time bills from the Post Time Bills Records form. Posting finalizes the time records, creates the associated journal entries for labor cost, and makes the hours permanent. Posted time bills feed into cost reporting and the Sales Opportunity Labor Conversion report.

## Before You Begin

- You have POST TIME BILLS permission.
- Unposted presales time bills exist (see SALES-PRESALES-003).
- You have reviewed the time bills for accuracy before posting.

## Steps

### Step 1: Open the Post Time Bills Form

Navigate to **Main Menu > Projects > Post Time Bills Records**. The form opens showing unposted time bill records based on the current filter settings.

### Step 2: Set Filters

In the **Filters** panel on the left side, set the following options as needed.

| Field | What to enter |
|---|---|
| Department | Select the department associated with the presales engineers. |
| Date Range | Adjust the start and end date to cover the period you want to review. |
| Other Filters | Set any additional filters such as branch or employee name to narrow results. |

Click **Run** or allow the filter to refresh the grid.

### Step 3: Review the Time Bills

The grid displays unposted time bill records summarized by person, by day, for each day within the chosen time period. A summary row appears per person. Review the following columns for accuracy:

- Duration and total time (Time Billed)
- Category and subcategory
- Wage type
- Linked opportunity

### Step 4: Select and Post

Select the time bill record(s) to post by clicking on them in the grid. You can select summary rows without issue. Click the **Post Selected** button.

## What Happens Next

Q360 posts the selected time bills and creates the corresponding labor cost journal entries. The posted hours and costs are now permanent and appear in:

- The opportunity's cost tracking.
- The **Sales Opportunity Labor Conversion** report, which compares presales labor against project labor (see SALES-RPT-009).
- General ledger entries for the labor expense accounts.

Posted time bills cannot be unposted. If an error is found after posting, a correcting journal entry or adjustment may be required.

## Common Issues

**No time bills appear in the grid.**
Adjust the filters - the date range, department, or branch may be excluding the records you expect to see. Also confirm unposted time bills exist for the selected period.

**The Post Selected button is grayed out.**
You must select at least one time bill row before the Post button becomes active. Click on the row(s) to select them.

**A time bill shows incorrect hours.**
Do not post inaccurate records. Have the employee who logged the time edit and correct the time bill before posting (see SALES-PRESALES-003).

**Posted time bills do not appear in the Labor Conversion report.**
The Sales Opportunity Labor Conversion report filters by date range, branch, and sales rep. Verify the report filters include the period and branch where the time was posted. Also check the Cost Type filter (Posted vs. Standard).

**You accidentally posted a time bill that should not have been posted.**
Posted time bills cannot be reversed through this form. Contact your administrator or accounting team to create a correcting journal entry.
