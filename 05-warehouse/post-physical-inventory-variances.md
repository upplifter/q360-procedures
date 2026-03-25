---
title: Post Physical Inventory Variances
id: WH-COUNT-003
module: Warehouse
screen: Physical Inventory Count
menu_path: Inventory > Physical Inventory Count > [select count]
applies_to:
  - Warehouse Manager
prerequisites:
  - Variance report has been reviewed (see WH-COUNT-002)
  - Variances are approved by management
related_procedures:
  - WH-COUNT-002
  - WH-RPT-005
  - WH-RPT-006
tags: physical inventory, variance, post, adjustment, GL entry
version: 1.0
last_updated: 2026-03-25
---

# Post Physical Inventory Variances

## What This Procedure Does

Post approved physical inventory variances to adjust system on-hand quantities to match the physical count. Posting creates adjusting journal entries in the general ledger to reconcile inventory accounts. This is the final step after counts are entered and variances are reviewed and approved.

## Before You Begin

- The variance report has been reviewed (see WH-COUNT-002) and printed or exported for documentation
- Management approval has been obtained for all variances to be posted
- You have confirmed that no transactions are in progress that might be affected by the adjustments
- You have Warehouse Manager role and inventory posting permissions
- The count session status is ready for posting

## Steps

### Step 1: Open the Count Session

Navigate to **Inventory > Physical Inventory Count**. Select the count session that contains the variances to be posted. The count session form opens.

Verify that the session contains all counted items and that the status shows counts are complete and ready for posting.

### Step 2: Verify Counts Are Final

Review the count session item list to ensure:

- All items in the count area have been counted and entered
- No placeholder or temporary entries remain
- Quantity and serial number entries are final and accurate

If any items need correction, do not proceed to posting. Make corrections to the count session first by re-entering the correct counts.

### Step 3: Access Process Actions

Click the **Process Actions** button (gear icon) on the count session form. A dropdown menu displays available actions for this count session.

### Step 4: Select Post Variances

From the Process Actions menu, click **Post Variances**. A confirmation dialog appears asking you to confirm posting.

The dialog displays:

- Count session number
- Total number of items in the count
- Total variance amount (sum of all positive and negative variances)
- Expected GL impact

Review the total variance amount to ensure it is reasonable based on your variance review. Click **Yes** or **Confirm** to proceed with posting.

### Step 5: System Processing

The system processes the posting:

1. System on-hand quantities are adjusted for all items with variances
2. Journal entries are automatically created in the general ledger to record the variances
3. Inventory accounts are debited or credited based on variance direction
4. Variances are marked as posted in the count session

A confirmation message appears showing:

- Count session has been posted successfully
- Number of adjustments made
- GL journal entry reference number

### Step 6: Verify Posting Results

After posting is complete, review the count session status. It should now show:

- Status: Posted
- Var. Used: Yes (variances have been used/posted)
- On-hand quantities updated to match counted quantities

Navigate to **Live Data > INVENTORY > Physical Inventory Variance** and reapply the count filter. Items that were posted should no longer show variances.

## What Happens Next

After posting, the count cycle is complete. System on-hand quantities now reflect the physical count. The general ledger entries record the variance adjustments for accounting purposes.

Variance reports can be reviewed from the Accounting module (see WH-RPT-005, WH-RPT-006) to reconcile the GL impact. Monthly or periodic inventory reconciliation can now proceed with accurate on-hand quantities.

## Common Issues

**Post Variances option is grayed out or unavailable**

The count session may not be in a status ready for posting. Verify that:

- All counts have been entered (session shows count status as complete)
- The count has not already been posted
- You have the Warehouse Manager role assigned

Contact your system administrator if the button remains unavailable.

**System shows error "Cannot post variance - negative on-hand would result"**

One or more variances would result in a negative on-hand quantity after posting. This is typically not allowed:

- Verify the count quantities are correct
- Check if items were issued or shipped between count start and completion
- Consider whether the count should be adjusted before posting

Resolve the underlying count accuracy issue before attempting to post again.

**GL accounts for variance are not configured**

The system cannot create GL entries because variance accounts are not configured on the master records. This typically requires setup by an Accounting or System Administrator:

- Ensure each master has variance GL accounts defined (often set at the master type or warehouse level)
- Check that GL chart of accounts includes inventory adjustment and variance accounts
- Contact your system administrator to configure missing GL accounts

Do not post until accounts are configured, as the GL will be unbalanced.

**Posting takes a very long time or times out**

Large counts with many items may take several minutes to post. Do not interrupt or close the browser window. If posting does not complete after 10-15 minutes, contact your system administrator to check for processing errors.

If the system times out:

- Check the count session to verify if posting completed (status should show "Posted")
- Contact your system administrator to verify GL entries were created
- If posting failed, correct any underlying issues and retry

**On-hand quantities in the system have not changed after posting**

Verify that posting completed successfully by checking the count session status. If status shows "Posted" but quantities did not update:

- Check that the physical warehouse location is correctly assigned to the count
- Verify warehouse settings are not preventing quantity updates
- Contact your system administrator to investigate the posting process

GL entries should have been created regardless. Check the GL journal to confirm the entries are present, even if quantities did not update in the warehouse module.
