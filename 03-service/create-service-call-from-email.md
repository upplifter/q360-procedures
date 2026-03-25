---
title: Create Service Call from Email
id: SVC-CALL-002
module: Service
screen: Email Queue
menu_path: Service > Work Queues > Email Q
applies_to: Customer Service Representatives, Service Managers
prerequisites:
  - Inbound email received in the Email Q
  - Customer and contact information must be present in the email
related_procedures:
  - SVC-CALL-001
  - SVC-CALL-005
tags:
  - service-call-creation
  - email-processing
version: 1.0
last_updated: 2026-03-25
---

# Create Service Call from Email

## What This Procedure Does

This procedure converts an inbound customer email into a service call. The system automatically pre-populates customer and contact information extracted from the email, reducing manual entry. You complete the remaining fields and save the call, which then enters OPEN status.

## Before You Begin

- Verify that an unprocessed email exists in the Email Q
- Confirm the email contains valid customer and contact information
- Ensure the sender is an existing customer in the system
- Review the email subject and body to determine the service type needed

## Steps

### Step 1: Access the Email Queue

Navigate to Service > Work Queues > Email Q. Alternatively, open the Service Overview workflow and click the Email Q bucket. The Email Q grid displays all unprocessed inbound emails.

### Step 2: Select the Email and Create Service Call

Click the email row to select it. Click Extended Menu (three vertical dots). Select Create Service Call. The Service Call form opens with customer and contact information automatically populated from the email.

### Step 3: Complete Required Call Fields

Fill in the following fields that are not pre-populated:

| Field | What to enter |
|-------|---------------|
| Call Type | Select the call type (SERVICE, REPAIR, PM, INSTALL, etc.) |
| Priority | Enter priority level 1-5 |
| Product | Select the product being serviced, if applicable |
| Problem Code | Select the problem code matching the issue |
| Problem Description | Review the pre-filled description and edit if needed |
| Branch | Select the home branch for technician assignment |
| Department | Select the service department |
| CSR | Select the Customer Service Representative handling the call |

### Step 4: Save the Call

Click Save (floppy disk icon). The system creates the service call with the pre-populated customer and contact information. The call status automatically changes to OPEN. The email is marked as processed and removed from the Email Q.

## What Happens Next

The service call is now created and appears in OPEN status. The original email content is linked to the call for reference. The call is ready for scheduling with a technician or you can proceed with SVC-CALL-005 to assign it to the Resource Console. The email is archived within the call for auditing purposes.

## Common Issues

**Customer Information Not Pre-Populated**
If the system cannot match the email sender to a customer record, you must manually select the customer from the dropdown. Verify the sender email address matches an active customer contact record in the system. If the customer does not exist, create the customer record first before creating the call.

**Email Marked as Processed Without Creating Call**
If you close the Service Call form without saving, the email may still be marked as processed. Return to the Email Q and verify the email status. You may need to manually create the call using SVC-CALL-001 and reference the original email content.

**Problem Description Too Long or Unclear**
If the email body contains excessive information or unclear problem details, edit the Problem Description field to include only relevant service information. You can also add notes to the Events tab (see SVC-CALL-009) to capture additional context from the original email.
