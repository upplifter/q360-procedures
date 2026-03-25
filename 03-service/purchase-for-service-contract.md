---
title: Purchase for Service Contract
id: SVC-CONTRACT-003
module: Service
screen: Service Contract > Line Items
menu_path: Service Contract > Line Items > Extended Menu > Create PO
applies_to: Service Managers, Purchasing Managers, Procurement Specialists
prerequisites:
  - Service contract must be created with line items
  - Products must be configured with vendor information
  - Purchase order master records must exist in the system
related_procedures:
  - SVC-CONTRACT-002b
  - PO-CREATE-001
tags:
  - purchasing
  - procurement
  - vendor management
version: 1.0
last_updated: 2026-03-25
---

# Purchase for Service Contract

## What This Procedure Does

Creates purchase orders for materials and services required to fulfill a service contract. For standard asset and quantity items, use the normal purchase order cycle. For M-type recurring items, set up vendor recurring purchases to automate replenishment.

## Before You Begin

- Service contract must be created with line items
- Products on the contract must have vendor master records assigned
- You must have access to the Service Contract form and Purchasing workflow
- Vendors must be configured with pricing for the products you want to purchase

## Steps

### Step 1: Navigate to Service Contract Line Items

Open the service contract from Service > Service Contracts. Click the Line Items tab to display the products assigned to the contract.

### Step 2: Identify Products Requiring Purchase

Review the Line Items grid and identify which products require procurement:

- Asset items and quantity items: Use standard purchase order process
- M-type recurring items (block amount contracts): Set up vendor recurring purchases
- Service items with no inventory: May not require purchase orders

Select the line item(s) for which you need to create purchase orders.

### Step 3A: Create Purchase Order for Standard Items

For standard asset and quantity items, click the Extended Menu (three vertical dots) and select "Create PO". The system opens a new purchase order form pre-populated with:

| Field | What is populated |
|-------|-------------------|
| Line Item Detail | Product, quantity, and description from the service contract |
| Vendor | Vendor assigned to the product (if configured) |
| Unit Cost | Standard cost from the product master |

Verify vendor, quantity, and cost. Add additional line items if needed. Proceed with the standard purchase order workflow (see PO-CREATE-001 for details).

### Step 3B: Set Up Recurring Vendor Purchases for M-Type Items

For M-type products in block amount contracts, configure recurring vendor purchases instead of one-time POs. Navigate to the Purchasing module and set up a Recurring Purchase order. Enter:

| Field | What to enter |
|-------|---------------|
| Vendor | Select the vendor supplying the item |
| Product | Select the M-type product |
| Quantity | Enter the quantity per recurring cycle |
| Frequency | Set frequency to match the service contract billing cycle |
| Start Date | Set to contract start date |
| End Date | Set to contract end date |

The system will generate purchase orders automatically on the defined frequency.

### Step 4: Process and Approve Purchase Orders

Once purchase orders are created, route them through your standard approval workflow. This may include:

- Manager approval
- Budget verification
- Vendor verification

Approve the purchase orders in the Purchasing workflow.

### Step 5: Link Purchase Orders to Service Contract

After purchase orders are approved, they are automatically linked to the service contract via the line items. Review the Purchase Order list to confirm the contracts are referenced correctly.

## What Happens Next

Approved purchase orders are transmitted to vendors. When materials are received, goods receipt transactions are recorded against the purchase orders. For M-type recurring items, the system generates recurring purchase orders on the configured schedule. Material costs are tracked against the service contract for profitability analysis.

## Common Issues

**Vendor is not assigned to the product**

Products must have a primary vendor configured in the Product Master module. If no vendor appears when creating a purchase order, navigate to the Product Master, edit the product, and assign a vendor in the Purchasing tab. Then return to create the purchase order.

**Create PO option does not appear in Extended Menu**

The Create PO option only appears for line items with products that support purchasing (asset or quantity items). Service-only or subscription products may not have this option. For those items, create purchase orders manually through the Purchasing menu as needed.

**Recurring purchase setup is not generating purchase orders**

Ensure the Recurring Purchase order Start Date is on or before today's date and the End Date is in the future. The system will generate orders based on the configured frequency. If orders do not generate, check the Purchasing background job settings to ensure recurring purchase processing is enabled. You can also manually trigger purchase order generation from the Purchasing menu.
