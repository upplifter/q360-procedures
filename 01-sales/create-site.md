---
title: Create a Site
id: SALES-SITE-001
module: Sales
screen: Customer Form - Sites Tab
menu_path: Main Menu > Sales > Customers > [Look up company] > Sites Tab
applies_to:
  - Sales Rep
  - Sales Manager
  - Project Manager
  - Service Coordinator
prerequisites:
  - CUSTOMER (View/Edit) permission to open and edit a company record
  - SITE (Create) permission assigned to your user or group
  - A company record already exists in Q360 (see SALES-PROSPECT-001)
related_procedures:
  - SALES-PROSPECT-001
  - SALES-CONTACT-001
  - SALES-OPP-001
tags: site, create site, new site, add site, location, address, job site, ship site, bill site, customer site, company address
version: 1.0
last_updated: 2026-03-25
---

# Create a Site

## What This Procedure Does

Adds a new site (physical location or address) to an existing company record in Q360. Sites represent the locations where work is performed, equipment is installed, or invoices are sent. Opportunities, projects, service calls, and invoices all reference a site to determine the job location, shipping destination, and tax jurisdiction.

## Before You Begin

- You have CUSTOMER (View/Edit) and SITE (Create) permissions.
- The company record (prospect, customer, or vendor) already exists in Q360 (see SALES-PROSPECT-001).
- You have the full address and a descriptive name for the new site.

## Steps

### Step 1: Look Up the Company

Navigate to **Main Menu > Sales > Customers**. Type the company name or customer number in the **Form Quick Search** field at the top left of the form tab and press **Enter**. The company record opens.

### Step 2: Open the Sites Tab

Click the **Sites** tab in the row of sub-tabs below the company header. The Sites grid displays all existing sites for this company.

### Step 3: Add a New Site

Click the **Grid Add Row** button (plus icon) on the Sites grid toolbar. A new site record opens in a separate form or inline row, depending on your system configuration.

### Step 4: Fill In the Site Fields

Enter the site details.

| Field | What to enter |
|---|---|
| Name | A descriptive name for the site (e.g., "Main Office", "Warehouse - East"). |
| Address | Street address of the site. |
| City | City where the site is located. |
| State | State or province abbreviation. |
| Zip | Postal or ZIP code for the site. |
| Country | Country code if different from the default. |
| Branch | The branch responsible for this site, if applicable. |
| Tax District | The tax applicable code for this location. This determines how tax is calculated on invoices and orders shipped to this site. |

### Step 5: Save the Site

Click the **Save Record** button (floppy disk icon) on the form action bar. Q360 assigns a site number automatically and the new site appears in the Sites grid on the company record.

## What Happens Next

The new site is available for selection on any record linked to this company, including opportunities, quotes, orders, projects, and service calls. When creating an opportunity or quote, you can select this site as the ship-to or job-site location.

If the site is the company's billing address, it can be designated as the Invoice Site No. on the company header by editing the company record and selecting the new site in the Invoice Site No. field.

To add contacts specific to this site, navigate to the **Contacts** tab (see SALES-CONTACT-001).

## Common Issues

**The Grid Add Row button on the Sites tab is grayed out.**
The company record may be in view mode or unsaved. Click the **Edit Record** button (pencil icon) on the form action bar, save any pending changes, then return to the Sites tab. If the button remains disabled, verify you have SITE (Create) permission.

**The Tax District field is empty or has no options.**
Tax districts are defined in General Codes. Contact your administrator to verify that tax district codes are configured in the system. If your organization uses Avalara AvaTax, tax codes may be managed automatically.

**You need to move a site to a different company.**
Use the extended menu on the Sites tab and select "Move Site to a Different Customer." This action requires the SITEMOVE (Execute) permission.

**The site does not appear when selecting a location on an opportunity or project.**
Verify the site status is set to Active. Inactive sites do not appear in site selection dropdowns on other forms. Open the site record and check its status.

**You entered the wrong address and need to correct it.**
Open the site record from the Sites tab, click the **Edit Record** button (pencil icon), correct the address fields, and click **Save Record** (floppy disk icon). You need SITE (Edit) permission to modify an existing site.
