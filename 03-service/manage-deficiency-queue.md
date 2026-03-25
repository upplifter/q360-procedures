---
title: Manage the Deficiency Queue
id: SVC-DEFICIENCY-001
module: Service
screen: Deficiency Queue
menu_path: Service > Work Queues > Deficiency Queue
applies_to: Service Managers, CSRs, Field Service Managers, Technicians
prerequisites:
  - Service module access
  - Field technicians have submitted inspection results with deficiencies
  - Access to create service calls or quotes
related_procedures:
  - SVC-CALL-012
  - SVC-CALL-001
tags:
  - quality assurance
  - inspections
  - work queue management
  - follow-up actions
version: 1.0
last_updated: 2026-03-25
---

# Manage the Deficiency Queue

## What This Procedure Does

Review and address items identified as deficient by field technicians during inspections. The Deficiency Queue displays failed inspection items needing attention. For each deficiency, create a repair quote for customer approval, create a follow-up service call, or add the item to an existing service call or quote.

## Before You Begin

- Service module is accessible
- Field technicians have completed inspections and logged deficiencies
- You have authority to create service calls or quotes
- You understand what each deficiency represents and the scope of required repair

## Steps

### Step 1: Navigate to Deficiency Queue

Go to Service menu > Work Queues > Deficiency Queue. Alternatively, access through the Service Overview workflow. The Deficiency Queue displays all inspection items marked as failed or deficient.

The queue shows:

| Column | Information |
|--------|------------|
| Deficiency ID | Unique identifier for the deficiency |
| Date Found | When technician identified the issue |
| Customer | Account where deficiency occurred |
| Location | Service site address |
| Item Description | What was found to be deficient |
| Technician | Who identified the deficiency |
| Priority | Urgency level for repair |

### Step 2: Select a Deficiency to Address

Click on a deficiency entry to open the detail view. The deficiency shows:

| Information | Details |
|------------|---------|
| Problem Description | What the technician found |
| Location/Component | Where the deficiency is located |
| Estimated Repair Cost | Initial estimate if available |
| Photos/Evidence | Any supporting images from inspection |
| Related Original Call | The service call during which it was found |

### Step 3: Choose Action - Option 1: Create a Repair Quote

For deficiencies requiring customer approval before repair, create a quote:

Click the Extended Menu (three vertical dots) or select Create Quote. The system generates a new quote document:

| Information | Pre-Filled From |
|-------------|-----------------|
| Customer | Deficiency record |
| Location | Service site from deficiency |
| Items/Description | Deficiency details |
| Estimated Cost | Initial estimate |

Complete the quote with final scope, pricing, and terms. Save and submit to customer for approval (see SVC-CALL-012 for quote approval process).

### Step 4: Choose Action - Option 2: Create Follow-up Service Call

For deficiencies requiring immediate service scheduling, create a new service call:

Click the Extended Menu or select Create Service Call. The system generates a new service call:

| Information | Pre-Filled From |
|-------------|-----------------|
| Customer | Deficiency record |
| Location | Service site |
| Problem Description | Deficiency details |
| Related Item | Link to original deficiency |

Complete the call with technician assignment, call type, and priority. The new call can be immediately dispatched to a technician (see SVC-CALL-001 for dispatch procedures).

### Step 5: Choose Action - Option 3: Add to Existing Call or Quote

For deficiencies that can be bundled with other work:

Click the Extended Menu or select Add to Existing. A dialog appears allowing you to select:

| Option | Purpose |
|--------|---------|
| Select Service Call | Add deficiency to an open call already in progress |
| Select Quote | Add deficiency to an existing quote awaiting approval |

Choose the target call or quote. The deficiency items are added to the selected document. Save the document.

### Step 6: Mark Deficiency as Addressed

Once an action has been taken (quote created, call created, or added to existing document), mark the deficiency as handled:

Click Mark as Resolved or Mark as Addressed (the button name varies). The deficiency moves out of the active queue. Select the resolution action type:

| Resolution Type | Meaning |
|-----------------|---------|
| Quote Created | Awaiting customer approval |
| Call Created | Scheduled for repair |
| Added to Existing | Combined with another work order |
| Deferred | Postponed for later action |
| Unable to Address | Referred or unable to proceed |

Save the resolution. The deficiency now shows as addressed in reporting.

## What Happens Next

Addressed deficiencies no longer appear in the active Deficiency Queue but remain in the system history for reference. Quotes generated from deficiencies are sent to customers for approval. Service calls created from deficiencies can be tracked through the normal call lifecycle (see SVC-CALL-001 through SVC-CALL-018). Once repair work is completed, the deficiency is fully resolved and archived. Deficiency metrics can be tracked to improve quality assurance and identify systemic issues.

## Common Issues

**Deficiency Queue shows no items or is empty**

Verify field technicians have completed inspections and logged deficiencies in the system. Check that inspections have been submitted and processed. If technicians are completing inspections but no deficiencies appear, check whether deficiencies are being logged correctly in the inspection module. Contact your service manager or system administrator.

**Cannot create quote or service call from deficiency**

Verify the customer is defined with complete information. Ensure you have permissions to create quotes or service calls. If the create button is disabled, the deficiency may already be marked as addressed. Try refreshing the page. If issues persist, contact your system administrator.

**Deficiency is marked as resolved but still appears in queue**

The queue view may not refresh immediately. Refresh the page or navigate away and return to Deficiency Queue. The resolved deficiency should no longer appear in the active list. If it still appears after refresh, verify the correct resolution status was saved.

**Multiple similar deficiencies exist for same customer**

Review all related deficiencies before creating separate quotes or calls. Consider bundling similar items into a single quote or call to reduce customer communication and improve efficiency. Use Option 3 (Add to Existing) to consolidate deficiencies when appropriate.
