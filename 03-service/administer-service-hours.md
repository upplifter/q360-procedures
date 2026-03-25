---
title: Administer Service Hours Profile
id: SVC-ADMIN-001
module: Service
screen: Service Hours Administration
menu_path: Accounting > Admin > Service Admin > Service Hours Administration
applies_to: Service Managers, System Administrators
prerequisites:
  - Access to Service Administration menu
  - Understanding of service level agreements and commitments
related_procedures:
  - SVC-ADMIN-002
tags:
  - Service Hours
  - SLA
  - Setup
  - Administration
version: 1.0
last_updated: 2026-03-25
---

# Administer Service Hours Profile

## What This Procedure Does

This procedure creates and maintains Service Hours Profiles that define when service is available, response time commitments, and resolution time commitments for service contracts. These profiles are assigned to contracts to track SLA compliance.

## Before You Begin

- Determine the coverage hours for your service organization
- Identify response time and resolution time commitments
- Have a list of holidays and blackout dates for the year
- Have permission to access Service Administration

## Steps

### Step 1: Open Service Hours Administration

Go to Accounting > Admin > Service Admin > Service Hours Administration. The system displays a list of existing profiles. Click the Add icon (plus sign) to create a new profile, or select an existing profile to edit.

### Step 2: Enter Profile Header Information

On the profile form, fill in the following fields:

| Field | What to enter |
|-------|---------------|
| Title | Enter a descriptive name (e.g., "Standard 8x5 Support") |
| Response Time Commitment | Enter hours for response (e.g., 2 hours, 4 hours) |
| Resolution Time Commitment | Enter hours for resolution (e.g., 24 hours, 48 hours) |

### Step 3: Define Coverage Hours

For each day of the week, enter the coverage start and end times:

| Field | What to enter |
|-------|---------------|
| Monday through Sunday | Enter start and end times (e.g., 8:00 AM to 5:00 PM) |
| Closed Days | Leave blank or mark as closed if no coverage |

### Step 4: Add Exemptions

Click the Exemptions tab to add holidays and blackout dates where the standard hours do not apply. Click Add to insert each exemption:

| Field | What to enter |
|-------|---------------|
| Date | Enter the holiday or blackout date |
| Description | Enter the reason (e.g., "New Year's Day", "Company Holiday") |

### Step 5: Save the Profile

Click Save (floppy disk icon). The profile is now available for assignment to service contracts.

## What Happens Next

The Service Hours Profile is saved in the system. To activate it, assign the profile to service contracts by opening the contract Header tab and selecting this profile in the SLA Profile field. Once assigned, the system will use these hours and commitments to calculate SLA compliance for calls under that contract.

## Common Issues

**Response or Resolution Times Not Calculated Correctly**
Verify that the Service Hours Profile is assigned to the contract in the Header tab SLA Profile field. Check that coverage hours are defined for the day the call was received. Review exemptions to ensure holidays are not incorrectly excluding business days.

**Profile Cannot Be Deleted**
The system prevents deletion of profiles assigned to active contracts. First remove the profile assignment from all contracts, then delete the profile.

**Exemptions Not Being Applied**
Confirm the exemption dates are entered in the correct format. Verify the exemption dates match the specific dates you intend to exclude (not date ranges).
