---
title: Run the Subcontractor LicenseTypes About to Expire Report
id: PO-RPT-005
module: Purchasing
screen: Subcontractor LicenseTypes About to Expire Report
menu_path: Live Data > Subcontractor LicenseTypes About to Expire
applies_to:
  - Purchasing Manager
  - Operations Manager
  - Compliance Manager
prerequisites:
  - User has permission to access Live Data reports
  - Subcontractor records exist with license types configured (see PO-SUB-001)
related_procedures:
  - PO-SUB-001
  - PO-RPT-004
  - PO-RPT-006
  - PO-RPT-007
  - PO-RPT-008
tags: subcontractor license, license expiration, compliance, license type, expiring license, subcontractor compliance, Q0073
version: 1.0
last_updated: 2026-03-25
---

# Run the Subcontractor LicenseTypes About to Expire Report

## What This Procedure Does

Run a live data report that identifies subcontractors with licenses nearing expiration or recently expired. This enables proactive compliance management by ensuring subcontractors maintain current professional licenses before being assigned work.

## Before You Begin

- You need permission to access Live Data reports.
- Subcontractor records must have license types configured with expiration dates (see PO-SUB-001).
- Know the day range you want to check for upcoming expirations.

## Steps

### Step 1: Open the Report

Navigate to **Live Data > Subcontractor LicenseTypes About to Expire** from the Main Navigation Sidebar (vertical panel, left edge). The report filter screen opens.

### Step 2: Set Report Filters

| Field | What to enter |
| --- | --- |
| Day Check Start | The starting number of days from today to begin checking for expirations (e.g., 0 for today). |
| Day Check End | The ending number of days from today (e.g., 90 to check expirations within the next 90 days). |
| Status | Filter by license status or leave as ALL. |
| Branch | Select a branch or leave as ALL. |

### Step 3: Run the Report

Click **Run Report** or **Search**. The report grid populates with subcontractors whose licenses expire within the specified window.

### Step 4: Review the Results

The report displays the following key columns:

| Field | What to enter |
| --- | --- |
| Vendor No | The subcontractor's vendor number. |
| Company | Subcontractor company name. |
| Contact Name | Primary contact name. |
| Phone | Contact phone number. |
| Fax | Contact fax number. |
| Email | Contact email address. |
| Branch | The branch associated with the subcontractor. |
| SubcontractorType | License type classification. |
| SubcontractorSubType | License sub-type classification. |
| Status | Current status of the license record. |
| Expiration Date | Date the license expires. |
| Days to Expiry | Number of days until expiration (negative values indicate already expired). |
| Last Activity | Date and details of the last communication activity with this subcontractor. |

### Step 5: Take Action on Expiring Licenses

Contact subcontractors with upcoming license expirations to request updated documentation. Update the subcontractor record when new license information is received (see PO-SUB-001).

## What Happens Next

After receiving updated license documentation, update the expiration dates and license numbers on the subcontractor's record (see PO-SUB-001). Run this report on a regular schedule as part of compliance management. Subcontractors with expired licenses may not legally perform certain types of work. The Last Activity column helps track when you last communicated with the subcontractor about their credentials.

## Common Issues

**Report returns no results.** The day range may be too narrow. Increase the Day Check End value. Verify subcontractor records have license types configured with expiration dates.

**Subcontractor's license type is not showing.** Only records flagged as Subcontractors in the vendor record are included. Verify the Subcontractor flag is checked on the vendor's Cust/Vend tab.

**Days to Expiry shows a negative number.** The license has already expired. Contact the subcontractor immediately to obtain a renewed license before assigning new work.

**Last Activity information is blank.** No communication activity has been logged against this subcontractor. After contacting them, create a sales activity or note on the vendor record to track the outreach.

**Need to filter by specific license type.** Use the grid's inline filter row (toggle with the funnel icon on the Grid Toolbar) to filter by SubcontractorType or SubcontractorSubType after the report loads.
