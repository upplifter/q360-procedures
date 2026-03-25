---
title: Mark Call as Technician Done
id: SVC-CALL-015
module: Service
screen: Service Call
menu_path: Service > Service Calls
applies_to: Technicians, Field Service Managers
prerequisites:
  - Service call is in status DISPATCHED
  - Field work is complete
  - Customer signature obtained (recommended)
related_procedures:
  - SVC-CALL-017a
  - SVC-CALL-018
  - SVC-CALL-014
tags:
  - call status
  - field completion
  - solution code
  - work tracking
version: 1.0
last_updated: 2026-03-25
---

# Mark Call as Technician Done

## What This Procedure Does

Update a service call status from DISPATCHED to TECHDONE to indicate field work is complete. TECHDONE status triggers internal events and notifies the CSR or dispatcher to review the call before final closure. You must provide a Solution Code and Solution Description documenting the resolution.

## Before You Begin

- All field work must be complete
- The service call must be in status DISPATCHED
- You must be the assigned technician or have dispatcher/manager access
- You must document the solution before marking TECHDONE

## Steps

### Step 1: Open the Service Call

Open the service call that is complete in the field.

### Step 2: Click Edit to Access Call Details

Click Edit (pencil icon) on the action bar. The call form enters edit mode, allowing field updates.

### Step 3: Set Status to TECHDONE

Locate the Status dropdown field on the call form. Click the dropdown and select TECHDONE from the available options. The status changes to TECHDONE.

### Step 4: Select a Solution Code

Locate the Solution Code dropdown on the call form. Click the dropdown to view available codes:

| Code | Meaning |
|------|---------|
| FIXED | Equipment repaired and operational |
| REPLACED | Component replaced |
| PM_COMPLETE | Preventive maintenance completed |
| NO_PROBLEM_FOUND | Equipment checked, no issue found |
| REFERRED | Work referred to specialist or customer |
| INSTALLED | New equipment installed |
| OTHER | Use with Solution Description |

Select the code that best describes the resolution. Save the selection.

### Step 5: Enter Solution Description

Locate the Solution Description field. Enter a detailed description of the work performed and the resolution reached:

| Field | What to enter |
|-------|--------------|
| Solution Description | Brief narrative (2-3 sentences) describing the solution, repair performed, parts replaced, or issue diagnosis |

Example: "Replaced failed compressor motor. Tested system operation. Unit now running normally at design specifications."

### Step 6: Save the Call

Click Save (floppy disk icon). The system updates the call status to TECHDONE and generates internal events.

## What Happens Next

The call moves from DISPATCHED to TECHDONE status. The system notifies the CSR or dispatcher that the call requires review before final closure. The technician's time and work are logged. Events are generated for follow-up tasks. Before the call can be closed (see SVC-CALL-018), a dispatcher or CSR must verify that all dispatch close validation checks pass (see SVC-CALL-017b). Once validation is complete, the call moves to COMPLETED status and can be closed and invoiced.

## Common Issues

**Status dropdown does not show TECHDONE as an option**

Verify the call is in DISPATCHED status. If the call is in a different status, TECHDONE may not be a valid transition. Check with your service manager. Refresh the page and try again. If the issue persists, contact your system administrator.

**Solution Code dropdown is empty or shows no options**

Verify the Solution Code lookup table is configured in your system. Contact your system administrator if no codes are available. If codes should be visible, try refreshing the page. In the meantime, select OTHER and provide a detailed Solution Description.

**Call will not save after setting TECHDONE status**

Verify all required fields are completed (Status, Solution Code, Solution Description). If an error message appears, note it and contact your system administrator. Check that you have proper permissions to mark calls as TECHDONE. Try refreshing the page and attempting to save again.
