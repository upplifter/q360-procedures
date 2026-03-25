---
title: Run the Subcontractor WorkTypes About to Expire Report
id: PO-RPT-008
module: Purchasing
screen: Subcontractor WorkTypes About to Expire Report
menu_path: Live Data > Subcontractor WorkTypes About to Expire
applies_to:
  - Purchasing Manager
  - Operations Manager
  - Compliance Manager
prerequisites:
  - User has permission to access Live Data reports
  - Subcontractor records exist with work types configured (see PO-SUB-001)
related_procedures:
  - PO-SUB-001
  - PO-RPT-004
  - PO-RPT-005
  - PO-RPT-007
tags: subcontractor work types, work type expiration, certification, qualification, expiring work types, subcontractor compliance, Q0076
version: 1.0
last_updated: 2026-03-25
---

# Run the Subcontractor WorkTypes About to Expire Report

## What This Procedure Does

Run a live data report that identifies subcontractors whose labor type qualifications or certifications are due to expire within a specified timeframe. This enables proactive management of subcontractor certifications to maintain service continuity and regulatory compliance.

## Before You Begin

- You need permission to access Live Data reports.
- Subcontractor records must have work types configured with expiration dates (see PO-SUB-001).
- Know the day range you want to check for upcoming expirations.

## Steps

### Step 1: Open the Report

Navigate to **Live Data > Subcontractor WorkTypes About to Expire** from the Main Navigation Sidebar (vertical panel, left edge). The report filter screen opens.

### Step 2: Set Report Filters

| Field | What to enter |
| --- | --- |
| Day Check Start | The starting number of days from today (e.g., 0 for today). |
| Day Check End | The ending number of days from today (e.g., 90 to check work types expiring within 90 days). |
| Status | Filter by work type status or leave as ALL. |
| Branch | Select a branch or leave as ALL. |

### Step 3: Run the Report

Click **Run Report** or **Search**. The report grid populates with subcontractors whose work type qualifications expire within the specified window.

### Step 4: Review the Results

The report displays the following key columns:

| Field | What to enter |
| --- | --- |
| Vendor No | The subcontractor's vendor number. |
| Company | Subcontractor company name. |
| Contact Name | Primary contact name. |
| Phone | Contact phone number. |
| Email | Contact email address. |
| Branch | Associated branch. |
| WorkType | Description of the work type qualification. |
| Category | Work type category. |
| Sub-Category | Work type sub-category. |
| Type | Work type classification. |
| SubType | Work type sub-classification. |
| Status | Current status of the work type record. |
| Expiration Date | Date the qualification expires. |
| Days to Expiry | Number of days until expiration (negative values indicate already expired). |
| Last Activity | Date and details of the last communication activity. |

### Step 5: Follow Up on Expiring Qualifications

Contact subcontractors with upcoming work type expirations to request updated certifications or proof of qualification renewal. Update the subcontractor record when new documentation is received (see PO-SUB-001).

## What Happens Next

After receiving updated certification documentation, update the work type expiration dates on the subcontractor's record (see PO-SUB-001). Subcontractors with expired certifications should be reviewed before being assigned to new work requiring those qualifications. Run this report regularly alongside the insurance (see PO-RPT-004), license (see PO-RPT-005), and rates (see PO-RPT-007) reports for comprehensive compliance management.

## Common Issues

**Report returns no results.** The day range may be too narrow, or no work types have expiration dates configured. Increase the Day Check End value and verify subcontractor records have work types with expiration dates set.

**Work type expired but subcontractor was still assigned work.** An expired work type qualification does not automatically block assignment. Review your organization's compliance policy and update the work type record to reflect the current status.

**Multiple work types appear for the same subcontractor.** Subcontractors may hold multiple qualifications (e.g., fire alarm installation, access control, CCTV). Each work type is tracked independently with its own expiration date.

**Cannot distinguish between different types of certifications.** Use the Category, Sub-Category, Type, and SubType columns to differentiate between qualification categories. Apply the grid's inline filter to focus on specific types.

**Last Activity information is outdated.** Log new activities against the vendor record each time you communicate with the subcontractor about their qualifications. This keeps the report's Last Activity column current for follow-up tracking.
