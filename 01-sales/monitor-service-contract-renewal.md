---
title: Monitor Service Contracts for Renewal
id: SALES-RENEWAL-001
module: Sales
screen: Service Overview Workflow
menu_path: Workflow > Service Overview > Expiring Service Contracts bucket
applies_to:
  - Sales Rep
  - Service Manager
prerequisites:
  - Access to the Service Overview workflow
  - SERVICECONTRACT (Edit) permission assigned to your user or group
  - OPPORTUNITY (Create) permission to create renewal opportunities
related_procedures:
  - SALES-RENEWAL-002
  - SALES-OPP-001
  - SALES-QUOTE-001
tags: service contract, renewal, expiring contract, pending renewal, service overview, contract expiration, renew contract, monitor contracts
version: 1.0
last_updated: 2026-03-25
---

# Monitor Service Contracts for Renewal

## What This Procedure Does

Reviews expiring service contracts from the Service Overview workflow and initiates the renewal process. When a contract requires customer approval for renewal, the status is changed to PENDING-RENEWAL and a new opportunity is created to track the renewal through the standard quote-to-order cycle.

## Before You Begin

- You have access to the Service Overview workflow.
- You have SERVICECONTRACT (Edit) permission.
- You have OPPORTUNITY (Create) permission to create renewal opportunities.

## Steps

### Step 1: Open the Service Overview Workflow

Navigate to **Workflow > Service Overview**. The workflow canvas displays with service-related buckets.

### Step 2: Open the Expiring Service Contracts Bucket

Click the **Expiring Service Contracts** bucket. A grid opens listing service contracts approaching their expiration date. Set report filters (date range, branch, customer) as needed.

### Step 3: Review Expiring Contracts

Review the list to identify contracts that need renewal action. Note the contract end date, customer, and contract value for each.

### Step 4: Set Contract to Pending Renewal

1. Drill into the service contract that requires renewal.
2. Click the **Edit Record** button (pencil icon).
3. Change the **Status** to **PENDING-RENEWAL**.
4. Click the **Save Record** button (floppy disk icon).

### Step 5: Create a Renewal Opportunity

1. From the Service Contract form, drill into the customer by clicking the blue hyperlink next to the **Bill To** customer name. The Customer form opens.
2. Create a new sales opportunity on the customer's **Sales Opps** tab (see SALES-OPP-001). Title it to indicate it is a renewal (e.g., "Service Contract Renewal - [Site Name]").
3. Set the opportunity value, close date, and other fields as appropriate for the renewal.

### Step 6: Create and Process the Renewal Quote

From the new opportunity, create a quote (see SALES-QUOTE-001), authorize it (see SALES-QUOTE-003), and submit it to the customer (see SALES-QUOTE-004). Once the customer approves, mark the quote as approved (see SALES-QUOTE-006) and approve the resulting order (see SALES-ORDER-001).

## What Happens Next

The renewal quote flows through the standard sales cycle. Once the order is approved, a new service contract is created. The original contract remains in PENDING-RENEWAL status until its term expires, at which point it should be set to RENEWED.

For a streamlined alternative that auto-creates the opportunity and quote from the service contract, see SALES-RENEWAL-002.

## Common Issues

**The Expiring Service Contracts bucket is empty.**
Adjust the workflow filters for date range and branch. The bucket may be filtered to show only contracts expiring within a specific window.

**You cannot change the status to PENDING-RENEWAL.**
Verify you have SERVICECONTRACT (Edit) permission. Some contract statuses may restrict transitions depending on configuration.

**The renewal opportunity does not link back to the service contract.**
When creating the opportunity manually, there is no automatic link to the service contract. Use the opportunity title and comments to reference the contract number for traceability.

**The customer declines the renewal.**
If the customer declines, set the opportunity Won/Lost Code to LOST. When the contract term expires, change the service contract status to EXPIRED instead of RENEWED.

**You need to renew without customer approval (auto-renew).**
If the contract auto-renews and does not require a quote cycle, your process may differ. Contact your administrator for auto-renewal workflows specific to your organization.
