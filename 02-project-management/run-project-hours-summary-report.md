---
title: Run the Project Hours Summary Report
id: PROJ-RPT-007
module: Projects
screen: Project Hours Summary Report
menu_path: Main Menu > Projects > Reports > Project Hours Summary
applies_to:
  - Project Manager
  - Operations Manager
prerequisites:
  - Access to the Projects module
  - Understanding of project labor forecasting and actuals
  - Access to time and labor tracking system
related_procedures:
  - PROJ-RPT-008
  - PROJ-RPT-009
  - PROJ-RPT-010
tags:
  - hours summary
  - labor hours
  - project hours
  - time analysis
  - labor report
  - project labor
version: "1.0"
last_updated: "2026-03-25"
---

# Run the Project Hours Summary Report

## What This Procedure Does

The Project Hours Summary Report provides a comprehensive overview of labor hours across your project portfolio. It summarizes projected hours (the original budget), scheduled hours (the revised plan), assigned hours (time allocated to resources), actual hours (time already worked), and remaining hours (time still to be expended). Use this report to monitor labor utilization, identify capacity constraints, and assess whether projects are progressing on schedule from a labor perspective.

## Before You Begin

- Have access to the Projects module with labor reporting permissions
- Know the date range you want to analyze
- Identify any filters you need (company, branch, department, project type, project manager)
- Understand the difference between projected, scheduled, assigned, and actual hours in your system

## Steps

### Step 1: Navigate to the Project Hours Summary Report

From the main menu, select **Projects > Reports > Project Hours Summary**. The report screen displays with filter options.

### Step 2: Set Your Filters

Configure the filters to specify which projects and time period to include:

| Field | What to enter |
|-------|---------------|
| Company | Select one or more companies, or leave blank for all |
| Branch | Select one or more branches, or leave as ALL for all branches |
| Department | Select one or more departments, or leave as ALL for all departments |
| Project Type | Select one or more project types, or leave as ALL for all types |
| Project Manager | Select one or more project managers, or leave as ALL |
| Date Range | Enter the start and end dates for the analysis period |

### Step 3: Click Run

Click the **Run** button to execute the report.

### Step 4: Review the Report Output

The report displays a grid with one row per project. Columns typically include:

- **Projected Hours:** Labor hours in the original project budget
- **Scheduled Hours:** Labor hours in the current revised schedule
- **Assigned Hours:** Labor hours allocated to specific team members
- **Actual Hours:** Labor hours already recorded as time entries
- **Remaining Hours:** Projected labor hours still to be performed (Projected minus Actual)
- **Variance %:** Variance between projected and actual hours (or between scheduled and assigned)

A totals row at the bottom sums hours across all projects.

### Step 5: Analyze Hour Utilization

Review each project to assess labor efficiency:

- **Projects where Actual exceeds Projected:** Labor is consuming more hours than budgeted, indicating scope creep, inefficiency, or underestimation
- **Projects where Remaining is low:** Nearly all budgeted labor has been consumed; project is near completion or approaching overrun
- **High Variance %:** Significant deviation between original plan and current actuals suggests either scope changes or estimation issues

### Step 6: Identify Capacity Constraints

Compare scheduled and assigned hours to identify whether you have sufficient labor assigned. If assigned hours are significantly lower than scheduled, you may have resource allocation gaps.

### Step 7: Export or Print (Optional)

Use the export or print functions to save the report as Excel, PDF, or hardcopy for team meetings, archives, or stakeholder communication.

## What Happens Next

After reviewing the Project Hours Summary Report, you may:

- Drill into specific projects to understand labor composition and task-level hour allocation
- Run the Employee Assignee Detail Forecast Report (PROJ-RPT-008) to see hours by individual resource
- Execute the Project Labor Forecast Report (PROJ-RPT-009) to plan future labor demand
- Run the Projected vs. Actual Hours Report (PROJ-RPT-010) for detailed task-level comparison
- Adjust resource assignments or project schedules to address capacity issues
- Initiate change orders to accommodate labor hour overruns

## Common Issues

**Actual hours are showing as zero for active projects**

Verify that time has been recorded against the projects in the time tracking system. If team members have not yet entered time entries, actual hours will not populate. Check the current date relative to your payroll/time entry cutoff dates.

**Projected hours are very different from Scheduled hours**

This variance typically occurs after project estimates have been revised due to scope changes or updated resource assessments. The discrepancy is normal and expected during project execution. Monitor the Remaining hours to see whether the updated schedule is realistic.

**Remaining hours shows a negative value**

A negative remaining hours value indicates the project has already consumed more labor than was originally budgeted. This signals an overrun and may require a change order, additional funding, or scope reduction to address. Investigate the cause and plan corrective action.

**The report doesn't break down hours by role or skill**

The summary report intentionally provides high-level totals by project. If you need hours broken down by role, skill, or individual employee, run the Employee Assignee Detail Forecast Report (PROJ-RPT-008) instead.

**I see a large discrepancy between Assigned and Actual hours**

Assigned hours represent the forecasted effort; Actual hours are hours already worked. Early in a project, assigned and actual may differ significantly. As the project progresses, actual hours should approach assigned hours. If actual is consistently lower, team members may be working on untracked activities or time entries may be incomplete.

**Hours data across time range looks inconsistent**

If you selected a date range spanning multiple reporting periods, hours may accumulate or reset depending on how your system calculates rolling totals. Verify that you are selecting appropriate date boundaries that align with your project reporting cycles.
