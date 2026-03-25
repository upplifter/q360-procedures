---
title: Review Service Call Reports
id: SVC-CALL-021
module: Service
screen: Service Overview
menu_path: Service > Work Queues, Service > Quick Views, Service > Reports
applies_to: CSRs, Service Managers, Operations Managers
prerequisites:
  - Access to Service module
  - Closed or completed service calls in the system
related_procedures:
  - SVC-CALL-018
  - SVC-CALL-019
tags:
  - reporting
  - analytics
  - profitability
  - work queue management
version: 1.0
last_updated: 2026-03-25
---

# Review Service Call Reports

## What This Procedure Does

Access ongoing call data and completed call profitability information through multiple reporting views. Use Work Queues for active call monitoring, Quick Views for profitability analysis, and the Reports section for detailed analytics. Cross-reference additional service reports as needed.

## Before You Begin

- Access to the Service module
- Service calls have been created and some are closed
- Appropriate reporting permissions for your role
- You understand the metrics you want to analyze (calls in progress, profitability, technician utilization)

## Steps

### Step 1: Access Work Queues for Active Calls

Navigate to Service menu > Work Queues. The Work Queues screen displays active call statuses:

| Queue | Content |
|-------|---------|
| Dispatch Q | Calls assigned to technicians but not yet started (DISPATCHED status) |
| In Progress | Calls where field work is actively underway |
| TECHDONE Queue | Calls completed by technicians awaiting CSR review (TECHDONE status) |
| Open Calls | All calls not yet closed |

Click on a queue name to see calls in that status. Review call details, assigned technician, customer, and estimated completion.

### Step 2: Monitor Calls in Dispatch Q

The Dispatch Q shows calls ready for technician pickup. Review:

| Information | Purpose |
|-------------|---------|
| Call Number | Unique call identifier |
| Customer | Account being served |
| Location | Service address |
| Priority | Urgency level |
| Assigned Tech | Technician assigned to call |

Use this queue to ensure calls are moving through the dispatch process efficiently. Identify any stuck calls that have been DISPATCHED too long.

### Step 3: Access Quick Views for Call Profitability

Navigate to Service menu > Quick Views. Select Call Profit view. The grid displays completed calls with profitability metrics:

| Column | Information |
|--------|------------|
| Call Number | Call identifier |
| Revenue | Total amount billed to customer |
| Material Cost | Cost of parts used |
| Labor Cost | Cost of technician time |
| Gross Profit | Revenue minus costs |
| Margin % | Profit as percentage of revenue |

Sort by any column to identify highest/lowest performing calls. Use this to identify calls that lost money or exceeded expectations.

### Step 4: Filter and Drill Down

Apply filters to narrow your view:

| Filter | Usage |
|--------|-------|
| Date Range | View calls from specific period |
| Technician | See individual technician performance |
| Customer | Analyze specific customer profitability |
| Service Type | Compare break/fix vs. PM profitability |

Click on a specific call to drill down into detail and see line-item breakdown.

### Step 5: Access Additional Reports

Navigate to Service menu > Reports. Available reports typically include:

| Report | Content |
|--------|---------|
| SVC-RPT-001 | Service Call Summary - Overview of all calls by status and date |
| SVC-RPT-002 | Technician Utilization - Hours and efficiency by technician |
| SVC-RPT-003 | Call Profitability - Detailed profit/loss by call |

Select the report you want to run. Configure parameters (date range, technician, customer) as needed. Click Run or Generate to create the report.

### Step 6: Analyze Report Results

Review the generated report on screen or export to PDF/Excel for analysis:

- Identify trends (improving or declining efficiency)
- Compare actual results to targets or forecasts
- Spot technicians or customers requiring attention
- Analyze service type profitability

### Step 7: Take Action

Based on report findings, take appropriate action:

- Adjust dispatch to improve technician utilization
- Review pricing if calls are unprofitable
- Recognize high-performing technicians
- Identify customer service level opportunities

## What Happens Next

Regular review of service call reports enables data-driven decisions about technician allocation, service pricing, and operational efficiency. Findings can be shared in management meetings or performance reviews. Reports can be scheduled to run automatically and be emailed to stakeholders on a regular basis.

## Common Issues

**Work Queue shows no calls or unexpected queue is empty**

Verify calls exist in the system (check by navigating to Service > Service Calls main list). If calls exist but queues are empty, they may have been completed and moved to CLOSED status. Adjust date filters or navigate to a broader view to see all calls. If queues are truly empty, contact your service manager to verify call creation process.

**Quick Views do not show profitability data**

Verify calls are closed (see SVC-CALL-018). Profitability metrics only appear for CLOSED calls with complete billing. For open or in-progress calls, profitability cannot be calculated. If closed calls do not show profitability, verify the call was invoiced (Bill This Service Call was run). Contact your system administrator if profitability columns are missing.

**Reports show unexpected or incorrect data**

Verify the report date range, filters, and parameters are correct. Run the report with broader filters (all dates, all technicians) to see if the issue is filter-related. If data is still incorrect, the underlying call records may be incomplete. Check individual call records for missing or incorrect information. Contact your system administrator if data quality issues persist.

**Cannot access Reports or Quick Views menu**

Verify your user role has permission to access Service reports. Some roles may have restricted access to profitability data. Contact your system administrator to request reporting permissions if needed.
