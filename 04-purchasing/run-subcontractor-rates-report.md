---
title: Run the Subcontractor Rates About to Expire Report
id: PO-RPT-007
module: Purchasing
screen: Subcontractor Rates About to Expire Report
menu_path: Live Data > Subcontractor Rates About to Expire
applies_to:
  - Purchasing Manager
  - Operations Manager
  - Compliance Manager
prerequisites:
  - User has permission to access Live Data reports
  - Subcontractor records exist with rate agreements configured (see PO-SUB-001)
related_procedures:
  - PO-SUB-001
  - PO-RPT-004
  - PO-RPT-005
  - PO-RPT-008
tags: subcontractor rates, rate expiration, rate renewal, subcontractor pricing, expiring rates, rate agreements, Q0075
version: 1.0
last_updated: 2026-03-25
---

# Run the Subcontractor Rates About to Expire Report

## What This Procedure Does

Run a live data report that identifies subcontractors whose service rate agreements are scheduled to expire within a specified number of days. This enables proactive renegotiation of rate agreements before they lapse, preventing billing gaps or unauthorized rate changes.

## Before You Begin

- You need permission to access Live Data reports.
- Subcontractor records must have rate agreements configured with expiration dates (see PO-SUB-001).
- Know the day range you want to check for upcoming expirations.

## Steps

### Step 1: Open the Report

Navigate to **Live Data > Subcontractor Rates About to Expire** from the Main Navigation Sidebar (vertical panel, left edge). The report filter screen opens.

### Step 2: Set Report Filters

| Field | What to enter |
| --- | --- |
| Day Check Start | The starting number of days from today (e.g., 0 for today). |
| Day Check End | The ending number of days from today (e.g., 60 to check rates expiring within 60 days). |
| Status | Filter by rate status or leave as ALL. |
| Branch | Select a branch or leave as ALL. |

### Step 3: Run the Report

Click **Run Report** or **Search**. The report grid populates with subcontractors whose rate agreements expire within the specified window.

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
| Rate Details | Details of the rate agreement approaching expiration. |
| Status | Current status of the rate record. |
| Expiration Date | Date the rate agreement expires. |
| Days to Expiry | Number of days until expiration (negative values indicate already expired). |
| Last Activity | Date and details of the last communication activity. |

### Step 5: Initiate Rate Renewals

Contact subcontractors with upcoming rate expirations to negotiate renewed rate agreements. Update the subcontractor record with new rates and expiration dates when agreements are finalized (see PO-SUB-001).

## What Happens Next

After renegotiating rates, update the rate records on the subcontractor's vendor record with new amounts, effective dates, and expiration dates (see PO-SUB-001). The updated rates are then used for cost estimation on future projects and service calls. Run this report monthly to stay ahead of rate expirations and maintain accurate cost projections.

## Common Issues

**Report returns no results.** The day range may be too narrow, or no rate agreements have expiration dates configured. Increase the Day Check End value and verify subcontractor records have rates with expiration dates.

**Rate expired but subcontractor is still being used.** An expired rate agreement does not prevent the subcontractor from being assigned to work. Update the rate agreement with new terms to ensure accurate cost tracking.

**Multiple rates appear for the same subcontractor.** A subcontractor may have different rates for different types of work (e.g., hourly installation rate vs. daily consulting rate). Each rate agreement is tracked independently.

**Last Activity shows no recent contact.** Log communication activities against the vendor record when reaching out about rate renewals. This maintains a follow-up trail visible on future report runs.

**Need to compare current rates across subcontractors.** This report focuses on expiration timing, not rate comparison. To compare rates, open individual subcontractor records and review their Rates tabs, or export the report data to a spreadsheet for analysis.
