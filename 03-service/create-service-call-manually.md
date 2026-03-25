---
title: Create Service Call Manually
id: SVC-CALL-001
module: Service
screen: Service Call Form
menu_path: Service > Service Calls > Add
applies_to: Customer Service Representatives, Service Managers
prerequisites:
  - Customer record exists in the system
  - Site information is available for the customer
related_procedures:
  - SVC-CALL-005
  - SVC-CALL-006
tags:
  - service-call-creation
  - dispatching
version: 1.0
last_updated: 2026-03-25
---

# Create Service Call Manually

## What This Procedure Does

This procedure creates a new service call directly in the system without using email or order automation. You can initiate a service call from a customer record or through the Service Calls menu. The call enters the system in OPEN status and awaits scheduling.

## Before You Begin

- Ensure the customer record exists in your system
- Have the customer's site information and contact details available
- Determine the service call type (SERVICE, REPAIR, PM, INSTALL, etc.)
- Know the priority level (1-5) for the call
- Identify the appropriate technician branch and department

## Steps

### Step 1: Access the Service Call Form

Navigate to Service > Service Calls > Add. Alternatively, open a customer record, go to the Service Calls tab, and click Add (plus icon). The Service Call form displays with the Call tab active.

### Step 2: Enter Call Header Information

Fill in the following fields:

| Field | What to enter |
|-------|---------------|
| Customer | Select the customer from the dropdown |
| Site | Select the site associated with the customer |
| Product | Select the product or equipment being serviced |
| Call Type | Select the call type (SERVICE, REPAIR, PM, INSTALL, etc.) |
| Priority | Enter priority level 1-5 (1 = highest priority) |
| Branch | Select the home branch for the technician assignment |
| Department | Select the service department handling the call |

### Step 3: Enter Problem Information

Complete the following problem-related fields:

| Field | What to enter |
|-------|---------------|
| Problem Code | Select the problem code that categorizes the issue |
| Problem Description | Enter a detailed description of the problem or service needed |
| CSR | Select the Customer Service Representative handling the call |

### Step 4: Save the Call

Click Save (floppy disk icon). The system creates the service call and assigns it a call number. The call status automatically changes to OPEN. The call is now visible in the Dispatch Q and Service Overview workflow.

## What Happens Next

The newly created service call appears in OPEN status and is ready for scheduling. The call entry stores customer, site, product, and problem information. You can now proceed to schedule the call with a technician using SVC-CALL-005, or request schedule options from the customer using SVC-CALL-004.

## Common Issues

**Customer or Site Not Found**
If the customer or site dropdown does not show the required entry, verify that the customer record exists in the system and that the site is linked to the customer. Return to the customer record and confirm the site setup before creating the service call.

**Missing Required Fields on Save**
The system will not save the call if required fields are blank. Review error messages to identify which fields need completion. Ensure Customer, Call Type, and CSR are populated at minimum before saving.

**Call Created but Not Visible in Dispatch Q**
After saving, the call may take a few moments to appear in the Dispatch Q. Click Refresh (circular arrow) in the Work Queues grid to see the updated list. Verify the call status is OPEN and that the correct branch/department filters are applied.
