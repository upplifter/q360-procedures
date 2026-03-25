---
title: Update Schedule of Values (SOV)
id: PROJ-SOV-002
module: Projects
screen: Project Form > SOV Tab
menu_path: Main Menu > Projects > Projects
applies_to:
  - Project Manager
  - Accounts Receivable
prerequisites:
  - PROJECT (Edit) permission
  - PROJECTSOV permission
  - SOV exists on the project (see PROJ-SOV-001)
related_procedures:
  - PROJ-SOV-001
  - PROJ-INV-001
  - PROJ-PROFIT-001
tags:
  - update SOV
  - schedule of values
  - completion percentage
  - progress billing
  - billing period
  - SOV update
version: 1.0
last_updated: 2026-03-25
---

# Update Schedule of Values (SOV)

## What This Procedure Does

This procedure allows you to update the progress of SOV line items to reflect work completed in the current billing period. You can enter completed amounts or percentages to track project advancement and drive progress billing and revenue recognition.

## Before You Begin

- Verify you have PROJECT (Edit) permission
- Confirm PROJECTSOV permission is assigned to your role
- Ensure an SOV exists on the project (see PROJ-SOV-001)
- Have current project progress information available for entry

## Steps

### Step 1: Navigate to the SOV Tab
Look up the project in the Projects module. Click on the SOV tab to access the Schedule of Values.

### Step 2: Enter Edit Mode
Click Edit (pencil icon) on the project form to enable editing of SOV data.

### Step 3: Update Progress Using Your Preferred Method
To update progress of one or more SOV line items, use one of the following methods:

a. Enter a monetary amount in the Comp. This Period column, or

b. Enter a percentage value in the Comp. This Period % column, or

c. With SOV items selected, click the Extended Menu (3 vertical dots) and select Set % Complete This Period for Selected Items, or

d. With SOV items selected, click the Extended Menu (3 vertical dots) and select Set Complete This Period to Remaining Balance.

### Step 4: Save Your Changes
Click Save (floppy disk icon) to record the SOV progress updates.

## What Happens Next

Your SOV progress updates are saved and reflected in the project's billing calculations. The updated completion amounts and percentages flow into invoicing and profit reporting, ensuring accurate progress billing for the current period. You can view the impact of these updates in the Project Profitability tab (see PROJ-PROFIT-001).

## Common Issues

**The Comp. This Period columns are not editable.**
Ensure you are in Edit mode by clicking the Edit (pencil icon) on the project form. The SOV grid is read-only outside of Edit mode. If columns remain non-editable after entering Edit mode, verify that you have PROJECT (Edit) permission.

**The Extended Menu option Set % Complete This Period for Selected Items does not appear.**
Verify that you have selected one or more SOV line items before accessing the Extended Menu. The options available in the Extended Menu are contextual and appear only when appropriate items are selected.

**SOV progress updates are not saved after clicking Save.**
After clicking Save, verify that the floppy disk icon is no longer displayed and that the system displays a success confirmation. If updates appear to be lost, check that you are not navigating away from the form before the save operation completes.

**Progress percentages exceed 100% after my entry.**
Verify that the percentage values you enter do not cumulate beyond 100% across billing periods. Enter only the completion percentage for the current period, not the total completion to date. The system does not restrict entries, so manual verification is necessary.

**Cannot set progress for certain line items even when selected.**
Some SOV line items may be locked or in a status that prevents updates. Verify the status of selected line items and confirm they are eligible for progress entry. Contact your system administrator if certain line items remain restricted.
