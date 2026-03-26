---
title: Create a Sales Opportunity
id: SALES-OPP-001
module: Sales
screen: Opportunity Form
menu_path: Main Menu > Sales > Customers > Sales Opps tab
applies_to:
  - Sales Rep
  - Sales Manager
prerequisites:
  - OPPORTUNITY (Create) permission assigned to your user or group
  - A prospect or customer record exists in Q360 (see SALES-PROSPECT-001)
related_procedures:
  - SALES-PROSPECT-001
  - SALES-OPP-002
  - SALES-OPP-003
  - SALES-QUOTE-001
  - SALES-PRESALES-001
tags: opportunity, create opportunity, new opportunity, sales opportunity, sales opp, pipeline, deal, sales opps tab
version: 1.0
last_updated: 2026-03-25
---

# Create a Sales Opportunity

## What This Procedure Does

Creates a new sales opportunity record linked to a company in Q360. The opportunity tracks the potential deal through the sales pipeline and serves as the parent record for quotes, presales labor, and funnel tracking. Once a quote linked to this opportunity is approved by the customer, the opportunity feeds into sales forecasting and booking reports.

## Before You Begin

- You have OPPORTUNITY (Create) permission.
- The prospect or customer record already exists (see SALES-PROSPECT-001).
- You know the estimated value, expected close date, and sale type for the opportunity.

## Steps

### Step 1: Look Up the Company

Navigate to **Main Menu > Sales > Customers**. Type part of the company name in the **Form Quick Search** field at the top left of the Customer form and press **Enter**. Select the correct company from the results.

### Step 2: Open the Sales Opps Tab

Click the **Sales Opps** tab on the Customer form. The Sales Opportunities grid displays any existing opportunities for this company.

### Step 3: Add a New Opportunity

Click the **Grid Add Row** button (plus icon) on the Sales Opps grid toolbar. A new Opportunity form opens.

### Step 4: Fill In the Opportunity Fields

Enter the opportunity details on the Opportunity form header.

| Field | What to enter |
|---|---|
| Title | A descriptive name for the opportunity (e.g., "Main Campus Access Control Upgrade"). |
| Sale Type | Select the type of sale from the dropdown (e.g., Project, Service, Install). |
| Site | Select the site associated with this opportunity, if known. |
| Contact | Select the primary customer contact for this deal. |
| Interest | Select the interest code that categorizes this opportunity (e.g., DES-BUILD, RETROFIT). |
| Source | Select the lead source that generated this opportunity (e.g., Referral, Trade Show, Website). |
| Value | Enter the estimated total revenue value of the opportunity. |
| Close Date | Enter the expected date the deal will close. |
| Sales Rep | Defaults to the company's assigned sales rep. Change if needed. |
| Alt. Sales Rep | Select a secondary sales rep if the deal is shared. |
| Branch | Defaults from the company record. Change if needed. |
| Department | Select the department associated with this opportunity. |

### Step 5: Save the Record

Click the **Save Record** button (floppy disk icon) on the form action bar. Q360 assigns an opportunity number automatically.

## What Happens Next

The opportunity now appears in the Sales Opps grid on the company record and in the **Sales Overview** workflow buckets. From here you can:

- Update the opportunity value, probability, and forecast date as the deal progresses (see SALES-OPP-002).
- Advance the opportunity through funnel steps (see SALES-OPP-003).
- Request presales engineering labor against this opportunity (see SALES-PRESALES-001).
- Create a quote linked to this opportunity from the **Quotes** tab on the Opportunity form (see SALES-QUOTE-001).

The opportunity feeds into the Sales Forecast quick view and other sales reports once probability and value are set.

## Common Issues

**The Grid Add button is grayed out on the Sales Opps tab.**
You may lack OPPORTUNITY (Create) permission. Contact your administrator to verify the permission is assigned to your user or group.

**The Site dropdown shows no options.**
Sites must be created on the company record before they appear in the dropdown. Add a site first from the Sites tab (see SALES-SITE-001).

**The opportunity does not appear in the Sales Forecast report.**
The Sales Forecast quick view filters by probability. Ensure the opportunity has a probability value greater than or equal to the report's minimum threshold (default is 20%). Also confirm the opportunity's Won/Lost status is Active.

**The Sale Type dropdown is empty.**
Sale Type values are controlled by the UNIFIEDTYP general code. Contact your administrator to confirm sale types have been configured.

**You cannot find the opportunity after saving.**
Use the Global Search Box at the top of the screen and type part of the opportunity title or number. You can also navigate to **Main Menu > Sales > Opportunities** and search from the Opportunities grid.
