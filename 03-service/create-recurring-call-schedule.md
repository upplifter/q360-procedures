---
title: Create Recurring Service Call Schedule
id: SVC-CONTRACT-004
module: Service
screen: Service Contract > Line Items > Recurring
menu_path: Service Contract > Line Items > Recurring Tab
applies_to: Service Managers, Technician Schedulers, Dispatch Managers
prerequisites:
  - Service contract must be created
  - Service contract line items must be added
  - Technician records must be configured
  - General code RDBILLCYCL must be configured for custom frequencies
related_procedures:
  - SVC-CONTRACT-002b
  - SVC-CONTRACT-005
tags:
  - recurring calls
  - scheduling
  - dispatch
version: 1.0
last_updated: 2026-03-25
---

# Create Recurring Service Call Schedule

## What This Procedure Does

Sets up a repeating schedule for service calls on a service contract product. Defines the frequency, dates, technician assignments, and checklist items for recurring maintenance or support visits.

## Before You Begin

- Service contract header must be created and saved
- Line items with products must be added to the contract
- Technician records must be configured in the system
- If using custom call frequencies, the RDBILLCYCL general code must be configured with your custom frequency options

## Steps

### Step 1: Open the Service Contract and Select a Product

Open the service contract from Service > Service Contracts. Click the Line Items tab. Click the pencil icon (Edit) for the product you want to set up recurring calls for.

### Step 2: Navigate to the Recurring Tab

Once in the product line item edit form, click the Recurring tab to display the recurring call configuration area.

### Step 3: Add a Recurring Call Schedule

In the Recurring Calls grid, click the Add button (plus icon) to create a new schedule entry. The form opens in edit mode.

### Step 4: Enter Schedule Details

Fill in the following fields for the recurring call schedule:

| Field | What to enter |
|-------|---------------|
| Start Date | Date the recurring schedule begins |
| End Date | Date the recurring schedule ends |
| Frequency | Monthly, Quarterly, Semi-Annually, Annually, or Custom (from RDBILLCYCL general code) |
| Warning Days | Days before a scheduled call to send a warning notification |
| Create Days in Advance | How many days in advance to auto-generate dispatch records |
| Auto Dispatch | Check this box to automatically dispatch calls without manual intervention |
| Technician | Assign the technician responsible for these calls |

### Step 5: Add Service Items to the Schedule

Click the Details tab within the recurring schedule. Add items that will be performed on each call:

| Field | What to enter |
|-------|---------------|
| Item | Service item, labor code, or product to be used |
| Quantity | Quantity per call |
| Rate | Labor rate or item price per call |

Add multiple items if the recurring call involves multiple tasks or materials.

### Step 6: Add Checklist Items

Click the Checklist tab within the recurring schedule. Add inspection or verification items that must be completed on each call:

| Field | What to enter |
|-------|---------------|
| Checklist Item | Description of task or item to verify |
| Required | Check if this item is mandatory to complete the call |

### Step 7: Save the Schedule

Click Save to create the recurring call schedule. The schedule is now associated with the product line item.

### Step 8: Generate Recurring Dispatch Records

Recurring calls do not automatically generate dispatch records. You must trigger generation using one of the following methods:

- From the contract Line Items tab, select the product, click Extended Menu > Generate Recurring Dispatch
- From Service menu, select Generate Recurring Dispatches to process all contracts at once
- Allow the background job include_servicecontract_recurring_generate to run on schedule (if configured)

## What Happens Next

Once the schedule is created and generation is triggered, the system creates Service Call records (dispatch records) based on the frequency and dates. Calls appear in the Service Overview workflow under the Dispatch Q and Scheduled Calls buckets. If Auto Dispatch is checked, calls are marked for dispatch automatically. Technicians receive work assignments for their scheduled calls. The system uses the Warning Days setting to generate alerts before each scheduled call.

## Common Issues

**Recurring calls are created but not generating dispatch records**

Dispatch records must be generated separately. The schedule definition alone does not create calls. Use the Generate Recurring Dispatch option from the Extended Menu or Service menu to create actual dispatch records. Check that the Generate Recurring Dispatch background job is enabled if you expect automatic generation.

**Custom frequency does not appear in the Frequency dropdown**

Custom frequencies are defined by the RDBILLCYCL general code table. If your desired frequency is not listed, contact your system administrator to add it to the general codes. You can only select frequencies that are pre-configured in the system.

**Auto Dispatch is checked but calls are not being dispatched automatically**

Auto Dispatch requires that the generate process is run (either manually or via background job) to create the dispatch records. Auto Dispatch does not prevent manual dispatch review or modification. Verify that the background job or manual generation process is executing on schedule.

**Technician field is empty and calls cannot be assigned**

Technician records must be configured in the system. If no technicians appear in the dropdown, create technician records in the Employee or Resource module first. You can leave the Technician field blank if you want to manually assign technicians to generated calls, but including a default technician here streamlines the dispatch process.
