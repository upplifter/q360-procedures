---
title: Run the Service Contract List Report
id: SVC-RPT-004
module: Service
screen: Service Contract List Report
menu_path: Service > Reports > Service Contract List
applies_to: Service Managers, Accounting Managers, Sales Staff
prerequisites:
  - Access to Service Reports
  - Permission to view service contract data
  - Service contracts must exist in the system
related_procedures:
  - SVC-RPT-013
  - SVC-RPT-014
tags:
  - Reports
  - Service Contracts
  - Contract Management
version: 1.0
last_updated: 2026-03-25
---

# Run the Service Contract List Report

## What This Procedure Does

The Service Contract List Report provides a comprehensive listing of all service contracts in the system with key contract details. Use this report for contract management, renewal tracking, and customer account reviews.

## Before You Begin

- Have permission to access Service Reports
- Determine the status and customer filters needed
- Identify the date range or contract scope

## Steps

### Step 1: Open Service Contract List Report

Go to Service > Reports > Service Contract List. The Print Report dialog opens with filter options.

### Step 2: Set Filter Criteria

Configure filters to define report scope:

| Field | What to select |
|-------|----------------|
| Company | Select the company |
| Branch | Select the branch (optional) |
| Department | Select the department (optional) |
| Contract Status | Select status (Active, Inactive, Expired, etc.) |
| Customer | Select customer (optional) |

### Step 3: Run the Report

Click Run Report. The report generates and displays in Print Report dialog or Live Data grid.

### Step 4: Review Contract Information

The report displays:

- Contract No
- Customer name
- Site location
- Contract Type
- Contract Status
- Start Date
- End Date
- Billing Terms
- Service hours profile (if assigned)
- Service rates profile (if assigned)

### Step 5: Analyze and Export Results

Review the contract list for upcoming renewals, expired contracts, or inactive accounts. Export to Excel for further analysis or customer contact lists. Use the report for contract renewal campaigns or account reviews.

## What Happens Next

The report shows current contract status as configured in the system. Active contracts are highlighted. Expired or inactive contracts are clearly marked. Use this report for renewal planning, compliance verification, and customer account management. Combine with other contract reports for comprehensive contract analysis.

## Common Issues

**No Results Displayed**
Verify the contract status filter includes the contracts you're searching for. Check that the company and branch filters are correct. Ensure contracts exist and are not deleted.

**Missing Contracts**
Expand the contract status filter to include more statuses (e.g., include Inactive if searching only for Active). Verify the customer filter is not too restrictive. Check date range if filtering by contract dates.

**Contract Details Incomplete**
Confirm all contract header information was entered during contract creation. Verify the Service Hours and Service Rates profiles are assigned. Some fields may be optional and not required.
