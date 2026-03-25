---
title: Add Parts or RMA to a Service Call
id: SVC-CALL-011
module: Service
screen: Service Call
menu_path: Service > Service Calls
applies_to: Technicians, CSRs, Field Service Managers
prerequisites:
  - Service call is open with status OPEN, SCHEDULED, or DISPATCHED
related_procedures:
  - SVC-CALL-001
  - SVC-CALL-010
tags:
  - parts management
  - inventory
  - RMA
  - call forms
version: 1.0
last_updated: 2026-03-25
---

# Add Parts or RMA to a Service Call

## What This Procedure Does

Add parts or components to a service call's parts list. Use the Find Product search to locate and add inventory items, or create RMA returns for defective components. Suggested companion items appear automatically to help identify add-on materials.

## Before You Begin

- Open the service call in which you need to add parts
- Know the part number, description, or supplier code for parts you wish to add
- For RMA items, identify the defective component currently on the call

## Steps

### Step 1: Navigate to the Parts Tab

Click the Parts tab on the service call form. The tab displays the current parts list and provides options to add new items.

### Step 2: Add Parts Using Find Product Search

Click the Find Product search button. The Find Product dialog opens.

Enter your search criteria:

| Field | What to enter |
|-------|--------------|
| Part Number | Exact or partial part number |
| Description | Product name or keyword |
| Supplier Code | Supplier part number if known |

Click Search. The system returns matching inventory items with stock levels and pricing.

Select one or more items from the search results. Click ADD TO ORDER. The selected items appear in the Parts tab with default quantities.

### Step 3: Use Suggested Companion Items

The Suggested checkbox column shows items commonly purchased with your selections:

- Green highlighting indicates alternate components
- Blue highlighting indicates suggested add-on items

Review the suggested items. Check the Suggested checkbox for any items you wish to add to the call. Click Save to include them.

### Step 4: Add RMA Items

If a component is defective and requires return, highlight the defective item in the Parts tab. Click ADD RMA ITEM. The system creates a return authorization linked to this call. The RMA generates a corresponding return order for shipment to the vendor.

### Step 5: Save the Call

Click Save (floppy disk icon). The parts list updates, and quantities are reserved or allocated to the call.

## What Happens Next

Added parts appear on the Parts tab with line item details. Stock quantities update in inventory. For RMA items, a return order is generated in the system. If the call is dispatched, the technician receives notification of parts availability. Parts can be billed to the customer on the final invoice (see SVC-CALL-018).

## Common Issues

**Parts do not appear in Find Product search results**

Verify the part number or description spelling. If the item is in inventory but not appearing, check that the location code matches your search scope. Try searching by a portion of the part number or description instead of the full code. Check that the item status is Active in inventory setup.

**Suggested checkbox appears but items are not adding**

Ensure the item has an available stock quantity greater than zero. If stock is zero, the item cannot be added via the Suggested function. Use the Find Product search instead to add items out-of-stock if needed. Save the call after checking Suggested to confirm the addition.

**RMA item creation fails**

Verify the item is marked as returnable in inventory setup. Check that the vendor accepts returns for this product. Ensure the call has an associated customer. If the vendor does not accept returns, the ADD RMA ITEM button may be disabled.
