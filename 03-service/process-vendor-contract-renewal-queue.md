---
title: Process the Vendor Service Contract Renewal Queue
id: SVC-VENDOR-CONTRACT-001
module: Service
screen: Vendor Contract Renewal Queue
menu_path: Service > Work Queues > Vendor Contract Renewal Queue
applies_to: Service Managers, Operations Managers, Contract Administrators
prerequisites:
  - Service module access
  - Vendor service contracts are set up and linked to customer contracts
  - Authority to renew or modify service contracts
  - Customer service agreements are defined
related_procedures:
  - SVC-CALL-001
tags:
  - vendor management
  - contracts
  - renewals
  - service level agreements
  - third-party vendors
version: 1.0
last_updated: 2026-03-25
---

# Process the Vendor Service Contract Renewal Queue

## What This Procedure Does

Review and process vendor service contract renewals. The Vendor Contract Renewal Queue displays third-party and pass-through vendor contracts approaching their renewal dates. For each contract, verify dates and terms, process the renewal if needed, and update linked customer service contracts to ensure continuous coverage under agreed service level agreements.

## Before You Begin

- Service module access is available
- Vendor service contracts are approaching renewal dates
- You have authority to renew contracts or escalate for approval
- Customer service contracts are linked to vendor contracts
- You understand the current terms and pricing for each vendor

## Steps

### Step 1: Navigate to Vendor Contract Renewal Queue

Go to Service menu > Work Queues > Vendor Contract Renewal Queue. The renewal queue displays all vendor contracts requiring attention:

| Column | Information |
|--------|------------|
| Vendor Contract ID | Unique identifier for vendor agreement |
| Vendor Name | Third-party service provider |
| Customer | Account under which vendor service is provided |
| Service Type | Type of service (maintenance, support, monitoring) |
| Current Expiration | When the contract ends |
| Days Until Expiration | How much time remains |
| Renewal Status | Current renewal processing status |

### Step 2: Prioritize Contracts Approaching Expiration

Review the "Days Until Expiration" column. Prioritize contracts expiring soonest:

| Days Remaining | Action |
|----------------|--------|
| 0-30 days | Immediate attention required |
| 31-60 days | Schedule for processing this week |
| 61-90 days | Plan renewal in next business cycle |

Start with the most urgent contracts to prevent service gaps.

### Step 3: Open Vendor Contract for Review

Click on a vendor contract to open the detail view. Review the contract information:

| Information | Verify |
|------------|--------|
| Vendor Details | Name, contact information, terms |
| Service Description | What services vendor provides |
| Pricing | Current rates and total annual cost |
| Terms & Conditions | Payment terms, SLAs, penalties |
| Coverage | What services are included |
| Exclusions | What is not covered |

### Step 4: Check Current Terms and Pricing

Review whether current terms and pricing remain acceptable:

| Check Item | Decision Needed |
|------------|-----------------|
| Pricing Increase | Is the new price acceptable, or do we negotiate? |
| Service Levels | Are SLAs still adequate for customer needs? |
| Coverage | Does the coverage match what customer requires? |
| Vendor Performance | Is the vendor meeting service obligations? |

If terms are unacceptable, escalate for negotiation or vendor replacement decision before proceeding.

### Step 5: Process the Renewal

Once contract terms are approved, proceed with renewal:

Click Renew Contract or Process Renewal button on the vendor contract. The system displays a renewal confirmation dialog:

| Field | Action |
|-------|--------|
| New Expiration Date | Confirm or adjust renewal period |
| Renewal Terms | Accept or modify terms |
| Pricing | Confirm new pricing or apply negotiated rates |

Review all fields and click Confirm Renewal to process.

### Step 6: Update Linked Customer Service Contract

The renewal updates the vendor contract, but the linked customer service contract may also require updating:

The system may automatically update linked customer contracts if terms change. Navigate to the related customer service contract (if not automatically opened) and verify:

| Information | Update As Needed |
|------------|-----------------|
| Service Coverage | Ensure customer SLA matches vendor capability |
| Expiration Date | Align with renewed vendor contract |
| Pricing | Update customer billing if pricing changed |
| Terms | Update customer terms to match vendor terms |

Save any changes to the customer service contract.

### Step 7: Document Renewal

Record the renewal in the contract system:

The system typically auto-documents renewal when you click Confirm Renewal. Verify a renewal record appears with:

- New expiration date
- Renewal date (today)
- Updated pricing (if applicable)
- Any notes or special terms

### Step 8: Update Queue Status

Mark the contract as processed in the renewal queue. Click Mark as Processed or Update Status. The contract moves to a "Renewed" status and no longer appears in the active renewal queue.

## What Happens Next

Renewed vendor contracts remain active with extended coverage. Linked customer service contracts are updated to reflect the renewal and any pricing changes. Customers can be notified of any changes to their service levels or pricing if needed. The renewal is documented in the vendor and customer contract history. The vendor contract returns to normal monitoring until it again approaches expiration. Future renewals can be scheduled based on the new expiration date.

## Common Issues

**Vendor Contract Renewal Queue shows no contracts or is empty**

Verify vendor contracts are set up in the system and linked to customer accounts. Check that contracts are approaching their expiration dates within your review window. If contracts should exist but do not appear, the system may use a different queue name or location. Contact your system administrator to locate the renewal queue.

**Vendor contract renewal shows error or cannot be processed**

Verify the contract is linked to a valid customer service agreement. Check that the vendor name and contact information are complete. If an error occurs during renewal, note the error message and contact your system administrator. Do not force the renewal without understanding the error.

**Customer service contract does not update automatically when vendor contract renews**

Verify the customer contract is linked to the vendor contract (the link should be visible on both sides). If linked, refresh the customer contract view to see updated information. If the link exists but the customer contract does not update, the system may require manual update. Open the customer contract and manually verify/update the expiration date and terms to match the renewed vendor contract.

**Pricing has changed significantly and customer may not accept**

If vendor pricing has increased substantially, escalate to management before confirming the renewal. Consider negotiating better terms with the vendor or evaluating alternative vendors. Determine whether to pass the price increase to the customer or absorb it. Once a decision is made, process the renewal with the agreed pricing.

**Vendor contract expired while still in queue**

If a contract expires before renewal is processed, contact the vendor immediately to ensure service is not interrupted. Process the renewal as expedited. Create a back-dated renewal or emergency renewal as your system allows. Notify the customer immediately to ensure they understand any service gaps.
