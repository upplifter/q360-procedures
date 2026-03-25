---
title: Top Up a Block Amount Service Contract
id: SVC-CONTRACT-009
module: Service
screen: Service Contract > Billing
menu_path: Service Contract > Billing Tab
applies_to: Service Managers, Finance Managers, Sales Representatives
prerequisites:
  - Block amount service contract must exist
  - Contract must have a block amount master item (M-type product) assigned
  - Config BLOCKAMOUNTMASTERNO must be set to the M-type product number
  - Block Amount Suspense account must be configured in the chart of accounts
related_procedures:
  - SVC-CONTRACT-002c
  - SVC-CONTRACT-003
tags:
  - block amount
  - contract billing
  - prepaid funds
version: 1.0
last_updated: 2026-03-25
---

# Top Up a Block Amount Service Contract

## What This Procedure Does

Adds additional prepaid funds to an existing block amount service contract. When a customer's prepaid block balance depletes through service calls, create a new quote using the block amount master item to replenish the balance.

## Before You Begin

- Contract must be a Block Amount contract type (configured on header)
- Contract must have a block amount master item (M-type product) with Warr/Def Rev flag checked
- Contract line items must be consuming block balance (service calls must be linked to contract)
- Config BLOCKAMOUNTMASTERNO must be set to the M-type master product number
- Block Amount Suspense account must be configured in chart of accounts

## Steps

### Step 1: Check Current Block Balance

Open the block amount service contract from Service > Service Contracts. Navigate to the Billing tab. Review the Block Balance field to see the remaining prepaid amount. The block balance decreases as service calls are performed and consumed against the prepaid pool.

### Step 2: Create a Sales Quote

If the block balance is low or depleted, create a new sales quote to replenish it. Navigate to Sales > Quotes > Add to create a new quote.

### Step 3: Populate Quote Header

Fill in the quote header with the customer information:

| Field | What to enter |
|-------|---------------|
| Customer | Select the customer for the block amount contract |
| Site | Select the site matching the service contract |
| Quote Date | Today's date |
| Quote Notes | Reference the service contract number and indicate this is a block amount top-up |

### Step 4: Add Block Amount Master Item to Quote

Click Add in the quote Line Items grid. Add the block amount master product:

| Field | What to enter |
|-------|---------------|
| Product | Select the M-type master product (referenced in config BLOCKAMOUNTMASTERNO) |
| Quantity | 1 (master items use quantity 1) |
| Unit Price | Enter the prepaid block amount (e.g., $5,000, $10,000) |
| Description | "Block Amount Top-Up - [Contract Number]" |

### Step 5: Verify Service Revenue Account

On the quote line item, verify that the Service Revenue account or Block Amount Suspense account is mapped correctly. The account mapping ensures the prepaid amount is recognized properly in the balance sheet and deferred revenue accounts.

### Step 6: Save and Process Quote

Click Save to save the quote. Then process the quote to a sales order by clicking Process Actions (gear icon) > Convert to Order. The system creates a sales order from the quote.

### Step 7: Approve the Sales Order

Navigate to the created sales order from Purchasing > Orders or through the Sales workflow. Review the order for accuracy. Click Approve to approve the order.

### Step 8: Link Order to Service Contract

After the order is approved, link it to the service contract. On the service contract Billing tab, set the Block Amount Order or Link field to reference the new order, or the system may automatically link orders containing the block amount master item to existing contracts.

### Step 9: Record Receipt and Invoice

Once the order is approved, proceed with normal purchasing workflow:

- Receive the goods (even though this is a service/prepaid item, the system may require a goods receipt)
- Invoice the customer for the prepaid block amount

The invoice posts to the Block Amount Suspense account as a deferred revenue liability.

### Step 10: Verify Block Balance Update

Return to the service contract Billing tab. Verify that the Block Balance has increased by the new prepaid amount. The balance is now available for consumption by future service calls.

## What Happens Next

The prepaid block balance increases by the amount of the new order. As future service calls are created and invoiced against the contract, the system decrements the block balance. The Block Amount Suspense account tracks the remaining prepaid liability. When the block balance reaches zero, another top-up is required. You can set up recurring block amount top-ups by creating a recurring purchase order for the master item if your contract requires periodic replenishment on a fixed schedule.

## Common Issues

**Block balance does not increase after order is approved**

The balance update may lag behind order approval. Click the Refresh button (circular arrow) on the contract form to reload the current balance from the database. If the balance still does not update, verify:

- The order contains the M-type master product with the correct unit price
- The order was approved and invoiced (not just in draft status)
- Config BLOCKAMOUNTMASTERNO is set to the correct M-type product number
- The Block Amount Suspense account is configured in the chart of accounts

**Config BLOCKAMOUNTMASTERNO is not set or is incorrect**

This configuration must be set for the system to recognize block amount master products. Contact your system administrator to verify the configuration setting and set it to the correct M-type product number. Once configured, restart any background services and re-process the order.

**Service Revenue account or Block Amount Suspense account is not mapped**

For the prepaid amount to be recognized correctly, the Service Revenue account must map to the Block Amount Suspense balance sheet account. Verify the account mapping in your chart of accounts configuration. If mapping is missing, add it and re-invoice the order to correct the posting.

**Block balance is consumed faster than expected**

Service calls are consuming the prepaid block faster than anticipated. Review the service call rates and determine if:

- The service rate per call is correct
- Calls are being allocated to the correct contract
- The block amount top-up quantity was appropriate for the contract term

You may need to increase the top-up amount or adjust service rates to maintain adequate block balance.
