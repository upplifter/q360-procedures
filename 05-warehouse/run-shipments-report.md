---
title: Run the Shipments Report
id: WH-RPT-004
module: Warehouse
screen: Shipments Report (Q0156)
menu_path: Live Data > ACCOUNTING > Shipments
applies_to:
  - Warehouse Manager
  - Accounting
  - Sales Manager
prerequisites:
  - Access to Live Data > ACCOUNTING section
related_procedures:
  - WH-SHIP-001
tags: reporting, shipments, sales-analysis, accounting
version: 1.0
last_updated: 2026-03-25
---

# Run the Shipments Report

## What This Procedure Does

This report displays all shipped order items within a specified date range. Use this to track shipments, reconcile sales to fulfillment, and support accounting and sales analysis.

## Before You Begin

- Determine the date range for the shipment report (start and end dates)
- Identify the specific company, branch, or department if you want to filter the results, or leave blank for all
- Have access to the Live Data Accounting reports section

## Steps

### Step 1: Navigate to the Report

Go to Live Data > ACCOUNTING > Shipments. The system opens the report filter screen.

### Step 2: Set the Report Parameters

Enter or select the desired filters:

| Field | What to enter |
|-------|---------------|
| Company | Select the company to include, or leave blank for all companies |
| Branch | Select the branch to include, or leave blank for all branches |
| Department | Select the department to include, or leave blank for all departments |
| Start Date | Beginning date for the shipment period |
| End Date | Ending date for the shipment period |

### Step 3: Run the Report

Click the appropriate button to generate or view the report. The system compiles shipment data for the specified date range and filters.

### Step 4: Review the Shipment Data

The report displays the following columns for each shipment:

| Column | Description |
|--------|-------------|
| Order No | Sales order number |
| Company | Company code |
| Sales Rep | Name or code of the sales representative |
| Total | Total dollar amount of the shipment |
| Ship Date | Date the order was shipped |
| Qty | Quantity of items shipped |
| Master No | Master inventory number for the item |
| Description | Item description |

### Step 5: Analyze the Results

Review the shipment quantities and values to confirm all orders were shipped in the period. Cross-reference with sales records to ensure complete reconciliation. Identify any orders with unusual quantities or values.

### Step 6: Export or Archive the Report

Use the Extended Menu (three vertical dots) to export the report to Excel or PDF. The report is commonly exported for month-end closing procedures and sales analysis.

## What Happens Next

The shipment data can be used to reconcile accounts receivable, verify revenue recognition, support financial statements, and analyze sales performance by region, department, or sales representative. Export the report as needed for analysis, management review, or audit support.

## Common Issues

**Report shows no shipments**
Verify the start and end dates include shipments you expect to see. Check that the company, branch, and department filters are correct. If filters are correct, no shipments may have occurred during that period.

**Shipment quantities do not match order quantities**
Some orders may have been partially shipped or split across multiple shipments. Review the order details in the sales module to confirm the total quantities across all shipments match the original order.

**Totals do not reconcile to accounts receivable**
Verify all relevant date filters and company selections match your accounting records. Some orders may have credits, returns, or adjustments that are not shown in the basic shipment report. Work with accounting to reconcile.

**Cannot filter by specific customer**
This report is organized by order and does not have a customer filter in the main interface. To analyze shipments by customer, export the report to Excel and filter by customer name or order number.

**Sales rep names are not displaying**
The sales rep field may show codes instead of names if the sales rep master records are not fully configured. Contact sales or accounting to verify sales rep codes are properly set up.
