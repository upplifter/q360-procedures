---
title: Run the Closed Project WIP Report
id: PROJ-RPT-021
module: Projects
screen: Closed Project WIP Report
menu_path: Main Menu > Projects > Reports > Closed Project WIP
applies_to: Finance, Controller
prerequisites: null
related_procedures:
  - PROJ-CLOSE-003
  - PROJ-RPT-004
  - PROJ-CLOSE-004
tags:
  - closed project WIP
  - residual WIP
  - closed projects
  - work in progress
  - WIP cleanup
version: 1.0
last_updated: 2026-03-25
---

# Run the Closed Project WIP Report

## What This Procedure Does

This procedure shows you how to run the Closed Project WIP Report. The report identifies work in progress balances remaining on closed projects, helping you locate residual costs that need to be adjusted or reclassified.

## Before You Begin

Ensure you have access to the Projects module and Reports section. You should understand your organization's project closure process and WIP adjustment procedures. Have your review period in mind before starting.

## Steps

### Step 1: Navigate to the Report

From the Main Menu, click **Projects**. In the Projects menu, click **Reports**. Select **Closed Project WIP** from the report list.

### Step 2: Set Filter Criteria

The report filter panel opens with fields for identifying residual WIP. Set the filters using the table below:

| Field | What to enter |
|-------|---------------|
| Project Status | Select Closed to view closed projects |
| Closure Date | Enter the date range for project closure |
| WIP Amount | Specify a minimum WIP amount to filter out trivial balances |
| Division | Select a division or leave blank for all |
| Account Type | Select all cost accounts or specific account types |

Click **Apply Filters** to update the report with your selections.

### Step 3: Run the Report

Click the **Run** or **Refresh** button to execute the report with your chosen filters.

### Step 4: Review the Report Output

The report displays residual work in progress balances on closed projects. Review each project and its WIP amount. Identify which accounts contain the residual WIP and determine whether the balance should be adjusted, reclassified, or investigated.

### Step 5: Export or Print (Optional)

To save the report, click **Export** and choose your format (Excel, PDF, or CSV). To print, click **Print** and follow your printer settings.

## What Happens Next

The closed project WIP data displays residual costs that require attention. Work with your accounting and project teams to resolve these balances. Create adjustment journal entries to move WIP to appropriate accounts, write off immaterial balances, or reclassify costs as needed. Track your WIP cleanup activities using the report to verify all balances have been addressed.

## Common Issues

**Report shows WIP on closed projects but cannot determine why**
Review the project ledger and transaction history to identify the source of the WIP balance. Check whether there are outstanding expenses, timekeeping entries, or material charges that have not been fully billed. Contact the project manager for context.

**WIP amounts are very small and seem immaterial**
Small residual balances may be due to rounding, pending adjustments, or minor unbilled charges. Determine your organization's threshold for immaterial balances and either write off small amounts or group them for adjustment. Document your cleanup actions.

**Cannot close a project because WIP balances remain**
Residual WIP may need to be addressed before formal project closure in the system. Create adjustment entries to clear the WIP to appropriate expense or revenue accounts, or reclassify to a suspense account for later review. Consult your accounting policies.

**Report shows projects that are not actually closed**
Verify that projects are truly marked as Closed in the system. Double-check the project status to confirm closure. If projects should not appear, adjust your filter to exclude them and rerun the report.

**WIP is concentrated in specific accounts or cost centers**
This pattern may indicate systematic issues with how costs are being charged to projects. Review those accounts and cost centers to identify process improvements. Address the root cause to prevent WIP issues on future projects.
