---
title: Send PO to Vendor
id: PO-SEND-001
module: Purchasing
screen: Purchase Order Form
menu_path: Inventory > Purchase Orders
applies_to:
  - Purchasing Agent
  - Purchasing Manager
prerequisites:
  - User has permission to confirm and send purchase orders
  - A PO exists in DATAENTRY status with all line items finalized (see PO-CREATE-001 or PO-CREATE-002)
related_procedures:
  - PO-CREATE-001
  - PO-CREATE-002
  - PO-UPDATE-001
tags: send PO, confirm PO, email PO, print PO, purchase order send, vendor notification, PO confirmation, approve PO
version: 1.0
last_updated: 2026-03-25
---

# Send PO to Vendor

## What This Procedure Does

Confirm a purchase order to finalize it, then print, preview, or email the PO document to the vendor. Confirming the PO changes its status from DATAENTRY to CONFIRMED, locking it from further edits, and activates the schedule for tracking.

## Before You Begin

- You need permission to confirm purchase orders.
- The PO must be in DATAENTRY status with all line items, quantities, and costs reviewed and finalized.
- If emailing the PO, verify the vendor's email address is configured in their Customer/Vendor record.

## Steps

### Step 1: Open the Purchase Order

Navigate to **Inventory > Purchase Orders** from the Main Navigation Sidebar (vertical panel, left edge) and search for the PO. Alternatively, from the Purchasing workflow, click the **Count of POs to Confirm** bucket to see all POs in DATAENTRY status. Double-click the PO to open it.

### Step 2: Confirm the PO

Click the **Process Actions** button (gear icon on the Form Action Bar). Select **Confirm PO** from the menu. The PO status changes from DATAENTRY to CONFIRMED. The PO can no longer be edited.

### Step 3: Print or Email the PO to the Vendor

Click the **Print Report** button (printer icon on the Form Action Bar). The Print Report dialog opens.

| Field | What to enter |
| --- | --- |
| Template | Select the PO report template from the list. Choose the standard PO template or your organization's custom template. |
| Destination | Select **Printer** to print a physical copy, **Preview** to view on screen, or **Email** to send directly to the vendor. |
| Format | Select the output format (e.g., PDF). |

1. If emailing, enter or confirm the vendor's email address in the recipient field. Add a subject line and any message text.
2. Click **Print** or **Send** to execute.

### Step 4: Record the Vendor Order Reference (If Available)

If the vendor provides an order confirmation number or reference, open the PO by clicking the **Edit Record** button (pencil icon on the Form Action Bar) if allowed, or note the reference in the PO's Vendor Order Ref field for tracking purposes.

## What Happens Next

The PO moves from the **Count of POs to Confirm** bucket to the **Count of POs to Receive** bucket on the Purchasing workflow. The items on the PO remain in On Order status on the master inventory until they are received. Proceed to update ETA and shipping information as the vendor provides it (see PO-UPDATE-001). When the items arrive, process the receiving in the Warehouse module (see WH-RECEIVE-001).

## Common Issues

**Confirm PO option is grayed out or unavailable.** The PO may already be confirmed or you may lack the required permission. Check the PO status in the header. Contact your system administrator if you need the permission to confirm POs.

**Vendor email address is missing when trying to email.** The email address is pulled from the vendor's Customer/Vendor record. Open the vendor record, add the email address on the Company or Contact tab, then return to the PO and retry.

**PO needs changes after confirmation.** Once confirmed, the PO cannot be edited through normal means. If critical changes are needed, contact your purchasing manager to determine whether the PO can be unconfirmed or whether a new PO should be created. For items that need to be removed, use the extended menu to cancel specific line items.

**Print template is not available.** Your system administrator configures available report templates. If the expected PO template is missing, contact your administrator to verify the template is assigned to the PO form.

**PO was confirmed but not sent to the vendor.** Confirming and sending are separate steps. A confirmed PO that was never printed or emailed still needs to be communicated to the vendor. Reopen the PO and use the Print Report button to send it.
