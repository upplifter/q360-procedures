---
title: Run the Project Backlog Projection Report
id: PROJ-RPT-016
module: Projects
screen: Project Backlog Projection Report
menu_path: Main Menu > Projects > Reports > Project Backlog Projection
applies_to: Finance, Operations Manager
prerequisites: null
related_procedures:
  - PROJ-RPT-013
  - PROJ-RPT-017
tags:
  - backlog projection
  - project backlog
  - backlog trajectory
  - revenue backlog
  - project forecast
version: 1.0
last_updated: 2026-03-25
---

# Run the Project Backlog Projection Report

## What This Procedure Does

This procedure shows you how to run the Project Backlog Projection Report. The report forecasts your project backlog trajectory, showing how backlog is expected to change over future periods based on current project activity and schedules.

## Before You Begin

Ensure you have access to the Projects module and Reports section. You should understand your organization's backlog metrics and which projects you want to analyze. Have your projection period in mind before starting.

## Steps

### Step 1: Navigate to the Report

From the Main Menu, click **Projects**. In the Projects menu, click **Reports**. Select **Project Backlog Projection** from the report list.

### Step 2: Set Filter Criteria

The report filter panel opens with fields for defining your backlog projection. Set the filters using the table below:

| Field | What to enter |
|-------|---------------|
| Project | Select specific projects or leave blank for all |
| Projection Period | Choose the period you want to project (next quarter, next year, etc.) |
| Backlog Type | Select revenue backlog, service backlog, or all types |
| Division | Choose a division or leave blank for all |
| Include Pending | Check to include pending or proposed projects in the projection |

Click **Apply Filters** to update the report with your selections.

### Step 3: Run the Report

Click the **Run** or **Refresh** button to execute the report with your chosen filters.

### Step 4: Review the Report Output

The report displays backlog projections over your selected time period. Review the trajectory to understand expected backlog changes. Examine individual project contributions to identify key drivers of backlog growth or decline.

### Step 5: Export or Print (Optional)

To save the report, click **Export** and choose your format (Excel, PDF, or CSV). To print, click **Print** and follow your printer settings.

## What Happens Next

The backlog projection data displays forecasted trajectory based on your selected parameters. Use this information for capacity planning, resource allocation, and business forecasting. Share the report with operations and finance teams for strategic planning and decision-making.

## Common Issues

**Backlog projection appears flat or unchanged**
Verify that projects in your filter have scheduled activity for the projection period. If many projects are complete or have no scheduled work, the backlog may show minimal change. Adjust your filter to include projects with planned activity.

**Projection shows negative backlog values**
This may indicate that scheduled work completion exceeds new project intake for certain periods. Review your project schedules and new business pipeline to confirm the projection is realistic. Contact the business development team if the forecast seems incorrect.

**Some projects are not included in the projection**
Check that projects are marked as Active or have pending status (if you checked the "Include Pending" option). Closed projects do not appear in forward-looking backlog projections. Verify your filter selections include the correct project statuses.

**Backlog amounts do not match the project list**
Confirm that the same filter criteria (division, project status, backlog type) are applied both in the report and when viewing the project list. Different filters will show different backlog totals.

**Report takes a long time to load**
Projections over very long periods can be slow to calculate. Try narrowing the projection period or selecting fewer projects. Run the report again after adjusting your filters for faster results.
