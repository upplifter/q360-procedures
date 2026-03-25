---
title: View Service Contract Profitability
id: SVC-CONTRACT-006
module: Service
screen: Service Contract > Profit
menu_path: Service Contract > Profit Tab
applies_to: Service Managers, Finance Managers, Business Analysts
prerequisites:
  - Service contract must be created and active
  - Service calls or orders must be recorded against the contract
  - Cost and revenue data must be posted to the contract
related_procedures:
  - SVC-CONTRACT-002a
  - SVC-RPT-013
tags:
  - profitability
  - analysis
  - reporting
version: 1.0
last_updated: 2026-03-25
---

# View Service Contract Profitability

## What This Procedure Does

Displays profitability metrics for a service contract including total revenue, total cost, gross profit, and gross margin percentage. Data sources include service calls performed, orders processed, and direct accounting postings to the contract.

## Before You Begin

- Service contract must be created and have line items
- Service calls must be performed and invoiced against the contract
- Orders or material receipts must be recorded against the contract line items
- Cost data must be posted from service calls and materials

## Steps

### Step 1: Open the Service Contract

Navigate to Service > Service Contracts. Find and open the contract you want to analyze.

### Step 2: Navigate to the Profit Tab

Click the Profit tab in the contract form. The profitability dashboard displays.

### Step 3: Review Profitability Metrics

The Profit tab shows the following key metrics:

| Metric | What it shows |
|--------|---------------|
| Total Revenue | Sum of all invoiced service calls, materials, and recurring charges for the contract period |
| Total Cost | Sum of all labor costs, material costs, and overhead allocated to service calls on the contract |
| Gross Profit | Total Revenue minus Total Cost |
| Gross Margin % | Gross Profit divided by Total Revenue, expressed as a percentage |

### Step 4: Analyze Revenue Sources

The Profit tab may display a breakdown of revenue by source:

- Service call revenue (labor hours billed)
- Material revenue (parts and supplies sold)
- Recurring contract billing (fixed monthly/quarterly fees)
- Other direct revenue postings

Review the revenue breakdown to understand which service types generate the most income.

### Step 5: Analyze Cost Sources

The Profit tab may display a breakdown of costs by source:

- Service call labor costs (technician hours)
- Material costs (parts consumed)
- Subcontract or outsourced work costs
- Allocated overhead

Review the cost breakdown to identify cost drivers and opportunities for improvement.

### Step 6: Identify Profit Trends

If the Profit tab displays data over time, review trends:

- Is profitability improving or declining?
- Are margins healthy relative to your service level agreements?
- Is revenue tracking to expectations for the contract type?

Use this analysis to determine if contract rates need adjustment or if service delivery efficiency needs improvement.

## What Happens Next

Profitability analysis can inform decisions about contract pricing, service delivery resources, and operational efficiency. If margins are below target, consider reviewing the service rate on the Customer Level tab or adjusting the contract terms. For ongoing monitoring, run the Service Contract Profitability report (see SVC-RPT-013) to compare multiple contracts and identify underperforming agreements. Export profitability data to your finance system for further analysis or reconciliation.

## Common Issues

**Profit tab shows zero or blank values**

Profitability data is populated from service calls and orders linked to the contract. If values are blank, verify that:

- Service calls have been created and completed with labor and material costs recorded
- Invoices have been generated for the service calls
- Cost data has been posted to the contract (not just invoiced, but costs recorded)
- The contract date range overlaps with the period of service calls

If service calls exist but profitability is still blank, verify that cost posting is enabled in your system configuration.

**Total Revenue does not match my invoices**

Revenue shown on the Profit tab is derived from invoiced service calls, materials, and recurring charges. If the amount does not match your invoice total, check:

- Whether all service calls are invoiced or if some remain in draft status
- Whether invoices include all line items or if some were removed
- Whether the contract period covers all invoices you expect to see

Reconcile the invoice total with the Profit tab data to identify any discrepancies.

**Gross Margin is negative**

A negative or low gross margin indicates that costs exceed revenue, resulting in a loss on the contract. This can occur if:

- Labor rates on the contract are too low for the service level provided
- Material costs are unexpectedly high
- Service calls are taking longer than estimated
- Warranty or free service work is not being tracked separately

Review the cost and revenue breakdown to identify the cause. You may need to renegotiate terms, adjust service rates, or improve operational efficiency.

**Data is outdated or does not reflect recent changes**

The Profit tab may cache data. Click the Refresh button (circular arrow) in the toolbar to reload the profitability metrics from the database. If data still appears stale, check that all recent service calls and invoices have been posted and that background job processing is current.
