---
title: Run the Project Status Quick View
id: PROJ-RPT-001
module: Projects
screen: Project Status Quick View
menu_path: Main Menu > Projects > Quick Views > Project Status
applies_to:
  - Project Manager
  - Operations Manager
  - Finance
prerequisites:
  - Access to the Projects module
  - Appropriate user role or permissions
related_procedures:
  - PROJ-PROFIT-001
  - PROJ-RPT-004
tags:
  - project status
  - quick view
  - WIP
  - backlog
  - financial summary
  - project overview
  - project health
version: "1.0"
last_updated: "2026-03-25"
---

# Run the Project Status Quick View

## What This Procedure Does

The Project Status Quick View provides an at-a-glance overview of all active projects, showing key financial and completion metrics. This quick view displays projected and actual revenue, costs, profit margins, work-in-progress (WIP) balances, and project completion percentages in a single grid. Use this view to monitor overall project health and financial performance.

## Before You Begin

- Ensure you have access to the Projects module with appropriate permissions to view financial data
- Know the date range or specific "as of" date you want to report on
- Identify any filters you need to apply (company, branch, project manager, etc.)

## Steps

### Step 1: Navigate to the Project Status Quick View

From the main menu, select **Projects > Quick Views > Project Status**. The quick view screen loads with default filters applied.

### Step 2: Set Your Filters

Configure the filters to focus on the projects you want to review. Use the following table as a guide:

| Field | What to enter |
|-------|---------------|
| Company | Select one or more companies, or leave as ALL for all companies |
| Branch | Select one or more branches, or leave as ALL for all branches |
| Department | Select one or more departments, or leave as ALL for all departments |
| Project Type | Select one or more project types, or leave as ALL for all types |
| Status | Select one or more project statuses, or leave as ALL for all statuses |
| Proj. Mgr | Select one or more project managers, or leave as ALL for all managers |
| Category | Select one or more project categories, or leave as ALL for all categories |
| Sub. Cat | Select one or more subcategories, or leave as ALL for all subcategories |
| As of Date | Enter the date you want the snapshot for; defaults to today |
| Active Only | Check this to show only active projects; leave unchecked to include all |

### Step 3: Click Run

Click the **Run** or **Refresh** button to execute the quick view with your selected filters.

### Step 4: Review the Output Grid

The quick view displays a grid with each project as a row. The columns show:

- **Projected Revenue/Cost/Profit/Margin:** Your expected financial outcomes based on the project budget
- **Actual Invoiced/Paid/Costs:** Real invoices, payments received, and expenses recorded to date
- **Earned Revenue/Costs:** Revenue and costs recognized under your revenue recognition method
- **WIP (Work-in-Progress):** The difference between earned and billed amounts
- **(Over)/Under Billing:** Whether you have overbilled or underbilled compared to work performed
- **% Complete:** Overall project completion percentage
- **% Complete Labor:** Labor-specific completion percentage
- **% Complete Cost:** Cost-based completion percentage
- **Job Cost Method:** The costing methodology applied to the project

A gray summary row at the bottom displays totals for all numeric columns.

### Step 5: Review Project Health

Use the metrics to assess project health. Look for projects with negative gross profit, high over-billing, or unexpectedly low completion percentages. These may indicate projects at risk.

### Step 6: Export or Print (Optional)

If you need to share the quick view data, use the export or print buttons to output the grid to Excel, PDF, or paper format.

## What Happens Next

After reviewing the Project Status Quick View, you may:

- Click on a project name to open the full project detail form and investigate further
- Use the delta report (PROJ-RPT-006) to compare this snapshot to an earlier one
- Generate the full WIP report (PROJ-RPT-004) for deeper financial analysis
- Take action on projects showing red flags, such as initiating a change order or adjusting schedules

## Common Issues

**The quick view shows no data or projects appear missing**

This typically happens when filters are too restrictive. For example, if you filter by a specific project manager and that person has no active projects, the grid appears empty. Try broadening your filters—remove the Project Manager filter or uncheck "Active Only" to include inactive projects.

**Financial numbers don't match my expectations**

Verify the "As of Date" filter matches the date you intend to report on. Also confirm that the "Active Only" checkbox is set correctly; unchecking it will show completed projects with zero remaining balance. If using a date in the past, WIP snapshots may not have been captured on that exact date.

**The grid is loading slowly**

When filtering across many companies, branches, or with a large portfolio of projects, the quick view may take time to load. Narrow your filters to a specific company or project type to improve performance. Alternatively, run the report during off-peak hours.

**I need more detail than the quick view provides**

The quick view is intentionally simplified for speed. For comprehensive financial analysis, run the Project WIP Report (PROJ-RPT-004) or the Project WIP Template LD Report (PROJ-RPT-002), which offer additional cost breakdowns and customization.

**The WIP balance is negative or unexpectedly high**

A negative WIP indicates you have overbilled the customer (received payment for work not yet earned). A high WIP indicates earned revenue exceeds amounts billed, meaning the customer owes you additional invoices. Check the project's invoicing schedule and revenue recognition settings to ensure they are configured correctly.
