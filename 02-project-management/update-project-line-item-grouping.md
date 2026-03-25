---
title: Update Project Line Items Grouping
id: PROJ-GROUP-001
module: Projects
screen: Project Form > Materials Tab
menu_path: Main Menu > Projects > Projects
applies_to: Project Manager
prerequisites: PROJECT (Edit) permission, Project has line items on the Materials tab
related_procedures:
  - PROJ-SOV-001
  - PROJ-MAT-002
tags:
  - grouping
  - line items
  - material grouping
  - group field
  - categorization
  - project materials
  - Group1
  - Group2
  - project organization
version: "1.0"
last_updated: 2026-03-25
---

# Update Project Line Items Grouping

## What This Procedure Does

This procedure updates the grouping fields on project line items to organize and categorize materials. Grouping fields organize project materials into logical categories such as phase, location, trade, or work type. Grouping facilitates reporting, cost analysis, and project organization.

## Before You Begin

- Verify you have PROJECT (Edit) permission
- Confirm the project has line items on the Materials tab
- Identify which line items need to be regrouped
- Determine the correct grouping values to apply
- Note that grouping column names may vary (typically Group1, Group2, Group3, etc.; check with your system administrator for actual names)

## Steps

### Step 1: Look Up the Project

Navigate to the project using Main Menu > Projects > Projects. Search for and open the project record containing the materials to be regrouped.

### Step 2: Navigate to Materials Tab

Click on the Materials tab to display the project's materials and line items grid.

### Step 3: Locate Grouping Columns

Scroll the grid horizontally to find the grouping columns. Grouping columns are typically named Group1, Group2, Group3, Group4, Group5, but they may have been renamed by your system administrator. Check with your administrator if you cannot locate the standard grouping columns.

### Step 4: Verify Project is Not in Edit Mode

Ensure the project form is NOT in Edit mode (pencil icon should not be active). Grouping updates are made from the Materials tab grid without entering full edit mode on the project. If the project is in Edit mode, click the Form Reset button (CCW curved arrow) to exit edit mode.

### Step 5: Select Line Items to Regroup

Highlight one or more line items within the grouping column you wish to change. Click the checkbox next to each line item to select them. All selected items should be in the same grouping column for consistency.

### Step 6: Open Update Group Fields Dialog

Click the Extended Menu (3 vertical dots) on the grid and select Update Group Fields. A dialog opens allowing you to change the grouping value for the selected items.

### Step 7: Select or Enter Grouping Value

In the dropdown menu, select one of the existing grouping values that are already used in your project. If the desired value already exists in the system, it appears in the list and maintains consistency with other materials.

### Step 8: Add New Grouping Value if Needed

If the desired grouping value does not exist in the dropdown, type the new value into the field and press Enter. Q360 creates and applies the new grouping value to the selected items.

### Step 9: Confirm the Changes

Click Ok to apply the grouping change to all selected line items. The grid updates immediately to show the new grouping values.

## What Happens Next

The updated grouping values are saved to the project materials. Line items are now organized under their new grouping categories. Reports and analysis based on grouping fields reflect the updated organization. Grouping changes facilitate project cost tracking by category and can improve project visibility and management.

## Common Issues

**Grouping columns are not visible in the Materials tab**
Scroll the Materials grid horizontally to locate grouping columns. If columns are not found, contact your system administrator to confirm that grouping columns are enabled in the system configuration. Grouping columns may have been renamed; check the actual column headers in your configuration.

**Cannot select line items for grouping update**
Ensure the project is not in Edit mode. Click the Form Reset button (CCW curved arrow) to exit edit mode if necessary. Verify you have PROJECT (Edit) permission. The checkboxes next to line items should be clickable; if not, refresh the form using the Refresh button (circular arrow icon).

**Update Group Fields option doesn't appear in Extended Menu**
Confirm at least one line item is selected. Verify you have PROJECT (Edit) permission. Refresh the form to reload the menu options using the Refresh button (circular arrow icon).

**New grouping value doesn't appear in dropdown after entering it**
Type the new value carefully and press Enter before closing the dropdown. The system creates the value when you press Enter. If the value still doesn't appear, try entering it again. The value becomes available for future use once created.

**Grouping changes didn't save to the project**
Verify that you clicked Ok to confirm the changes. The grid should update immediately to show the new values. If changes are not visible, refresh the Materials tab using the Refresh button (circular arrow icon). If values still revert, verify you have sufficient permissions and contact your system administrator.

**Need to revert grouping changes**
Select the line items again and use Update Group Fields to change them back to their original grouping values. If you remember the original values, select them from the dropdown. There is no automatic undo for grouping changes, so reselect items and apply the correct grouping manually.
