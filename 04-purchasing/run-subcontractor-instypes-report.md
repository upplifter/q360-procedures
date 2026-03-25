---
title: Run the Subcontractor InsTypes About to Expire Report
id: PO-RPT-004
module: Purchasing
screen: Subcontractor InsTypes About to Expire Report
menu_path: Live Data > Subcontractor InsTypes About to Expire
applies_to:
  - Purchasing Manager
  - Operations Manager
  - Compliance Manager
prerequisites:
  - User has permission to access Live Data reports
  - Subcontractor records exist with insurance types configured (see PO-SUB-001)
related_procedures:
  - PO-SUB-001
  - PO-RPT-005
  - PO-RPT-006
  - PO-RPT-007
  - PO-RPT-008
tags: subcontractor insurance, insurance expiration, compliance, insurance type, expiring insurance, subcontractor compliance, Q0072
version: 1.0
last_updated: 2026-03-25
---

# Run the Subcontractor InsTypes About to Expire Report

## What This Procedure Does

Run a live data report that identifies subcontractors with insurance policies nearing expiration within a user-defined timeframe. This enables proactive management of subcontractor compliance by flagging policies that need renewal before they lapse.

## Before You Begin

- You need permission to access Live Data reports.
- Subcontractor records must have insurance types configured with expiration dates (see PO-SUB-001).
- Know the day range you want to check for upcoming expirations.

## Steps

### Step 1: Open the Report

Navigate to **Live Data > Subcontractor InsTypes About to Expire** from the Main Navigation Sidebar (vertical panel, left edge). The report filter screen opens.

### Step 2: Set Report Filters

| Field | What to enter |
| --- | --- |
| Day Check Start | The starting number of days from today to begin checking for expirations (e.g., 0 for today). |
| Day Check End | The ending number of days from today (e.g., 90 to check expirations within the next 90 days). |
| Status | Filter by insurance status (e.g., Active) or leave as ALL. |
| Branch | Select a branch or leave as ALL. |

### Step 3: Run the Report

Click **Run Report** or **Search**. The report grid populates with subcontractors whose insurance policies expire within the specified window.

### Step 4: Review the Results

The report displays the following key columns:

| Field | What to enter |
| --- | --- |
| Vendor No | The subcontractor's vendor number. |
| Company | Subcontractor company name. |
| Contact Name | Primary contact name. |
| Phone | Contact phone number. |
| Email | Contact email address. |
| Insurance Type | The type of insurance policy (e.g., General Liability, Workers Comp). |
| Status | Current status of the insurance record. |
| Expiration Date | Date the insurance policy expires. |
| Days to Expiry | Number of days until expiration (negative values indicate already expired). |

### Step 5: Take Action on Expiring Policies

For each subcontractor with an upcoming expiration, contact them to request updated certificates of insurance. Update the subcontractor record when new documentation is received (see PO-SUB-001).

## What Happens Next

After contacting subcontractors and receiving updated insurance certificates, update the expiration dates on their records (see PO-SUB-001). Run this report regularly - weekly or monthly - as part of your compliance management routine. Subcontractors with expired insurance should not be assigned to new projects or service calls until their coverage is renewed.

## Common Issues

**Report returns no results.** The day range may be too narrow. Increase the Day Check End value to capture a wider window. Also verify that subcontractor records have insurance types configured with expiration dates.

**Subcontractor appears with an already-expired policy.** The Day Check Start value of 0 or a negative number includes already-expired policies. Negative Days to Expiry values indicate the policy has already lapsed. Contact the subcontractor immediately.

**Contact information is missing.** The contact details are pulled from the subcontractor's vendor record. Update the contact information on the Customer/Vendor form if it is incomplete.

**Some insurance types are not appearing.** Verify the Status filter is set to include the relevant statuses. If filtering by Active only, expired or inactive insurance records are excluded.

**Need to track insurance for a subcontractor not in the report.** The subcontractor must have the Subcontractor flag checked on their vendor record and insurance types configured. See PO-SUB-001 to set up insurance tracking.
