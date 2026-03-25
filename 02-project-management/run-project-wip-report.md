---
title: Run the Project WIP Report
id: PROJ-RPT-004
module: Projects
screen: Project WIP Report
menu_path: Main Menu > Projects > Reports > Project WIP
applies_to:
  - Finance
  - Operations Manager
  - Project Manager
prerequisites:
  - Access to the Projects module with financial reporting permissions
  - Understanding of revenue recognition methods
  - Familiarity with project costing structures
related_procedures:
  - PROJ-RPT-002
  - PROJ-RPT-003
  - PROJ-RPT-005
tags:
  - project WIP
  - work in progress
  - WIP report
  - detailed WIP
  - financial analysis
  - revenue recognition
  - project financials
version: "1.0"
last_updated: "2026-03-25"
---

# Run the Project WIP Report

## What This Procedure Does

The Project WIP Report is the comprehensive work-in-progress financial analysis tool for active projects. It provides detailed information on projected and actual revenue and costs, profit margins, percent complete by cost and labor, over/under billing, backlog amounts, and retention. Use this report for complete financial visibility into each project's status, profitability, and billing position.

## Before You Begin

- Verify you have access to the Projects module with permissions to view financial data
- Confirm the "as of" date you want the report for
- Identify any filters you need (company, branch, project type, etc.)
- Understand your organization's revenue recognition and cost accounting methods

## Steps

### Step 1: Navigate to the Project WIP Report

From the main menu, select **Projects > Reports > Project WIP**. The report screen displays with filter options.

### Step 2: Set Your Filters

Configure the filters to scope the report to your area of interest:

| Field | What to enter |
|-------|---------------|
| Company | Select one or more companies, or leave blank for all |
| Branch | Select one or more branches, or leave as ALL for all branches |
| Department | Select one or more departments, or leave as ALL for all departments |
| Project Type | Select one or more project types, or leave as ALL for all types |
| Status | Select one or more project statuses (Active, Closed, On Hold, etc.) |
| Project Manager | Select one or more project managers, or leave as ALL |
| As of Date | Enter the date for the WIP snapshot; defaults to today |

### Step 3: Click Run

Click the **Run** button to execute the report with your selected filters.

### Step 4: Review the Report Output

The report displays a detailed grid with one row per project. Key columns include:

**Revenue and Cost Metrics:**
- **Projected Revenue/Cost:** Current estimate to complete based on the latest project forecast
- **Actual Revenue/Cost:** Invoices recorded and expenses incurred to date
- **Earned Revenue/Cost:** Revenue and costs recognized under your revenue recognition method

**Profitability:**
- **Gross Profit (GP):** Revenue minus costs
- **Gross Margin (%):** Gross profit as a percentage of revenue
- **Over/Under Billing:** Cumulative amount of underbilled (positive) or overbilled (negative) work

**Completion Metrics:**
- **% Complete (by Cost):** Progress measured as actual costs incurred divided by estimated total costs
- **% Complete (by Labor):** Progress measured by labor-specific metrics
- **Backlog:** Remaining work or revenue to be earned

**Billing and Retention:**
- **Invoiced Amount:** Total customer invoices issued
- **Amounts Paid:** Total payments received from the customer
- **Retention:** Any amounts withheld by the customer pending project completion

### Step 5: Analyze Financial Health

Review gross margin percentages to identify profitable and unprofitable projects. Projects with margins below your cost of capital or strategic targets may need intervention. Examine the over/under billing position to understand cash flow timing—positive values indicate you have earned more than billed, while negative values indicate overbilling.

### Step 6: Monitor Progress

Compare percent complete by cost versus labor to identify projects where one discipline is progressing faster than the other. This can indicate labor efficiency issues or cost structure problems.

### Step 7: Export or Print (Optional)

Use the export or print options to save the report in Excel, PDF, or hardcopy format for meetings, archives, or distribution.

## What Happens Next

After reviewing the Project WIP Report, you may:

- Investigate individual projects in detail by opening the project form
- Run the WIP Reconciliation Report (PROJ-RPT-005) if you need to verify GL account reconciliation
- Execute the Delta Report (PROJ-RPT-006) to compare this snapshot to a previous period
- Prepare financial statements or customer invoices based on the earned revenue data
- Initiate project reviews or change orders to address cost overruns

## Common Issues

**Gross margin is negative across multiple projects**

Negative margins indicate projects are operating at a loss. Verify that project pricing is set correctly and that all billable costs are being recorded. Check whether significant change orders have reduced scope or pricing without corresponding cost reductions. Consider whether you are capturing all billable time and materials.

**Percent Complete by Cost and Labor are very different**

When cost and labor completion percentages diverge significantly, it suggests one cost component (such as materials) is progressing faster or slower than labor. For example, if material costs are nearly complete but labor is only 30% done, it may indicate a supply delivery issue or scheduling problem. Investigate the underlying tasks and costs to understand the cause.

**The Over/Under Billing balance appears incorrect**

Verify that the project's invoicing schedule and revenue recognition settings are configured correctly. The over/under billing calculation depends on accurate earned revenue determination. If invoices have been manually adjusted or written off, those changes may not be reflected in the earned revenue calculation. Check the project's accounting history.

**Retention amounts seem too high or are zero across the board**

Check the customer contract to confirm retention terms. If contracts specify retention but the report shows zero, the project may not have been configured with retention terms. If retention appears high, verify that the percentage and conditions are accurate. Run individual project invoices to confirm the retention amounts applied.

**The report shows completed projects with outstanding balances**

Closed projects may still show WIP balances if final invoices have not been issued or if retainage is being held pending final inspection or punch-list completion. Contact the project manager to determine whether the balance represents uncollected revenue or a configuration issue.

