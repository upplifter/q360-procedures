---
title: Track Subcontractor Information
id: PO-SUB-001
module: Purchasing
screen: Customer/Vendor Form
menu_path: Accounting > Customer/Vendor
applies_to:
  - Purchasing Agent
  - Purchasing Manager
  - Operations Manager
  - System Administrator
prerequisites:
  - User has SUBCCONSOL permission (view) and relevant SUBC* permissions (create/edit)
  - A vendor record exists for the subcontractor with type CUSTVEND (see PO-VENDOR-001)
related_procedures:
  - PO-VENDOR-001
  - PO-RPT-004
  - PO-RPT-005
  - PO-RPT-006
  - PO-RPT-007
  - PO-RPT-008
tags: subcontractor, subcontractor tracking, insurance, license, rates, skills, regions, compliance, subcontractor management, contractor
version: 1.0
last_updated: 2026-03-25
---

# Track Subcontractor Information

## What This Procedure Does

Log and monitor a subcontractor's skills, licenses, insurance policies, rates, and service regions on their vendor record. This enables compliance tracking so your organization can verify that subcontractors maintain current credentials before assigning them to projects or service calls.

## Before You Begin

- You need the following permissions:
  - **SUBCCONSOL** (view) - to view the subcontractor flag and tab on the Customer/Vendor form.
  - **SUBCLICTYP** - to manage subcontractor license types.
  - **SUBINSTYP** - to manage subcontractor insurance types.
  - **SUBCRATE** - to manage subcontractor rates.
  - **SUBCREGION** - to manage subcontractor regions.
  - **SUBCSKILLS** - to manage subcontractor skills.
- A vendor record must exist for the subcontractor with type CUSTVEND (see PO-VENDOR-001).
- Have the subcontractor's current license numbers, insurance policy details, expiration dates, rate sheets, and service region coverage available.

## Steps

### Step 1: Open the Vendor Record

Navigate to **Accounting > Customer/Vendor** from the Main Navigation Sidebar (vertical panel, left edge). Search for the subcontractor's vendor record using the Form Quick Search (text input at the top-left of the form tab).

### Step 2: Enable the Subcontractor Flag

Click the **Edit Record** button (pencil icon on the Form Action Bar). On the **Cust/Vend** tab, locate the **Subcontractor** flag and check it. This activates the subcontractor-specific tabs and fields on the record. Click **Save Record** (floppy disk icon).

### Step 3: Add Insurance Types

Click the **Subcontractor** tab (or the Insurance sub-tab if organized as sub-tabs). Click the grid **Add** button (plus icon on the Grid Toolbar).

| Field | What to enter |
| --- | --- |
| Insurance Type | Select the type of insurance (e.g., General Liability, Workers Compensation, Auto). |
| Policy Number | The vendor's insurance policy number. |
| Carrier | The insurance company name. |
| Effective Date | Policy start date. |
| Expiration Date | Policy expiration date. This drives the expiration reports. |
| Coverage Amount | The policy coverage limit amount. |
| Status | Set to Active for current policies. |

Repeat for each insurance policy. Click **Save**.

### Step 4: Add License Types

Navigate to the Licenses sub-tab or section. Click the grid **Add** button.

| Field | What to enter |
| --- | --- |
| License Type | Select the license type (e.g., Electrical, Low Voltage, Fire Alarm). |
| License Number | The subcontractor's license number. |
| Category | License category classification. |
| Sub-Category | License sub-category if applicable. |
| Effective Date | License issue date. |
| Expiration Date | License expiration date. This drives the expiration reports. |
| Status | Set to Active for current licenses. |

Repeat for each license. Click **Save**.

### Step 5: Add Skills and Work Types

Navigate to the Skills or Work Types sub-tab. Click the grid **Add** button.

| Field | What to enter |
| --- | --- |
| Work Type | The type of work the subcontractor is qualified to perform. |
| Description | Description of the work type qualification. |
| Category | Work type category. |
| Sub-Category | Work type sub-category. |
| Expiration Date | Date the qualification expires, if applicable. |
| Status | Set to Active for current qualifications. |

Repeat for each skill or work type. Click **Save**.

### Step 6: Add Rates

Navigate to the Rates sub-tab. Click the grid **Add** button.

| Field | What to enter |
| --- | --- |
| Rate Type | The type of rate (e.g., hourly, daily, per project). |
| Rate | The agreed rate amount. |
| Effective Date | Date the rate agreement begins. |
| Expiration Date | Date the rate agreement expires. This drives the expiration reports. |
| Status | Set to Active for current rate agreements. |

Repeat for each rate agreement. Click **Save**.

### Step 7: Add Service Regions

Navigate to the Regions sub-tab. Click the grid **Add** button.

| Field | What to enter |
| --- | --- |
| Region | The geographic region the subcontractor covers. |
| Description | Description of the coverage area. |

Repeat for each service region. Click **Save**.

## What Happens Next

The subcontractor's credentials are now tracked in Q360 with expiration dates. Several reports monitor expiring subcontractor information: Insurance Types (see PO-RPT-004), License Types (see PO-RPT-005), Rates (see PO-RPT-007), and Work Types (see PO-RPT-008). Run these reports regularly to proactively renew or update expiring credentials. The Subcontractor Prospects report (see PO-RPT-006) tracks subcontractors still in the prospect stage. When assigning subcontractors to projects, the system can reference these records to verify compliance.

## Common Issues

**Subcontractor tab is not visible on the vendor record.** You need the SUBCCONSOL permission to see the subcontractor flag and tab. Contact your system administrator to grant this permission.

**Cannot add insurance or license records.** Each data type requires its own permission: SUBINSTYP for insurance, SUBCLICTYP for licenses, SUBCRATE for rates, SUBCSKILLS for skills, and SUBCREGION for regions. Verify you have the appropriate create permission.

**Expiration dates are not triggering report alerts.** The subcontractor expiration reports use a day-check range that you specify when running the report. Ensure you set the day range wide enough to capture upcoming expirations. Also verify the Status field is set to Active - expired or inactive records may be filtered out.

**Subcontractor flag was not checked before adding details.** The Subcontractor flag must be enabled on the Cust/Vend tab before the subcontractor-specific tabs become available. Edit the vendor record, check the flag, save, then proceed to add details.

**1099 type should not be SUB for subcontractors.** When setting up 1099 reporting for a subcontractor, use the 1099 Type of NONEMP rather than SUB. This is a specific Q360 requirement for correct 1099 classification.
