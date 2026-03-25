---
title: Create Internal Change Order (ICO)
id: PROJ-ICO-001
module: Projects
screen: Project Form > Materials Tab / Orders Tab
menu_path: Main Menu > Projects > Projects
applies_to: Project Manager, Engineer
prerequisites: PROJECT (Edit) permission, ORDER (Create) permission, Project exists with materials
related_procedures:
  - PROJ-CCO-001
  - PROJ-CCO-002
  - PROJ-MAT-002
tags:
  - ICO
  - internal change order
  - change order
  - cost change
  - project scope
  - add items
  - remove items
  - replace items
  - RMA
version: "1.0"
last_updated: 2026-03-25
---

# Create Internal Change Order (ICO)

## What This Procedure Does

This procedure creates an internal change order to modify project materials and costs internally without customer involvement. ICOs are used to remove project items, replace items with alternatives, or add new items to the project scope. ICOs reflect cost changes that are internal decisions and do not require customer approval.

## Before You Begin

- Verify you have PROJECT (Edit) permission and ORDER (Create) permission
- Confirm the project exists and has materials on the Materials tab
- Gather details on items to be removed, replaced, or added
- Identify whether you are modifying existing line items or adding new items

## Steps for Removing or Replacing Line Items

### Step 1: Look Up the Project

Navigate to the project using Main Menu > Projects > Projects. Search for and open the project record containing the materials to be changed.

### Step 2: Navigate to Materials Tab

Click on the Materials tab to display the project's current materials and line items.

### Step 3: Select Line Items to Change

Select one or more lines that need to be removed or replaced. Click the checkbox next to each line item.

### Step 4: Split Quantity if Needed

If you need to change only a partial quantity of a line item, use the Extended Menu (3 vertical dots) and select the Split function to extract the desired quantity into a separate line. This allows you to change part of an item while keeping the rest intact.

### Step 5: Create ICO for Selected Items

Click the Extended Menu (3 vertical dots) and select Create ICO for Selected Item(s). Q360 creates an ICO order containing the selected items.

## Steps for Adding New Line Items

### Step 1: Look Up the Project

Navigate to the project using Main Menu > Projects > Projects. Search for and open the project record.

### Step 2: Navigate to Orders Tab

Click on the Orders tab to display project orders.

### Step 3: Create a New ICO Order

Click the Add button (plus icon) and choose the ICO option from the dropdown. Q360 creates a new ICO order record.

## Steps for Completing the ICO

### Step 1: Edit the ICO Order

Click Edit (pencil icon) on the newly created ICO. The ICO form opens for editing.

### Step 2: Fill in the ICO Title

Enter a descriptive title in the title field that explains the change (e.g., "ICO to add extra hours" or "ICO to replace contractor labor with staff").

### Step 3: Navigate to Line Items Tab

Click on the Line Items tab to view and modify the items in the ICO.

### Step 4: Add Additional Items

To add more items to the ICO, use the Find Product panel on the Line Items tab. Search for the product or material to be added. Select it and adjust quantity and pricing as needed.

### Step 5: Add RMA Items

For items not found in the project Materials grid, use the Find Product subtab at the bottom of the Line Items grid. To process a return or replacement (RMA), add a master record with a negative quantity for the item being returned. Then use the Add RMA Item button to create the RMA reference.

### Step 6: Add More Items to Existing ICO

If you need to add additional items to the same ICO, go back to the Materials tab and use the Extended Menu (3 vertical dots) > Add Selected Item(s) to Existing ICO. Select the ICO order from the dialog and the items are appended to that ICO.

### Step 7: Save the ICO

Click Save (floppy disk icon) to save all changes to the ICO order.

### Step 8: Process and Approve the ICO

Click the Process Actions button (gear icon). Select the option to confirm and approve the ICO. This finalizes the ICO and integrates it into the project's materials and costs. Once approved, the ICO cannot be reversed without creating an offsetting ICO.

## What Happens Next

The approved ICO updates the project's materials list and costs. Removed items are reflected with negative quantities or separate removal lines. Replaced items are recorded with their new specifications and costs. Added items appear in the materials grid with their associated labor or material costs. The project financials are recalculated to include ICO impacts.

## Common Issues

**Create ICO option doesn't appear in Extended Menu**
Verify you have PROJECT (Edit) permission and ORDER (Create) permission. Confirm you have selected at least one line item. Refresh the form using the Refresh button (circular arrow icon) to reload the menu.

**Cannot find the product to add in the Find Product panel**
Verify the product is set up in the system's product master. Check the product name spelling. If adding a custom item, you may need to create it in the product master first or contact your system administrator.

**RMA Item button is not available or grayed out**
Confirm you've added a master record with negative quantity for the item being returned. The RMA Item button becomes available only after a return line is created. Verify the line item is properly formatted with negative quantity.

**ICO shows in the order list but approval fails**
Check that all required fields in the ICO are completed (title, line items, costs). Verify quantities and unit costs are valid numbers. If validation errors appear, correct them before attempting approval again.

**Need to modify an ICO after approval**
Once approved and integrated, ICOs cannot be directly edited. To reverse or adjust an ICO, create a new offsetting ICO with opposite values (negative quantities for items to remove, etc.) and process it as a new change order.
