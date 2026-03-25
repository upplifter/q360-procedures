---
title: Initiate a Physical Inventory Count
id: WH-COUNT-001a
module: Warehouse
screen: Physical Inventory Count
menu_path: Workflow > Warehouse > Inventory Count OR Inventory > Physical Inventory Count
applies_to:
  - Warehouse Manager
prerequisites:
  - Management has approved the physical count
  - Warehouse operations can be paused or slowed
  - Count dates and scope have been determined
  - Warehouse staff is available for count execution
related_procedures:
  - WH-COUNT-001b
  - WH-COUNT-001c-alt
  - WH-COUNT-002
tags: physical inventory, inventory count, warehouse count, stock verification
version: 1.0
last_updated: 2026-03-25
---

# Initiate a Physical Inventory Count

## What This Procedure Does

Create a physical inventory count session, define the scope of items to count, lock the warehouse to prevent order fulfillment activity, and distribute count sheets to warehouse staff. This is the first step in verifying actual on-hand inventory against system records.

## Before You Begin

- Management approval for physical count has been obtained
- Warehouse operations can be paused or significantly slowed during the count
- Count dates and schedule have been determined
- Warehouse staff is notified and available for count execution
- User has Warehouse Manager privileges

## Steps

### Step 1: Open Physical Inventory Count Screen

Navigate to **Workflow > Warehouse** and click **Inventory Count**.

Alternatively, navigate to **Inventory > Physical Inventory Count** from the left navigation sidebar.

The Physical Inventory Count screen displays options to create a new count session.

### Step 2: Create New Count Session

Click the **Add New** button (plus icon) to create a new count session.

A form appears to configure the count parameters.

### Step 3: Select Company and Branch

On the count form, select the **Company** from the dropdown menu.

| Field | What to enter |
|-------|---------------|
| Company | Select the company performing the count |
| Branch | Select the branch where the count will occur |

Verify the correct company and branch are selected. Most counts are performed at a single branch.

### Step 4: Set Count Date Range

Enter the **Count Start Date** and **Count End Date** for the physical count.

| Field | What to enter |
|-------|---------------|
| Count Start Date | Enter the date counting begins (often today's date) |
| Count End Date | Enter the date counting ends (often same day or next business day) |

This date range determines which inventory transactions are locked during the count.

### Step 5: Select Masters to Count

Choose the scope of items to include in the count.

| Option | When to select |
|--------|----------------|
| All Masters | Count entire warehouse inventory; most comprehensive |
| Active Masters Only | Count only items marked as Active; excludes inactive/obsolete items |
| Selected Masters | Count specific products; choose individual masters to include |
| Date Range | Count only masters received or modified within a date range |

If selecting **Selected Masters**, a dialog appears to choose specific product masters by search or category.

Check the checkbox next to each master you want to count, or click **Select All** to include all active masters.

### Step 6: Configure Count Parameters

On the count form, configure additional count settings:

| Field | What to enter |
|-------|---------------|
| Count Method | Select: Physical Count, Cycle Count, or ABC Analysis (depends on configuration) |
| Include Serial Numbers | Check if count will track individual asset serial numbers (A-type) |
| Include Quantities | Check if count will track quantity counts (Q-type) |
| Allow Adjustments | Check if staff can propose inventory adjustments during count |

Select the parameters appropriate for your count type.

### Step 7: Lock the Warehouse

Before distributing count sheets, lock the warehouse to prevent order picking and shipping during the count.

On the count form, check the **Lock Warehouse** checkbox.

| Field | What to check |
|--------|---------------|
| Lock Warehouse | Check this box to freeze warehouse fulfillment activity |
| Lock Reason | Note: "Physical Inventory Count" |

Alternatively, click the **Lock Warehouse** button on the form action bar.

A confirmation dialog appears asking you to confirm the warehouse lock.

Click **Confirm** to lock the warehouse. No new picks or shipments can be processed until the count is complete.

### Step 8: Generate and Distribute Count Sheets

Click the **Print Report** icon (printer) to generate count sheets.

Count sheets print with:
- Count session ID and date range
- List of masters to count with on-hand system quantities
- Columns for physical counts and variance notes
- Sections for serial numbers (A-type) or quantity tallies (Q-type)

Distribute printed count sheets to warehouse staff assigned to the count.

Alternatively, count sheets may be available on-screen for staff to use handheld scanners or tablets during the count.

### Step 9: Notify Warehouse Staff

Communicate to all warehouse staff that:
- Physical inventory count is in progress
- Warehouse is locked to picking and shipping
- All staff must submit actual counts on their assigned count sheets
- Questions should be directed to the Warehouse Manager

Assign count teams to specific warehouse zones or product categories as needed.

### Step 10: Save Count Session

Click the **Save** button (floppy disk icon) to record the count session.

The count session is created with status ACTIVE or IN PROGRESS.

The audit trail records the count session creation with timestamp and Warehouse Manager name.

## What Happens Next

The warehouse is now locked and fulfillment activity is paused. Warehouse staff proceeds with physical counts using the distributed count sheets (see WH-COUNT-001b for count execution details). Staff submits actual counts which are recorded. Once all counts are submitted, the Warehouse Manager reviews discrepancies and determines adjustments (see WH-COUNT-002). The count is completed and warehouse is unlocked for normal operations.

## Common Issues

**Cannot select All Masters or Selected Masters**
If master selection is grayed out, verify that at least one active master exists in the system. If no active masters exist, the count cannot proceed. Create or activate master products before initiating count.

**Warehouse lock fails or does not apply**
Verify your user account has Warehouse Manager privileges. If the lock fails, check that no users are currently in the middle of processing orders. Complete any in-progress picks or shipments before applying the warehouse lock.

**Printing count sheets produces no output**
Verify the warehouse printer is online and has paper loaded. Check printer settings in system administration. If the printer is offline, contact IT. Count can proceed with on-screen sheets if printing is unavailable.

**Locked warehouse is preventing critical urgent orders**
If a critical order must ship during the count, contact Warehouse Manager to temporarily unlock for that order, then relock. Document the exception in the count session. Minimizing exceptions is important for count accuracy.

**Count session created but warehouse not locked**
Verify you checked the Lock Warehouse checkbox on the form and clicked Save. If the warehouse remains unlocked, manually apply the lock using the Lock Warehouse button. Confirm the lock is active by attempting to pick an order (which should fail if locked).
