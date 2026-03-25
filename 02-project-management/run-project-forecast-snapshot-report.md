---
title: Run the Project Forecast Snapshot Analysis Report
id: PROJ-RPT-019
module: Projects
screen: Project Forecast Snapshot Analysis Report
menu_path: Main Menu > Projects > Reports > Project Forecast Snapshot Analysis
applies_to: Finance, Operations Manager
prerequisites: null
related_procedures:
  - PROJ-RPT-006
  - PROJ-RPT-001
tags:
  - forecast snapshot
  - snapshot analysis
  - historical forecast
  - actuals comparison
  - project forecast
  - trend analysis
version: 1.0
last_updated: 2026-03-25
---

# Run the Project Forecast Snapshot Analysis Report

## What This Procedure Does

This procedure shows you how to run the Project Forecast Snapshot Analysis Report. The report compares historical forecasts to actual results, helping you evaluate forecast accuracy and identify trends in project performance.

## Before You Begin

Ensure you have access to the Projects module and Reports section. You should understand your organization's forecast history and which projects you want to analyze. Have the snapshot dates and analysis period in mind before starting.

## Steps

### Step 1: Navigate to the Report

From the Main Menu, click **Projects**. In the Projects menu, click **Reports**. Select **Project Forecast Snapshot Analysis** from the report list.

### Step 2: Set Filter Criteria

The report filter panel opens with fields for defining your snapshot analysis. Set the filters using the table below:

| Field | What to enter |
|-------|---------------|
| Project | Select specific projects or leave blank for all |
| Snapshot Date | Choose the historical forecast date to analyze |
| Actual Period | Choose the period with actual results to compare |
| Metric | Select revenue, cost, backlog, or gross profit |
| Division | Select a division or leave blank for all |

Click **Apply Filters** to update the report with your selections.

### Step 3: Run the Report

Click the **Run** or **Refresh** button to execute the report with your chosen filters.

### Step 4: Review the Report Output

The report displays forecasted amounts from the snapshot date alongside actual results from the actual period. Review the variance column to see how accurate the forecasts were. Examine trends across multiple snapshots to evaluate forecast reliability and identify patterns.

### Step 5: Export or Print (Optional)

To save the report, click **Export** and choose your format (Excel, PDF, or CSV). To print, click **Print** and follow your printer settings.

## What Happens Next

The snapshot analysis data displays historical forecast accuracy based on your selected parameters. Use this information to evaluate your forecasting process, identify systematic biases, and improve future predictions. Share the report with forecast and finance teams for process improvement discussions.

## Common Issues

**No snapshot data available for the selected date**
Verify that the snapshot date you selected corresponds to a date when forecasts were actually created and saved. Forecasts are typically created at regular intervals (monthly, quarterly). Select a different snapshot date if data is not available.

**Actual period data appears incomplete**
Confirm that the actual period you selected is in the past and that all transactions have been recorded and posted. If the actual period is recent, some transactions may still be pending. Select a completed period for accurate comparison.

**Variance amounts seem unusually large**
Large variances can indicate significant changes in project scope, schedule, or costs since the forecast was created. Review the project history and change orders to understand what drove the variance. Contact the project manager for context on major changes.

**Report includes too many data points**
Narrow your analysis by selecting fewer projects or focusing on specific metrics. Reduce the number of snapshot dates included to make the report more manageable. Run the report again with more focused selections.

**Forecast accuracy appears to be getting worse over time**
This may indicate changes in your forecasting process, business conditions, or project characteristics. Investigate the causes of declining accuracy by reviewing specific projects with large variances. Consider updating your forecasting methodology or assumptions.
