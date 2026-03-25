---
title: Manage Quote Revisions
id: SALES-QUOTE-002
module: Sales
screen: Quote Form - Revision Tab
menu_path: Main Menu > Sales > Quotes > Revision tab
applies_to:
  - Sales Rep
  - Sales Manager
prerequisites:
  - QUOTE (Edit) permission assigned to your user or group
  - A quote exists (see SALES-QUOTE-001)
related_procedures:
  - SALES-QUOTE-001
  - SALES-QUOTE-003
  - SALES-QUOTE-004
tags: quote revision, revision, baseline, compare revision, restore revision, rename revision, delete revision, version control, quote history
version: 1.0
last_updated: 2026-03-25
---

# Manage Quote Revisions

## What This Procedure Does

Creates, compares, renames, deletes, or restores quote revisions from the Revision tab on the Quote form. Revisions allow you to save snapshots of the quote at different points in time, compare changes between versions, and roll back to a previous version if needed.

## Before You Begin

- You have QUOTE (Edit) permission.
- A quote exists in Q360 (see SALES-QUOTE-001).
- Note the current Revision No. on the Header tab before creating a new revision.

## Steps

### Step 1: Open the Quote

Navigate to **Main Menu > Sales > Quotes**. Search for and open the quote you want to manage revisions on.

### Step 2: Open the Revision Tab

Click the **Revision** tab on the Quote form. The Revisions grid shows any existing revisions for this quote.

### Step 3: Create a New Revision

1. Click the grid **Extended Menu** (three vertical dots).
2. Select **Create Revision from Current**.
3. Enter a revision note or name in the prompt (e.g., "Rev A - Initial Estimate" or "Pre-customer feedback").
4. Click **Submit**.

Q360 saves a snapshot of the current quote contents as a new revision. The Revision No. on the Header tab increments.

### Step 4: View a Revision

To view a saved revision, drill into the revision row in the Revisions grid. A read-only Quote form opens showing the line items and pricing from that snapshot. This view can be printed like any other quote.

### Step 5: Compare Revisions

1. Select a revision in the grid.
2. Click the grid **Extended Menu** and select **Compare With Selected**.
3. Q360 displays a comparison between the current quote and the selected revision, highlighting differences.

### Step 6: Restore a Revision (Replace Current)

1. Select the revision you want to restore.
2. Click the grid **Extended Menu** and select **Replace Current with Revision**.
3. Confirm the action. Q360 overwrites the current quote contents with the selected revision's data.

### Step 7: Rename or Delete a Revision

- To rename: Click the grid **Extended Menu** and select **Rename Revision**. Enter the new name and confirm.
- To delete: Click the grid **Extended Menu** and select **Delete Revision**. Confirm the deletion. This action cannot be undone.

## What Happens Next

Revisions are preserved for historical reference and audit purposes. When you are ready to submit the final version, proceed with authorization (see SALES-QUOTE-003) and customer submission (see SALES-QUOTE-004).

The current Revision No. appears on printed quote documents, allowing customers to identify which version they are reviewing.

## Common Issues

**The Create Revision from Current option is not available.**
Ensure the quote is saved before creating a revision. The revision captures the last saved state of the quote.

**The Replace Current with Revision action removes items you recently added.**
Replacing with a revision fully overwrites the current quote contents. Create a new revision of the current state before replacing to preserve your recent changes.

**You accidentally deleted a revision.**
Revision deletion is permanent and cannot be undone. Always compare revisions before deleting to confirm you are removing the correct version.

**The comparison shows no differences.**
If no changes were made between the current quote and the selected revision, the comparison shows identical data. This can occur if you created a revision immediately after saving without making changes.

**You cannot find the revision you created.**
Check the Revision tab grid. Revisions are listed in order of creation. If the grid appears empty, verify you are looking at the correct quote record.
