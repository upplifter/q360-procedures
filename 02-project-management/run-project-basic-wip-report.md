---
title: Run the Project Basic WIP Report
id: PROJ-RPT-003
module: Projects
screen: Project Basic WIP Report
menu_path: Main Menu > Projects > Reports > Project Basic WIP
applies_to:
  - Project Manager
  - Finance
prerequisites:
  - Access to the Projects module
  - Permission to view project financial data
  - Understanding of work-in-progress concepts
related_procedures:
  - PROJ-RPT-002
  - PROJ-RPT-004
tags:
  - basic WIP
  - work in progress
  - simplified WIP
  - project report
  - financial summary
version: "1.0"
last_updated: "2026-03-25"
---

# Run the Project Basic WIP Report

## What This Procedure Does

The Project Basic WIP Report is a simplified, quick-reference alternative to the full WIP report. It provides an overview of work-in-progress balances for active projects, showing projected revenue, projected cost, actual cost, earned revenue, earned cost, and the WIP balance per project. Use this report when you need a high-level financial snapshot without the detailed cost breakdowns and extensive metrics of the comprehensive WIP report.

## Before You Begin

- Have access to the Projects module with appropriate permissions
- Know the date you want to report on (defaults to today)
- Identify any project filters you want to apply (company, branch, department, etc.)
- Understand that this report is designed for quick review rather than detailed analysis

## Steps

### Step 1: Navigate to the Project Basic WIP Report

From the main menu, select **Projects > Reports > Project Basic WIP**. The report screen loads with filter fields and a Run button.

### Step 2: Set Your Filters

Configure the filters to specify which projects to include in the report:

| Field | What to enter |
|-------|---------------|
| Company | Select one or more companies to report on |
| Branch | Select one or more branches, or leave as ALL for all branches |
| Department | Select one or more departments, or leave as ALL for all departments |
| Project Type | Select one or more project types, or leave as ALL for all types |
| Status | Select one or more project statuses (Active, Closed, On Hold, etc.) |
| Project Manager | Select one or more project managers, or leave as ALL for all managers |
| As of Date | Enter the date for the WIP snapshot; defaults to today |

### Step 3: Click Run

Click the **Run** button to execute the report with your selected filters.

### Step 4: Review the Output

The report displays a simple grid with one row per project. Columns include:

- **Project Name/ID:** The project identifier
- **Projected Revenue:** Estimated total revenue based on current project estimate
- **Projected Cost:** Estimated total cost based on current project estimate
- **Actual Cost:** Costs recorded to the project to date
- **Earned Revenue:** Revenue recognized under your revenue recognition method
- **Earned Cost:** Costs associated with recognized revenue
- **WIP Balance:** The difference between earned and billed amounts

A totals row at the bottom sums the numeric columns across all displayed projects.

### Step 5: Compare Projected to Actual

Examine the difference between projected and actual costs. Projects where actual cost significantly exceeds projected cost indicate cost overruns requiring investigation or mitigation.

### Step 6: Assess WIP Balances

Review the WIP Balance column to identify which projects have the largest outstanding balances. Large positive WIP indicates significant unbilled revenue; large negative WIP indicates overbilling situations.

### Step 7: Export or Print (Optional)

Use the export or print buttons to save the report as Excel, PDF, or hardcopy for distribution or archival purposes.

## What Happens Next

After reviewing the Project Basic WIP Report, you may:

- Open a specific project in the project form to investigate further
- Run the comprehensive Project WIP Report (PROJ-RPT-004) for detailed cost category breakdowns
- Use the Delta Report (PROJ-RPT-006) to compare this snapshot to an earlier one
- Initiate corrective actions for projects with significant cost variances or WIP imbalances

## Common Issues

**The report shows no data**

Verify that your filter selections match projects that exist in the system. If filtering by a specific project manager or department, confirm that assigned projects match your selections. Try broadening your filters or check the "As of Date" to ensure it is a valid snapshot date.

**Projected and Actual costs are identical**

This typically occurs when a project has just been created or no additional transactions have been recorded since the original budget was established. As the project progresses and costs are recorded, the actual cost will diverge from the projection.

**WIP Balance is negative for all projects**

A negative WIP across the portfolio indicates widespread overbilling, which is unusual and suggests either a configuration issue or systematic customer prepayment. Investigate whether customer contracts include advance payments or retainers that are inflating the WIP balances.

**The report is too basic for my needs**

If you require more detailed cost breakdowns by category (material, labor, subcontractor), completion percentages, or other metrics, run the full Project WIP Report (PROJ-RPT-004) instead. The basic report is intentionally simplified for quick review.

**I cannot see labor hour metrics**

The basic WIP report does not include labor hour details. If you need labor hours, hours productivity ratios, or labor-specific completion percentages, use the Project Labor Forecast Report (PROJ-RPT-009) or the Projected vs. Actual Hours Report (PROJ-RPT-010).
