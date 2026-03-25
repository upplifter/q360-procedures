---
title: Spin Off Service Contract from Project
id: SVC-CONTRACT-001
module: Service
screen: Project
menu_path: Project > Extended Menu > Spin Off Service Contract
applies_to: Service Managers, Project Managers
prerequisites:
  - Project must be in SUBSTCOMP (substantially complete) status
  - Project must have customer and products assigned
related_procedures:
  - SVC-CONTRACT-002a
tags:
  - contract creation
  - warranty
  - project completion
version: 1.0
last_updated: 2026-03-25
---

# Spin Off Service Contract from Project

## What This Procedure Does

Creates a warranty service contract from a substantially complete project. The new contract inherits the project's customer, site, and product details. Use this when a project nears completion and will transition to ongoing service support.

## Before You Begin

- The project must be in SUBSTCOMP status
- The project must have a customer and site assigned
- The project must have billable products in its line items
- You must have access to the Project form and Service menu

## Steps

### Step 1: Verify Project Status

Navigate to the Project form for the project you want to convert. Check the Status field. The project must show SUBSTCOMP (substantially complete) status. If the project is not yet substantially complete, update its status before proceeding.

### Step 2: Access Spin Off Service Contract

From the Project form, click the Extended Menu (three vertical dots) in the toolbar. Select "Spin Off Service Contract" from the menu options.

### Step 3: Confirm Contract Details

Review the information displayed in the spin-off dialog:

| Field | What to enter |
|-------|---------------|
| Customer | Auto-populated from project |
| Site | Auto-populated from project |
| Products | Auto-populated from project line items |
| Start Date | Auto-populated as today's date (can adjust) |

Verify all details are correct, then click Proceed or OK to create the contract.

### Step 4: Review the New Service Contract

The system creates a new service contract and opens its header form. The contract is populated with the project's customer, site, and products as line items. Review the Header, Line Items, and other tabs to ensure all information transferred correctly.

## What Happens Next

The new warranty service contract is created with status ACTIVE. It is linked to the originating project and appears in the Service Overview workflow under Active Contracts bucket. Configure billing, service schedules, and rates on the contract's other tabs as needed. The project record is updated to reference the new service contract.

## Common Issues

**Project status is not SUBSTCOMP**

The spin-off option only appears when the project is in SUBSTCOMP status. Update the project's Status field to substantially complete before attempting the spin-off. This status indicates the project work is nearly finished but not yet fully closed.

**No products appear in the new contract**

The spin-off uses products from the project's Line Items tab. If products are missing, return to the project and verify that billable items are present on its Line Items tab with the appropriate product master records assigned before attempting the spin-off again.

**Contract is created but linked to wrong customer or site**

The contract inherits the project's customer and site at the moment of spin-off. If the project customer or site is incorrect, update the project details first, then either manually correct the new contract or delete it and re-run the spin-off with the corrected project.
