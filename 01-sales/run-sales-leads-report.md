---
title: Run the Sales Leads Report
id: SALES-RPT-011
module: Sales
screen: Sales Leads Report
menu_path: Live Data > Sales Leads
applies_to:
  - Sales Rep
  - Sales Manager
prerequisites:
  - Access to Live Data reports
  - Sales leads exist in the system (see SALES-LEAD-001)
related_procedures:
  - SALES-LEAD-001
  - SALES-RPT-012
  - SALES-RPT-013
tags: sales leads, lead report, lead pipeline, lead list, lead status, lead tracking, lead follow-up, lead management
version: 1.0
last_updated: 2026-03-25
---

# Run the Sales Leads Report

## What This Procedure Does

Runs the Sales Leads report to display a comprehensive overview of potential sales leads with key attributes including company and contact details, financial metrics, status indicators, and follow-up reminders. The report enables sales teams to assess lead quality, prioritize follow-up, and track conversion progress.

## Before You Begin

- You have access to Live Data reports.
- Sales leads have been created in the system (see SALES-LEAD-001).

## Steps

### Step 1: Open the Report

Navigate to **Live Data** and select **Sales Leads**.

### Step 2: Set Filters

| Field | What to enter |
|---|---|
| Lead Status | Select one or more lead statuses or leave blank for all. |
| Start Date | Set the beginning of the date range (default is beginning of calendar year). |
| End Date | Set the end of the date range (default is today). |
| Company No. | Select a company or ALL. |
| Branch | Select a branch or ALL. |
| Assigned Salesrep | Select a specific sales rep or ALL. |

### Step 3: Review the Report

The report displays one row per lead with the following columns:

- **Zoom Drilldown** - link to the lead record.
- **Title** - the lead title or subject.
- **CO#** - company number.
- **Branch** - branch location.
- **Date Entered** - when the lead was created.
- **Lead Status** - current progression status.
- **Company** - the company name.
- **Type** - lead classification.
- **Annual Revenue** - the company's annual revenue figure.
- **Address** and **State** - geographic information.
- **Source** - how the lead was generated.
- **Sic** - Standard Industrial Classification code.
- **Contact**, **Contact Email**, **Phone**, **Ext**, **Mobile** - contact details.
- **Interest** - level or type of interest.
- **Close Date** - projected close date.
- **Reminder** and **Reminder Date** - follow-up notes and dates.
- **Salesrep** - the assigned sales representative.

### Step 4: Prioritize and Act

Sort or filter the grid by Lead Status, Reminder Date, or Annual Revenue to prioritize follow-up actions. Click the drilldown link on any row to open the full lead record.

## What Happens Next

Use the report to manage the lead pipeline, ensure timely follow-up, and identify leads ready for conversion to prospects or opportunities. For analysis of lead source effectiveness, see SALES-RPT-012 and SALES-RPT-013.

## Common Issues

**The report returns no leads.**
Adjust the date range - it filters by the lead's Date Entered. Also check the Lead Status filter.

**A lead you created does not appear.**
Verify the lead's Date Entered falls within the filtered Start Date and End Date range. Also check branch and company filters.

**The Annual Revenue column is blank for most leads.**
Annual Revenue is an optional field on the lead record. It only displays if populated during lead creation.

**You need to see leads assigned to a specific rep.**
Use the Assigned Salesrep filter to narrow the view to a single representative.

**Lead statuses do not match your process.**
Lead statuses are controlled by the LEADSTATUS general code. Contact your administrator to review or add status values.
