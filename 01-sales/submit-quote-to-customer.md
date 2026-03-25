---
title: Submit Quote to Customer
id: SALES-QUOTE-004
module: Sales
screen: Quote Form / Print Report Dialog
menu_path: Workflow > Sales Overview > Authorized Quotes bucket
applies_to:
  - Sales Rep
  - Sales Manager
prerequisites:
  - QUOTE (View) permission assigned to your user or group
  - The quote is in AUTHORIZED status (see SALES-QUOTE-003)
related_procedures:
  - SALES-QUOTE-003
  - SALES-QUOTE-005
  - SALES-QUOTE-006
tags: submit quote, email quote, print quote, send quote to customer, quote PDF, authorized quote, customer submission, quote delivery
version: 1.0
last_updated: 2026-03-25
---

# Submit Quote to Customer

## What This Procedure Does

Prints and emails an authorized quote to the customer. The quote can be previewed on screen before sending. Submitting the quote changes its status and moves it to the Submitted Quotes bucket in the Sales Overview workflow, where it awaits customer approval.

## Before You Begin

- The quote is in AUTHORIZED status (see SALES-QUOTE-003).
- You know the customer contact's email address.
- You have selected the correct print template for your organization.

## Steps

### Step 1: Open the Authorized Quote

Navigate to **Workflow > Sales Overview** (or **Workflow > My Sales**). Click the **Authorized Quotes** bucket. Drill into the quote you want to submit.

### Step 2: Preview the Quote (Recommended)

1. Click the **Print Report** button (printer icon) on the form action bar.
2. In the Print Report dialog, select the desired template.
3. Set **Print Destination** to **Screen**.
4. Click **Print**. A preview opens in a new browser tab.
5. Review the output for accuracy. If changes are needed, return to the quote, edit and save, then refresh the preview tab.

### Step 3: Email the Quote to the Customer

1. Return to the Print Report dialog (click the **Print Report** button again if the dialog closed).
2. Set **Print Destination** to **Email**.
3. Select a recipient in the Print dialog, or type the email address in the compose window that opens when you click **Print**.
4. Before clicking Print, check the **Add PDF to Quote** box to save the emailed PDF as an attachment on the quote record.
5. Click **Print**. The email compose window opens. Review the message and click **Send**.

## What Happens Next

The quote status changes to SUBMITTED. It appears in the **Submitted Quotes** bucket in the Sales Overview workflow. The customer reviews the quote and communicates their decision.

When the customer approves the quote, mark it as customer approved to convert it to an order (see SALES-QUOTE-006).

## Common Issues

**The Print Report dialog shows no templates.**
Print templates must be configured by your administrator. Contact them to verify templates are available and assigned to the Quote form.

**The email does not send.**
Verify the recipient email address is correct. Check that your Q360 email configuration (SMTP) is set up properly. Contact your administrator if emails fail consistently.

**The PDF attachment is not saved to the quote.**
Ensure you checked the **Add PDF to Quote** box in the Print dialog before clicking Print. If missed, re-send the quote with the box checked to attach the PDF.

**You need to resubmit a revised quote.**
If the quote was returned to an earlier status for revisions, make the changes, save, re-confirm, re-authorize, and re-submit using the same steps.

**The customer received the quote but the status did not change.**
The status change depends on completing the Print/Email action through the Print Report dialog. If you emailed the document outside of Q360 (e.g., from your personal email), the quote status may not have updated automatically. Use the Process Actions menu to update the status manually if your system supports it.
