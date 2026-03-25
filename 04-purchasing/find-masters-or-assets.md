---
title: Find Masters or Assets
id: PO-MASTER-001
module: Purchasing
screen: Find Product
menu_path: Inventory > Find Product
applies_to:
  - Purchasing Agent
  - Warehouse Manager
  - Project Manager
  - Service Manager
prerequisites:
  - User has permission to access the Inventory module
  - At least one master record exists in the system
related_procedures:
  - PO-MASTER-002
  - PO-MASTER-004
  - PO-CREATE-001
tags: find master, search master, find product, find asset, inventory search, master lookup, asset lookup, serial number search, part number search
version: 1.0
last_updated: 2026-03-25
---

# Find Masters or Assets

## What This Procedure Does

Search for inventory master records and serialized assets using the Find Product screen. This allows you to locate items by master number, description, manufacturer, serial number, or asset number to view inventory levels, vendor associations, and item details.

## Before You Begin

- You need view permission for the Inventory module.
- Know at least one identifying detail about the item you are searching for, such as a partial master number, description keyword, manufacturer name, or serial/asset number.

## Steps

### Step 1: Open the Find Product Screen

Navigate to **Inventory > Find Product** from the Main Navigation Sidebar (vertical panel, left edge). The Find Product form opens in a new tab.

### Step 2: Enter Search Criteria

Use the search fields at the top of the form to narrow results.

| Field | What to enter |
| --- | --- |
| Master No | Full or partial master number. Use wildcard characters if needed. |
| Description | Keyword or partial description of the item. |
| Manufacturer | Manufacturer name to filter by a specific brand or supplier. |
| Serial No / Asset No | Exact serial number or asset number for A-type (serialized) items. |
| Master Type | Select a type to filter results: A (Asset), Q (Quantitative), M (Miscellaneous), K (Kit), or leave blank for all types. |

### Step 3: Execute the Search

Click the **Search** button or press **Enter**. The results grid populates with matching master records.

### Step 4: Review Search Results

The grid displays key inventory fields for each matching item:

| Field | What to enter |
| --- | --- |
| Master No | The item's master number identifier. |
| Description | Item description text. |
| On Hand | Total quantity of all inventory across the company. |
| Picked | Quantity on hand that is assigned or reserved for existing jobs. |
| Available | On Hand minus Allocated quantity. |
| On Order | Quantity ordered from vendors but not yet received. |
| Allocated | Quantity on confirmed or approved orders not yet shipped. |
| Vend RMA | Quantity pending vendor replacement via RMA. |
| RMA Test | Quantity of items returned from customers awaiting testing. |

### Step 5: Open a Master Record

Double-click a row in the results grid or highlight the row and press **Enter** to open the full Master Inventory form. From here you can view tabs for vendor associations, alternate items, inventory by branch, and transaction history.

## What Happens Next

The Master Inventory form opens showing all details for the selected item. You can review inventory levels, check vendor pricing, view alternate items on the **Alt. Items** tab, or navigate to related purchase orders. If you need to purchase the item, proceed to the Purchasing workflow (see PO-CREATE-001). If the item does not exist, create a new master record (see PO-MASTER-004).

## Common Issues

**No results returned for a known item.** The search criteria may be too restrictive. Remove one or more filter values and search again. Verify you are searching the correct master type. A-type items require a serial or asset number for precise matches.

**Inventory quantities do not match expectations.** The On Hand figure includes all inventory across branches. Check the branch-level breakdown on the Master Inventory form. Picked and Allocated quantities reduce the Available count, which is the quantity actually free for new orders.

**Cannot find a serialized asset.** Ensure you are entering the serial number or asset number in the correct field. Serial numbers are case-sensitive. If the asset was recently created, confirm the record was saved and refresh the grid using the Refresh Form button (circular arrow icon on the Form Action Bar).

**Master record shows On Order but no PO is visible.** The On Order quantity reflects items on purchase orders in DATAENTRY, CONFIRMED, or APPROVED status. The PO may be assigned to a different branch. Check the PO grid on the Master Inventory form or search for the PO directly in the Purchasing module.

**Search is slow or returns too many results.** Add more specific criteria to narrow the search. Use the Master Type filter to limit results to the relevant item type. Avoid searching with only a single-character wildcard.
