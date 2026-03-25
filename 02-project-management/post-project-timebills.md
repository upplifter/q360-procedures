---
title: Post Project Time Bills
id: PROJ-TB-002
module: Projects
screen: Post Timebill Records Form
menu_path: Main Menu > Projects > Post Timebill Records
applies_to: Project Manager
prerequisites: TIMEBILL (Execute) permission, Unposted time bills exist for the project
related_procedures:
  - PROJ-TB-001
  - PROJ-PROFIT-001
tags:
  - post time bills
  - timebill
  - posting
  - labor cost
  - project costing
  - unposted time bills
version: "1.0"
last_updated: 2026-03-25
---

# Post Project Time Bills

## What This Procedure Does

This procedure posts unposted time bill records to the project, finalizing labor costs and making them part of the official project costing. Posting time bills locks them from further editing and integrates them into project financials.

## Before You Begin

- Verify you have TIMEBILL (Execute) permission
- Confirm unposted time bills exist for the project you want to post
- Ensure all time bill entries are accurate before posting, as posting locks them from editing

## Steps

### Step 1: Navigate to Post Timebill Records Form

Go to Main Menu > Projects > Post Timebill Records. The form displays unposted time bill records based on your chosen filters.

### Step 2: Understand the Display Format

Review the displayed records to understand their organization:

- Displayed records are summarized by person and by day
- Each day within the chosen time period shows individual entries
- A time period summary row appears per person

### Step 3: Apply Filters

Set desired filters in the Filters panel:

| Field | What to enter |
|-------|---------------|
| Project Manager | Name of the project manager whose related time bills you want to post |
| Date Range | Start and end dates for the time bills to include |
| Project | Specific project, if filtering by project |

### Step 4: Review Time Bill Records

Examine the displayed time bill records for accuracy:

| Field | What to enter |
|-------|---------------|
| Duration | Hours worked per entry |
| Time Billed | Total time for the summary row |
| Category | Type of work or labor category |
| Wage Type | Classification of labor (hourly, salary, etc.) |

### Step 5: Select Records to Post

Select one or more time bill records to post. Tip: Colored summary rows can be safely selected without issue.

### Step 6: Post Selected Records

Click the Post Selected button. Q360 posts the selected time bills to the project, locking them from further editing and integrating them into project costs.

## What Happens Next

Once posted, the time bills appear in project financials and contribute to labor cost totals. Posted time bills cannot be edited directly; to correct a posted time bill, you must create an adjustment or reversal entry. The unposted time bill list is updated to reflect the newly posted records.

## Common Issues

**Time bills don't appear in the list**
Verify that unposted time bills actually exist for the selected project and date range. Check the filters to ensure they match the time bills you're looking for. If filtering by project manager, confirm the project manager name is spelled correctly and matches your system.

**Colored summary rows appear alongside individual entries**
These colored summary rows are totals for each person and time period. You can safely select them along with individual entries without creating duplicate postings. Selecting summary rows in addition to detail rows is supported.

**Cannot find a specific employee's time bills**
Confirm the employee name in the filter matches the exact name in the system. Check that the date range includes the dates when the time was logged. Verify the employee had TIMEBILL (Create) permission during the period when entries were made.

**Post Selected button is inactive or grayed out**
Ensure at least one time bill record is selected. Verify you have TIMEBILL (Execute) permission. If permissions are correct, refresh the form using the Refresh button (circular arrow icon).

**Posted time bills still appear in the unposted list**
Refresh the form to reload the current data. The unposted list is cached and may not update immediately. Click the Refresh button (circular arrow icon) to see the most current state.
