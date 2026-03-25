---
title: Run the Project Material Scheduling Summary Report
id: PROJ-RPT-011
module: Projects
screen: Project Material Scheduling Summary Report
menu_path: Main Menu > Projects > Reports > Project Material Scheduling Summary
applies_to:
  - Project Manager
  - Purchasing Manager
prerequisites:
  - Access to the Projects module
  - Understanding of purchase order processes and material scheduling
  - Access to project material requisition and PO data
related_procedures:
  - PROJ-MAT-001
  - PROJ-MAT-002
tags:
  - material scheduling
  - materials report
  - PO status
  - requisition
  - material summary
  - purchasing schedule
  - project materials
version: "1.0"
last_updated: "2026-03-25"
---

# Run the Project Material Scheduling Summary Report

## What This Procedure Does

The Project Material Scheduling Summary Report reviews project material requisition dates and purchase order (PO) status across projects. It shows PO release dates, request dates, estimated time of arrival (ETA) dates, received dates, and order item status for each project's materials. Use this report to track material procurement progress, identify materials at risk of delay, and ensure project timelines are supported by material availability.

## Before You Begin

- Have access to the Projects module with material tracking permissions
- Know the date range you want to analyze
- Identify any filters you need (company, branch, project type, project manager)
- Understand your organization's purchasing and material receipt processes

## Steps

### Step 1: Navigate to the Project Material Scheduling Summary Report

From the main menu, select **Projects > Reports > Project Material Scheduling Summary**. The report screen displays with filter options.

### Step 2: Set Your Filters

Configure the filters to specify which projects and time period to include in the material schedule review:

| Field | What to enter |
|-------|---------------|
| Company | Select one or more companies, or leave blank for all |
| Branch | Select one or more branches, or leave as ALL for all branches |
| Project Type | Select one or more project types, or leave as ALL for all types |
| Project Manager | Select one or more project managers, or leave as ALL |
| Date Range | Enter the start and end dates for the analysis period |

### Step 3: Click Run

Click the **Run** button to execute the report.

### Step 4: Review the Report Output

The report displays a grid with one row per material item. Columns typically include:

- **Project Name/ID:** The project requiring the material
- **Material Description:** Item name and specification
- **Material Quantity:** Number of units requested
- **Request Date:** When the material was requisitioned from the project
- **PO Release Date:** When the purchase order was released to the vendor
- **PO Number:** The purchase order reference number
- **ETA (Estimated Time of Arrival):** When the material is expected to arrive at the site
- **Received Date:** When the material was actually received (if received)
- **Order Status:** Current status (Ordered, In Transit, Received, Cancelled, etc.)
- **Days Until Due:** Days remaining until the ETA (if not yet received)

### Step 5: Identify Critical Materials

Look for materials that require immediate attention:

- **Overdue Materials:** Materials with received dates past the ETA or with ETAs approaching the current date
- **At-Risk Materials:** Materials ordered late or with short lead times between request and ETA
- **Long Lead Time Items:** Materials with significant gaps between request and ETA, indicating early planning

### Step 6: Check Material Status

Review the Order Status column to identify:

- **Cancelled Orders:** Materials that were requisitioned but the order was cancelled (may indicate scope reduction or substitution)
- **In-Transit Status:** Materials on the way but not yet received (verify ETAs are still realistic)
- **Received Status:** Materials already on-site and available for use

### Step 7: Assess Project Impact

For any materials at risk of delay:

- Determine the impact on the project schedule (whether the material is on the critical path)
- Contact the vendor to verify actual delivery dates and expedite if necessary
- Identify alternative materials or sources if the primary material will be delayed
- Notify the project manager and affected trades or work crews

### Step 8: Export or Print (Optional)

Use the export or print functions to save the report as Excel, PDF, or hardcopy for distribution to purchasing and project teams.

## What Happens Next

After reviewing the Project Material Scheduling Summary Report, you may:

- Contact vendors to verify or expedite delivery of at-risk materials
- Revise project schedules to accommodate material delays
- Identify alternative suppliers or materials if necessary
- Brief the project team on material status and any constraints
- Update material requisitions or purchase orders as needed
- Run detailed material reports (PROJ-MAT-001 or PROJ-MAT-002) for deeper analysis

## Common Issues

**The report shows no materials or very few items**

Verify that materials have been requisitioned and purchase orders created. If projects are in early stages or material procurement has not yet begun, the report may be empty. Check with the purchasing department to confirm whether material orders have been released.

**All materials show a Received status with no ETA dates**

This is normal for projects where all materials have already been delivered. If you want to monitor future material needs, adjust your date range to look ahead to upcoming project phases or future projects.

**A material shows an ETA date in the past but no Received date**

This indicates the material is overdue and has not been received. Contact the vendor immediately to determine the cause and actual delivery date. This material may impact the project schedule and requires urgent follow-up.

**The Request Date is much earlier than the PO Release Date**

A gap between request and PO release indicates the material was requisitioned but the PO was not immediately released to the vendor. This delay increases the risk of late delivery. Investigate whether purchasing was slow to act or whether the delay was intentional (e.g., awaiting customer approval or budget confirmation).

**I see materials for cancelled projects**

Cancelled projects may remain in the report if orders were not explicitly cancelled in the system. Check the project status and, if the project was cancelled, verify whether the associated purchase orders were also cancelled. If not, contact purchasing to cancel outstanding orders.

**The material descriptions are too brief or technical**

If descriptions are unclear, refer to the PO numbers or project documentation for complete specifications. Alternatively, contact the project manager or purchasing department for clarification on specific materials.
