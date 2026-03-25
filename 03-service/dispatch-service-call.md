---
title: Dispatch a Service Call
id: SVC-CALL-006
module: Service
screen: Service Call Form
menu_path: Service > Service Calls
applies_to: Customer Service Representatives, Service Managers, Dispatch Coordinators
prerequisites:
  - Service call exists in SCHEDULED status
  - Technician is assigned to the call
  - Dispatch date is within technician's availability
related_procedures:
  - SVC-CALL-005
  - SVC-CALL-007
tags:
  - dispatching
  - technician-notification
version: 1.0
last_updated: 2026-03-25
---

# Dispatch a Service Call

## What This Procedure Does

This procedure sends a service call to a technician for execution. Dispatching triggers an automated notification email or mobile alert to the assigned technician with call details, customer information, and site location. The call status changes to DISPATCHED, indicating the technician has been notified and is ready to begin the service work.

## Before You Begin

- Service call exists in SCHEDULED status
- Technician is assigned to the call on the Dispatch tab
- Dispatch date is today or in the near future
- Technician mobile access is configured (for mobile notifications)

## Steps

### Step 1: Open the Service Call

Navigate to Service > Service Calls or the Service Calls tab on the customer record. Click the call number to open the Service Call form. Verify the call status is SCHEDULED and that a technician assignment is visible on the Dispatch tab.

### Step 2: Access Dispatch Options

Click Extended Menu (three vertical dots) at the top of the form. Select Dispatch. Alternatively, open the Dispatch tab and click the Dispatch button if visible on the scheduled row.

### Step 3: Confirm Dispatch Details

A confirmation dialog appears showing the assigned technician, scheduled date/time, and customer location. Review the information for accuracy. Confirm that the technician is correct and the date/time matches the intended dispatch window.

### Step 4: Execute Dispatch

Click Dispatch or Confirm in the dialog. The system sends an automated notification to the assigned technician via email and/or mobile app (if configured). The call status automatically changes to DISPATCHED.

## What Happens Next

The technician receives a notification containing the call details, customer name, contact information, site address, product details, and problem description. The call now appears in the technician's task list and mobile app for real-time access during field work. The call status remains DISPATCHED until the technician completes the work and updates the call status.

The technician can begin the time billing process using SVC-CALL-007 to track labor hours. Once work is complete, the technician updates the call status to TECHDONE.

## Common Issues

**Dispatch Notification Not Received by Technician**
Verify the technician email address is configured in their user profile. Check that mobile notifications are enabled for the technician if using mobile field access. Resend the dispatch notification by opening the call and repeating the Dispatch action.

**Call Reverted to SCHEDULED After Dispatch**
If the call status does not change to DISPATCHED or reverts immediately, check that the technician assignment is still active on the Dispatch tab. Confirm no system errors occurred during the dispatch action. Retry the dispatch action.

**Multiple Dispatch Notifications Sent to Technician**
Avoid clicking Dispatch multiple times in succession, as this may trigger duplicate notifications. Wait for the system confirmation before closing the dialog. If duplicate notifications were sent, contact the technician to confirm they only need to respond to one dispatch.
