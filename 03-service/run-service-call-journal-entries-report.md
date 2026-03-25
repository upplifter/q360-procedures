---
title: Run the Service Call Journal Entries Report
id: SVC-RPT-021
module: Service
screen: Service Call Journal Entries Report
menu_path: Service > Reports > Service Call Journal Entries
applies_to: Service Managers, Accounting Managers, Finance Staff
prerequisites:
  - Access to Service Reports or Accounting Reports
  - Permission to view general ledger data
  - Service calls must have posted entries
related_procedures:
  - SVC-RPT-013
tags:
  - Reports
  - Journal Entries
  - General Ledger
  - Accounting Integration
version: 1.0
last_updated: 2026-03-25
---

# Run the Service Call Journal Entries Report

## What This Procedure Does

The Service Call Journal Entries Report lists all general ledger entries linked to a specific service call. This report is used to reconcile service call financials with accounting records, verify proper posting, and support audit requirements.

## Before You Begin

- Have permission to access Service or Accounting Reports
- Identify the service call to analyze
- Determine the date range if searching multiple calls
- Understand your chart of accounts and account categories

## Steps

### Step 1: Open Service Call Journal Entries Report

Go to Service > Reports > Service Call Journal Entries (or Accounting > Reports). The Print Report dialog opens with filter options.

### Step 2: Set Filter Criteria

Configure filters to identify the call(s) to report on:

| Field | What to enter |
|-------|---------------|
| Company | Select the company |
| Call No | Enter the service call number |
| Date Range | Enter transaction date range |

### Step 3: Run the Report

Click Run Report. The report generates and displays in Print Report dialog or Live Data grid.

### Step 4: Review Journal Entries

The report displays all GL entries linked to the call:

- Entry No (GL Entry ID)
- Transaction Date
- Account Number
- Account Name
- Master No (cost center, department, etc.)
- Amount (debit or credit)
- Description/Comments
- Reference (call number, invoice, PO)
- Posted Date

Entries are listed chronologically or by account number.

### Step 5: Reconcile and Verify Entries

Verify all expected revenue and cost entries appear. Check that debit and credit amounts balance. Confirm amounts match related time bills, parts, or charges. Use comments to understand the posting rationale.

## What Happens Next

Results support financial reporting and audit requirements. Use the report to verify service call profitability calculations. Investigate any unexpected entries or amounts. Support customer inquiries about billing by providing GL detail. Maintain records for external audit.

## Common Issues

**No Entries Displayed**
Verify the call number is correct. Check that time bills, parts, or charges have been posted to the call. Ensure the date range includes the posting period. Confirm the call status allows GL posting.

**Entry Amounts Do Not Match Expected Values**
Compare entries to original time bills and parts invoices. Check for posted adjustments or credits. Verify no duplicate postings occurred. Consult with accounting on calculation methodology.

**Missing Entries**
Confirm all time bills and parts for the call have been posted. Check if any entries are on hold pending approval. Verify the general ledger is not filtered to exclude certain account types.
