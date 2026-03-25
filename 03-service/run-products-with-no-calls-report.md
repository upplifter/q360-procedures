---
title: Run the Products With No Calls Report
id: SVC-RPT-006
module: Service
screen: Products With No Calls Report
menu_path: Service > Reports > Products With No Calls
applies_to: Service Managers, Sales Managers, Product Support
prerequisites:
  - Access to Service Reports
  - Permission to view product and service call data
  - Products and service calls must exist in the system
related_procedures:
  - SVC-RPT-005
  - SVC-RPT-007
tags:
  - Reports
  - Product Analysis
  - Service Opportunities
  - Utilization
version: 1.0
last_updated: 2026-03-25
---

# Run the Products With No Calls Report

## What This Procedure Does

The Products With No Calls Report identifies products with no service calls logged during a specified period. Use this report to find under-serviced assets, identify service opportunities, or validate data completeness.

## Before You Begin

- Have permission to access Service Reports
- Determine the date range for analysis
- Identify customer or company filters if needed
- Have a list of products expected to be in service

## Steps

### Step 1: Open Products With No Calls Report

Go to Service > Reports > Products With No Calls. The Print Report dialog opens with filter options.

### Step 2: Set Filter Criteria

Configure filters to define the analysis:

| Field | What to select |
|-------|----------------|
| Company | Select the company |
| Customer | Select customer (optional) |
| Date Range | Enter start and end dates for the analysis period |

### Step 3: Run the Report

Click Run Report. The report generates and displays in Print Report dialog or Live Data grid.

### Step 4: Review Products Without Service Calls

The report displays:

- Product Master No
- Product Description
- Customer who owns/uses the product
- Product Type
- Installation Date
- Last Service Call (if any)

Products are listed without calls in the selected period. Cross-reference with your customer contracts to identify if these products should be under service agreements.

### Step 5: Analyze Results

Identify products that should have received service but did not. This may indicate:
- Missed preventive maintenance opportunities
- Underutilized service contracts
- Products no longer in service
- Data quality issues

Use results to contact customers about service opportunities or investigate why expected calls did not occur.

## What Happens Next

Use this report to identify sales opportunities (customers with products but no service contracts), validate service agreement coverage, or improve preventive maintenance scheduling. Results help balance service utilization across the product portfolio.

## Common Issues

**Too Many Products in Results**
Filter by specific customer or product type to narrow results. Use the date range to focus on recent periods. Consider whether inactive products should be excluded.

**Products Should Have Calls But Do Not**
Verify the date range is correct. Check that service calls are properly linked to products. Contact customers to understand why products did not require service.

**Cannot Identify Why Product Has No Calls**
Review the product record to verify it is active and in service. Check the customer contract to see if the product is under a service agreement. Investigate manually if needed.
