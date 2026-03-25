---
title: Run the Subcontractor Prospects Report
id: PO-RPT-006
module: Purchasing
screen: Subcontractor Prospects Report
menu_path: Live Data > Subcontractor Prospects
applies_to:
  - Purchasing Manager
  - Operations Manager
prerequisites:
  - User has permission to access Live Data reports
  - Subcontractor prospect records exist in the system (see PO-SUB-001)
related_procedures:
  - PO-SUB-001
  - PO-VENDOR-001
  - PO-RPT-004
  - PO-RPT-005
tags: subcontractor prospects, prospect pipeline, potential subcontractors, subcontractor recruitment, Q0074
version: 1.0
last_updated: 2026-03-25
---

# Run the Subcontractor Prospects Report

## What This Procedure Does

Run a live data report that lists entities identified as potential subcontractors in the PROSPECT stage. The report provides key contact details and last communication information, helping manage the subcontractor recruitment pipeline.

## Before You Begin

- You need permission to access Live Data reports.
- Vendor records must exist with the Subcontractor flag checked and a Type or status of PROSPECT (see PO-SUB-001).

## Steps

### Step 1: Open the Report

Navigate to **Live Data > Subcontractor Prospects** from the Main Navigation Sidebar (vertical panel, left edge). The report loads or a filter screen opens.

### Step 2: Set Report Filters (If Available)

| Field | What to enter |
| --- | --- |
| Branch | Select a branch or leave as ALL. |
| Status | Leave as PROSPECT to see only prospective subcontractors. |

### Step 3: Run the Report

Click **Run Report** or **Search**. The report grid populates with subcontractor prospect records.

### Step 4: Review the Results

The report displays the following key columns:

| Field | What to enter |
| --- | --- |
| Vendor No | The prospect's vendor number in Q360. |
| Company | Prospect company name. |
| Contact Name | Primary contact person. |
| Phone | Contact phone number. |
| Fax | Contact fax number. |
| Email | Contact email address. |
| Branch | Associated branch. |
| Type | Classification type (PROSPECT). |
| SubType | Sub-classification of the prospect. |
| Last Activity Date | Date of the last recorded communication. |
| Contact Person | Person who last contacted the prospect. |
| Activity Type | Type of the last communication activity. |
| Activity Title | Title or subject of the last communication. |

### Step 5: Follow Up on Prospects

Review prospects with stale or missing Last Activity Dates to identify follow-up opportunities. Contact prospects to advance them through the onboarding process toward becoming active subcontractors.

## What Happens Next

As prospects are vetted and approved, update their vendor records to active subcontractor status and configure their insurance, licenses, rates, and skills (see PO-SUB-001). Once fully onboarded, they no longer appear on this prospect report and instead appear on the active subcontractor expiration reports (see PO-RPT-004 through PO-RPT-008). Use the Last Activity information to prioritize outreach to prospects you have not contacted recently.

## Common Issues

**Report returns no results.** No vendor records are flagged as subcontractors with PROSPECT status. Verify that prospect subcontractors have the Subcontractor flag checked and are classified as PROSPECT on their vendor record.

**A subcontractor appears as a prospect but is already active.** The vendor record's type or status may not have been updated when the subcontractor was onboarded. Edit the vendor record and update the classification from PROSPECT to the appropriate active status.

**Last Activity Date is blank for many prospects.** Communication activities have not been logged against these vendor records. Create activities when contacting prospects to maintain an audit trail and enable this report to show current engagement status.

**Need to see prospects by work type or region.** This report shows the prospect pipeline at a summary level. For work type or region detail, open the individual vendor record and review the Skills, Work Types, and Regions tabs (see PO-SUB-001).

**Cannot add a new subcontractor prospect.** Create a vendor record with type CUSTVEND, enable the Subcontractor flag, and set the classification to PROSPECT (see PO-VENDOR-001 and PO-SUB-001).
