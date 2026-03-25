---
title: Renew Service Contract Through Quote
id: SALES-RENEWAL-002
module: Sales
screen: Service Contract Form
menu_path: Main Menu > Service > Service Contract > Extended Menu
applies_to:
  - Sales Rep
  - Service Manager
prerequisites:
  - SERVICECONTRACT (Edit) permission assigned to your user or group
  - OPPORTUNITY (Create) and QUOTE (Create) permissions
  - The service contract exists and is approaching expiration
related_procedures:
  - SALES-RENEWAL-001
  - SALES-QUOTE-001
  - SALES-QUOTE-003
  - SALES-QUOTE-004
  - SALES-QUOTE-006
  - SALES-ORDER-001
tags: renew contract, service contract renewal, create renewal quote, renewal opportunity, contract renewal workflow, service contract quote
version: 1.0
last_updated: 2026-03-25
---

# Renew Service Contract Through Quote

## What This Procedure Does

Creates a renewal quote directly from an expiring service contract using the extended menu. Q360 can automatically create both a renewal opportunity and a pre-populated quote with line items and prices carried over from the existing contract. The renewal then follows the standard quote-to-order cycle, resulting in a new service contract.

## Before You Begin

- You have SERVICECONTRACT (Edit), OPPORTUNITY (Create), and QUOTE (Create) permissions.
- The service contract exists and is approaching or past its expiration date.
- You have reviewed the existing contract terms, line items, and pricing.

## Steps

### Step 1: Open the Service Contract

Navigate to **Main Menu > Service > Service Contract**. Search for and open the service contract to be renewed.

### Step 2: Create the Renewal Quote

1. Click the service contract form **Extended Menu** (three vertical dots).
2. Select **Create Renewal Quote**.
3. In the prompt, choose whether to create an opportunity and/or a quote. Creating both is recommended.
4. Click **OK**. Q360 creates the records pre-populated with data from the existing service contract.

### Step 3: Update the Renewal Opportunity

Open the newly created renewal opportunity. Update the following as needed:

- Value, close date, and probability per standard opportunity procedures (see SALES-OPP-002).
- Title to clearly indicate it is a renewal.

### Step 4: Update the Renewal Quote

Open the renewal quote (created with line items and prices from the existing contract). Review and adjust as needed:

- Update pricing if rates have changed.
- Add or remove line items to reflect the new contract scope.
- Follow standard quote procedures for any modifications (see SALES-QUOTE-001).

### Step 5: Process the Quote Through the Sales Cycle

1. Confirm the quote (see SALES-QUOTE-001, Step 7).
2. Authorize the quote (see SALES-QUOTE-003).
3. Submit the quote to the customer (see SALES-QUOTE-004).
4. Once the customer approves, mark the quote as approved (see SALES-QUOTE-006).
5. Approve the resulting order (see SALES-ORDER-001). This creates a new service contract.

### Step 6: Manage the Outgoing Service Contract

1. Until the outgoing contract's term expires, keep its status in **PENDING-RENEWED**.
2. Once the contract term is up, change its status to **RENEWED**.

You can monitor the outgoing contract from the **Service Contract Renewal Q**.

## What Happens Next

A new service contract is created from the approved renewal order. The new contract begins where the old one ends, maintaining continuity of service coverage. The outgoing contract retains its full history for billing and reporting purposes.

This approach is recommended over extending the current contract, as it preserves the billing and service history of the original contract while starting fresh on the renewal.

## Common Issues

**The Create Renewal Quote option is not in the extended menu.**
Verify you have the correct permissions and that the service contract is in an eligible status. Some configurations restrict this action to specific contract statuses.

**The renewal quote has incorrect pricing.**
The quote inherits pricing from the existing contract. If rates need updating, edit the quote line items and adjust unit cost and unit price before confirming.

**The new service contract does not link to the original.**
Q360 creates the renewal as a separate contract. Use the contract title, comments, or a custom field to reference the original contract number for traceability.

**You are unsure whether to extend the existing contract or create a new one.**
Creating a new contract from a renewal order is the recommended practice. It maintains clean billing history on the original contract and allows independent tracking of the renewal period.

**The outgoing contract's status options do not include PENDING-RENEWED or RENEWED.**
These statuses are controlled by the service contract status general code. Contact your administrator to verify these values exist in your configuration.
