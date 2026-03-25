---
title: Post Service Time Bills
id: SVC-CALL-008
module: Service
screen: Post Timebill Records
menu_path: Service > Post Timebill Records
applies_to: Service Managers, Accounting
prerequisites:
  - Unposted time bill entries exist in the system
  - Time bill entries are complete with employee, start time, end time, and work type
related_procedures:
  - SVC-CALL-007
  - PROJ-TB-002
tags:
  - time-posting
  - labor-cost
  - accounting
version: 1.0
last_updated: 2026-03-25
---

# Post Service Time Bills

## What This Procedure Does

This procedure posts unposted service time bills to the accounting system. Posting converts time bill entries into cost entries that are charged against the service call and can be billed to the customer. Posted time bills generate labor cost records and update project labor tracking.

## Before You Begin

- Unposted service time bills exist in the system
- All time bills are complete with required information (employee, start/end times, work type)
- Time entries are verified for accuracy before posting
- You have appropriate permission to post time bills

## Steps

### Step 1: Access Post Timebill Records Screen

Navigate to Service > Post Timebill Records. The grid displays all unposted service time bills across all service calls and employees.

### Step 2: Filter Time Bills (Optional)

Use the filter options at the top of the grid to narrow results by date range, employee, or branch:

| Filter | What to enter |
|--------|---------------|
| Date Range | Select start and end date for time entries to post |
| Employee | Select specific employee if posting for one technician |
| Branch | Select branch to post time bills for a specific location |

Click Filter or Apply to refresh the grid with matching time bills.

### Step 3: Review and Select Time Bills

Review all time bills in the filtered grid. Verify employee names, dates, durations, and work types are correct. Select the time bills you want to post by clicking the row checkbox for each entry. You can click Select All to select all visible time bills at once.

### Step 4: Post Selected Time Bills

Click Post (or Extended Menu > Post Selected) at the top of the grid. A confirmation dialog appears listing the count of time bills to be posted and the total labor cost impact.

### Step 5: Confirm Posting

Review the posting summary. Click Confirm or Post to execute the posting. The system processes the time bills and generates cost entries in the accounting module.

## What Happens Next

Posted time bills are removed from the unposted grid and become permanent cost entries on their respective service calls. The labor costs are now reflected in the call's total cost and can be viewed on the call's Details or AR Journal tabs. If the call is set up for customer billing, the labor costs are included in the next billing invoice. Time bills cannot be unposted after confirmation, so verify accuracy before posting.

## Common Issues

**Some Time Bills Cannot Be Posted**
If the system displays an error message for specific time bills, review those entries for missing required fields (Employee, Work Type, or invalid date ranges). Complete the missing information on the Time Bills tab before attempting to post again.

**Posted Time Bills Not Appearing on Service Call**
After posting, refresh the Service Call form (click Refresh - circular arrow icon) to see updated labor costs on the Details tab or AR Journal tab. Posted time bills may take a few moments to synchronize with the call record.

**Duplicate Posts for Same Time Bill**
If the same time bill appears to post twice, verify that you did not click Post multiple times in succession. Check the call's cost entries or AR Journal tab to confirm the amount was posted only once. Contact system administration if duplicate postings occurred.
