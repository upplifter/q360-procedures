---
title: Create New Service Call from Approved Customer Order
id: SVC-CALL-003
module: Service
screen: Service Call Form
menu_path: Service > Service Calls
applies_to: Customer Service Representatives, Service Managers
prerequisites:
  - Approved customer order with Create Type = "Call"
  - Order line items populated with product details
related_procedures:
  - SALES-ORDER-001
  - SVC-CALL-001
  - SVC-CALL-005
tags:
  - service-call-creation
  - order-integration
version: 1.0
last_updated: 2026-03-25
---

# Create New Service Call from Approved Customer Order

## What This Procedure Does

When a customer order is approved with the Create Type set to "Call," the system automatically generates a service call. The call inherits customer, site, and line item details from the order. You review and schedule the generated call without manual data re-entry.

## Before You Begin

- Verify the order has been approved (not in draft or pending status)
- Confirm the order Create Type is set to "Call"
- Review the order line items to understand what products are being serviced
- Ensure the customer site is correctly identified in the order

## Steps

### Step 1: Locate the Generated Service Call

Open the customer record. Navigate to the Service Calls tab. The automatically generated call appears in the list with a status of OPEN and references the original order number. Alternatively, navigate to Service > Work Queues > Dispatch Q to locate the new call.

### Step 2: Open the Service Call

Click the call number to open the Service Call form. The Call tab displays with customer, site, and product information already populated from the order. Review the pre-filled fields for accuracy.

### Step 3: Verify and Complete Call Information

Review the following fields that were inherited from the order:

| Field | What is populated |
|-------|-------------------|
| Customer | Customer from the order |
| Site | Site from the order header |
| Product | Products from order line items |
| Call Type | Inherited from order configuration |
| Branch | Inherited from order branch |

Complete any additional fields not filled from the order:

| Field | What to enter |
|-------|---------------|
| Priority | Enter priority level 1-5 if not auto-populated |
| Problem Code | Select a problem code if needed |
| Problem Description | Add service details beyond what the order specifies |
| CSR | Select the Customer Service Representative |
| Department | Select the appropriate service department |

### Step 4: Save the Call

Click Save (floppy disk icon). The system retains the call in OPEN status and maintains the link to the original order.

## What Happens Next

The service call is now created and ready for scheduling. The call remains linked to the original order for billing and tracking purposes. Order line items are available on the Parts tab for reference. You can proceed with SVC-CALL-005 to schedule the call with a technician, or use SVC-CALL-004 to request schedule options from the customer.

## Common Issues

**Service Call Not Generated After Order Approval**
Verify that the order's Create Type is actually set to "Call." If it is set to a different type (e.g., "Invoice"), the system will not auto-generate a service call. Review the order configuration or manually create the call using SVC-CALL-001.

**Call Information Does Not Match Order Details**
If the call shows incomplete or incorrect customer or site information, the order data may not have been properly linked. Open the original order to confirm customer and site details, then manually update the service call fields as needed.

**Multiple Calls Created for a Single Order**
If the order has multiple line items, the system may create separate calls for each product line. Review the Service Calls tab to confirm you have the correct call number. Link related calls in the Events tab (SVC-CALL-009) if coordination between calls is needed.
