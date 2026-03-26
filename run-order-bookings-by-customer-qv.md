---
title: Run the Order Bookings By Customer Quick View
id: SALES-RPT-006
module: Sales
screen: Order Bookings By Customer Quick View
menu_path: Sales > Quick Views > Order Bookings By Customer
applies_to:
  - Sales Rep
  - Sales Manager
prerequisites:
  - Access to Sales Quick Views
  - Approved orders exist in the system (see SALES-ORDER-001)
related_procedures:
  - SALES-ORDER-001
  - SALES-RPT-005
tags: order bookings by customer, customer bookings, booking by customer, customer analysis, top customers, booking volume, customer revenue
version: 1.0
last_updated: 2026-03-25
---

# Run the Order Bookings By Customer Quick View

## What This Procedure Does

Runs the Order Bookings By Customer quick view to display a summarized financial overview of order bookings grouped by customer. The report calculates each customer's total booking value and their percentage share of total bookings, making it easy to identify top customers and analyze sales distribution.

## Before You Begin

- You have access to Sales Quick Views.
- Approved orders exist in the system.

## Steps

### Step 1: Open the Order Bookings By Customer Quick View

Navigate to **Sales > Quick Views** and select **Order Bookings By Customer**.

### Step 2: Set Filters

| Field | What to enter |
|---|---|
| Company No. | Select a company or leave for all. |
| Branch | Select a branch or leave for all. |
| Time Period | Set the date range for the bookings to analyze. |

### Step 3: Review the Report Grid

The grid displays one row per customer with the following columns:

- **Customer** - the customer name.
- **Total** - the total monetary value of order bookings for this customer in the selected period.
- **%** - the customer's percentage share of total bookings (Customer Total divided by Grand Total times 100).

A footer row shows the grand total of all bookings across customers.

The grid is sorted by Total in descending order by default, showing top customers first.

### Step 4: Analyze the Data

Use the grid to identify top revenue-generating customers, review customer concentration risk, and compare booking volumes across the customer base.

## What Happens Next

Use this data for account planning, identifying growth opportunities with under-penetrated customers, and evaluating customer portfolio balance. For detailed order-level booking data, see SALES-RPT-005.

## Common Issues

**The report shows no data.**
Verify the Time Period filter includes the range you expect. Only approved orders are counted as bookings.

**Percentages do not add up to 100%.**
The percentages are calculated against the grand total. If rounding is applied, the sum may differ slightly from 100%.

**A customer you expect is not listed.**
The customer may not have any approved orders in the selected time period. Adjust the date range or verify orders exist for that customer.

**The grand total differs from the Sales Booking report.**
The two reports may use different filter settings. Align the company, branch, and time period filters across both reports for a consistent comparison.

**You need more detail per customer.**
This is a summary view. For order-level detail, use the Sales Booking quick view (SALES-RPT-005) and filter by the specific customer.
