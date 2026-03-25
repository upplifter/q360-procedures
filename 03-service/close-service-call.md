---
title: Close a Service Call
id: SVC-CALL-018
module: Service
screen: Service Call
menu_path: Service > Service Calls
applies_to: CSRs, Service Managers, Dispatchers
prerequisites:
  - Service call is in status TECHDONE or COMPLETED
  - Dispatch close validation has been completed and passed
  - Field work is complete
  - Customer authorization obtained if required
related_procedures:
  - SVC-CALL-017b
  - SVC-CALL-017a
  - SVC-CALL-019
tags:
  - call closure
  - billing
  - invoicing
  - status management
version: 1.0
last_updated: 2026-03-25
---

# Close a Service Call

## What This Procedure Does

Finalize a service call by setting its status to CLOSED. For billable work, use the Bill This Service Call function to generate a customer invoice and automatically close the call. For non-billable work, manually set the status to CLOSED. All calls must pass dispatch close validation before closure.

## Before You Begin

- The service call must be in status TECHDONE or COMPLETED
- Dispatch close validation checks must pass (see SVC-CALL-017b)
- All time bills must be posted
- All purchase orders must be received
- All journal entries must be linked
- Customer authorization must be obtained if the call was quoted

## Steps

### Step 1: Open the Service Call

Open the service call ready for closure.

### Step 2: Verify Dispatch Close Validation

Before proceeding to close, ensure all validation checks pass. If you have not yet run dispatch close validation, follow SVC-CALL-017b to verify:

- All time bills are POSTED
- All POs are RECEIVED
- All journal entries are LINKED

Do not proceed if validation checks fail.

### Step 3: For Billable Calls - Generate Invoice

If the call includes billable labor or parts, proceed to invoice the call:

Click the Extended Menu (three vertical dots) on the action bar. Select Bill This Service Call. The billing dialog opens.

Review the billing summary:

| Item | Description |
|------|-------------|
| Labor Total | Sum of all posted time entries |
| Parts Total | Sum of all parts used or supplied |
| Deposits Applied | Any prepayments or deposits deducted |
| Total Due | Final amount to bill customer |

Adjust the total if necessary (e.g., to apply a discount or adjustment). Click OK or Confirm Billing to generate the invoice.

### Step 4: Review Generated Invoice

The system generates a customer invoice linked to the service call. The invoice is created in the accounts receivable system and is ready for delivery to the customer. Verify the invoice number and amount appear on the call.

### Step 5: For Non-Billable Calls - Set Status to CLOSED

If the call is non-billable (e.g., warranty, internal maintenance), click Edit (pencil icon) on the action bar. Locate the Status dropdown and select CLOSED. Click Save (floppy disk icon).

### Step 6: Confirm Closure

The call status updates to CLOSED. A confirmation message appears. The call is now archived and no longer appears in active call queues.

## What Happens Next

A closed service call is archived in the system history. The call record remains available for reference, reporting, and historical analysis. The customer invoice (if generated) is sent to the customer or can be retrieved for delivery. If a deposit was collected, it is applied to the invoice. The call no longer appears in open call lists or dispatch queues. Time and materials are locked and cannot be edited. The call appears in historical reports and profitability analysis (see SVC-CALL-021).

## Common Issues

**Bill This Service Call option does not appear in Extended Menu**

Verify the call is in status COMPLETED or TECHDONE. Ensure the call has billable items (labor time or parts). If the option still does not appear, the call may be flagged as non-billable or there may be a configuration issue. Contact your service manager or system administrator.

**Invoice generation shows error or displays unexpected amounts**

Verify all time bills are posted (see SVC-CALL-017b). Check that parts and labor costs are entered correctly on the call. If costs are missing or incorrect, edit them before attempting to bill. If the error persists, note it and contact your system administrator.

**Status will not change to CLOSED when clicking Save**

Verify dispatch close validation has passed. If any checks failed (unposted time, unreceived POs, unlinked journal entries), address those items first (see SVC-CALL-017b). Once validation passes, the status should update successfully. If the issue persists, refresh the page and try again.

**Call shows as CLOSED but appears to still be in open queue**

The system may take a brief moment to update queue views. Refresh the page or navigate away and return. If the call still appears in the open queue after a few minutes, contact your system administrator to verify the status updated correctly in the database.
