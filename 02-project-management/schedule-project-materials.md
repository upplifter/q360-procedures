---
title: Schedule or Update Project Materials Requisition
id: PROJ-MAT-001
module: Projects
screen: Project Form > Materials Tab
menu_path: Main Menu > Projects > Projects
applies_to: Project Manager
prerequisites: PROJECT (Edit) permission, Project has line items on the Materials tab
related_procedures:
  - PROJ-MAT-002
  - PROJ-RESOURCE-001
tags:
  - materials
  - requisition
  - PO release date
  - request date
  - purchasing
  - picking
  - material scheduling
  - project materials
version: 1.0
last_updated: 2026-03-25
---

# Schedule or Update Project Materials Requisition

## What This Procedure Does

This procedure sets PO Release Date and Request Date on project materials to control when they are released for purchasing or picking. Setting these dates enables materials to flow into the purchasing and warehouse picking queues at the appropriate time in the project schedule.

## Before You Begin

Ensure you have PROJECT (Edit) permission. The project must have line items already added to the Materials tab. Materials are typically added to projects during the sales order or project setup phase.

## Steps

### Step 1: Open the Project

Navigate to Main Menu > Projects > Projects. Search for and open the desired project.

### Step 2: Navigate to Materials Tab

Click the Materials tab on the project form. The grid displays all line items associated with the project.

### Step 3: Select Material Line Items

In the Materials grid, click on one or more line items that are ready to be released for purchasing or picking. You can select multiple items by clicking while holding the Ctrl key (or Cmd on Mac), or select a range by clicking the first item and Shift-clicking the last item.

### Step 4: Access Set PO Release Date

Click the Materials grid Extended Menu (3 vertical dots). A menu appears with action options for the selected materials.

### Step 5: Set PO Release Date

Click Set PO Release Date from the menu. A date picker dialog opens.

### Step 6: Choose Release Date

Select a current or future date when the material should be released to the purchasing department. Click Okay to apply the date to all selected line items. Materials with a PO Release Date now appear in the Purchasing queue.

### Step 7: Access Set Request Date

Click the Materials grid Extended Menu (3 vertical dots) again. The menu reappears for the same selected items.

### Step 8: Set Request Date

Click Set Request Date from the menu. A date picker dialog opens.

### Step 9: Choose Request Date

Select a future date when the materials are needed on the project site or in the warehouse. This date drives picking and delivery scheduling. Click Okay to apply the request date to all selected line items.

## What Happens Next

Materials with PO Release Dates now appear in the Purchasing queue for the procurement department to process purchase orders. Materials with Request Dates are scheduled for picking and delivery coordination. Track material status and progress using PROJ-MAT-002 to monitor PO status, ETAs, and received dates.

## Common Issues

**Cannot Find Set PO Release Date Option in Extended Menu**
Ensure you have selected one or more line items in the Materials grid before accessing the Extended Menu. The menu options only appear when items are selected. If the option is still missing, verify you have PROJECT (Edit) permission.

**PO Release Date Not Taking Effect or Materials Not Appearing in Purchasing Queue**
After setting the PO Release Date, the materials should appear in the Purchasing queue within a short time. If they do not appear, refresh the Projects view or navigate away and back to the project. Verify the date you selected is the current date or later.

**Request Date Is Set to a Past Date**
The Request Date should always be in the future. If you set it to a past date, the materials will be immediately overdue. Update the Request Date to a realistic future date when the materials will actually be needed.

**Need to Set Dates for Many Materials at Once**
You can select multiple materials at once and set PO Release Date and Request Date for all of them simultaneously. This is more efficient than setting dates individually. Select all items you want to update before accessing the Extended Menu options.

**Materials Appear in Both Purchasing and Picking Queues**
This is normal behavior. Materials with a PO Release Date appear in the Purchasing queue until a purchase order is confirmed. Once the material is received, it appears in the Picking queue. A material can transition between queues as it progresses through its procurement and fulfillment lifecycle.
