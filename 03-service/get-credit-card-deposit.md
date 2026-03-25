---
title: Get Credit Card Deposit on Call
id: SVC-CALL-016
module: Service
screen: Service Call
menu_path: Service > Service Calls
applies_to: Technicians, CSRs, Service Managers
prerequisites:
  - Service call is open
  - Authorize.net integration is configured in the system
  - SHOWBETAAPICREDITCARD configuration is enabled
  - Customer is present and has payment authorization
related_procedures:
  - SVC-CALL-001
  - SVC-CALL-018
tags:
  - payment processing
  - deposits
  - credit card
  - field billing
version: 1.0
last_updated: 2026-03-25
---

# Get Credit Card Deposit on Call

## What This Procedure Does

Process a credit card deposit payment on a service call in the field or office. The system opens a payment dialog pre-populated with the call's estimated bill amount. You can adjust the amount and process the payment through the Authorize.net payment gateway. The deposit is recorded against the call and applied to the final invoice.

## Before You Begin

- The service call must be open
- Authorize.net payment integration must be configured by your system administrator
- The SHOWBETAAPICREDITCARD configuration setting must be enabled
- The customer must authorize payment and have a valid credit card available
- The call should have an estimated or final billing amount

## Steps

### Step 1: Open the Service Call

Open the service call for which you need to collect a deposit or payment.

### Step 2: Access the Credit Card Deposit Function

Click the Extended Menu (three vertical dots) on the action bar. Select Credit Card Deposit from the menu options. The "Enter a Value" payment window opens.

### Step 3: Review and Adjust Payment Amount

The payment window displays the call's estimated bill amount pre-populated:

| Field | Description |
|-------|-------------|
| Amount | Pre-filled with call bill total; adjust if needed |
| Payment Type | Credit Card |

Review the amount. If you need to collect a partial deposit, edit the amount to the required deposit value. Click OK to proceed to the payment form.

### Step 4: Enter Credit Card Details

The payment form opens. Enter the customer's credit card information:

| Field | What to enter |
|-------|--------------|
| Card Number | Full 16-digit credit card number |
| Expiration Date | MM/YY format |
| CVV | 3 or 4-digit security code |
| Cardholder Name | Name on card |
| Cardholder Address | Billing address for the card |

Ensure the customer is present and authorizes the charge. Do not enter card details without explicit customer consent.

### Step 5: Process the Payment

Click Process Payment or Submit. The system transmits the payment to Authorize.net for processing. A confirmation message appears with transaction details and confirmation number.

### Step 6: Save the Deposit to the Call

The system automatically records the processed payment as a deposit on the service call. The deposit appears in the call's financial summary. The amount is reserved against the final invoice.

## What Happens Next

The credit card deposit is recorded and linked to the service call. The deposit amount is deducted from the final invoice total when the call is closed (see SVC-CALL-018). A payment receipt is generated and can be provided to the customer. The payment is logged in the accounts receivable system. When the call is invoiced, the remaining balance is billed separately if applicable.

## Common Issues

**Credit Card Deposit option does not appear in Extended Menu**

Verify that Authorize.net integration is configured in system settings. Confirm that the SHOWBETAAPICREDITCARD configuration is enabled. Check that your user role has permissions to process payments. If the option still does not appear, contact your system administrator.

**Payment is declined by Authorize.net**

Verify the credit card information is entered correctly (number, expiration date, CVV). Confirm with the customer that the card is active and has sufficient funds. Check that the card is not flagged for fraud. If the card is declined multiple times, ask the customer to contact their bank or use a different card.

**Payment processes but does not appear on the service call**

Verify the payment was confirmed with a transaction number. The deposit may be delayed briefly while the system syncs. Refresh the service call to see the updated deposit status. If the payment still does not appear after several minutes, note the transaction number and contact your system administrator to verify the payment was recorded in the accounts receivable system.
