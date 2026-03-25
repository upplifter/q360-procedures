---
title: Run the Chronic Problem Product Report
id: SVC-RPT-005
module: Service
screen: Chronic Problem Product Report
menu_path: Service > Reports > Chronic Problem Product
applies_to: Service Managers, Operations Staff, Product Engineers
prerequisites:
  - Access to Service Reports
  - Permission to view service call data
  - Service calls must exist with product assignments
related_procedures:
  - SVC-RPT-006
  - SVC-RPT-007
tags:
  - Reports
  - Problem Analysis
  - Product Quality
  - Recurring Issues
version: 1.0
last_updated: 2026-03-25
---

# Run the Chronic Problem Product Report

## What This Procedure Does

The Chronic Problem Product Report identifies products with recurring service issues based on service call history. Use this report to identify quality problems, warranty issues, or products requiring additional support.

## Before You Begin

- Have permission to access Service Reports
- Determine the minimum incident threshold for your analysis
- Decide on the date range for the report

## Steps

### Step 1: Open Chronic Problem Product Report

Go to Service > Reports > Chronic Problem Product. The Print Report dialog opens with filter options.

### Step 2: Set Filter Criteria

Configure filters to define the analysis:

| Field | What to select |
|-------|----------------|
| Company | Select the company |
| Branch | Select the branch (optional) |
| Date Range | Enter start and end dates |
| Minimum Incidents | Enter the threshold (e.g., 3 or more calls) |

The report will only show products with calls exceeding the minimum incidents threshold.

### Step 3: Run the Report

Click Run Report. The report generates and displays in Print Report dialog or Live Data grid.

### Step 4: Review Problem Products

The report displays:

- Product Master No
- Product Description
- Call Count (number of service calls)
- First Call Date
- Most Recent Call Date
- Issues listed (common problem descriptions)

Products are sorted by call count. Summary rows show totals by product category or department.

### Step 5: Investigate High-Problem Products

Focus on products with the highest call counts and narrowest date ranges (indicating concentrated problems). Review individual call records for patterns in problem types, failure modes, or customer impact.

## What Happens Next

Results highlight products requiring engineering review, customer communication, or process improvement. Use the report to justify product redesigns, warranty programs, or customer notifications. Track improvements by re-running the report in future periods.

## Common Issues

**No Products Displayed**
Increase the Minimum Incidents threshold if it was set too high. Expand the date range to include more historical calls. Ensure products are correctly assigned to service calls.

**Threshold Too Low or Too High**
Adjust the Minimum Incidents value to balance between identifying real issues and including noise. Start with 3-5 incidents and adjust based on your data volume.

**Cannot Link to Specific Calls**
Click product name or call count to drill down to individual calls. If drill-through is not available, search for calls manually using the Call History Quick View.
