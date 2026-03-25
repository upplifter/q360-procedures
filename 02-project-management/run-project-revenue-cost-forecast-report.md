---
title: Run the Project Revenue/Cost Forecast Report
id: PROJ-RPT-012
module: Projects
screen: Project Revenue/Cost Forecast Report
menu_path: Main Menu > Projects > Reports > Project Revenue/Cost Forecast
applies_to:
  - Finance
  - Operations Manager
  - Project Manager
prerequisites:
  - Access to the Projects module with forecasting permissions
  - Understanding of project invoicing milestones and schedules
  - Current project task schedules and revenue recognition settings
related_procedures:
  - PROJ-RPT-013
  - PROJ-RPT-014
  - PROJ-RPT-015
tags:
  - revenue forecast
  - cost forecast
  - project forecast
  - revenue projection
  - cost projection
  - financial forecast
  - project financials
version: "1.0"
last_updated: "2026-03-25"
---

# Run the Project Revenue/Cost Forecast Report

## What This Procedure Does

The Project Revenue/Cost Forecast Report projects expected project revenue and cost over upcoming periods based on task schedules and invoicing milestones. It breaks down projected revenue and cost into future time periods (typically weeks or months), providing a forward-looking view of expected financial performance. Use this report for cash flow planning, revenue recognition forecasting, and identifying timing mismatches between cost incurrence and revenue realization.

## Before You Begin

- Have access to the Projects module with forecasting and reporting permissions
- Know the forecast start date and duration you want to analyze
- Identify any filters you need (company, branch, project type, project manager)
- Ensure project schedules are current and invoicing milestones are configured

## Steps

### Step 1: Navigate to the Project Revenue/Cost Forecast Report

From the main menu, select **Projects > Reports > Project Revenue/Cost Forecast**. The report screen displays with filter and date options.

### Step 2: Set Your Filters

Configure the filters to specify which projects and time period to forecast:

| Field | What to enter |
|-------|---------------|
| Company | Select one or more companies, or leave blank for all |
| Branch | Select one or more branches, or leave as ALL for all branches |
| Project Type | Select one or more project types, or leave as ALL for all types |
| Project Manager | Select one or more project managers, or leave as ALL |
| Forecast Start Date | Enter the date when the forecast should begin (typically today or the next period) |

### Step 3: Click Run

Click the **Run** button to execute the forecast.

### Step 4: Review the Report Output

The report displays a grid with revenue and cost projections across future time periods. The structure typically includes:

- **Project Name/ID:** Each active project in the forecast
- **Period Columns:** Future time periods starting from the Forecast Start Date
  - Each period shows:
    - **Projected Revenue:** Revenue expected to be earned in that period based on invoicing milestones and revenue recognition method
    - **Projected Cost:** Costs expected to be incurred in that period based on the task schedule

The report may also include:
- A totals row summing revenue and cost across all projects for each period
- A summary showing total forecasted revenue minus total forecasted cost (GP) by period
- Period start and end dates for clarity

### Step 5: Analyze Revenue and Cost Timing

Review the period columns to understand cash flow and profitability timing:

- **Periods with High Revenue/Low Cost:** Favorable periods where revenue is earned with lower cost burden
- **Periods with High Cost/Low Revenue:** Periods where significant costs are incurred but revenue has not yet been earned or recognized (potential cash flow strain)
- **Timing Mismatches:** Situations where costs are front-loaded but revenue is back-loaded, or vice versa

### Step 6: Assess Profitability by Period

For each period, compare total revenue to total cost:

- **Positive Spread (Revenue > Cost):** Periods with favorable profitability
- **Negative Spread (Cost > Revenue):** Periods where profitability may be constrained by cost incurrence preceding revenue recognition
- **Break-even Periods:** Periods where revenue and cost are balanced

### Step 7: Identify Peak Periods

Look for periods with exceptionally high or low activity:

- **High-Revenue Periods:** When major invoicing milestones are scheduled (e.g., major completion phases)
- **High-Cost Periods:** When significant material purchases or labor effort is concentrated
- **Cash Constraints:** Periods where cost precedes revenue, potentially straining project cash flow

### Step 8: Export or Print (Optional)

Use the export or print functions to save the forecast as Excel, PDF, or hardcopy for financial planning, management meetings, and cash flow analysis.

## What Happens Next

After reviewing the Project Revenue/Cost Forecast Report, you may:

- Adjust project schedules or invoicing milestones to improve cash flow timing
- Plan working capital or short-term financing to cover periods with negative cash flow
- Brief management on forecasted revenue and profitability by period
- Use the forecast to inform corporate financial projections and guidance
- Identify opportunities to accelerate revenue or defer costs to improve period profitability

## Common Issues

**The forecast shows no data or very low revenue/cost**

Verify that projects have task schedules with estimated costs and that invoicing milestones are configured. Projects in early planning phases without detailed schedules may show minimal forecasted activity. Confirm that milestones have estimated revenue amounts assigned.

**Revenue and cost appear unbalanced across periods**

This is normal when invoicing milestones are not evenly distributed or when cost is front-loaded (typical for projects with significant upfront material or labor). Use this insight to plan cash flow and discuss with project managers whether milestone timing can be adjusted.

**The forecast shows zero cost or revenue for an active project**

Verify that the project has been configured with task schedules and cost estimates. If the project lacks detailed planning, cost and revenue will not forecast. Work with the project manager to add schedule details and milestone information.

**Forecast periods are too long or too short**

Forecast period granularity (weekly vs. monthly) is typically determined by system configuration. If you need different period groupings, consult with your system administrator. Alternatively, export the data and regroup in Excel or your financial system to match your reporting needs.

**I need to understand which specific tasks drive the revenue/cost in each period**

The summary forecast shows period totals by project. For task-level detail, you may need to open individual projects and review their schedules, or run detailed task-level cost and revenue reports. The forecast report is designed for period-level planning rather than task-level drill-down.

**Revenue forecast doesn't match my invoicing plan**

Verify that invoicing milestones are configured in each project and that milestone dates and revenue amounts are accurate. Also confirm that your revenue recognition method is correctly configured—some methods recognize revenue by milestone, while others recognize by earned value or other criteria. Check with your finance team to confirm the correct recognition method.
