---
title: Administer Service Rates Profile
id: SVC-ADMIN-002
module: Service
screen: Service Rate Administration
menu_path: Accounting > Admin > Service Admin > Service Rate Administration
applies_to: Service Managers, Accounting Managers, System Administrators
prerequisites:
  - Access to Service Administration menu
  - Understanding of service call types and pricing
  - Call Type, Category, and Subcategory codes must exist
related_procedures:
  - SVC-ADMIN-001
tags:
  - Service Rates
  - Pricing
  - Discounts
  - Setup
  - Administration
version: 1.0
last_updated: 2026-03-25
---

# Administer Service Rates Profile

## What This Procedure Does

This procedure creates Service Rates Profiles that define discount rules applied to service call time bills and parts based on call type, category, item type, and other factors. These profiles are assigned to contracts to automatically apply the correct discounts.

## Before You Begin

- Determine the discount percentages for each call type and category
- Have a list of applicable item types
- Have permission to access Service Administration
- Ensure Call Type, Category, and Subcategory codes are configured in the system

## Steps

### Step 1: Open Service Rate Administration

Go to Accounting > Admin > Service Admin > Service Rate Administration. The system displays existing profiles. Click the Add icon (plus sign) to create a new profile, or select an existing profile to edit.

### Step 2: Enter Profile Header Information

On the profile form, fill in the following fields:

| Field | What to enter |
|-------|---------------|
| Title | Enter a descriptive name (e.g., "Premium Customer Discount") |

### Step 3: Add Service Rate Details

In the Service Rate Details grid, click the Add icon (plus sign) to add discount rules. For each rule, fill in:

| Field | What to enter |
|-------|---------------|
| Call Type | Select the call type this discount applies to |
| Category | Select the service category |
| Subcategory | Select the subcategory (optional) |
| Master No | Enter a master inventory number if limiting to specific items |
| Item Type | Select the item type (Labor, Material, Subcontractor, etc.) |
| Discount Percentage | Enter the discount percentage (e.g., 10, 15, 20) |

Add multiple rows for different combinations of call types, categories, and item types as needed.

### Step 4: Save the Profile

Click Save (floppy disk icon). The profile is now configured and ready for assignment.

## What Happens Next

The Service Rates Profile is saved in the system. To activate it, go to the service contract > Customer Level tab > Service Rates dropdown and select this profile. Once assigned, discounts are automatically applied when time bills and parts are entered on calls under that contract. Discount percentages reduce the standard rates for matching line items.

## Common Issues

**Discounts Not Appearing on Time Bills or Parts**
Verify the Service Rates Profile is assigned to the contract on the Customer Level tab. Check that the Call Type, Category, and Item Type on the time bill or parts line match the rules defined in the profile. Confirm discount percentages are greater than zero.

**Wrong Discount Applied**
Review the Service Rate Details grid to ensure rules are in the correct priority order. If multiple rules match, the system may apply the first matching rule. Adjust the rule sequence if needed.

**Cannot Delete or Modify Profile**
The system prevents modification of profiles assigned to active contracts. First remove the profile from all contracts, then delete or modify it.
