---
title: View Inventory Levels
id: WH-INV-001
module: Warehouse
screen: Find Product / Inventory Master Valuation Report
menu_path: Inventory > Find Product OR Workflow > Warehouse > On Hand Inventory
applies_to:
  - Purchaser
  - Warehouse Staff
prerequisites:
  - User has access to Inventory module
related_procedures:
  - WH-RPT-001
  - WH-RPT-002
tags: inventory, stock levels, master inventory, on-hand quantities
version: 1.0
last_updated: 2026-03-25
---

# View Inventory Levels

## What This Procedure Does

Check current inventory levels and on-hand quantities for any master product. You can view inventory across branches, track quantities for Q-type items, and verify availability of A-type assets using three different methods.

## Before You Begin

- User has access to the Inventory module
- Product masters exist in the system
- You know the branch(es) you want to check

## Steps

### Method 1: Using Find Product Screen

Navigate to **Inventory > Find Product** to open the Find Product screen.

Enter search criteria in the available fields to locate the product. You can filter by product name, product code, or other identifiers.

Click the product name in the results grid to open the master form.

On the master form, click the **Inventory** tab to view:

| Field | What to enter |
|-------|---------------|
| Branch | Shows each branch with current on-hand inventory |
| On Hand | Quantity available at each branch |
| Committed | Quantity allocated to orders |
| Available | On-hand minus committed |

### Method 2: Using Master Valuation Report

Navigate to **Workflow > Warehouse** and click **On Hand Inventory** to open the Inventory Master Valuation Report.

Use the filter options at the top of the report:

| Filter | What to enter |
|--------|---------------|
| Company | Select the company to view |
| Branch | Select one or more branches |
| Status | Filter by inventory type (Active, Inactive, etc.) |

Click the Grid Filter icon (funnel) to add additional filter criteria such as product category, inventory type, or range.

Click **Refresh** (circular arrow) to update the report with your filter selections.

The report displays all master products with on-hand, committed, and available quantities for each branch.

### Method 3: Using Individual Master Form

Navigate to **Inventory > Masters** and search for the specific master product.

Open the product record by clicking its name in the results.

Click the **Inventory** tab on the master form to view current stock levels by branch and status.

For A-type inventory, the form also shows individual asset records with status (Available, Picked, Shipped, etc.).

For Q-type inventory, quantities are displayed as totals by location and status.

## What Happens Next

The inventory information you view can inform purchasing decisions, order fulfillment, and stock rebalancing between branches. To adjust inventory, proceed to transfer procedures (see WH-TRANSFER-001) or create a physical count (see WH-COUNT-001a).

## Common Issues

**Cannot find the product in search results**
If the product does not appear, verify the master was created before viewing. Use partial name or code search rather than exact matches. Check that the product is not marked as Inactive in the master record.

**On-hand quantity does not match physical stock**
This may indicate missing or incomplete receipts, unrecorded shipments, or inventory discrepancies. Initiate a physical inventory count (see WH-COUNT-001a) to reconcile. Check for pending PO receipts or returns that have not been recorded.

**Inventory shows as committed but order appears unallocated**
Committed inventory reflects picks that have been started but not yet shipped. Once the order ships (see WH-SHIP-001), committed inventory releases and the quantity moves to Available. Check the order status to confirm if items are still in transit.

**Different quantities shown on different screens**
Ensure you are looking at the same branch and date range on each screen. The Find Product screen may show cached data; click Refresh to update. Master Valuation Report filters may exclude certain branches or statuses by default.

**A-type asset status shows as Missing**
Individual asset records flagged as Missing indicate the serial number could not be located during the last count or receipt process. Contact Warehouse Manager to investigate discrepancy and update the asset status (see WH-COUNT-002).
