---
title: Adjust Recurring Service Call Schedule
id: SVC-CONTRACT-005
module: Service
screen: Service Contract > Line Items > Recurring
menu_path: Service Contract > Line Items > Recurring Tab
applies_to: Service Managers, Technician Schedulers, Dispatch Managers
prerequisites:
  - Service contract must be created
  - Recurring call schedule must already exist
  - Service line item must be in edit mode
related_procedures:
  - SVC-CONTRACT-004
  - SVC-CONTRACT-006
tags:
  - recurring calls
  - scheduling
  - adjustment
version: 1.0
last_updated: 2026-03-25
---

# Adjust Recurring Service Call Schedule

## What This Procedure Does

Modifies an existing recurring service call schedule to change frequency, dates, technician assignments, auto-dispatch settings, or service items. Changes apply to future calls generated from the updated schedule.

## Before You Begin

- Service contract must exist with recurring call schedules
- You must have access to the Service Contract line item in edit mode
- You should review the Call List tab to understand which calls have already been generated
- Changes to the schedule affect only future calls, not calls already generated

## Steps

### Step 1: Open the Service Contract and Select the Product

Open the service contract from Service > Service Contracts. Click the Line Items tab. Click the pencil icon (Edit) for the product whose recurring schedule you want to modify.

### Step 2: Navigate to the Recurring Tab

Once in the product line item edit form, click the Recurring tab to display all recurring call schedules for this product.

### Step 3: Select the Schedule to Modify

In the Recurring Calls grid, click the pencil icon (Edit) next to the schedule you want to adjust. The schedule form opens in edit mode.

### Step 4: Update Schedule Details

Modify any of the following fields as needed:

| Field | What to change |
|-------|-----------------|
| Start Date | Change the schedule start date if recurring calls should begin at a different time |
| End Date | Adjust the end date to extend or shorten the schedule period |
| Frequency | Change from Monthly to Quarterly, or vice versa |
| Warning Days | Adjust advance notification timing |
| Create Days in Advance | Change how far ahead dispatch records are pre-generated |
| Auto Dispatch | Enable or disable automatic dispatch for future calls |
| Technician | Assign a different technician or change from one technician to another |

### Step 5: Modify Service Items (if needed)

Click the Details tab within the schedule. You can add, edit, or remove service items performed on each recurring call:

- Click Add to add a new service item
- Click Edit (pencil icon) to modify an existing item
- Click Delete (trash can) to remove an item

### Step 6: Modify Checklist Items (if needed)

Click the Checklist tab within the schedule. Add, edit, or remove checklist items as needed for the revised call procedure.

### Step 7: Save the Changes

Click Save to apply all adjustments to the recurring schedule. The updated schedule is saved.

### Step 8: Review Previously Generated Calls

After saving the schedule, click the Call List tab to review calls that were already generated under the previous schedule. Depending on your business process, you may want to manually adjust technician assignments on previously generated calls or leave them as-is.

## What Happens Next

The adjusted schedule is applied to future call generation. When calls are generated next (manually or via background job), they will use the updated frequency, technician, and service item settings. Previously generated calls are not automatically updated; you must manually modify them if needed. If you changed the schedule end date to be sooner, no new calls will be generated beyond the new end date.

## Common Issues

**Changes to the schedule are not reflected in calls already generated**

Changes to a recurring schedule only affect future calls generated from that schedule. Calls that were already generated retain their original technician, date, and items. To modify previously generated calls, open each call individually and edit it manually, or use the Service call bulk edit function if available.

**Frequency change causes calls to generate on unexpected dates**

When you change frequency (for example, from Monthly to Quarterly), calls will be generated based on the new frequency interval. Existing calls from the old schedule remain unchanged. Future calls will follow the new frequency. If you want to clean up old call records, you must delete or cancel them manually before the new frequency takes effect.

**Technician reassignment did not update existing dispatch assignments**

Updating the Technician field on the schedule only affects future calls. Existing dispatch records for already-generated calls retain their original technician assignments. To reassign existing calls to a different technician, open each dispatch record and change the Technician field manually.

**Call List tab shows no calls even though I expected calls to be generated**

Recurring schedules do not automatically generate calls. You must use the Generate Recurring Dispatch function from the Extended Menu or Service menu to create dispatch records from the schedule. If you have not run the generation process, no calls will appear in the Call List. Check that generation has been triggered before expecting to see calls listed.
