---
title: Run the Sales Booking Quick View
id: SALES-RPT-005
module: Sales
screen: Dashboard Sales Order Bookings Quick View
menu_path: Sales > Quick Views > Sales Booking
applies_to:
  - Sales Rep
  - Sales Manager
prerequisites:
  - Access to Sales Quick Views
  - Approved orders exist in the system (see SALES-ORDER-001)
related_procedures:
  - SALES-ORDER-001
  - SALES-RPT-006
tags: sales booking, order bookings, sales order booking, dashboard bookings, booking report, booking analysis, sales performance, order tracking
version: 1.0
last_updated: 2026-03-25
---

# Run the Sales Booking Quick View

## What This Procedure Does

Runs the Sales Booking (Dashboard Sales Order Bookings) quick view to provide a comprehensive overview of sales order bookings. The report details financial performance, sales rep involvement, commission splits, and linkages to quotes, projects, and service calls. It serves as the primary tool for monitoring booking activity and sales performance over time.

## Before You Begin

- You have access to Sales Quick Views.
- Approved orders exist in the system.

## Steps

### Step 1: Open the Sales Booking Quick View

Navigate to **Sales > Quick Views** and select **Sales Booking**.

Alternatively, navigate to **Workflow > Sales Overview** and click the **Sales Bookings this Month** bucket.

### Step 2: Set Filters

Adjust filters in the Filters panel to focus the report. Common filters include Company, Branch, Department, Sales Rep, Sale Type, and time period.

### Step 3: Review the Bookings Grid

The grid displays one row per order with detailed financial columns including:

- Order identification: Order No., Quote No., Customer Name, Title.
- Financial metrics: Total Amount, Gross Profit, Gross Margin.
- Sales rep details and commission split information.
- Linked records: Project No., Service Call No., Service Contract No.
- Order type classification (e.g., New Sale, Change Order, Work Order).

Summation rows provide subtotals and grand totals for key financial columns.

### Step 4: Drill Into Orders

Click the zoom drilldown on any row to open the full Order form for detailed review.

## What Happens Next

Use the bookings data to track monthly and quarterly sales targets, analyze profitability by order, and review sales rep performance. For a customer-focused breakdown, see SALES-RPT-006.

## Common Issues

**The report shows no bookings for the current month.**
Verify the time period filter includes the current month. Also confirm that orders have been approved - only approved orders appear as bookings.

**Gross profit or margin appears incorrect.**
GP is calculated from the order's cost and price data. Verify line item costs and prices are accurate on the order.

**Commission information is missing.**
Commission data depends on commission configuration. If no commission rules are set up, the commission columns appear empty.

**You cannot see orders from other sales reps.**
The report respects your sales group access permissions. Adjust the Sales Rep filter or contact your administrator for broader access.

**The linked project number is blank.**
Not all orders create projects. The Project No. column is populated only for orders whose Sale Type triggers project creation during approval.
