---
title: Create a Service Contract Header
id: SVC-CONTRACT-002a
module: Service
screen: Service Contract
menu_path: Service > Service Contracts > Add
applies_to: Service Managers, Contract Administrators
prerequisites:
  - Customer master record must exist
  - Site must be assigned to the customer
  - Service hours (SLA) profile must be configured
related_procedures:
  - SVC-CONTRACT-002b
  - SVC-CONTRACT-002c
tags:
  - contract creation
  - header
  - setup
version: 1.0
last_updated: 2026-03-25
---

# Create a Service Contract Header

## What This Procedure Does

Creates the header structure of a new service contract by entering contract-level details such as customer, contract type, dates, and service level agreement profile. This establishes the contract shell to which products and line items are added.

## Before You Begin

- A customer master record must already exist in the system
- The customer must have at least one site assigned
- You must have a service hours (SLA) profile configured for the desired coverage window
- You must know the contract type you want to use (warranty, recurring billing, block amount, or T&M)

## Steps

### Step 1: Navigate to Service Contracts

Go to the Service menu and select Service Contracts. The Service Contract list appears. Click the Add button (plus icon) in the toolbar to create a new contract.

### Step 2: Enter Contract Header Information

The new contract form opens with focus on the header section. Fill in the following fields:

| Field | What to enter |
|-------|---------------|
| Customer | Select the customer from the dropdown or lookup |
| Site | Select the site from the dropdown (auto-filtered by customer) |
| Contract Type | Select from the UNIFIEDTYP general code list (warranty, recurring billing, block amount, T&M) |
| Start Date | Enter the contract start date |
| End Date | Enter the contract end date |
| Branch | Select the branch responsible for the contract |
| Department | Select the department responsible for the contract |
| SLA Profile | Select the service hours profile defining coverage and SLA commitments |
| Priority | Select priority level (if applicable) |

### Step 3: Verify and Save

Review all header entries for accuracy. Click the Save button (floppy disk icon) to create the contract shell. The system assigns a contract number and saves the header.

### Step 4: Proceed to Configure the Contract

After saving, the contract form remains open. The Line Items, Billing, Customer Level, and other tabs are now available for configuration. Proceed to add line items and configure additional contract settings.

## What Happens Next

The service contract header is created with status ACTIVE. The contract appears in the Service Overview workflow and the Service Contract list. You must now add products via the Line Items tab (see SVC-CONTRACT-002b), configure billing settings (see SVC-CONTRACT-002c), and assign service rates on the Customer Level tab before the contract is fully operational.

## Common Issues

**Customer or site does not appear in dropdown**

Ensure the customer and site master records exist in the system. The site must be assigned to the selected customer. If records are missing, create them in the Customer or Location modules first, then return to create the service contract.

**SLA Profile is blank or unavailable**

Service hours profiles must be pre-configured in the system. If no profile appears in the dropdown, contact your system administrator to set up a profile with the desired service hours and SLA terms. You can proceed without an SLA profile, but add one later if needed.

**Contract Type selections do not match expected list**

Contract types are defined by the UNIFIEDTYP general code table. If you do not see warranty, recurring billing, block amount, or T&M options, verify that these codes are configured in your system's general code settings or contact your system administrator.
