---
title: Respond to Presales Labor Request
id: SALES-PRESALES-002
module: Sales
screen: Engineering Workflow
menu_path: Workflow > Engineering
applies_to:
  - Engineering Manager
prerequisites:
  - Access to the Engineering workflow
  - OPPORTUNITY (Edit) permission assigned to your user or group
  - A presales labor request exists in OPEN status (see SALES-PRESALES-001)
related_procedures:
  - SALES-PRESALES-001
  - SALES-PRESALES-003
  - SALES-OPP-001
tags: presales, respond presales, assign presales, engineering workflow, requested presales, engineering manager, assign resource
version: 1.0
last_updated: 2026-03-25
---

# Respond to Presales Labor Request

## What This Procedure Does

Reviews and assigns a presales labor request from the Engineering workflow. The engineering manager evaluates the opportunity, assigns a resource to the funnel step, and updates the status. Once assigned, the request moves to the Assigned bucket in the Engineering workflow and appears in the assignee's task list.

## Before You Begin

- You have access to the Engineering workflow.
- You have OPPORTUNITY (Edit) permission.
- A presales request exists in the Requested Presales bucket (see SALES-PRESALES-001).
- You know which resource to assign to the presales work.

## Steps

### Step 1: Open the Engineering Workflow

Navigate to **Workflow > Engineering**. The Engineering workflow canvas displays with workflow buckets.

### Step 2: Open the Requested Presales Bucket

Click the **Requested Presales** bucket. A grid opens listing presales requests awaiting assignment.

### Step 3: Review the Opportunity

Drill into the opportunity by clicking the opportunity row in the grid. Review the opportunity details including scope, value, and any comments left by the sales rep in the funnel step.

### Step 4: Open the Funnel Step

From the opportunity, drill into the funnel step that contains the presales request.

### Step 5: Assign a Resource

Click the **Edit Record** button (pencil icon). Update the following fields.

| Field | What to enter |
|---|---|
| Status | Confirm the status is **OPEN**. |
| Assignee | Select the engineer or designer to assign to this presales work. |

### Step 6: Save the Record

Click the **Save Record** button (floppy disk icon).

## What Happens Next

The presales request moves from the Requested Presales bucket to the **Assigned** bucket in the Engineering workflow. The assigned resource sees the opportunity task in their **My Tasks** list and can begin logging time (see SALES-PRESALES-003).

The sales rep can monitor the assignment by checking the funnel step on the opportunity.

## Common Issues

**The Requested Presales bucket is empty.**
Verify the workflow filters match the branch and department of the incoming presales requests. Adjust the filters if needed to see all pending requests.

**The Assignee dropdown does not show the desired resource.**
The dropdown may be limited to users with specific roles or permissions. Contact your administrator to verify the resource has the appropriate role or is part of the correct department.

**The request does not move to the Assigned bucket after saving.**
Confirm you selected an Assignee and that the Status is OPEN. Both conditions must be met for the request to appear in the Assigned bucket.

**You want to reassign the request to a different resource.**
Open the funnel step, enter edit mode, change the Assignee to a different person, and save. The task list updates automatically.

**The assigned resource does not see the task in My Tasks.**
The resource's task list filters may need to be adjusted. Have them check their My Tasks filters for the correct date range and department.
