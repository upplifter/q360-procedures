---
title: Get Customer Authorization on Service Call
id: SVC-CALL-012
module: Service
screen: Service Call
menu_path: Service > Service Calls
applies_to: CSRs, Service Managers, Technicians
prerequisites:
  - Service call is open
  - Customer must be defined on the call
  - Parts or labor estimates are populated
related_procedures:
  - SVC-CALL-011
  - SALES-QUOTE-004
tags:
  - customer authorization
  - quotes
  - approval workflow
  - customer communication
version: 1.0
last_updated: 2026-03-25
---

# Get Customer Authorization on Service Call

## What This Procedure Does

Convert a service call into a quote for customer pre-approval. The system generates a quote document pre-populated with the call's customer, service location, and estimated parts and labor. Submit the quote to the customer for review and approval before proceeding with work.

## Before You Begin

- The service call must be in status OPEN, SCHEDULED, or DISPATCHED
- The customer and service location must be defined on the call
- Parts or labor estimates should be entered on the call
- You must have the ability to send documents to the customer or have a communication method available

## Steps

### Step 1: Open the Service Call

Open the service call for which you need customer authorization.

### Step 2: Access the Create Quote Function

Click the Extended Menu (three vertical dots) on the action bar. Select Create Quote or Get Authorization from the menu options. The system generates a new quote document.

### Step 3: Review the Generated Quote

The quote form opens pre-populated with:

- Customer information from the service call
- Service location (site/address)
- Line items reflecting parts and estimated labor from the call
- Pricing and totals calculated from the call estimates

Review all details for accuracy. Update any quantities, descriptions, or pricing if needed.

### Step 4: Complete the Quote

Fill in any missing fields required for quote approval:

| Field | What to enter |
|-------|--------------|
| Quote Expiration Date | Date by which customer must approve |
| Terms | Payment terms and conditions |
| Special Notes | Any terms, warranty, or conditions |
| Quote Method | Select quote delivery method (Email, Print, etc.) |

### Step 5: Submit to Customer

Save the quote. Click the Send or Submit button to deliver the quote to the customer. Follow your standard communication process to ensure the customer receives and reviews the quote. Reference SALES-QUOTE-004 for detailed quote management procedures.

## What Happens Next

The quote is logged in the system and linked to the original service call. A unique quote number is assigned. The customer receives notification and can approve or request modifications. Once the customer approves the quote, the system links the approved quote back to the service call. The work authorization is documented, and the technician can proceed with the call (see SVC-CALL-001). If the customer approves, the call status updates to reflect authorization, and work can resume.

## Common Issues

**Quote creation fails or shows error**

Verify the customer is defined with complete contact information on the service call. Check that the service location is valid and associated with the customer. Ensure parts or labor items are entered on the call before creating the quote. If the error persists, try refreshing the call form and attempting again.

**Customer cannot locate or access the quote**

Confirm the quote was sent to the correct email address or contact method. Check the customer's email spam folder if delivery method was email. Re-send the quote using the Extended Menu > Send/Resend Quote option. If the customer still cannot access, verify contact information is correct and try an alternate delivery method.

**Approved quote is not linking back to the service call**

Verify the approval was processed in the quote record (see SALES-QUOTE-004). Check that the quote status shows as Approved in the system. The link may be delayed briefly while the system processes. Refresh the service call form to see the updated status. If not linked within a few minutes, contact your system administrator.
