---
title: Create a Sales Lead
id: SALES-LEAD-001
module: Sales
screen: Sales Lead Form
menu_path: Main Menu > Sales > Sales Leads
applies_to:
  - Sales Rep
  - Sales Manager
  - Marketing
prerequisites:
  - SALESLEAD (Create) permission assigned to your user or group
related_procedures:
  - SALES-PROSPECT-001
  - SALES-OPP-001
  - SALES-RPT-011
  - SALES-RPT-012
tags: sales lead, create lead, new lead, lead capture, top of funnel, lead entry, prospect lead, HubSpot lead, lead management, lead conversion
version: 1.0
last_updated: 2026-03-25
---

# Create a Sales Lead

## What This Procedure Does

Captures and tracks a top-of-funnel sales lead in Q360. Leads represent potential business that has not yet been qualified as a prospect or opportunity. They can be entered manually or imported via the HubSpot integration. Once vetted, a lead can be converted to a prospect record and/or opportunity for the sales team to pursue.

## Before You Begin

- You have SALESLEAD (Create) permission.
- You have the lead's company name, contact information, and source details.

## Steps

### Step 1: Open the Sales Leads Form

Navigate to **Main Menu > Sales > Sales Leads**. The Sales Leads grid displays existing leads.

### Step 2: Add a New Lead

Click the **Add New Record** button (plus icon) on the form action bar. A blank Sales Lead form opens.

### Step 3: Fill In the Lead Details

| Field | What to enter |
|---|---|
| Title | A descriptive title for the lead (e.g., "New Office Build - Downtown Tower"). |
| Company | The company name associated with the lead. |
| Contact | The primary contact person's name. |
| Contact Email | The contact's email address. |
| Phone | The primary phone number. |
| Mobile | The mobile phone number, if available. |
| Address | The company's primary address. |
| State | The state or region. |
| Branch | Select the branch location for this lead. |
| Source | Select the lead source (e.g., Website, Trade Show, Referral, Marketing Campaign). |
| Interest | Select the type or level of interest. |
| Annual Revenue | Enter the company's annual revenue if known. |
| SIC | Enter the Standard Industrial Classification code if known. |
| Lead Status | Set the initial status (e.g., New, Assigned). |
| Assigned Salesrep | Select the sales rep responsible for vetting this lead. |
| Close Date | Enter the projected close date if applicable. |
| Reminder | Enter any follow-up notes. |
| Reminder Date | Set a follow-up reminder date. |

### Step 4: Save the Lead

Click the **Save Record** button (floppy disk icon) on the form action bar.

## What Happens Next

The lead is now tracked in Q360 and appears in the Sales Leads report (see SALES-RPT-011). The assigned sales rep can review the lead, make contact, and determine if it qualifies for conversion.

To convert a qualified lead:

1. Create a prospect record from the lead information (see SALES-PROSPECT-001).
2. Create an opportunity on the prospect (see SALES-OPP-001).
3. Update the lead status to reflect its conversion.

The lead's Source value feeds into the Sales Lead Source Report for marketing attribution analysis (see SALES-RPT-012).

If your organization uses the HubSpot integration, leads captured via HubSpot forms are automatically imported into Q360 as sales leads with mapped field values.

## Common Issues

**The Sales Leads menu option is not visible.**
You may lack SALESLEAD permission. Contact your administrator to verify the permission is assigned.

**The Lead Status dropdown has no values.**
Lead statuses are controlled by the LEADSTATUS general code. Contact your administrator to configure status values.

**The Source dropdown is empty.**
Lead source values are populated from data across opportunities, quotes, customers, orders, and invoices. If no source values exist in the system yet, contact your administrator to seed initial values.

**You want to import leads in bulk.**
The HubSpot integration can import leads automatically from HubSpot forms. For manual bulk import, consult your administrator about available import tools or load sheets.

**The lead was converted but still shows as active.**
Update the Lead Status manually after creating the prospect and opportunity. The system does not automatically update the lead status upon prospect creation.
