---
title: Add a Serialized Asset
id: WH-ADJUST-001b
module: Warehouse
screen: Master Form (A-Type) > Asset Tab
menu_path: Inventory > Masters > [search A-type master] > Asset tab
applies_to:
  - Warehouse Manager
prerequisites:
  - Master is A-type (serialized/asset)
  - Serial number is known and available
  - User has asset management permission
related_procedures:
  - WH-ADJUST-001a
  - WH-ADJUST-001c
  - WH-ASSET-001
tags: asset, serialized, A-type, serial number, inventory
version: 1.0
last_updated: 2026-03-25
---

# Add a Serialized Asset

## What This Procedure Does

Add a new serialized asset record to an A-type (asset) inventory master. This records a physical serialized asset in the system and associates it with the master record, creating a permanent tracking record for the asset.

## Before You Begin

- The master you want to add an asset to is A-type (serialized/asset-based)
- You have the serial number for the asset you are adding
- The asset is physically present and ready to be tracked
- You have Warehouse Manager role and asset management permissions

## Steps

### Step 1: Search and Open the A-Type Master

Navigate to **Inventory > Masters**. Search for the A-type master to which you want to add the asset. Use the master number, description, or code.

Click on the master in the search results to open the master form.

### Step 2: Navigate to Asset Tab

On the master form, click the **Asset Tab** to display the list of assets currently associated with this master. The asset grid shows all previously recorded serial numbers for this master.

### Step 3: Click Add New on Asset Grid

On the asset grid toolbar, click the **Add New** button (plus icon). A new asset row is created in the grid, or an asset entry form opens depending on the system interface.

### Step 4: Enter Asset Serial Number

In the serial number field, type the serial number from the physical asset. The serial number should match exactly as printed or marked on the asset itself.

For example:

- Asset barcode: SN-2024-001234
- Manufacturer serial: ABC-123-XYZ-789

Use the exact format as it appears on the asset.

### Step 5: Enter Asset Details

Depending on your system configuration, you may be prompted to enter additional details:

| Field | What to enter |
|-------|---------------|
| Serial Number | The asset's serial number (required) |
| Location | Warehouse location or bin where the asset is stored |
| Condition | Asset condition (e.g., New, Used, Refurbished) |
| Received Date | Date the asset was received (if not auto-populated) |
| Cost | Unit cost of the asset (if not auto-populated from master) |
| Notes | Any additional information about the asset |

Complete required fields marked with an asterisk (*).

### Step 6: Save the Asset Record

Click the **Save** button (floppy disk icon) to save the new asset record. The system:

1. Creates a new asset record linked to the master
2. Assigns an initial status of "Available"
3. Records the creation date and timestamp
4. Makes the asset available for allocation to sales orders and transactions

The new asset appears in the asset grid with status Available and is now tracked in the system.

## What Happens Next

The newly added asset is now part of the A-type master's inventory. The asset:

- Can be allocated to sales orders and shipments
- Can be tracked and scanned as it moves through the warehouse
- Can have its serial number updated if needed (see WH-ASSET-001)
- Can be scrapped if damaged or no longer usable (see WH-ADJUST-001c)
- Appears in asset inquiry and reporting screens

The asset status will change as transactions occur (e.g., Shipped when included in a shipment, Returned if a return is received).

## Common Issues

**Asset grid shows "Read-only" or does not allow adding new assets**

The master form may be locked or your user role may not have asset edit permissions. Verify that:

- You have the Warehouse Manager role assigned
- The master is not locked or in a status preventing changes
- Your user account has asset management permissions enabled

Try clicking **Edit** (pencil icon) on the master form to enable edit mode if it is available.

**Serial number is rejected as invalid or duplicate**

The serial number either:

- Already exists on this master (cannot have duplicate serial numbers)
- Does not match the expected serial number format for this master type
- Contains invalid characters

Verify the serial number is correct by checking the physical asset. If the serial number is a duplicate, confirm you want to add the same asset or check if it was already recorded.

If the format is invalid, check the master settings for serial number format requirements (e.g., length, character types).

**Cannot find the A-type master**

Verify the master number is correct and the master exists in the system. Confirm the master is A-type (not Q-type). If the master was recently created, refresh the search or try searching with a partial match.

If the master does not exist, it must be created before you can add assets to it.

**Asset status shows as something other than "Available"**

New assets should be created with status "Available". If the status is different:

- Check master settings for default asset status
- The asset may have been created with a non-standard status setting

Contact your system administrator if the default status is incorrect and needs to be changed.

**Location field is required but I do not know the location code**

If a location is required but not specified, check:

- The warehouse location where the asset is physically stored
- The location code in your warehouse/inventory settings
- The asset master configuration for location requirements

Enter the correct warehouse location code or consult your Warehouse Manager for the appropriate location code.
