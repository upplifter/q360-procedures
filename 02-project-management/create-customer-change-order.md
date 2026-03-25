---
title: Create Customer Change Order (CCO)
id: PROJ-CCO-001
module: Projects
screen: Project Form > Materials Tab / Orders Tab
menu_path: Main Menu > Projects > Projects
applies_to: Project Manager, Sales Rep
prerequisites: PROJECT (Edit) permission, QUOTE (Create) permission, ORDER (Create) permission, Project exists with materials
related_procedures:
  - PROJ-ICO-001
  - PROJ-CCO-002
  - PROJ-MAT-002
tags:
  - CCO
  - customer change order
  - change order
  - scope change
  - project quote
  - price change
  - customer approval
version: "1.0"
last_updated: 2026-03-25
---

# Create Customer Change Order (CCO)

## What This Procedure Does

This procedure creates a customer change order to propose scope changes, additions, or removals that require customer approval. CCOs start as quotes presented to the customer for authorization. Once approved by the customer, the quote converts to an order that is integrated into the project. CCOs adjust pricing and scope with customer consent.

## Before You Begin

- Verify you have PROJECT (Edit) permission, QUOTE (Create) permission, and ORDER (Create) permission
- Confirm the project exists and has materials on the Materials tab
- Gather details on items to be removed, replaced, or added
- Have pricing information ready for items being added or changed

## Steps for Removing or Replacing Line Items

### Step 1: Look Up the Project

Navigate to the project using Main Menu > Projects > Projects. Search for and open the project record containing the materials to be changed.

### Step 2: Navigate to Materials Tab

Click on the Materials tab to display the project's current materials and line items.

### Step 3: Select Line Items to Change

Select one or more lines that need to be removed or replaced. Click the checkbox next to each line item.

### Step 4: Split Quantity if Needed

If you need to change only a partial quantity of a line item, use the Extended Menu (3 vertical dots) and select the Split function to extract the desired quantity into a separate line.

### Step 5: Create CCO Quote for Selected Items

Click the Extended Menu (3 vertical dots) and select Create CCO Quote for Selected Item(s). Q360 creates a CCO quote containing the selected items.

## Steps for Adding New Line Items

### Step 1: Look Up the Project

Navigate to the project using Main Menu > Projects > Projects. Search for and open the project record.

### Step 2: Navigate to Orders Tab

Click on the Orders tab to display project orders.

### Step 3: Create a New CCO Quote

Click the Add button (plus icon) and choose the CCO option from the dropdown. Q360 creates a new CCO quote record in DATAENTRY status.

## Steps for Completing the CCO Quote

### Step 1: Edit the CCO Quote

Click Edit (pencil icon) on the newly created CCO. The CCO form opens for editing.

### Step 2: Fill in the CCO Title

Enter a descriptive title in the title field that explains the change (e.g., "CCO to add premium materials" or "CCO scope reduction").

### Step 3: Navigate to Line Items Tab

Click on the Line Items tab to view and modify the items in the CCO.

### Step 4: Add Additional Items Using Find Product

To add more items to the CCO, use the Find Product panel on the Line Items tab. Search for products or materials. Select items and adjust quantities and pricing for customer approval. Set unit price (customer price) as what the customer will be charged.

### Step 5: Add RMA Items

For items not in the project Materials grid, use the Find Product subtab at the bottom of the Line Items grid. Add a master record with a negative quantity for items being returned. Use the Add RMA Item button to create the RMA reference.

### Step 6: Preserve Pricing on Changed Items

When coming from Scenario 1 (removing or replacing existing items), do NOT change the quantity, unit cost, or unit price for lines that are being changed out. These fields should reflect the original project pricing for comparison purposes. New items and additions should have their own pricing.

### Step 7: Add More Items to Existing CCO

If the CCO is still in DATAENTRY status, go back to the Materials tab and use the Extended Menu (3 vertical dots) > Add Selected Item(s) to Existing CCO. Select the CCO quote from the dialog.

### Step 8: Save the CCO Quote

Click Save (floppy disk icon) to save all changes to the CCO quote.

### Step 9: Confirm the Quote

Click the Process Actions button (gear icon) and select Confirm. The CCO status changes to confirmed and is ready for authorization.

### Step 10: Authorize the Quote

In the Extended Menu (3 vertical dots), select the Authorize option. This unlocks the quote for submission to the customer.

### Step 11: Submit Quote to Customer

Select the option to submit the quote to the customer. Q360 sends the quote document to the customer's contact email with a request for approval. The quote moves to SUBMITTED status.

### Step 12: Wait for Customer Approval

Monitor the quote status. Once the customer approves the quote through the approval link or by email response, Q360 automatically creates a corresponding order from the approved quote.

### Step 13: Review and Approve the Resulting Order

After customer approval, an order is created from the CCO quote. Review the order record to confirm all items and pricing match the approved quote. Click the Process Actions button (gear icon) to approve the order.

### Step 14: Complete the Integration

Approving the CCO order integrates it into the existing project. The project's materials list, costs, and scope are updated to reflect the customer-approved changes.

## What Happens Next

The approved CCO order updates the project materials, scope, and customer pricing. Items removed with customer approval are noted with credit amounts. Added items are included in the project deliverables. The project revenue is recalculated based on the approved CCO pricing. Customer change orders create an audit trail of scope and price modifications agreed upon by both parties.

## Common Issues

**Create CCO Quote option doesn't appear in Extended Menu**
Verify you have PROJECT (Edit) permission, QUOTE (Create) permission, and ORDER (Create) permission. Confirm at least one line item is selected. Refresh the form using the Refresh button (circular arrow icon).

**Cannot find the product to add in Find Product panel**
Verify the product exists in the product master. Check spelling and product codes. For custom items not in the master, contact your system administrator to add them or create a generic line item with description.

**Customer approval email not sent or customer link doesn't work**
Verify the customer contact has a valid email address in the system. Check that the quote was successfully authorized before submission. If submission failed, confirm internet connectivity and try resubmitting through the Extended Menu.

**Cannot change quantity or pricing on items being removed**
This is intentional. When replacing or removing items from the original project, preserve the original pricing to show what was changed. Only new items and additions should have new pricing information.

**Order created but doesn't show all CCO items**
Verify all items were saved in the CCO quote before customer approval. If items are missing, check that the quote was properly confirmed before submission. Contact your system administrator if items were lost during the conversion from quote to order.

**Customer approved quote but order wasn't created automatically**
Some configurations require manual order creation from approved quotes. Check the quote status to confirm approval was received. You may need to manually create the order from the approved quote using the Extended Menu option.
