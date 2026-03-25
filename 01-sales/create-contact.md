---
title: Create a Contact
id: SALES-CONTACT-001
module: Sales
screen: Customer Form - Contacts Tab
menu_path: Main Menu > Sales > Customers > [Look up company] > Contacts Tab
applies_to:
  - Sales Rep
  - Sales Manager
  - Project Manager
  - Service Coordinator
prerequisites:
  - CUSTOMER (View/Edit) permission to open and edit a company record
  - CONTACT (Create) permission assigned to your user or group
  - A company record already exists in Q360 (see SALES-PROSPECT-001)
related_procedures:
  - SALES-PROSPECT-001
  - SALES-SITE-001
  - SALES-OPP-001
tags: contact, create contact, new contact, add contact, person, company contact, customer contact, email, phone, main contact
version: 1.0
last_updated: 2026-03-25
---

# Create a Contact

## What This Procedure Does

Adds a new contact person to an existing company record in Q360 via the Contacts tab. Contacts are the individuals you communicate with at a company. They can be referenced on opportunities, quotes, orders, service calls, and invoices. Adding contacts through the Contacts tab is the standard method when you need to add people beyond the initial main contact created with the prospect record.

## Before You Begin

- You have CUSTOMER (View/Edit) and CONTACT (Create) permissions.
- The company record (prospect, customer, or vendor) already exists in Q360 (see SALES-PROSPECT-001).
- You have the contact's name, and ideally their title, phone number, and email address.

## Steps

### Step 1: Look Up the Company

Navigate to **Main Menu > Sales > Customers**. Type the company name or customer number in the **Form Quick Search** field at the top left of the form tab and press **Enter**. The company record opens.

### Step 2: Open the Contacts Tab

Click the **Contacts** tab in the row of sub-tabs below the company header. The Contacts grid displays all existing contacts for this company.

### Step 3: Add a New Contact

Click the **Grid Add Row** button (plus icon) on the Contacts grid toolbar. A new contact record opens.

### Step 4: Fill In the Contact Fields

Enter the contact's information.

| Field | What to enter |
|---|---|
| First Name | Contact's first name. |
| Last Name | Contact's last name. |
| Title | Contact's job title or role at the company. |
| Phone | Primary phone number. |
| Mobile | Mobile phone number, if available. |
| Email | Contact's email address. This is used for emailing quotes, invoices, and other correspondence through Q360. |
| Site | The site this contact is associated with, if applicable. Select from the dropdown of sites on this company record. |
| Department | The contact's department within their organization, if applicable. |

### Step 5: Save the Contact

Click the **Save Record** button (floppy disk icon) on the form action bar. Q360 assigns a contact number automatically and the new contact appears in the Contacts grid.

## What Happens Next

The new contact is available for selection on any record linked to this company. When creating opportunities, quotes, orders, or service calls, you can select this contact as the primary point of communication.

To set this contact as the company's main contact, go back to the company header tab, click the **Edit Record** button (pencil icon), select the new contact in the **Main Contact** dropdown, and click **Save Record** (floppy disk icon).

To send an email to the contact directly from Q360, click the **Send Email** button (envelope icon) next to the contact's email field. This opens the email composer modal.

## Common Issues

**The Grid Add Row button on the Contacts tab is grayed out.**
The company record may need to be saved first, or you may lack CONTACT (Create) permission. Verify the company record is saved (not in a new unsaved state) and confirm your permissions with your administrator.

**A contact with the same name already exists.**
Q360 allows multiple contacts with the same name because different people can share names. Verify you are not creating a duplicate by reviewing the existing Contacts grid before adding. If you need to distinguish between them, include differentiating information in the Title or Department fields.

**You need to associate the contact with a specific site.**
When filling in the contact record, select the appropriate site from the Site dropdown. If the site does not exist yet, create it first (see SALES-SITE-001), then return to add the contact.

**The contact does not appear in the dropdown on an opportunity or quote.**
The contact must belong to the same company record as the opportunity or quote. Verify the contact was added to the correct company. Also check that you are looking at the correct company record by confirming the customer number.

**You need to remove or deactivate a contact.**
Select the contact row in the Contacts grid and click the **Grid Delete Row** button (trash can icon), or open the contact record and change its status to Inactive. Deleting a contact requires CONTACT (Delete) permission. Contacts linked to existing records (opportunities, calls, invoices) cannot typically be deleted - set them to Inactive instead.
