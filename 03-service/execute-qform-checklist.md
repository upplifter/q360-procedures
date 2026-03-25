---
title: Execute a QForm Checklist
id: SVC-QFORMS-001
module: Service
screen: Mobile Dispatch / Service Call
menu_path: Dispatched Service Call > Checklist Section
applies_to: Service Technicians, Field Service Personnel
prerequisites:
  - Mobile device with Q360 access
  - Dispatched service call assigned to technician
  - QForm checklist configured for the call type or customer
related_procedures:
  - SVC-ADMIN-001
tags:
  - Mobile
  - QForms
  - Checklists
  - Inspections
version: 1.0
last_updated: 2026-03-25
---

# Execute a QForm Checklist

## What This Procedure Does

This procedure completes a QForm checklist on a mobile device during a service call. QForms are custom checklists or inspections configured by your organization to ensure consistent field procedures and data capture.

## Before You Begin

- Mobile device must have Q360 access and QForms enabled
- Service call must be dispatched to your technician
- QForm must be configured for the call type or customer
- Have the materials and tools needed to complete the inspection

## Steps

### Step 1: Open Dispatched Service Call

On the mobile device, open the dispatched service call. Navigate to the checklist section or use the QForms link if configured on the call. The QForm loads with the pre-defined checklist items.

### Step 2: Complete Checklist Items

For each item in the QForm checklist, complete the following:

| Field | What to enter |
|-------|---------------|
| Checklist Item | Review the item name and instructions |
| Pass/Fail | Mark the item as Pass, Fail, or N/A as appropriate |
| Notes | Add any relevant observations or findings |
| Photos | Attach photos documenting the condition or issue |

Work through each checklist item in order. If an item requires further investigation, document the finding with notes and photos.

### Step 3: Add Supporting Information

As you complete items, add supporting information such as equipment readings, measurements, or observations. Use the notes field to explain any failures or unusual conditions. Attach photos showing the current state of equipment or identified problems.

### Step 4: Submit the QForm

After completing all checklist items, click Submit to send the completed form to the Q360 system. The QForm is processed and linked to the service call record.

## What Happens Next

The completed QForm results are saved to the service call record and visible in Q360. The checklist results are available in the call detail view and included in call reports. QForm submissions may trigger notifications, work orders, or follow-up actions if specific conditions are met (e.g., equipment failure detected, threshold exceeded).

## Common Issues

**QForm Not Appearing on Dispatch**
Verify that a QForm has been configured for the call type or customer. Check that the mobile device has the latest QForms configuration downloaded. Contact your system administrator if QForms are not syncing to the mobile device.

**Cannot Submit QForm**
Ensure all required fields are completed. Check mobile device connectivity to the Q360 system. If offline, the form may save locally and sync when connectivity is restored.

**Photos Not Attaching**
Verify the mobile device has camera access enabled in system settings. Check available storage space on the device. Ensure photo file sizes are within system limits.
