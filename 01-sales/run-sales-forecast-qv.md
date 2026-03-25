---
title: Run the Sales Forecast Quick View
id: SALES-RPT-001
module: Sales
screen: Sales Forecast Quick View
menu_path: Sales > Quick Views > Sales Forecast
applies_to:
  - Sales Rep
  - Sales Manager
prerequisites:
  - Access to Sales Quick Views
  - Opportunities exist with value and probability set (see SALES-OPP-002)
related_procedures:
  - SALES-OPP-002
  - SALES-RPT-002
  - SALES-RPT-014
tags: sales forecast, pipeline, quick view, weighted value, opportunity forecast, sales pipeline report, revenue forecast, close date periods
version: 1.0
last_updated: 2026-03-25
---

# Run the Sales Forecast Quick View

## What This Procedure Does

Runs the Sales Forecast quick view to display a comprehensive overview of the sales pipeline by sales rep and probability. The report shows opportunity values broken into time-period buckets based on close dates, weighted totals, quoted amounts, and historical changes to key metrics. It is the primary tool for monitoring pipeline health and forecasting revenue.

## Before You Begin

- You have access to Sales Quick Views.
- Opportunities have been created with value, probability, and close date populated (see SALES-OPP-002).

## Steps

### Step 1: Open the Sales Forecast Quick View

Navigate to **Sales > Quick Views** and select **Sales Forecast**. The quick view opens with default filter settings.

Alternatively, navigate to **Workflow > Sales Overview** and click the **Sales Forecast** bucket.

### Step 2: Set Filters

Adjust the filters in the Filters panel on the left.

| Field | What to enter |
|---|---|
| Company | Select a specific company or leave blank for all. |
| Branch | Select a branch or ALL. |
| Department | Select a department or ALL. |
| Sales Rep | Select a specific sales rep or ALL to see all accessible reps. |
| Prob. >= | Set the minimum probability threshold (default is 20%). |
| Forecast From | Set the baseline date for period calculations (default is today). |

### Step 3: Review the Forecast Grid

The grid displays one row per opportunity with the following key columns:

- **Company** and **Title** - identify the opportunity. New opportunities (added within the last 30 days) may be highlighted in light green.
- **Value** - total estimated revenue. Color-coded: light green if increased, light red if decreased since last recorded history.
- **Gross Profit** - estimated GP (Value minus Cost).
- **Weighted Total** - probability-adjusted value (Value times Probability divided by 100).
- **Close Date** - expected close. Color-coded: green if moved earlier, red if moved later.
- **%** (Probability) - likelihood of winning. Color-coded for changes.
- **Over Due**, **0-30**, **31-60**, **61-90**, **> 90** - opportunity value distributed across time-period buckets relative to the Forecast From date.
- **Quote Amt**, **Quote Cost**, **Quote GP**, **Quote GM** - totals from linked non-optional quotes.
- Equipment, Labor, Subcontractor, and Other breakdowns from quoted items.
- **Quoted RMR** - recurring monthly revenue from quoted warranty or service items.

Subtotal rows appear in light gray per Sales Rep and in light blue for branch subtotals.

### Step 4: Use Extended Features

- Click the **Edit** button to make inline edits on columns marked with a pencil icon (e.g., updating close dates directly).
- Use the grid **Extended Menu** to **Change Close Date** on selected opportunities at once.
- Click the zoom drilldown link on any row to open the full Opportunity form.

### Step 5: Save Filters (If Needed)

To save your filter settings as default, click the disk-shaped icon in the Filters panel. To save as a named filter set, click the down arrow next to Default, type a name, and press **Enter**.

## What Happens Next

Use the forecast data to prioritize sales efforts, identify overdue opportunities, and prepare pipeline review meetings. The report data updates in real time as opportunities are modified.

For a manufacturer-focused forecast that projects demand by product, see SALES-RPT-014. For a funnel-phase-based view, see SALES-RPT-002.

## Common Issues

**The forecast shows no opportunities.**
Adjust the Prob. >= filter - it defaults to 20%, which excludes lower-probability opportunities. Also verify the Branch and Sales Rep filters include your opportunities.

**Historical color indicators are not appearing.**
Historical comparison uses the Days Out history period setting. If no historical data exists within that window, no color changes appear.

**The weighted totals seem incorrect.**
Weighted Total is calculated as Value multiplied by Probability divided by 100. Verify that both Value and Probability are entered correctly on each opportunity.

**You see opportunities from other sales reps.**
The Sales Rep filter respects your sales group access permissions. If set to ALL, you see all reps accessible to your group. Change the filter to your own name for a personal view.

**Quoted amounts show zero even though quotes exist.**
Only non-optional quotes with non-optional, non-cancelled line items are included. Verify the quotes are not marked as optional and have active line items.
