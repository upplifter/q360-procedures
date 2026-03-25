---
title: Convert Prospect to Customer
id: SALES-CUSTOMER-001
module: Sales
screen: Customer Form
menu_path: Main Menu > Sales > Customers
applies_to:
  - Accounting
  - AR
  - Sales Manager
prerequisites:
  - CUSTOMER (Edit) permission assigned to your user or group
  - The prospect record exists (see SALES-PROSPECT-001)
  - Payment terms, tax code, and credit information are available
related_procedures:
  - SALES-PROSPECT-001
  - SALES-QUOTE-006
  - SALES-ORDER-001
tags: convert prospect, prospect to customer, change type, customer type, CustVend, payment terms, tax code, credit limit, company type
version: 1.0
last_updated: 2026-03-25
---

# Convert Prospect to Customer

## What This Procedure Does

Changes a prospect company record's type from PROSPECT to CUSTOMER (or CUSTVEND if the company is also a vendor) and sets the required financial fields such as payment terms and tax code. This conversion must happen before a quote can be approved and converted to an order, because Q360 requires the Bill To company to be of type CUSTOMER or CUSTVEND for order creation.

## Before You Begin

- You have CUSTOMER (Edit) permission.
- The prospect record exists in Q360 (see SALES-PROSPECT-001).
- You have the payment terms, tax code, and any credit limit information to configure.

## Steps

### Step 1: Open the Prospect Record

Navigate to **Main Menu > Sales > Customers**. Search for the prospect by name in the **Form Quick Search** field and press **Enter**. Open the prospect record.

### Step 2: Enter Edit Mode

Click the **Edit Record** button (pencil icon) on the form action bar.

### Step 3: Change the Company Type

On the **Cust/Vend** tab (or the main header area, depending on your form layout), locate the **Type** field. Change the value from **PROSPECT** to **CUSTOMER**. If the company is also a vendor, select **CUSTVEND** instead.

### Step 4: Set Financial Fields

Navigate to the appropriate subtab (typically the **Company** subtab under the Cust/Vend tab) and fill in the following fields.

| Field | What to enter |
|---|---|
| Payment Terms | Select the payment terms for this customer (e.g., Net 30, Net 60). |
| Tax Code | Select the applicable tax code for this customer's jurisdiction. |
| Credit Limit | Enter the credit limit, if applicable. |
| Currency | Verify the currency is correct for this customer. |

### Step 5: Save the Record

Click the **Save Record** button (floppy disk icon) on the form action bar.

## What Happens Next

The company record is now of type CUSTOMER (or CUSTVEND). Quotes linked to this company can now be approved and converted to orders (see SALES-QUOTE-006). The customer appears in AR-related forms and reports.

Payment terms and tax code are applied automatically to new invoices generated for this customer.

## Common Issues

**The Type dropdown does not show CUSTOMER.**
Your permissions may restrict the types available. Contact your administrator to verify you have CUSTOMER (Edit) permission and access to the CUSTOMER type.

**You cannot find the Payment Terms or Tax Code fields.**
These fields are typically on the Company subtab under the Cust/Vend tab. If your form layout differs, check other subtabs or contact your administrator for the field location.

**A quote fails to approve after conversion.**
Verify the Type change was saved successfully by reopening the record. Also check that the quote's Bill To field references this company and that the company status is ACTIVE.

**You need to convert the company back to PROSPECT.**
Edit the record and change the Type back to PROSPECT. Be aware that any orders or invoices created while the company was a CUSTOMER will remain in the system.

**The tax code you need is not in the dropdown.**
Tax codes are configured by the administrator. Contact them to verify the correct tax code exists or to create a new one for this customer's jurisdiction.
