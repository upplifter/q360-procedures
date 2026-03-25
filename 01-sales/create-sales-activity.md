---
title: Create a Sales Activity
id: SALES-ACTIVITY-001
module: Sales
screen: Activity Form
menu_path: Main Menu > Sales > Customers > Activities tab (or Opportunity form > Activities tab)
applies_to:
  - Sales Rep
  - Sales Manager
prerequisites:
  - ACTIVITY (Create) permission assigned to your user or group
  - A customer or opportunity record exists (see SALES-PROSPECT-001, SALES-OPP-001)
related_procedures:
  - SALES-OPP-001
  - SALES-RPT-007
  - SALES-RPT-008
  - SALES-RPT-010
tags: sales activity, create activity, log call, log meeting, log email, customer touchpoint, activity record, communication log, sales engagement
version: 1.0
last_updated: 2026-03-25
---

# Create a Sales Activity

## What This Procedure Does

Logs a sales activity record such as a call, email, meeting, or other customer touchpoint against an opportunity or customer record. Activities maintain a communication history, feed into sales reporting (Activity List, Activities by Sales Rep, Sales Score Card), and help track engagement levels across the pipeline.

## Before You Begin

- You have ACTIVITY (Create) permission.
- The customer or opportunity record exists in Q360.
- You know the activity type, date, and details to record.

## Steps

### Step 1: Navigate to the Activity Location

**Option A - From a Customer record:**
Look up the customer from **Main Menu > Sales > Customers**. Click the **Activities** tab on the Customer form.

**Option B - From an Opportunity record:**
Look up the opportunity from **Main Menu > Sales > Opportunities**. Click the **Activities** tab on the Opportunity form.

### Step 2: Add a New Activity

Click the **Grid Add Row** button (plus icon) on the Activities grid. A new Activity form opens.

### Step 3: Fill In the Activity Details

| Field | What to enter |
|---|---|
| Activity Type | Select the type of activity from the dropdown (e.g., Call, Meeting, Email, Task). |
| Title | Enter a brief subject or objective for the activity. |
| Date | Set the date the activity occurred (defaults to today). |
| Contact | Select the customer contact associated with this activity. |
| Sales Rep | Defaults to your user. Change if logging on behalf of another rep. |
| Status | Set the activity status (e.g., Completed, Planned, In Progress). |
| Comment | Enter detailed notes about the activity content, outcomes, and next steps. |
| Follow Up Date | Set a future date for follow-up if needed. |

### Step 4: Save the Activity

Click the **Save Record** button (floppy disk icon) on the form action bar.

## What Happens Next

The activity record is saved and linked to the customer and/or opportunity. It appears in:

- The Activities tab on the Customer and Opportunity forms.
- The **Activity List** report (see SALES-RPT-007).
- The **Activities by Sales Rep - Sales Opp Only** report if linked to an opportunity (see SALES-RPT-008).
- The **Sales Score Card** as part of the Activity Score (see SALES-RPT-010).
- The Last Activity date on the opportunity record in the Sales Forecast quick view.

## Common Issues

**The Activities tab is not visible on the form.**
The Activities tab may be hidden based on your form configuration or permissions. Contact your administrator to verify the ACTIVITY permission is assigned.

**The Activity Type dropdown is empty.**
Activity types are controlled by the ACTTYPE general code. Contact your administrator to verify activity types are configured.

**The activity does not appear in the Activities by Sales Rep report.**
That report only includes activities linked to sales opportunities. If the activity was logged against a customer without an opportunity link, it appears in the Activity List report instead.

**You want to log an activity for a past date.**
Edit the Date field to set it to the correct past date before saving. The activity is recorded with the specified date.

**Emails sent from Q360 do not create activities automatically.**
If the "Save Sent Outlook Email" option is configured and an EMAIL activity type exists in the ACTTYPE general code, emails sent from the Contact record create Contact Activities of type EMAIL automatically. Contact your administrator if this feature is not working.
