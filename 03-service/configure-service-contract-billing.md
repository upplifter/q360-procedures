---
title: Configure Service Contract Billing
id: SVC-CONTRACT-002c
module: Service
screen: Service Contract > Billing
menu_path: Service Contract > Billing Tab
applies_to: Service Managers, Finance Managers, Contract Administrators
prerequisites:
  - Service contract header must be created
  - Service contract line items must be added
  - Line item prices must be entered
related_procedures:
  - SVC-CONTRACT-002a
  - SVC-CONTRACT-002b
tags:
  - billing
  - recurring
  - deferred revenue
  - configuration
version: 1.0
last_updated: 2026-03-25
---

# Configure Service Contract Billing

## What This Procedure Does

Sets up billing methods, frequency, and amounts for a service contract. This determines how often the customer is invoiced and how revenue is recognized. Billing configuration applies to the entire contract and its line items.

## Before You Begin

- Service contract header must be created with Start Date and End Date
- All service contract line items must be added with pricing
- You must know the desired billing frequency (monthly, quarterly, annual)
- You must know the billing method (Recurring, Block Amount, T&M)
- For deferred revenue tracking, your chart of accounts must have a Block Amount Suspense account configured

## Steps

### Step 1: Open the Contract and Navigate to Billing

Open the service contract from Service > Service Contracts. Click the Billing tab to display billing configuration options.

### Step 2: Select Billing Frequency

Set the Billing Frequency field to one of the following:

| Field | What to enter |
|-------|---------------|
| Billing Frequency | Monthly, Quarterly, or Annual |

Choose the interval at which the customer will be invoiced for service.

### Step 3: Select Billing Method

Set the Billing Method field based on your service contract type:

| Field | What to enter |
|-------|---------------|
| Billing Method | Recurring (fixed amount per period), Block Amount (prepaid pool), or T&M (time and materials) |

For recurring and block amount contracts, enter the Bill Amount. For T&M contracts, billing will be calculated based on actual service usage.

### Step 4: Configure Billing Cycle and Amount

Enter the following billing parameters:

| Field | What to enter |
|-------|---------------|
| Bill Amount | The total invoice amount per billing cycle (for Recurring billing) |
| Billing Cycle Day | The day of the month on which invoices are generated (defaults to SCBILLDATE config if set) |
| Block Amount | Total prepaid amount (for Block Amount contracts only) |
| Block Amount Master | The M-type product number representing the prepaid block (for Block Amount contracts) |

### Step 5: Configure Deferred Revenue

If your organization uses deferred revenue accounting, configure the following:

| Field | What to enter |
|-------|---------------|
| Deferred Revenue Account | Account number for recognizing service revenue ratably over the contract period |
| Recognition Method | Straight-line or other method (based on system config) |

### Step 6: Review Proration Settings

The system will automatically apply proration when line items are added mid-billing-cycle. Review the Proration section to understand how billing amounts will be adjusted for partial periods. No action is required here unless you need to disable proration.

### Step 7: Save Billing Configuration

Click the Save button (floppy disk icon) to apply all billing settings. The system validates the configuration and saves it to the contract.

## What Happens Next

Billing configuration is applied to the contract. When invoices are generated, they use the frequency, method, and amount settings defined here. For recurring contracts, invoices are generated automatically on the Billing Cycle Day. For block amount contracts, the prepaid balance is tracked and decremented as service calls are consumed. For T&M contracts, invoices are created based on actual service hours and materials used. Deferred revenue is recognized according to the configured method and schedule.

## Common Issues

**Billing Cycle Day is set but invoices generate on wrong date**

The Billing Cycle Day is the preferred day for invoice generation. If the system generates invoices on a different date, check the SCBILLDATE configuration setting in your system. Some systems use the configuration default if no Billing Cycle Day is entered on the contract. Verify your config setting matches the desired billing date.

**Block Amount contract requires Master No but field is empty**

For block amount contracts, the Block Amount Master field must reference an M-type product with the Warr/Def Rev flag checked. Ensure the product is configured correctly in the Product Master module, then return to the Billing tab and enter the Master No. The Block Amount account must also be mapped to a Balance Sheet account for the prepaid balance to be tracked correctly.

**Proration is reducing my bill amount unexpectedly**

Proration applies automatically when line items have different dates than the contract header or when items are added mid-cycle. If line items were added after the contract Start Date or have earlier end dates than the header, the system calculates pro-rata amounts. To avoid proration, ensure Sync Dates is checked on all line items to match the header dates exactly.

**Deferred revenue is not being recognized**

Deferred revenue recognition requires that the Deferred Revenue Account is populated with a valid G/L account. The Block Amount Suspense account (for block amount contracts) must also be configured. If revenue is not recognized, verify that the account mappings are set up correctly in your chart of accounts and that the Deferred Revenue Account field on the Billing tab is filled in.
