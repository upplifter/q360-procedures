---
title: Run the Project Delta Report
id: PROJ-RPT-006
module: Projects
screen: Project Delta Report
menu_path: Main Menu > Projects > Reports > Project Delta
applies_to:
  - Project Manager
  - Operations Manager
  - Finance
prerequisites:
  - Access to the Projects module
  - Availability of at least two WIP snapshot dates for comparison
  - Understanding of period-over-period financial analysis
related_procedures:
  - PROJ-RPT-001
  - PROJ-RPT-018
tags:
  - project delta
  - period over period
  - changes
  - variance
  - project changes
  - financial delta
  - trend analysis
version: "1.0"
last_updated: "2026-03-25"
---

# Run the Project Delta Report

## What This Procedure Does

The Project Delta Report analyzes period-over-period financial changes for projects by comparing WIP snapshots at two different points in time. It shows changes in projected revenue, projected cost, projected gross profit, earned revenue, actual cost, and other key metrics between two dates. Use this report to identify which projects have experienced significant financial movement, such as scope changes, cost adjustments, or shifts in completion estimates.

## Before You Begin

- Ensure you have access to the Projects module with reporting permissions
- Identify two different WIP snapshot dates to compare (Start Period and End Period)
- Determine which companies, branches, or project types to include
- Know the period-over-period changes you want to investigate

## Steps

### Step 1: Navigate to the Project Delta Report

From the main menu, select **Projects > Reports > Project Delta**. The report screen displays with filter options for date selection and project filtering.

### Step 2: Set Your Filters

Configure the filters to specify the comparison periods and projects:

| Field | What to enter |
|-------|---------------|
| Company | Select one or more companies to analyze, or leave blank for all |
| Branch | Select one or more branches, or leave as ALL for all branches |
| Project Type | Select one or more project types, or leave as ALL for all types |
| Start Period As Of Date | Enter the earlier date (the "from" snapshot) |
| End Period As Of Date | Enter the later date (the "to" snapshot) |
| Project Manager | Select one or more project managers, or leave as ALL |

### Step 3: Click Run

Click the **Run** button to execute the report and calculate the deltas between your two selected periods.

### Step 4: Review the Report Output

The report displays a grid with one row per project and columns showing:

**Starting Period Columns (at Start Period As Of Date):**
- Projected Revenue, Projected Cost, Projected GP (Gross Profit)
- Earned Revenue, Actual Cost
- Other baseline metrics

**Ending Period Columns (at End Period As Of Date):**
- Projected Revenue, Projected Cost, Projected GP
- Earned Revenue, Actual Cost
- Other comparative metrics

**Delta Columns (Change from Start to End Period):**
- Change in Projected Revenue
- Change in Projected Cost
- Change in Projected GP
- Change in Earned Revenue
- Change in Actual Cost
- Other metric deltas

### Step 5: Identify Large Changes

Sort or filter the delta columns to find projects with significant changes. Positive deltas indicate increases; negative deltas indicate decreases. Focus on:

- **Large Positive GP Deltas:** Projects that have become more profitable
- **Large Negative GP Deltas:** Projects where profitability has declined
- **Significant Revenue Changes:** Possible scope additions or reductions
- **Cost Changes:** Actual costs trending above or below projections

### Step 6: Investigate Root Causes

For projects with notable deltas, determine what caused the change:

- **Scope Changes:** Were change orders approved that added or removed deliverables?
- **Cost Adjustments:** Did project managers revise cost estimates based on new information?
- **Progress Variance:** Did actual costs come in better or worse than originally projected?
- **Billing Changes:** Were invoicing rates or milestones adjusted?

### Step 7: Export or Print (Optional)

Use the export or print functions to save the report as Excel, PDF, or hardcopy for presentation and archival.

## What Happens Next

After reviewing the Project Delta Report, you may:

- Drill into individual projects to investigate significant changes
- Review change orders or project adjustments that explain large variances
- Run the detailed WIP Report (PROJ-RPT-004) for deeper analysis of a specific project
- Brief management or customers on significant project financial changes
- Adjust future project estimates based on historical delta trends

## Common Issues

**The report shows no delta (all changes are zero)**

This indicates that the two WIP snapshot dates have identical financial data for the selected projects. Verify that you have selected two different dates and that at least one transaction (invoice, cost, estimate change) occurred between those dates. If you are using very recent dates, transactions may not have posted yet.

**One of my selected dates has no WIP snapshot data**

WIP snapshots are created on a periodic basis (typically monthly). If you select a date when no snapshot was captured, the report cannot calculate a delta. Check with your finance team for the standard snapshot schedule, or select dates that correspond to actual snapshot captures.

**The delta shows large changes that don't match known change orders**

Verify that the change orders were approved and recorded in the project system. Alternatively, the delta may reflect cost adjustments made by project managers that were not formally documented as change orders. Review the project's recent transaction history and manager notes to identify the source of the change.

**Projected changes are large but earned revenue shows no change**

This is normal when project managers update estimates without affecting work that has already been completed and earned. The projected delta reflects management's revised outlook, while the earned revenue delta reflects only the value of work actually performed during the period.

**I need to understand which specific transactions caused the delta**

The delta report shows the net change between two points in time but does not list individual transactions. To see transaction-level detail, open the specific project and review its cost and invoice histories. Alternatively, run cost or invoice detail reports filtered to the time period between your two delta dates.

**Multiple projects show negative GP deltas—should I be concerned?**

If multiple projects show declining profitability, it could indicate:
- Systematic cost inflation across the portfolio
- Issues with cost estimation or resource allocation
- Market or supply chain changes affecting material or labor costs
- Pricing that is not keeping pace with costs

Investigate trends to determine whether this is normal variation or a signal of structural problems.
