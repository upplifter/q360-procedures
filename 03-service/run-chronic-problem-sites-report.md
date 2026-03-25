---
title: Run the Chronic Problem Sites Report
id: SVC-RPT-007
module: Service
screen: Chronic Problem Sites Report
menu_path: Service > Reports > Chronic Problem Sites
applies_to: Service Managers, Operations Staff, Facilities Management
prerequisites:
  - Access to Service Reports
  - Permission to view service call data
  - Service calls must exist with site assignments
related_procedures:
  - SVC-RPT-005
  - SVC-RPT-006
tags:
  - Reports
  - Problem Analysis
  - Site Management
  - Recurring Issues
version: 1.0
last_updated: 2026-03-25
---

# Run the Chronic Problem Sites Report

## What This Procedure Does

The Chronic Problem Sites Report identifies customer sites with recurring service issues based on call volume during a specified period. Use this report to focus management attention on problem locations and plan service improvements.

## Before You Begin

- Have permission to access Service Reports
- Determine the minimum incident threshold
- Decide on the date range for analysis
- Identify the company and branch scope

## Steps

### Step 1: Open Chronic Problem Sites Report

Go to Service > Reports > Chronic Problem Sites. The Print Report dialog opens with filter options.

### Step 2: Set Filter Criteria

Configure filters to define the analysis:

| Field | What to select |
|-------|----------------|
| Company | Select the company |
| Branch | Select the branch (optional) |
| Date Range | Enter start and end dates |
| Minimum Incidents | Enter the threshold (e.g., 5 or more calls) |

The report will only show sites with calls exceeding the minimum incidents threshold.

### Step 3: Run the Report

Click Run Report. The report generates and displays in Print Report dialog or Live Data grid.

### Step 4: Review Problem Sites

The report displays:

- Site No
- Site Name
- Customer
- Call Count (total service calls)
- Date of First Call
- Date of Most Recent Call
- Primary Issues (common problem types)

Sites are sorted by call count with highest-problem sites at the top. Summary rows aggregate totals by branch or region.

### Step 5: Investigate and Plan Interventions

For sites with the highest call volumes, plan targeted interventions:
- Review root causes of repeated issues
- Plan preventive maintenance visits
- Upgrade equipment or processes
- Increase SLA or response commitments
- Contact customer for joint problem-solving

## What Happens Next

Results guide resource allocation and customer management strategy. High-problem sites may warrant dedicated technicians, enhanced monitoring, or equipment upgrades. Track improvements by re-running the report after implementing changes.

## Common Issues

**No Sites Displayed**
Increase the Minimum Incidents threshold if set too high. Expand the date range to include more historical calls. Verify sites are correctly assigned to service calls.

**Threshold Too Low Creates Too Many Results**
Increase the Minimum Incidents value (e.g., from 3 to 5) to focus on the most significant problem sites. Alternatively, filter by branch or customer to narrow focus.

**Cannot Drill Into Individual Calls**
Use the Call History Quick View to search for calls by site. Filter by site name or number to find individual call records.
