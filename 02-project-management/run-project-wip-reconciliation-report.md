---
title: Run the Project WIP Reconciliation Report
id: PROJ-RPT-005
module: Projects
screen: Project WIP Reconciliation Report
menu_path: Main Menu > Projects > Reports > Project WIP Reconciliation
applies_to:
  - Finance
  - Controller
prerequisites:
  - Access to the Projects module with financial reporting permissions
  - Accounting background and understanding of GL reconciliation
  - Knowledge of WIP account structures in the GL
related_procedures:
  - PROJ-RPT-004
  - PROJ-RPT-006
tags:
  - WIP reconciliation
  - GL reconciliation
  - general ledger
  - WIP balance
  - reconcile
  - project accounting
version: "1.0"
last_updated: "2026-03-25"
---

# Run the Project WIP Reconciliation Report

## What This Procedure Does

The Project WIP Reconciliation Report compares project WIP balances from the project subledger against the corresponding General Ledger (GL) account balances. This report helps finance and accounting teams identify and resolve discrepancies between the project accounting system and the GL, ensuring that financial records are accurate and auditable. Use this report as part of your month-end close process or whenever you suspect a GL reconciliation issue.

## Before You Begin

- Have access to the Projects module with GL reconciliation permissions
- Have access to the General Ledger module to reference account balances
- Know the "as of" date for which you are reconciling
- Identify the WIP GL accounts that should reconcile to project balances
- Ensure both project and GL transactions have been posted through the reconciliation date

## Steps

### Step 1: Navigate to the Project WIP Reconciliation Report

From the main menu, select **Projects > Reports > Project WIP Reconciliation**. The report screen displays with filter options.

### Step 2: Set Your Filters

Configure the filters to specify which entities and time period to reconcile:

| Field | What to enter |
|-------|---------------|
| Company | Select one or more companies to reconcile |
| Branch | Select one or more branches, or leave as ALL for all branches |
| As of Date | Enter the date through which to reconcile; defaults to today |

### Step 3: Click Run

Click the **Run** button to execute the reconciliation report.

### Step 4: Review the Report Output

The report displays a reconciliation grid comparing project and GL balances. Columns typically include:

- **Company/Branch:** The entity being reconciled
- **WIP Account Number:** The GL account used for WIP tracking
- **Project Subledger Balance:** Total WIP balance from the project accounting system
- **GL Account Balance:** Balance in the corresponding GL account
- **Variance:** The difference between project subledger and GL balance (Project balance minus GL balance)
- **Status:** Indicates whether the balance matches (Reconciled) or does not match (Out of Balance)

A summary row may appear at the bottom showing total variance across all accounts.

### Step 5: Identify Discrepancies

Review the Variance column to identify accounts that do not reconcile. Any non-zero variance indicates a potential issue requiring investigation. Accounts marked "Out of Balance" should be your priority.

### Step 6: Investigate Variances

For any discrepancy, determine the cause:

- **Timing Differences:** Check whether transactions were recorded in the project module but not yet posted to the GL (or vice versa). GL posting may lag project transaction recording.
- **Manual GL Adjustments:** Verify whether the GL account has been adjusted manually (through journal entries) without corresponding project adjustments.
- **Project Adjustments:** Confirm whether project balances have been adjusted (through write-offs, reversals, or corrections) that may not have corresponding GL entries.
- **Missing Transactions:** Check whether all project costs and invoices have been recorded and properly allocated to WIP accounts.

### Step 7: Resolve Discrepancies

Once you have identified the cause, take appropriate action:

- If the variance is due to timing, rerun the report after all GL transactions have posted
- If a manual GL adjustment was made, create a corresponding project adjustment to match
- If project transactions are missing, record them and rerun the reconciliation
- If a legitimate difference exists, document the variance and its cause for audit purposes

### Step 8: Export or Print the Report

Save the reconciliation report as Excel, PDF, or hardcopy for your audit file and financial records.

## What Happens Next

After completing the WIP reconciliation, you may:

- Prepare a reconciliation summary for your accounting team or auditors
- Adjust project or GL balances as needed to achieve reconciliation
- Document any known variances and their causes in your audit workpapers
- Proceed with month-end close procedures and financial statement preparation
- Investigate systematic reconciliation issues that may indicate configuration or process problems

## Common Issues

**The reconciliation shows a large variance**

A significant variance suggests either a systematic issue or a large transaction has not been recorded in one of the two systems. Verify that the report is using the correct WIP GL accounts and that all project transactions through the reconciliation date have been posted to the GL. Check whether a large invoice, change order, or cost adjustment was recorded in one system but not the other.

**Only some company/branch combinations show variances**

If reconciliation issues are isolated to specific entities, check whether those projects have unique accounting or posting configurations. Verify whether those branches or companies use different WIP accounts or revenue recognition methods that might cause timing or classification differences.

**The project balance is higher than the GL balance**

This indicates the project system recognizes more WIP than the GL currently shows. Check whether project transactions (invoices or costs) have been recorded but GL posting has not yet occurred. Alternatively, a project adjustment or write-off may have been applied in the GL without corresponding project adjustment.

**The GL balance is higher than the project balance**

The opposite situation—GL balance exceeding the project balance—suggests GL transactions that the project system does not reflect. Check for manual GL journal entries or GL transactions from external sources (such as consolidation or automated posting) that may not be recorded in projects.

**I cannot identify which GL account corresponds to a project**

Verify the GL account mapping in your project configuration. WIP accounts must be properly assigned at the project or company level. Check with your accounting manager or system administrator to confirm which GL accounts are designated for WIP tracking.

**The variance is small and appears to be rounding differences**

Small variances (typically under 1 dollar or cent) may be the result of rounding in calculations. Determine whether your reconciliation policy tolerates small rounding differences or requires exact matching. Document any approved rounding tolerance in your financial procedures.
