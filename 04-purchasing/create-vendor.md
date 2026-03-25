---
title: Create a Vendor
id: PO-VENDOR-001
module: Purchasing
screen: Customer/Vendor Form
menu_path: Accounting > Customer/Vendor
applies_to:
  - Purchasing Agent
  - Accounts Payable Clerk
  - System Administrator
prerequisites:
  - User has permission to create Customer/Vendor records
  - Vendor company name, address, and payment terms are known
related_procedures:
  - PO-MASTER-003
  - PO-CREATE-001
  - PO-DEPOSIT-001
  - PO-SUB-001
tags: create vendor, new vendor, vendor setup, supplier, vendor record, CUSTVEND, vendor payment terms, vendor tax code, vendor banking
version: 1.0
last_updated: 2026-03-25
---

# Create a Vendor

## What This Procedure Does

Create a new vendor (supplier) record in Q360 with company details, payment terms, tax code, and banking information. This record is required before purchase orders or vouchers can be created for the vendor.

## Before You Begin

- You need create permission for the Customer/Vendor form.
- Have the vendor's legal company name, address, phone, and email ready.
- Know the agreed payment terms (e.g., Net 30, Net 60).
- Have the vendor's tax identification number if 1099 reporting is required.
- If the vendor is also a subcontractor, have their license and insurance information available (see PO-SUB-001).

## Steps

### Step 1: Open the Customer/Vendor Form

Navigate to **Accounting > Customer/Vendor** from the Main Navigation Sidebar (vertical panel, left edge). The Customer/Vendor form opens in a new tab.

### Step 2: Add a New Record

Click the **Add New Record** button (plus icon on the Form Action Bar). A blank record form opens.

### Step 3: Set the Record Type

On the **Cust/Vend** tab, set the **Type** field to **CUSTVEND**. This designates the record as a vendor that can receive purchase orders and vouchers. If the company is both a customer and a vendor, CUSTVEND handles both roles in a single record.

### Step 4: Enter Company Information

On the **Company** sub-tab, fill in the vendor's company details.

| Field | What to enter |
| --- | --- |
| Company | The vendor's legal company name. |
| Address | Street address, city, state/province, and postal code. |
| Phone | Primary phone number. |
| Fax | Fax number, if applicable. |
| Website | Vendor's website URL. |

### Step 5: Configure Vendor-Specific Settings

Click the **Vendor** sub-tab and enter vendor payment and tax details.

| Field | What to enter |
| --- | --- |
| Payment Terms | Select the payment terms from the dropdown (e.g., NET30, NET60, DUE ON RECEIPT). |
| Tax Code | Select the applicable tax code for purchases from this vendor. |
| 1099 Flag | Check this box if the vendor requires 1099 reporting. This must be set before any vouchers are created against the vendor. |
| 1099 Number | Enter the vendor's Tax Identification Number (TIN) if 1099 Flag is checked. |
| 1099 Type | Select the 1099 type from the dropdown. For subcontractors, use NONEMP rather than SUB. |
| Currency | Select the vendor's billing currency if different from your company default. |

### Step 6: Enter Banking Information (If Applicable)

If your organization pays this vendor via electronic funds transfer, enter the banking details on the appropriate tab or section as configured by your administrator.

### Step 7: Configure the Vendor Deposit Account (If Applicable)

If you anticipate making vendor deposits (prepayments) on purchase orders for this vendor, navigate to the **Asset** tab and populate the **Vendor Deposit Account** field with the appropriate GL account. This is required before creating vendor deposits (see PO-DEPOSIT-001).

### Step 8: Save the Record

Click the **Save Record** button (floppy disk icon on the Form Action Bar). Q360 assigns a vendor number and saves the record.

## What Happens Next

The vendor is now available for selection when creating purchase orders (see PO-CREATE-001) and when associating vendors with master inventory items (see PO-MASTER-003). Vouchers can be created against this vendor for invoice processing. If the vendor is a subcontractor, proceed to configure subcontractor-specific details (see PO-SUB-001).

## Common Issues

**Cannot create a purchase order for the new vendor.** The record Type must be set to CUSTVEND on the Cust/Vend tab. If it is set to CUSTOMER only, the vendor functionality is not enabled. Edit the record and change the type.

**1099 reporting does not include this vendor.** The 1099 Flag checkbox must be checked before vouchers are created against the vendor. Vouchers created before the flag was set do not retroactively appear on the 1099 report. Check the flag, then verify the 1099 Type is set on each subsequent voucher.

**Vendor does not appear in the vendor dropdown on POs.** Verify the record was saved successfully and the Type is CUSTVEND. If the vendor was just created, try refreshing the form or search using the Form Quick Search (text input at the top-left of the form tab).

**Vendor Deposit option is unavailable.** The Vendor Deposit Account field on the Asset tab must be populated before vendor deposits can be created. Edit the vendor record and enter the appropriate GL account number.

**Payment terms are not applying to vouchers.** Confirm the Payment Terms field on the Vendor sub-tab is set correctly. The terms selected here become the default for new vouchers but can be overridden at the voucher level.
