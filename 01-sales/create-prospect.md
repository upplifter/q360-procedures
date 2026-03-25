---
title: Create a Prospect
id: SALES-PROSPECT-001
module: Sales
screen: Customer Form
menu_path: Main Menu > Sales > Customers
applies_to:
  - Sales Rep
  - Sales Manager
prerequisites:
  - CUSTOMER (Create) permission assigned to your user or group
  - PROSPECT (Create) permission assigned if "Restrict Customers by Type" is enabled
  - CONTACT (Create) permission assigned to add a primary contact
related_procedures:
  - SALES-SITE-001
  - SALES-CONTACT-001
  - SALES-OPP-001
  - SALES-CUSTOMER-001
tags: prospect, create prospect, new prospect, new company, add prospect, company record, customer form, sales lead, potential customer
version: 1.0
last_updated: 2026-03-25
---

# Create a Prospect

## What This Procedure Does

Creates a new prospect company record in Q360 with a primary address and main contact. This record serves as the starting point for all sales activity - opportunities, quotes, and orders are linked to it. The prospect must later be converted to a Customer type before an order can be booked (see SALES-CUSTOMER-001).

## Before You Begin

- You have CUSTOMER (Create) permission and, if applicable, PROSPECT (Create) permission.
- You have CONTACT (Create) permission to add the primary contact during prospect creation.
- You know the company name, address, and at least one contact name for the prospect.
- You know which Branch and Sales Rep to assign to the prospect.

## Steps

### Step 1: Open the Customer Form

Navigate to **Main Menu > Sales > Customers**. The Customer form opens in the main workspace.

### Step 2: Add a New Record

Click the **Add New Record** button (plus icon) on the form action bar. A blank Customer form opens in edit mode.

### Step 3: Fill In the Header Fields

Enter the prospect's company information in the header fields.

| Field | What to enter |
|---|---|
| Name | The full legal or commonly used company name. |
| Address | The primary street address for the prospect. |
| City | City for the primary address. |
| State | State or province abbreviation. |
| Zip | Postal or ZIP code. |
| Country | Country code if outside the default country. |
| Type | Select **PROSPECT** from the dropdown. |
| Company No. | Select the correct financial entity (defaults to 01 in most configurations). |
| Branch | Select the branch location associated with this prospect. |
| Sales Rep | Select the sales representative responsible for this prospect. |
| SIC | Enter the Standard Industrial Classification code if known. |

### Step 4: Add the Primary Contact

1. Click the **Main Contact** dropdown field and type the contact's full name.
2. Press **Enter**. A popup contact form appears.
3. Fill in the contact details in the popup form.

| Field | What to enter |
|---|---|
| First Name | Contact's first name. |
| Last Name | Contact's last name. |
| Title | Contact's job title. |
| Phone | Primary phone number. |
| Email | Contact's email address. |

4. Click **Confirm** to save the contact and return to the Customer form. The contact now appears in the Main Contact field.

### Step 5: Save the Record

Click the **Save Record** button (floppy disk icon) on the form action bar. Q360 saves the new prospect and assigns a customer number automatically.

## What Happens Next

The prospect record is now available throughout Q360. You can look it up from Main Menu > Sales > Customers or via the Global Search Box at the top of the screen.

From this prospect record you can:

- Add additional sites by clicking the **Sites** tab (see SALES-SITE-001).
- Add additional contacts by clicking the **Contacts** tab (see SALES-CONTACT-001).
- Create a sales opportunity by clicking the **Sales Opps** tab (see SALES-OPP-001).
- Create a quote directly from the **Quotes** tab (see SALES-QUOTE-001).

When the prospect is ready to place an order, Accounting changes the Type from PROSPECT to CUSTOMER and sets payment terms, tax code, and credit information (see SALES-CUSTOMER-001).

## Common Issues

**The Type dropdown does not show PROSPECT.**
Your system may have "Restrict Customers by Type" enabled in Q360Admin > System Config > General tab. Ask your administrator to assign the PROSPECT (Create) permission to your user or group.

**The Save button is grayed out or nothing happens when you click it.**
One or more fields that your system configuration expects are empty. Verify that Name, Type, Branch, and Company No. are filled in. Check the form for any highlighted or flagged fields indicating missing data.

**The Main Contact popup does not appear after pressing Enter.**
Ensure you are typing a new name that does not already exist in the system. If the name matches an existing contact, Q360 may select that contact instead of opening the popup. Clear the field and type a unique name, or add the contact separately from the Contacts tab (see SALES-CONTACT-001).

**You cannot find the prospect after saving.**
The default search on the Customer form may filter to Active customers only. Clear any filters or uncheck the Active Only checkbox above the grid. Also confirm the record was saved by looking for a customer number in the header.

**The Branch dropdown shows no options or is missing your branch.**
Branch options are populated based on the Company No. selected and the branch configuration. Verify the correct Company No. is selected. If your branch still does not appear, contact your administrator to confirm the branch is associated with that company number in Accounting > Admin > Branch and Dept Maintenance.
