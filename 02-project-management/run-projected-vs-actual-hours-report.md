---
title: Run the Projected vs. Actual Hours Report
id: PROJ-RPT-010
module: Projects
screen: Projected vs. Actual Hours Report
menu_path: Main Menu > Projects > Projects (via Print button) OR Main Menu > Projects > Reports
applies_to:
  - Project Manager
  - Operations Manager
prerequisites:
  - Access to the Projects module
  - Understanding of labor hour tracking and Internal Change Orders (ICOs)
  - Access to project time entry and task data
related_procedures:
  - PROJ-RPT-007
  - PROJ-RPT-009
  - PROJ-ICO-001
tags:
  - projected vs actual
  - hours comparison
  - labor performance
  - actual hours
  - projected hours
  - variance
  - labor analysis
version: "1.0"
last_updated: "2026-03-25"
---

# Run the Projected vs. Actual Hours Report

## What This Procedure Does

The Projected vs. Actual Hours Report compares projected labor hours against actual hours worked for each task category in a project. This report shows variance between what was estimated and what actually occurred, helping you understand labor performance and efficiency. A unique feature of this report is the Adjustment column, which allows you to create an Internal Change Order (ICO) directly from the report to formally adjust labor hour budgets when actual hours differ from projections.

## Before You Begin

- Have access to the Projects module with appropriate permissions
- Identify whether you want to run the report from a specific project or across multiple projects
- Understand that this report is used to review labor performance and plan hour adjustments
- Be prepared to create Internal Change Orders if significant variances warrant budget adjustment

## Steps

### Step 1: Navigate to the Projected vs. Actual Hours Report

You can access this report in two ways:

**Option A: From a Specific Project**
- Open the project form from **Main Menu > Projects**
- Click the **Print** button on the project form
- Select **Projected vs. Actual Hours Report** from the print menu

**Option B: From the Reports Menu**
- Select **Main Menu > Projects > Reports**
- Select **Projected vs. Actual Hours Report**
- Apply project filters to focus on specific projects (see Step 2)

### Step 2: Set Your Filters (Reports Menu Only)

If you accessed the report from the Reports menu, configure filters to specify which projects to analyze. If you accessed the report from a project's Print button, the report automatically filters to that project only.

### Step 3: Click Run

Click the **Run** or **Refresh** button to execute the report.

### Step 4: Review the Report Output

The report displays a grid with one row per task category. Columns typically include:

- **Task Category/Phase:** The work phase or task grouping
- **Projected Hours:** Labor hours budgeted for this task category
- **Actual Hours:** Labor hours already worked or recorded
- **Variance Hours:** Difference between Projected and Actual (Actual minus Projected)
- **Variance %:** Variance expressed as a percentage
- **Adjustment:** A column where you can enter additional hours to adjust the budget

Tasks where Actual exceeds Projected show positive variance (overrun). Tasks where Actual is less than Projected show negative variance (underrun).

### Step 5: Analyze Labor Performance

Review each task category to understand labor efficiency:

- **Positive Variance (Overruns):** More hours were spent than estimated, indicating scope creep, inefficiency, or scope complexity underestimation
- **Negative Variance (Underruns):** Fewer hours were spent than estimated, indicating efficiency gains or potentially underestimated productivity
- **Large Variance %:** Significant deviation from projection warrants investigation

### Step 6: Determine Adjustments (Optional)

If you want to formally adjust labor hour budgets to reflect actual performance or revised estimates, enter the adjustment hours in the **Adjustment** column:

- **Positive Adjustment:** Increases the budget to accommodate additional hours
- **Negative Adjustment:** Decreases the budget if fewer hours are needed than originally projected
- **Zero Adjustment:** No change to the budget

### Step 7: Create an Internal Change Order (If Needed)

If you have entered adjustments and want to formalize them as a change to the project budget:

1. Click **Extended Menu** or the menu icon
2. Select **Process ICO** (Internal Change Order)
3. Review the ICO that is created, which includes your adjustment amounts
4. Approve and save the ICO to update the project labor hour budget

The system creates an ICO-type order with the hour adjustments specified in the Adjustment column. This formally documents the budget change and updates the project's projections.

### Step 8: Export or Print (Optional)

Use the export or print functions to save the report as Excel, PDF, or hardcopy for project records and team communication.

## What Happens Next

After reviewing the Projected vs. Actual Hours Report, you may:

- Create Internal Change Orders (PROJ-ICO-001) to formally adjust labor budgets for tasks with significant variance
- Investigate root causes of large variances with the project team
- Adjust task scheduling or resource allocation to improve performance on remaining work
- Use variance patterns to improve future project estimates
- Update the customer of labor hour changes if applicable to billing

## Common Issues

**Actual hours are showing as zero**

Verify that time entries have been recorded against the project tasks. If team members have not yet entered time, actual hours will not appear. Check the current date and your time entry cutoff to confirm whether time has been submitted and posted.

**I cannot find the Adjustment column**

The Adjustment column may be hidden if the report view has been customized. Check whether the report allows scrolling to the right to reveal additional columns, or look for a column visibility setting to unhide the Adjustment column.

**The Process ICO button is not available**

Verify that you have sufficient permissions to create change orders. Also confirm that adjustments have actually been entered in the Adjustment column; if the column is empty, the Process ICO option may be disabled. Enter adjustment values and try again.

**I created an ICO but the project budget didn't change**

After creating the ICO, it may require approval before it updates the project budget. Check the status of the ICO in the change orders list. Once approved and committed, the ICO will update the project's hours and projections. In the interim, the original budget remains in effect.

**The variance percentage seems incorrect**

Verify the calculation by dividing the variance hours by the projected hours. Some systems calculate variance as (Actual - Projected) / Projected; others may use different methodologies. Check your system documentation or with your accounting team to confirm the calculation method.

**Projected hours for some tasks are zero or very low**

If a task has zero or minimal projected hours, it may indicate:
- The task was not estimated when the budget was created
- The task estimate was deleted or removed
- The task is a newly identified scope item not in the original budget
- The task was included as part of another larger task

Review the project estimate or work breakdown structure to understand whether this is intentional or an error in the budget.
