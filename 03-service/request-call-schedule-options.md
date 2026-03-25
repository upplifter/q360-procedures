---
title: Request Call Schedule Options
id: SVC-CALL-004
module: Service
screen: Service Call Form
menu_path: Service > Service Calls
applies_to: Customer Service Representatives, Service Managers
prerequisites:
  - Service call exists in OPEN status
  - Customer email address is on file
related_procedures:
  - SVC-CALL-001
  - SVC-CALL-005
tags:
  - scheduling
  - customer-communication
version: 1.0
last_updated: 2026-03-25
---

# Request Call Schedule Options

## What This Procedure Does

This procedure sends an automated scheduling request to the customer, asking them to provide preferred dates and times for the service call. The customer receives an email with available time slots and responds with their preferred option. You then review the response and schedule the call accordingly using SVC-CALL-005.

## Before You Begin

- Ensure the service call is in OPEN status
- Verify the customer contact has an email address on file
- Confirm the service type and estimated duration are known
- Check technician availability window for the service

## Steps

### Step 1: Open the Service Call

Navigate to Service > Service Calls or open the Service Calls tab on the customer record. Click the call number to open the Service Call form. Verify the call status is OPEN.

### Step 2: Request Schedule Options

Click Extended Menu (three vertical dots) at the top of the form. Select Request Schedule Options. A confirmation dialog appears showing the customer email address and scheduling request template.

### Step 3: Confirm and Send

Review the email recipient address to ensure it is correct. Click Send (or Confirm) to dispatch the scheduling request. The system sends an automated email to the customer containing available time windows and asks them to select preferred dates/times for the service call.

### Step 4: Monitor Customer Response

The customer responds to the automated email with their preferred schedule option. Responses are typically routed back to the Email Q (see SVC-CALL-002) or appear as events on the call record. Review the customer's preferred dates and times from their email response.

## What Happens Next

Once you receive the customer's schedule preference, open the service call and proceed with SVC-CALL-005 to schedule the call with an available technician on the customer's preferred date and time. If the preferred dates do not align with technician availability, you may negotiate alternative dates with the customer or assign the call to the next available technician slot.

## Common Issues

**Email Not Sent to Customer**
Verify the customer contact has a valid email address in the system. If the email field is blank or incorrect, update the customer contact record with the correct email address and retry the Request Schedule Options action.

**Customer Does Not Respond to Scheduling Request**
Follow up with the customer directly by phone or email if they do not respond within 24-48 hours. You can manually create a schedule using the last known preferred dates or create an alternative time slot based on technician availability.

**Multiple Responses from Customer**
If the customer sends multiple scheduling responses, review all responses and select the most recent or most specific one. Discard earlier responses and proceed with the latest customer preference. Document which response you used in the call Events tab.
