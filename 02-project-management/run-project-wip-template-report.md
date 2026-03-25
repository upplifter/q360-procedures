---
title: Run the Project WIP Template LD Report
id: PROJ-RPT-002
module: Projects
screen: Project WIP Template LD Report
menu_path: Main Menu > Projects > Reports > Project WIP Template LD
applies_to:
  - Project Manager
  - Finance
  - Operations Manager
prerequisites:
  - Access to the Projects module
  - Understanding of WIP snapshot dates
  - Ability to interpret financial variance data
related_procedures:
  - PROJ-RPT-003
  - PROJ-RPT-004
  - PROJ-RPT-005
tags:
  - WIP template
  - live data
  - work in progress
  - project WIP
  - financial analysis
  - customizable report
  - project report
version: "1.0"
last_updated: "2026-03-25"
---

# Run the Project WIP Template LD Report

## What This Procedure Does

The Project WIP Template LD (Live Data) Report provides a comprehensive, customizable financial overview of work-in-progress projects. It displays budget, projected, and earned columns for revenue and costs broken down by category (material, labor, subcontractor, miscellaneous, and warranty). This report also includes gross profit, gross margin, labor hours, percent complete, backlog, invoicing amounts, and budget-to-projected variance. The "template" nature of this report allows you to copy it and add or remove columns to match your specific reporting needs.

## Before You Begin

- Have access to the Projects module with appropriate permissions
- Identify the WIP snapshot date (or range of dates) you want to analyze
- Know which companies, branches, and project types to include
- Consider whether you need to customize column selections for this report

## Steps

### Step 1: Navigate to the Project WIP Template LD Report

From the main menu, select **Projects > Reports > Project WIP Template LD**. The report screen displays with filter options and a template column configuration area.

### Step 2: Set Your Filters

Configure the filters to specify which projects and data to include in the report:

| Field | What to enter |
|-------|---------------|
| As Of Date | Select the WIP snapshot date you want to report on; this determines which point-in-time financial data appears |
| Entity No. | Select one or more companies, or leave as the default current company |
| Branch | Select one or more branches, or leave as ALL to include all branches |
| Project Type | Select one or more project types, or leave as ALL for all types |

### Step 3: Configure Columns (Optional)

If you want to customize the columns displayed in the report, click the column configuration button or icon. The template allows you to:

- Add columns for additional financial metrics
- Remove columns you don't need
- Reorder columns for easier viewing
- Adjust column widths

To create a permanent customized version, save the template with a new name so your column selections are preserved for future runs.

### Step 4: Click Run or Refresh

Click **Run** or **Refresh** to execute the report with your selected filters and column configuration.

### Step 5: Review the Report Output

The report displays a grid with one row per project. Standard columns include:

- **Budget Revenue/Cost:** Amounts established in the original project budget
- **Projected Revenue/Cost:** Current estimate to complete, replacing the original budget if conditions have changed
- **Earned Revenue/Cost:** Revenue and costs recognized under your revenue recognition method
- **Costs by Category:** Material, labor, subcontractor, miscellaneous, and warranty costs shown separately
- **Gross Profit (GP) and Gross Margin (GM):** Overall profitability metrics
- **Labor Hours:** Projected and actual hours
- **GP/HR:** Gross profit per labor hour, a productivity metric
- **% Complete:** Overall project progress
- **Backlog:** Remaining work or revenue not yet earned
- **Invoiced Totals/Amounts Paid:** Customer billing and payment status
- **Budget-to-Projected Variance:** The difference between original budget and current projection

### Step 6: Analyze Variance and Performance

Focus on the budget-to-projected variance column to identify projects where financial expectations have shifted. Projects with large negative variance may indicate cost overruns or reduced revenue. Look at GP/HR to compare labor productivity across projects.

### Step 7: Export or Print (Optional)

Use the export or print function to save the report as Excel, PDF, or hardcopy for sharing or archival.

## What Happens Next

After running and reviewing the Project WIP Template LD Report, you may:

- Compare results to previous WIP snapshots by running the Delta Report (PROJ-RPT-006)
- Drill into a specific project for detailed cost analysis
- Save your customized column template for reuse in future reporting periods
- Use the variance data to inform project adjustments or change orders
- Share the report with stakeholders for financial review meetings

## Common Issues

**The As Of Date filter shows no available dates**

WIP snapshots are typically captured on a monthly or periodic basis. If you select a date when no snapshot was created, the report may show no data. Check with your finance team to determine the standard snapshot dates, or run the report using the most recent available snapshot date.

**Columns are missing from the report output**

After running the report, verify your column configuration was saved. If you customized columns but did not save the template, the next run may revert to default columns. Always save customized templates with a unique name to preserve your settings.

**The report takes a long time to load**

Large project portfolios with many cost detail records can slow report performance. Narrow your filters to specific companies, branches, or project types. Running the report on a subset of data will improve speed.

**Budget and Projected columns show the same values**

When budget and projected values are identical, it indicates no changes have been made to the project scope or estimates since the budget was approved. This is normal for projects early in their lifecycle or those progressing exactly as planned.

**Gross Margin percentages appear negative**

Negative gross margin indicates the project is unprofitable—actual or projected costs exceed revenue. This requires immediate attention. Review the project's pricing, scope, and cost controls to understand the cause and determine whether to adjust estimates, pursue change orders, or restructure the engagement.
