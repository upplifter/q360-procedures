---
title: Use Tech Stock on Call
id: SVC-CALL-013
module: Service
screen: Service Call
menu_path: Service > Service Calls
applies_to: Technicians, Field Service Managers
prerequisites:
  - Service call is open and assigned to a technician
  - Technician has inventory allocated in Tech Stock
  - Mobile device or in-field access to the call
related_procedures:
  - SVC-CALL-011
  - SVC-CALL-001
tags:
  - tech inventory
  - field stock
  - parts allocation
  - technician tools
version: 1.0
last_updated: 2026-03-25
---

# Use Tech Stock on Call

## What This Procedure Does

Draw from a technician's assigned field inventory (Tech Stock) to supply parts needed on a service call. Tech Stock represents materials carried by the technician in the field. Selecting items from Tech Stock adds them to the call's parts list and deducts quantities from the technician's inventory.

## Before You Begin

- The service call must be assigned to a technician
- You must be the assigned technician or have field service manager access
- The technician must have items allocated in their Tech Stock inventory
- You need access to the call in the field (mobile device or terminal)

## Steps

### Step 1: Open the Service Call

Open the service call on which you are working or for which you are managing parts.

### Step 2: Access Tech Inventory or Tech Stock

Click the Extended Menu (three vertical dots) on the action bar and select Tech Inventory, or navigate to the Parts tab and look for a Tech Stock function or button. The Tech Stock selection window opens showing the assigned technician's field inventory.

### Step 3: Review Available Tech Stock

The Tech Stock window displays all items allocated to the technician's inventory:

| Column | Meaning |
|--------|---------|
| Item | Part name or description |
| Part Number | System part code |
| Available Qty | Quantity in field stock |
| Unit Cost | Cost per unit |

Review the available quantities. Select items you need for the call.

### Step 4: Select and Enter Quantities

Click on the item you wish to use. Enter the quantity needed to complete the service call. The system shows current stock quantity, preventing you from exceeding available amounts. Enter quantities for all needed items.

### Step 5: Save and Add to Call

Click Save or Add Items to Call. The selected items are added to the call's Parts tab with quantities, and the technician's Tech Stock inventory is reduced by the amounts used.

## What Happens Next

Items appear on the Parts tab with cost and pricing details. The technician's Tech Stock inventory is updated in real-time to reflect the deduction. When the call is closed and invoiced, these parts are billed to the customer at the appropriate markup. The cost of Tech Stock items is tracked against the call for profitability analysis. On the next inventory count, Tech Stock can be replenished for the technician.

## Common Issues

**Tech Stock items are not displaying in the Tech Inventory window**

Verify the technician is assigned to the service call. Check that the technician has an active inventory location and stock allocation in the system. If items should be available but are not showing, refresh the page or close and reopen the call. Contact your service manager to verify Tech Stock allocation for the technician.

**Cannot enter quantity greater than available**

The system prevents over-allocating Tech Stock. If you need more of an item than is available in the technician's field inventory, contact your dispatcher or service manager. They can arrange delivery of additional stock or purchase the item separately for the call.

**Items added to call do not match what I selected**

Verify you clicked Save or Add Items to Call after entering quantities. If incorrect items were added, remove them from the Parts tab and repeat the process. Ensure the correct quantities are entered before saving. If the wrong items continue to be added, try refreshing the call and attempting again.
