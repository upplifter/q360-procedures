---
title: Update Call Status and Solution
id: SVC-CALL-017a
module: Service
screen: Service Call
menu_path: Service > Service Calls
applies_to: Technicians, CSRs, Service Managers
prerequisites:
  - Service call is open
  - Field work or service activity is complete
related_procedures:
  - SVC-CALL-015
  - SVC-CALL-017b
  - SVC-CALL-018
tags:
  - call status
  - solution documentation
  - problem description
  - call resolution
version: 1.0
last_updated: 2026-03-25
---

# Update Call Status and Solution

## What This Procedure Does

Document the final problem description and resolution on a service call. Update the call's Problem Description field with customer-facing narrative, select a Solution Code, and enter Solution Description with resolution details. Adjust call status as appropriate for closure workflow.

## Before You Begin

- The service call must be open
- Field work or service activity should be substantially complete
- You must have details of the problem found and the resolution applied
- You should understand the solution code options available in your system

## Steps

### Step 1: Open the Service Call

Open the service call requiring status and solution updates.

### Step 2: Click Edit to Access Call Form

Click Edit (pencil icon) on the action bar. The call form enters edit mode.

### Step 3: Update Problem Description

Locate the Problem Description field on the Call tab. Click in the field and enter or revise the customer-facing problem statement. Write a clear, concise description from the customer's perspective:

| Field | What to enter |
|-------|--------------|
| Problem Description | What issue the customer reported or what was discovered during inspection (1-3 sentences) |

Example: "Customer reported heating system not producing hot water. Thermostat not responding to input."

### Step 4: Select Solution Code

Locate the Solution Code dropdown on the call form. Select the code most accurately reflecting the resolution:

| Code | Meaning |
|------|---------|
| FIXED | Equipment repaired and operational |
| REPLACED | Component replaced |
| PM_COMPLETE | Preventive maintenance completed |
| NO_PROBLEM_FOUND | Equipment checked, no issue found |
| REFERRED | Work referred to specialist or customer |
| INSTALLED | New equipment installed |
| OTHER | Use with detailed Solution Description |

### Step 5: Enter Solution Description

Locate the Solution Description field. Enter a detailed narrative explaining the resolution applied. This is typically technical and more detailed than the Problem Description:

| Field | What to enter |
|-------|--------------|
| Solution Description | What was done to resolve the issue, parts replaced, or diagnosis reached (2-4 sentences) |

Example: "Replaced failed thermostat control board. Cleaned heating exchanger. Tested system recovery. Verified hot water production at correct temperature."

### Step 6: Update Call Status

Locate the Status dropdown. Adjust the status based on where the call is in the closure workflow:

- TECHDONE: Field work is complete; awaiting CSR review and validation
- COMPLETED: Call ready for billing; all prerequisites met
- CLOSED: Call is fully billed and archived

If the call is transitioning to COMPLETED or CLOSED status, refer to SVC-CALL-017b (Dispatch Close Validation) before saving.

### Step 7: Save the Call

Click Save (floppy disk icon). The system updates all fields and generates any necessary events.

## What Happens Next

The call record is updated with the problem description and solution details. These details appear on printed call reports and are available for customer communication and record retention. If status was updated to TECHDONE, the dispatcher or CSR is notified for review. If status was updated to COMPLETED or CLOSED, the call moves toward final invoicing. CSRs can refer to these details when closing the call (see SVC-CALL-018) and when creating the final invoice.

## Common Issues

**Solution Code dropdown shows limited options or is empty**

Verify the Solution Code lookup table is configured in your system. If codes are not appearing, try refreshing the page. Contact your system administrator to ensure the lookup is active. In the meantime, select OTHER and provide a detailed Solution Description to document the resolution.

**Problem Description or Solution Description field will not accept text**

Verify the call is in edit mode (Edit button was clicked). Ensure you have edit permissions for the service call. If the field is read-only, check that the call status permits editing. Some statuses may lock the call from further changes. Contact your system administrator if editing is restricted unexpectedly.

**Status change to COMPLETED or CLOSED is not allowed**

The call may fail validation checks. Before setting status to COMPLETED or CLOSED, run the dispatch close validation procedures (see SVC-CALL-017b). Verify that all time bills are posted, all purchase orders are received, and all journal entries are linked. Address any outstanding items before attempting to change status.
