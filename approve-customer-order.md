---
title: Approve Customer Order
id: SALES-ORDER-001
module: Sales
screen: Order Form
menu_path: Workflow > Sales Overview > Quotes Converted to Confirmed Orders bucket
applies_to:
  - AR
  - Sales Manager
prerequisites:
  - ORDER (Execute) permission assigned to your user or group
  - The order is in CONFIRMED status and was created from an approved quote (see SALES-QUOTE-006)
  - PO number or customer approval documentation is attached
related_procedures:
  - SALES-QUOTE-006
  - SALES-RENEWAL-002
tags: approve order, order approval, confirmed order, create project, create service call, create service contract, order processing, gear button, sales overview
version: 1.0
last_updated: 2026-03-25
---

# Approve Customer Order

## What This Procedure Does

Reviews and approves a confirmed customer order from the Sales Overview workflow. Approving the order changes its status to APPROVED, locks it from further item changes, and triggers the creation of downstream records such as a project, service call, or service contract depending on the order's sale type.

## Before You Begin

- You have ORDER (Execute) permission.
- The order is in CONFIRMED status.
- A PO number is entered or customer approval documentation is attached in the Documents tab.
- Company, Branch, and Department selections are accurate.
- Taxation code and value are accurate.
- If the order is project-based and includes a workmanship warranty, at least one M-type warranty-flagged line item is present.

## Steps

### Step 1: Open the Order

Navigate to **Workflow > Sales Overview**. Click the **Quotes Converted to Confirmed Orders** bucket. Drill into the order to approve.

### Step 2: Verify Order Details

Review the following before approving:

1. **PO #** is entered on the Header tab, or supporting documentation is attached in the **Documents** tab.
2. **Company**, **Branch**, and **Department** selections are correct.
3. **Tax code** and calculated tax amount are accurate.
4. If the order is for a project that includes a workmanship warranty, verify that at least one M-type line item with the warranty flag (Warr/Def Rev checkbox) is present in the Line Items tab.

### Step 3: Approve the Order

Click the **Process Actions** button (gear icon) on the form action bar. Click **Approve**.

### Step 4: Respond to Creation Prompts

Depending on the order's Sale Type, Q360 may prompt you to create a related record:

- **Project prompt:** Select a project template and a default start date (the PM can change the date later). Click **OK**.
- **Service Call prompt:** Click **OK** to create the associated service call.
- **Service Contract prompt:** Click **OK** to create the associated service contract.

If the order is already linked to an existing project (e.g., from an Internal or Customer Change Order), Q360 does not prompt for a new project. Instead, it automatically adds the order contents to the existing project's Materials list and updates project financials.

### Step 5: Handle Service Contract Billing (If Applicable)

If a service contract was created from the order and all billable items are on the service contract, prevent duplicate billing on the order by clicking the order form **Extended Menu** (three vertical dots) and selecting **Mark This Order as Billed**.

## What Happens Next

The order status changes to APPROVED. It now appears in both the **Orders Pick Q** and the **Shipping Q**. Adding or removing line items is no longer permitted on an approved order.

Downstream records created during approval (project, call, or service contract) are available for their respective teams to begin work:

- A project manager can assign tasks and resources.
- A dispatcher can schedule and dispatch a service call.
- A service manager can configure contract billing and coverage.

## Common Issues

**The Approve action is not available in the Process menu.**
Verify the order is in CONFIRMED status. Also confirm you have ORDER (Execute) permission.

**The system does not prompt to create a project.**
The prompt depends on the order's Sale Type. If the Sale Type does not map to project creation, no prompt appears. Also, if the order is already linked to a project (e.g., change order), the system adds items to the existing project silently.

**The tax amount is incorrect.**
Return to the order, enter edit mode, correct the tax code or tax values, save, and then attempt approval again.

**You approved the order but forgot to attach the PO documentation.**
Open the order and attach the documentation in the Documents tab. While the order is already approved, the documentation should still be added for audit purposes.

**Items cannot be changed after approval.**
An approved order is locked. If changes are required, create an Internal Change Order (ICO) or Customer Change Order (CCO) against the associated project. Contact your project manager to initiate the change order process.
