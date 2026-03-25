---
title: Update Asset Serial Number
id: WH-ASSET-001
module: Warehouse
screen: Master Form (A-Type) > Asset Tab > Asset Form
menu_path: Inventory > Masters > [search A-type master] > Asset tab > [select asset]
applies_to:
  - Warehouse Manager
prerequisites:
  - Asset exists in the system
  - User has asset management permission
  - New serial number is known and available
related_procedures:
  - WH-ADJUST-001b
  - WH-ADJUST-001c
tags: asset, serial number, update, A-type
version: 1.0
last_updated: 2026-03-25
---

# Update Asset Serial Number

## What This Procedure Does

Change the serial number on an existing asset record via the asset form extended menu. Use this when a serial number was entered incorrectly, needs to be corrected due to a recount or verification, or when the asset's actual serial number is discovered to be different from what was initially recorded.

## Before You Begin

- The asset you want to update exists in the system
- You have the correct serial number that should be recorded on the asset
- You have Warehouse Manager role and asset management permissions
- The new serial number is not already used by another asset on the same master

## Steps

### Step 1: Search and Open the A-Type Master

Navigate to **Inventory > Masters**. Search for the A-type master containing the asset whose serial number you want to update. Use the master number, description, or code.

Click on the master in the search results to open the master form.

### Step 2: Navigate to Asset Tab

On the master form, click the **Asset Tab** to display the list of assets. The asset grid shows all assets associated with this master, including their serial numbers and statuses.

### Step 3: Select the Asset to Update

In the asset grid, locate and click on the asset row with the serial number you want to change. The asset record opens (either inline or in a separate asset form).

Verify that this is the correct asset you want to update by checking the current serial number and any other identifying information.

### Step 4: Access Extended Menu

On the asset form, click the **Extended Menu** button (three vertical dots) in the toolbar. A menu appears with additional options for this asset.

### Step 5: Select Update Serial Number

From the Extended Menu, click **Update Serial Number**. A dialog opens to update the serial number.

The dialog displays:

- Current serial number (the old/incorrect number)
- New serial number field (where you enter the correction)
- Optional confirmation message showing the change will be made

### Step 6: Enter New Serial Number

In the new serial number field, type the correct serial number. The new serial number should match exactly as printed or marked on the physical asset.

For example, if correcting from an old number to a new one:

- Old (incorrect) serial: SN-2024-00123
- New (correct) serial: SN-2024-01234

Type the new serial number carefully to match the asset exactly.

### Step 7: Confirm Update

Click the **Save** button (floppy disk icon) or **Confirm** button in the dialog. The system:

1. Validates that the new serial number is not already used on this master
2. Updates the asset record with the new serial number
3. Records the change in asset history with timestamp
4. Makes the change available immediately in the system

A confirmation message appears indicating the serial number has been successfully updated.

### Step 8: Verify the Update

Return to the asset grid. The asset now displays the new serial number in the Serial Number column. Verify that:

- The new serial number is correct and matches the physical asset
- The asset is in the correct status
- Other asset details remain unchanged

## What Happens Next

The asset's serial number is now updated in the system. The asset:

- Is referenced by the new serial number in all future transactions
- Can be tracked, allocated, and shipped using the new serial number
- Appears in asset inquiries and reports with the corrected serial number
- Has the change recorded in its history for audit purposes

## Common Issues

**Update Serial Number option is not available in the Extended Menu**

Your user role may not have asset management permissions. Verify that you have the Warehouse Manager role assigned and asset management permissions are enabled for your account.

Contact your system administrator if permissions need to be granted.

**System rejects the new serial number as invalid or duplicate**

The new serial number either:

- Already exists on this master (each asset must have a unique serial number)
- Does not match the expected serial number format for this master type
- Contains invalid characters or is not allowed

Verify the new serial number is correct by checking the physical asset. If the serial number already exists, confirm whether you should be using a different asset record or serial number.

If the format is invalid, check the master settings for serial number format requirements.

**Cannot find the correct asset in the grid**

Verify the current serial number is correct and the asset exists on this master. If the asset was recently added, refresh the asset grid view. If the asset is not in the grid:

- Confirm the correct A-type master is open
- Search for the asset by a different identifier if available
- Check if the asset may be on a different master

**Update is processed but the change does not appear in the grid**

The change has been saved but the grid may not have refreshed immediately. Refresh the asset grid view by:

- Clicking **Refresh** or **Reload** on the grid toolbar
- Closing and reopening the master form
- Navigating away and back to the master

The new serial number should appear after refresh.

**Need to change serial number for a shipped or unavailable asset**

Serial numbers can typically only be changed when the asset is in available status. If the asset is shipped, missing, or in another status:

- Consider whether the serial number change is necessary while the asset is unavailable
- Document the change need with the current serial number for reference
- Contact your system administrator for options to change serial numbers on non-available assets

Establish a procedure with your Warehouse Manager before attempting changes on assets in other statuses.

**Accidentally updated with wrong serial number**

If the wrong serial number was entered, immediately update it again with the correct one using this same procedure. There is no "undo" function, but serial numbers can be corrected by running the Update Serial Number process again with the correct value.
