---
title: Run the Project Labor Forecast Report
id: PROJ-RPT-009
module: Projects
screen: Project Labor Forecast Report
menu_path: Main Menu > Projects > Reports > Project Labor Forecast
applies_to:
  - Project Manager
  - Operations Manager
  - Resource Manager
prerequisites:
  - Access to the Projects module
  - Understanding of project scheduling and labor forecasting
  - Current project schedules with resource assignments
related_procedures:
  - PROJ-RPT-007
  - PROJ-RPT-008
  - PROJ-RPT-010
tags:
  - labor forecast
  - project labor
  - future labor
  - capacity planning
  - resource forecast
  - labor projection
version: "1.0"
last_updated: "2026-03-25"
---

# Run the Project Labor Forecast Report

## What This Procedure Does

The Project Labor Forecast Report projects future labor demand across active projects. It breaks down scheduled and assigned hours by time period (weekly or monthly), enabling managers to forecast upcoming labor needs and identify capacity constraints before they impact project delivery. Use this report for workforce planning, identifying peak demand periods, and ensuring adequate resource availability.

## Before You Begin

- Have access to the Projects module with forecasting permissions
- Know the forecast start date and duration you want to analyze
- Identify any filters you need (company, branch, project type, project manager)
- Ensure project schedules and resource assignments are current

## Steps

### Step 1: Navigate to the Project Labor Forecast Report

From the main menu, select **Projects > Reports > Project Labor Forecast**. The report screen displays with filter and date options.

### Step 2: Set Your Filters

Configure the filters to specify which projects and time period to forecast:

| Field | What to enter |
|-------|---------------|
| Company | Select one or more companies, or leave blank for all |
| Branch | Select one or more branches, or leave as ALL for all branches |
| Department | Select one or more departments, or leave as ALL for all departments |
| Project Type | Select one or more project types, or leave as ALL for all types |
| Project Manager | Select one or more project managers, or leave as ALL |
| Forecast Start Date | Enter the date when the forecast should begin (typically today or the next period) |

### Step 3: Click Run

Click the **Run** button to execute the forecast.

### Step 4: Review the Report Output

The report displays a grid showing labor hours projected across time periods. The structure typically shows:

- **Project Name/ID:** Each project in the forecast
- **Period Columns:** Time periods (weekly or monthly) starting from the Forecast Start Date
  - Each period column shows:
    - **Scheduled Hours:** Labor hours planned for that period per the project schedule
    - **Assigned Hours:** Labor hours allocated to specific team members for that period

The report may also include:
- A totals row summing hours across all projects for each period
- A summary table showing total demand by period
- Peak demand indicators or warning flags for periods with high labor demand

### Step 5: Identify Peak Demand Periods

Review the period columns to identify weeks or months with high total labor demand:

- **High-Demand Periods:** When total hours spike, indicating potential resource constraints
- **Low-Demand Periods:** When total hours dip, indicating available capacity
- **Uneven Distribution:** When labor demand varies significantly period to period, requiring flexibility in resource allocation

### Step 6: Assess Resource Availability

Compare forecasted demand to available capacity:

- If peak demand periods exceed your team's capacity, plan to hire contractors, reallocate resources across projects, or adjust schedules to smooth demand
- If low-demand periods are followed by peaks, plan to retain resources or retain contractors through slower periods

### Step 7: Identify Assignment Gaps

Look for projects with scheduled hours that exceed assigned hours:

- **High Scheduled/Low Assigned:** Labor is planned but not yet allocated to specific team members. Follow up with project managers to formalize assignments.
- **Zero Assigned:** No resources are committed to these periods, indicating a planning gap that needs resolution

### Step 8: Export or Print (Optional)

Use the export or print functions to save the forecast as Excel, PDF, or hardcopy for workforce planning meetings and capacity discussions.

## What Happens Next

After reviewing the Project Labor Forecast Report, you may:

- Run the Employee Assignee Detail Forecast Report (PROJ-RPT-008) to see how individual employees are assigned across this forecast period
- Adjust project schedules or assignments to level capacity across periods
- Initiate hiring or contractor engagement to cover peak demand periods
- Brief management on anticipated resource needs and any constraints
- Use the forecast to plan training, vacation time, and other capacity factors

## Common Issues

**The forecast shows no data or very low hours**

Verify that projects have been properly scheduled and resource assignments have been entered. If projects are in early stages without detailed schedules, forecasted hours may be minimal or zero. Confirm that tasks in the schedule have assigned resources and duration estimates.

**Scheduled hours are much higher than Assigned hours**

This gap indicates labor has been planned but not yet formally assigned to team members. This is common in early project phases. Follow up with project managers to create specific assignments, or the forecast may underestimate actual resource needs.

**The forecast shows capacity that I know we don't actually have**

Forecasts based on project data alone may not account for non-project work, administrative overhead, time off, or other commitments. Add capacity planning buffers manually if your system does not account for these factors. Communicate realistic available capacity to project managers.

**The report covers too long or too short a period**

Adjust the Forecast Start Date to rerun the report with your desired time horizon. If you want a quarterly forecast, set the start date to the first day of the quarter and rerun. The report duration is typically configurable based on your selections.

**I see scheduled hours but no assigned hours even though people are assigned to tasks**

Verify that assignments are recorded with start and end dates that fall within your forecast period. Assignments recorded for dates outside your report range will not appear. Check assignment configuration to ensure dates are current.

**Some projects are missing from the forecast**

Verify that all projects you want to include match your filter selections. Inactive projects or those with no scheduled hours may not appear. Uncheck filters or select specific projects to verify they are included in the forecast.
