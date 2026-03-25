---
title: Run the Block Amount Detail Report
id: SVC-RPT-018
module: Service
screen: Block Amount Detail Report
menu_path: Service > Reports > Block Amount Detail
applies_to: Service Managers, Accounting Managers, Customer Service Staff
prerequisites:
  - Access to Service Reports
  - Permission to view block amount transaction data
  - Service contracts with block amounts must exist
related_procedures:
  - SVC-RPT-017
  - SVC-RPT-019
tags:
  - Reports
  - Block Amounts
  - Transactions
  - Detailed Tracking
version: 1.0
last_updated: 2026-03-25
---

# Run the Block Amount Detail Report

## What This Procedure Does

The Block Amount Detail Report shows individual block amount transactions per contract including beginning balance, purchases, usage, and ending balance. Use this report to audit block transactions, verify accuracy, and investigate balance discrepancies.

## Before You Begin

- Have permission to access Service Reports
- Identify the contract or customer to analyze
- Determine the date range for analysis
- Understand the units of measurement (hours, credits, dollars)

## Steps

### Step 1: Open Block Amount Detail Report

Go to Service > Reports > Block Amount Detail. The Print Report dialog opens with filter options.

### Step 2: Set Filter Criteria

Configure filters to define the analysis:

| Field | What to select |
|-------|----------------|
| Company | Select the company |
| Contract No | Enter contract number (optional) |
| Date Range | Enter start and end dates |

### Step 3: Run the Report

Click Run Report. The report generates and displays in Print Report dialog or Live Data grid.

### Step 4: Review Block Amount Transactions

The report displays per contract and transaction:

- Contract No
- Customer Name
- Transaction Date
- Transaction Type (Purchase, Usage, Adjustment, Expiration)
- Beginning Balance
- Transaction Amount (+ for purchases, - for usage)
- Ending Balance
- Reference (Call No if usage, PO No if purchase)
- Notes (reason for transaction)

Transactions are listed chronologically showing the running balance history.

### Step 5: Verify Transaction Accuracy

Review each transaction for accuracy. Verify purchases match invoices or contracts. Confirm usage matches actual service calls. Investigate unusual adjustments or discrepancies.

## What Happens Next

Results provide audit trail for block amount management. Use the report to verify customer-reported balances, investigate disputes, and explain balance changes. Track transactions to ensure prepaid amounts are correctly consumed and managed.

## Common Issues

**Missing Transactions**
Verify the date range is wide enough to capture all activity. Check that the contract number is correct. Ensure all block transactions are posted in the system.

**Balance Does Not Match Customer Statement**
Compare report ending balance to contract balance field. Verify the end date in the report. Check if any manual adjustments were made to block amounts.

**Cannot Find Usage Transactions**
Verify service calls are posting block amount usage. Check that calls are linked to the correct contract. Ensure time bills or parts are configured to consume block amounts.
