---
title: Expire Service Contract Manually
id: SVC-CONTRACT-008
module: Service
screen: Service Contract
menu_path: Service > Service Overview OR Service > Service Contracts
applies_to: Service Managers, Contract Administrators
prerequisites:
  - Service contract must exist
  - Contract must be in ACTIVE status to be manually expired
related_procedures:
  - SVC-CONTRACT-002a
tags:
  - contract status
  - expiration
  - lifecycle
version: 1.0
last_updated: 2026-03-25
---

# Expire Service Contract Manually

## What This Procedure Does

Manually changes a service contract status from ACTIVE to EXPIRED when the contract term ends or the customer terminates the agreement. Expired contracts are removed from active service buckets in the Service Overview workflow and archived for historical reference.

## Before You Begin

- Service contract must exist and be in ACTIVE status
- All outstanding service calls should be completed and invoiced before expiring the contract
- You should have documented the reason for expiration (natural term end, early termination, etc.)
- Check if any recurring dispatches are still pending

## Steps

### Step 1: Locate the Contract to Expire

Navigate to the Service Contract list via Service > Service Contracts. Find the contract you want to expire. You can also access it from Service > Service Overview workflow under the Expiring Contracts bucket if the contract is approaching its end date.

### Step 2: Open the Contract

Click the contract name or ID to open the contract form in view mode.

### Step 3: Enter Edit Mode

Click the Edit button (pencil icon) in the toolbar to enter edit mode. The contract form is now editable.

### Step 4: Verify Contract Status

Confirm the Status field shows ACTIVE. If the status is already EXPIRED or CANCELLED, no further action is needed.

### Step 5: Change Status to EXPIRED

Click the Status field dropdown and select EXPIRED from the list of available statuses.

### Step 6: Add Expiration Notes (Optional)

In the Notes or Remarks field, document why the contract is being expired:

- Natural end of term
- Customer requested early termination
- Non-renewal decision
- Other reason

### Step 7: Save the Contract

Click the Save button (floppy disk icon) in the toolbar. The system saves the status change and updates the contract to EXPIRED.

### Step 8: Verify Removal from Active Buckets

Navigate to Service > Service Overview workflow. Verify that the expired contract no longer appears in the Active Contracts bucket. It may appear in an Archived or Expired Contracts bucket if your workflow includes one.

## What Happens Next

The contract status changes to EXPIRED and is removed from active service management workflows. Expired contracts still appear in historical reports and contract searches but are excluded from:

- Active Contracts bucket in Service Overview
- Service call generation
- Recurring dispatch processing
- Active contract reports

Historical data on the expired contract remains intact for profitability analysis and audit purposes. If the customer wants to renew service, create a new service contract rather than reactivating the expired one.

## What About Auto-Expiration

Your system may be configured to automatically expire contracts based on inactivity or contract end date. If auto-expiration is enabled:

- The Service Contract Inactive Days configuration setting controls how many days of inactivity trigger auto-expiration
- The Service Contract Inactive Status configuration setting defines the status assigned by auto-expiration (usually EXPIRED)
- The background job include_servicecontract_setinactive runs periodically to process auto-expirations
- Manually expired contracts bypass these automatic rules

You do not need to use this manual procedure if auto-expiration is already configured and active in your system.

## Common Issues

**Status field shows EXPIRED but contract still appears in Active Contracts bucket**

After saving the status change, the Service Overview workflow may take a few minutes to refresh. Click the Refresh button (circular arrow) in the Service Overview to force an update. If the contract still appears as active after refresh, check that the status was saved correctly by opening the contract again and confirming the Status field shows EXPIRED.

**Cannot change status to EXPIRED because field is read-only**

Some systems restrict status changes to certain user roles or based on contract conditions. If the Status field is read-only:

- Verify you have the appropriate user role for contract management
- Check if there are pending service calls that must be completed first
- Contact your system administrator if status change permissions need to be granted

**Recurring dispatches are still being generated for the expired contract**

Once you expire the contract, recurring dispatch generation should stop. If calls are still being generated:

- Verify the contract status is saved as EXPIRED (not ACTIVE)
- Check the Recurring tab on line items to see if schedules still have future dates
- Manually disable auto-dispatch on recurring schedules if they are still active
- Run a refresh on the Service Overview workflow to update processing rules

**Customer wants to renew the contract**

Do not reactivate an expired contract. Instead, create a new service contract with updated terms. You can reference the expired contract as a prior agreement, but a fresh contract avoids confusion and allows for updated rates, products, and billing terms.
