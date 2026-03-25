---
title: Scrap an Asset
id: WH-ADJUST-001c
module: Warehouse
screen: Master Form (A-Type) > Asset Tab > Asset Form
menu_path: Inventory > Masters > [search A-type master] > Asset tab > [select asset]
applies_to:
  - Warehouse Manager
prerequisites:
  - Asset is in Available status
  - User has asset management permission
  - Scrap GL account is configured on the master
related_procedures:
  - WH-ADJUST-001b
  - WH-ASSET-001
tags: asset, scrap, A-type, inventory disposal, GL entry
version: 1.0
last_updated: 2026-03-25
---

# Scrap an Asset

## What This Procedure Does

Remove a serialized asset from available inventory by marking it as scrapped. This records the asset as no longer usable and removes it from available inventory, while creating a GL entry to record the scrap loss at cost.

## Before You Begin

- The asset is in Available status (not already scrapped, shipped, or missing)
- The asset is physically present and confirmed to be damaged, unusable, or no longer needed
- You have Warehouse Manager role and asset management permissions
- A scrap GL account is configured on the A-type master for recording disposal cost
- You have approval to scrap the asset if required by your procedures

## Steps

### Step 1: Search and Open the A-Type Master

Navigate to **Inventory > Masters**. Search for the A-type master containing the asset you want to scrap. Use the master number, description, or code.

Click on the master in the search results to open the master form.

### Step 2: Navigate to Asset Tab

On the master form, click the **Asset Tab** to display the list of assets. The asset grid shows all assets associated with this master, including their serial numbers and current statuses.

### Step 3: Select the Asset to Scrap

In the asset grid, locate and click on the asset row you want to scrap. The asset record opens (either inline or in a separate asset form, depending on system interface).

Verify that:

- Serial number matches the asset being scrapped
- Status shows as "Available" (not already scrapped or in another status)
- Location and other details are correct

### Step 4: Access Process Actions

On the asset form, click the **Process Actions** button (gear icon) in the toolbar. A dropdown menu displays available actions for this asset.

### Step 5: Select Scrap Status

From the Process Actions menu, click **Scrap** or **Change Status to Scrapped**. A scrapping confirmation dialog opens.

The dialog displays:

- Asset serial number
- Current status (Available)
- New status (Scrapped)
- Scrap reason field
- GL account that will be used for the scrap entry

### Step 6: Enter Scrap Reason

In the Reason or Comments field, enter a brief explanation for why the asset is being scrapped:

- "Physical damage - not repairable"
- "Failed quality inspection"
- "End of life - obsolete"
- "Unrecoverable loss - warehouse flood"

This reason is recorded in the asset history and GL entries for audit and compliance purposes.

### Step 7: Confirm Scrap

Click the **Save** button (floppy disk icon) or **Confirm** button in the dialog. The system processes the scrap:

1. Asset status changes from "Available" to "Scrapped"
2. Asset is removed from available inventory for allocations and sales
3. GL journal entry is created to record the scrap cost:
   - Debit: Scrap Expense or Disposal account
   - Credit: Inventory account (at average cost)
4. Scrap reason and timestamp are recorded in asset history

The asset form closes or updates to show the new status as "Scrapped".

### Step 8: Verify Scrap Entry

Return to the asset grid. The scrapped asset now shows:

- Status: Scrapped
- No longer available for allocations
- Visible in asset inquiries with scrap notation

## What Happens Next

The scrapped asset is permanently removed from available inventory. The asset:

- Can no longer be allocated to sales orders or shipments
- Appears in asset reports with Scrapped status
- Is included in scrap/disposal reports and historical records
- Has a GL entry recording the cost of disposal for accounting purposes

The scrap GL entry is available for reconciliation and appears in inventory and asset reports.

## Common Issues

**Scrap option is not available or is grayed out**

The asset may not be in Available status. Scrap can only be performed on available assets. Verify the asset status by checking the asset grid. If the status is not "Available":

- Shipped assets cannot be scrapped; manage returns if applicable
- Missing assets may need to be resolved separately
- Check if the asset is in a different status preventing scrap

**System shows error "Scrap GL account not configured"**

The master does not have a scrap GL account assigned. This account is needed to record the scrap cost in the general ledger.

Contact your Accounting or System Administrator to:

- Configure a scrap/disposal GL account on the A-type master
- Verify the GL chart of accounts includes appropriate expense accounts
- Check if a default scrap account is set at the warehouse or master type level

Do not attempt to scrap until the GL account is configured.

**Cannot find the asset in the grid**

Verify the asset serial number is correct. If the asset was recently added, refresh the asset grid view. If the asset is not in the grid:

- Confirm the correct A-type master is open
- The asset may have already been scrapped or processed
- Check the asset serial number spelling and format

**Scrap is processed but inventory and GL entries are not updated**

Verify that scrapping was actually completed by refreshing the asset grid and checking the status. If status shows "Scrapped":

- GL entries should have been created (check GL journal for the entry)
- Inventory availability should update within a few minutes
- Try refreshing inventory inquiry screens to see the update

If the GL entry was not created, contact your system administrator to verify GL posting is configured correctly.

**Need to reverse a scrap entry**

If an asset was scrapped in error, it typically cannot be unscraped through standard procedures. Options include:

- Contact your system administrator to reverse the scrap GL entry
- Create a new asset record with a different serial number if needed
- Document the error in asset history for audit purposes

Establish a change procedure with your Accounting team before attempting to reverse scrap entries.
