---
title: Process a Customer Change Order from the Material Tab
id: PROJ-CCO-002
module: Projects
screen: Project Form > Materials Tab
menu_path: Main Menu > Projects > Projects
applies_to: Project Manager, Sales Rep
prerequisites: PROJECT (Edit) permission, QUOTE (Create) permission, Project has materials on the Materials tab
related_procedures:
  - PROJ-CCO-001
  - PROJ-ICO-001
  - PROJ-MAT-002
tags:
  - CCO
  - material tab
  - scope reduction
  - part substitution
  - change order
  - material change
  - customer change order
version: "1.0"
last_updated: 2026-03-25
---

# Process a Customer Change Order from the Material Tab

## What This Procedure Does

This procedure creates and processes a customer change order (CCO) starting from the project's Materials tab. This approach is useful when you want to make scope reductions, substitute parts, or modify existing materials and need to obtain customer approval for those changes. The CCO is created directly from selected material line items and includes the full authorization and customer approval workflow.

## Before You Begin

- Verify you have PROJECT (Edit) permission and QUOTE (Create) permission
- Confirm the project has materials on the Materials tab
- Identify which materials need to be changed (removed, replaced, or reduced in quantity)
- Gather replacement item information if substituting parts

## Steps

### Step 1: Look Up the Project

Navigate to the project using Main Menu > Projects > Projects. Search for and open the project record containing the materials to be changed.

### Step 2: Access the Materials Tab

Click on the Materials tab to display the project's current materials and line items grid.

### Step 3: Select Line Items to Change

Identify and select the line items that need to be removed, replaced, or modified. Click the checkbox next to each line item you want to change.

### Step 4: Split Quantity if Needed

If only a partial quantity of a line item needs to be changed, use the Extended Menu (3 vertical dots) and select the Split function. This creates a separate line with the partial quantity that you can change independently while keeping the remainder in the original line.

### Step 5: Create CCO Quote for Selected Items

Click the Extended Menu (3 vertical dots) and select Create CCO Quote for Selected Item(s). Q360 creates a new CCO quote record containing the selected material lines. The quote is created in draft status ready for editing.

### Step 6: Drill Into the CCO Quote

Open the CCO quote record to view and modify it. Click Edit (pencil icon) to open the quote for editing.

### Step 7: Add Replacement or Additional Items

Navigate to the Line Items tab. Use the Find Product panel to search for replacement products or additional items needed. Add these items to the CCO quote with appropriate quantities and pricing for customer approval.

### Step 8: Review the Quote Details

Ensure the CCO includes all items being removed, replaced, or added. Verify quantities are correct. Confirm pricing reflects the customer charges for the change order.

### Step 9: Save the CCO Quote

Click Save (floppy disk icon) to save the CCO quote with all selected materials and any additions.

### Step 10: Confirm the Quote

Click the Process Actions button (gear icon) and select Confirm. The CCO moves to confirmed status and is ready for authorization.

### Step 11: Authorize the Quote

Access the Extended Menu (3 vertical dots) and select Authorize. This unlocks the quote for submission to the customer.

### Step 12: Submit Quote to Customer

Select the submit option from the Extended Menu to send the quote to the customer for approval. Q360 sends the quote with a request for customer authorization. Monitor the quote status as it moves to SUBMITTED.

### Step 13: Obtain Customer Approval

Wait for the customer to review and approve the quote. The customer receives the quote via email and can approve it through the provided approval link. Q360 automatically creates a corresponding order once customer approval is received.

### Step 14: Approve the Resulting Order

After customer approval, access the resulting order record created from the approved CCO quote. Review all items and pricing to confirm they match the approved quote. Click the Process Actions button (gear icon) and select Approve to finalize the order.

### Step 15: Complete the Workflow

Approving the CCO order integrates the customer-approved changes into the project. The project's materials, costs, and scope are updated to reflect the approved change order.

## What Happens Next

The approved CCO order becomes part of the project's official record. Items marked for removal are credited to the project. Replacement items appear in the project materials with their approved pricing. The project scope and budget are updated accordingly. All changes are documented with customer approval, creating a clear audit trail of scope modifications.

## Common Issues

**Create CCO Quote option is not visible in Extended Menu**
Verify you have PROJECT (Edit) permission and QUOTE (Create) permission. Confirm at least one line item is selected on the Materials tab. Refresh the form using the Refresh button (circular arrow icon) to reload the menu options.

**CCO quote was created but items are missing**
Verify all items were properly selected before creating the CCO. If critical items are missing, you can add more items to the CCO using the Find Product panel on the Line Items tab while the quote is still in DATAENTRY status.

**Cannot find replacement products in the Find Product panel**
Verify the replacement product is set up in the system's product master. Check the product name and code. If the product doesn't exist, it may need to be added to the product master by your system administrator.

**Customer approval email not received**
Verify the customer contact has a valid email address in the system. Check that the quote was properly authorized and submitted. If submission failed silently, attempt to resubmit through the Extended Menu > Submit option.

**Order created from approved quote but doesn't include all items**
Verify the CCO quote was complete before customer approval. All items should have been added to the quote during the editing phase. If items are unexpectedly missing from the order, contact your system administrator to investigate the quote-to-order conversion process.

**Need to revise the CCO before submitting to customer**
As long as the CCO is in DATAENTRY status, you can click Edit (pencil icon) and modify items, quantities, and pricing. Once confirmed and authorized, some fields may be locked; you may need to cancel the quote and create a new one if substantial revisions are required.
