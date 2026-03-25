---
title: Run the Block Amount Summary Report
id: SVC-RPT-017
module: Service
screen: Block Amount Summary Report
menu_path: Service > Reports > Block Amount Summary
applies_to: Service Managers, Accounting Managers, Customer Service Staff
prerequisites:
  - Access to Service Reports
  - Permission to view block amount data
  - Service contracts with block amounts must exist
related_procedures:
  - SVC-RPT-018
  - SVC-RPT-019
tags:
  - Reports
  - Block Amounts
  - Prepaid Hours
  - Balance Tracking
version: 1.0
last_updated: 2026-03-25
---

# Run the Block Amount Summary Report

## What This Procedure Does

The Block Amount Summary Report shows aggregated block amounts sold versus used per contract with remaining balance. Block amounts are prepaid service hours or value on service contracts. Use this report to monitor prepaid balance inventory and identify at-risk balances.

## Before You Begin

- Have permission to access Service Reports
- Determine the end date for the balance snapshot
- Identify company and branch scope
- Understand your block amount units (hours, credits, dollars)

## Steps

### Step 1: Open Block Amount Summary Report

Go to Service > Reports > Block Amount Summary. The Print Report dialog opens with filter options.

### Step 2: Set Filter Criteria

Configure filters to define the analysis:

| Field | What to select |
|-------|----------------|
| Company | Select the company |
| Branch | Select the branch (optional) |
| End Date | Enter the date for balance snapshot |

### Step 3: Run the Report

Click Run Report. The report generates and displays in Print Report dialog or Live Data grid.

### Step 4: Review Block Amount Summary

The report displays per contract:

- Contract No
- Customer Name
- Block Amount Sold (total prepaid units)
- Block Amount Used (consumed to date)
- Remaining Balance
- Usage Percentage (%)
- Expiration Date (if applicable)

Rows are sorted by remaining balance. Summary totals show company-wide or branch-wide prepaid amounts.

### Step 5: Drill Into Detail

Click a contract row to drill down to the Block Amount Detail report (SVC-RPT-018) to see individual block amount transactions.

## What Happens Next

Results help monitor prepaid balance inventory and identify customers with low remaining balances. Use the report for customer communications about balance status or renewal. Monitor balances nearing zero to plan replenishment or contract renegotiation.

## Common Issues

**No Block Amounts Displayed**
Verify block amounts are configured on service contracts. Check that contracts have active block amount items. Ensure the company and branch filters are correct.

**Balance Appears Incorrect**
Verify the end date is correct. Check that all block amount transactions (purchases, usage) are properly recorded. Ensure usage postings are complete.

**Cannot Identify Which Customers Need Balance Renewals**
Review the Remaining Balance column. Contact customers with low or expiring balances. Filter the report by balance threshold to identify at-risk customers.
