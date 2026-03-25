---
title: Check Dispatch Close Validation
id: SVC-CALL-017b
module: Service
screen: Service Call
menu_path: Service > Service Calls
applies_to: CSRs, Service Managers, Dispatchers
prerequisites:
  - Service call is in status TECHDONE or COMPLETED
  - Field work is complete
  - Call is ready for closure review
related_procedures:
  - SVC-CALL-015
  - SVC-CALL-017a
  - SVC-CALL-018
tags:
  - call closure
  - validation
  - time tracking
  - purchase orders
  - journal entries
version: 1.0
last_updated: 2026-03-25
---

# Check Dispatch Close Validation

## What This Procedure Does

Verify that a service call meets all requirements before closure. Dispatch close validation checks three critical areas: (1) all time bills must be posted, (2) all purchase orders must be received, and (3) all journal entries must be linked. Resolve any outstanding items before proceeding to close the call.

## Before You Begin

- The service call must be in status TECHDONE or COMPLETED
- Field work must be complete
- You are preparing the call for closure and billing
- You have access to the Time Bills, Parts, and AR Journal tabs

## Steps

### Step 1: Open the Service Call

Open the service call requiring validation before closure.

### Step 2: Check Time Bills Tab for Unposted Entries

Click the Time Bills tab on the service call form. Review all time entries:

| Column | Check For |
|--------|-----------|
| Date | All work dates are present |
| Hours | Hours match field work completed |
| Technician | Correct technician assigned |
| Status | All entries show POSTED status |

Identify any time bills with status other than POSTED. These entries must be posted before the call can close.

### Step 3: Post Unposted Time Bills

For any time bill not showing POSTED status, click the entry to open it. Verify the hours, labor code, and technician are correct. Click Post (or equivalent button per your system). The entry status updates to POSTED. Post all remaining entries.

### Step 4: Check Parts Tab for Unreceived Purchase Orders

Click the Parts tab on the service call. Review all parts added to the call:

| Column | Check For |
|--------|-----------|
| Item | All parts used or ordered |
| Quantity | Quantities match what was used |
| PO Status | All entries show RECEIVED or N/A |
| Supplier | Correct vendor for each item |

Identify any POs with status other than RECEIVED or N/A. These orders must be received before closure.

### Step 5: Receive Unreceived Purchase Orders

For any PO not showing RECEIVED status, contact your receiving department or supplier to expedite delivery. Once the PO is received and recorded in inventory, return to the Parts tab and verify the status updates to RECEIVED. Do not proceed to closure until all POs are received.

### Step 6: Check AR Journal Tab for Unlinked Journal Entries

Click the AR Journal tab on the service call. Review all accounting entries associated with the call:

| Column | Check For |
|--------|-----------|
| Entry Date | Journal entry dates are correct |
| Amount | Amounts match parts and labor |
| Link Status | All entries show LINKED or N/A |
| Account | Correct GL accounts are used |

Identify any journal entries with status other than LINKED or N/A. These entries must be linked to close.

### Step 7: Link Unlinked Journal Entries

For any journal entry not showing LINKED status, click the entry to review it. Verify the GL accounts and amounts are correct. Click Link or equivalent button. The entry status updates to LINKED. Link all remaining entries.

### Step 8: Validation Complete

Once all three tabs show: all time bills POSTED, all POs RECEIVED, and all journal entries LINKED, the call passes validation and is ready for closure.

## What Happens Next

A call that passes all validation checks can safely proceed to closure (see SVC-CALL-018). The call can be marked COMPLETED and invoiced. The billing process can generate the final customer invoice without encountering blocking errors. Financial records are complete and ready for reconciliation.

## Common Issues

**Time bills show UNPOSTED status and cannot be posted**

Verify the time entry is complete with hours, labor code, and technician. Check that the hours are reasonable and match the work performed. If an error message appears when posting, note it and contact your system administrator. Do not close the call until all time bills are posted.

**Purchase order status shows UNRECEIVED but items are at the site**

The PO receipt may not have been recorded in the system. Contact your receiving department to confirm the items were logged as received. Ask them to verify the PO status in inventory or the receiving module. Request they update the status to RECEIVED if not already done. Refresh the service call to see the updated status.

**Journal entries cannot be linked or show errors**

Verify the GL accounts and amounts on the journal entry are correct and match supporting documents (invoices, purchase orders). If the entry is incorrect, it may need to be reversed and recreated. Contact your accounting department or system administrator for assistance. Do not close the call until all journal entries are linked.

**Call fails validation for an unknown reason**

A message should appear indicating which check failed. Review that section above and address the outstanding items. If the error message is unclear, note it and contact your system administrator. Provide the call number and a screenshot of the error message.
