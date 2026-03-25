---
title: Request Presales Labor
id: SALES-PRESALES-001
module: Sales
screen: Opportunity Funnel Step Form
menu_path: Main Menu > Sales > Opportunities > Funnel Step
applies_to:
  - Sales Rep
  - Sales Manager
prerequisites:
  - OPPORTUNITY (Edit) permission assigned to your user or group
  - An opportunity exists with a funnel definition assigned (see SALES-OPP-001)
related_procedures:
  - SALES-OPP-001
  - SALES-OPP-003
  - SALES-PRESALES-002
  - SALES-PRESALES-003
tags: presales, presales labor, request engineering, design, funnel step, engineering workflow, assign presales, presales request
version: 1.0
last_updated: 2026-03-25
---

# Request Presales Labor

## What This Procedure Does

Requests presales engineering or design labor by configuring a funnel step on a sales opportunity. Once saved, the request appears in the Engineering workflow for a manager to review and assign a resource. This allows the sales team to formally request technical support during the presales process.

## Before You Begin

- You have OPPORTUNITY (Edit) permission.
- The opportunity exists and has a funnel definition with steps (see SALES-OPP-001).
- You know the approximate dates and category for the presales work.

## Steps

### Step 1: Look Up the Opportunity

Navigate to **Main Menu > Sales > Opportunities**. Search for and open the opportunity that requires presales labor.

### Step 2: Drill Into the Funnel Step

On the Opportunity form, locate the funnel steps grid. Drill into the appropriate funnel step that represents the presales work (e.g., a Design or Engineering step) by clicking on the step row.

### Step 3: Configure the Funnel Step

Click the **Edit Record** button (pencil icon) on the funnel step form. Fill in the following fields.

| Field | What to enter |
|---|---|
| Scheduled Start | The date presales work should begin. |
| Scheduled End | The date presales work should be completed by. |
| Time Bill Category | Select **Design** or the appropriate presales category. |
| Status | Set to **OPEN** to make the request visible in the Engineering workflow. |
| Assignee | If the person to assign is known, select them. If unknown (requesting from a department manager), leave blank. |
| Comments | Enter any additional instructions or scope details for the presales work. |

### Step 4: Save the Record

Click the **Save Record** button (floppy disk icon) on the form action bar.

## What Happens Next

The presales request now appears in the **Engineering workflow** under the Requested Presales bucket. An engineering manager can review the opportunity details, assign a resource, and update the status (see SALES-PRESALES-002).

Once a resource is assigned and begins work, they log time against the opportunity (see SALES-PRESALES-003). The logged time feeds into presales cost tracking and the Sales Opportunity Labor Conversion report (see SALES-RPT-009).

## Common Issues

**The funnel step does not appear in the Engineering workflow.**
Verify the step Status is set to OPEN. Steps in DATAENTRY status do not appear in the workflow. Also confirm the Time Bill Category is set to a presales-related category.

**You do not see the Assignee dropdown.**
The Assignee field may be restricted based on permissions. Contact your administrator if the field is not visible on your form layout.

**The Engineering manager does not see the request.**
Confirm the Engineering workflow filters match the opportunity's branch and department. The workflow may be filtered to a specific branch that does not include this opportunity.

**You want to cancel a presales request.**
Edit the funnel step and change the Status back to DATAENTRY or a cancelled status. This removes it from the Engineering workflow.

**The Time Bill Category dropdown does not include Design.**
The available categories are controlled by general code configuration. Contact your administrator to verify that a Design or presales category exists in the system.
