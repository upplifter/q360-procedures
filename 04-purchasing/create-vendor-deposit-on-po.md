---
title: Create Vendor Deposit (Prepayment) on PO
id: PO-DEPOSIT-001
module: Purchasing
screen: Purchase Order Form
menu_path: Inventory > Purchase Orders
applies_to:
  - Purchasing Agent
  - Accounts Payable Clerk
  - Purchasing Manager
prerequisites:
  - User has VENDDEPOSIT permission
  - A PO exists for the vendor
  - The vendor's Customer/Vendor record has a Vendor Deposit Account configured on the Asset tab (see PO-VENDOR-001)
related_procedures:
  - PO-VENDOR-001
  - PO-CREATE-001
  - PO-SEND-001
tags: vendor deposit, prepayment, advance payment, deposit on PO, vendor prepay, vendor advance, deposit voucher, vendor deposit account
version: 1.0
last_updated: 2026-03-25
---

# Create Vendor Deposit (Prepayment) on PO

## What This Procedure Does

Create and post a deposit-type vendor voucher from a purchase order. A vendor deposit is a prepayment made before the final invoice is due, before work begins, or before product ships. The deposit is recorded as an asset and is later applied against the vendor's final invoice.

## Before You Begin

- You need the VENDDEPOSIT permission.
- A PO must exist for the vendor requiring the deposit.
- The vendor's Customer/Vendor record must have the **Vendor Deposit Account** field populated on the **Asset** tab. This GL account is where the deposit asset is tracked. If this field is empty, edit the vendor record first (see PO-VENDOR-001).

## Steps

### Step 1: Open the Purchase Order

Navigate to **Inventory > Purchase Orders** from the Main Navigation Sidebar (vertical panel, left edge). Search for and open the PO that requires a vendor deposit.

### Step 2: Verify the Vendor Deposit Account

Confirm the vendor's Vendor Deposit Account is configured. If uncertain, open the vendor's Customer/Vendor record, navigate to the **Asset** tab, and verify the GL account is populated.

### Step 3: Create the Vendor Deposit

Click the **Extended Menu** (three vertical dots on the Form Action Bar) on the PO form. Select **Create a Vendor Deposit**. A vendor voucher form opens for the miscellaneous expense deposit.

### Step 4: Enter Deposit Details

| Field | What to enter |
| --- | --- |
| Amount | The deposit amount to be paid to the vendor. |
| Description | A description of the deposit purpose (e.g., "50% deposit per vendor terms"). |

The voucher type is automatically set to DEPOSIT. The Vendor Order Reference Number is inherited from the PO if one was entered.

### Step 5: Save the Voucher

Click the **Save Record** button (floppy disk icon on the Form Action Bar) to save the deposit voucher.

### Step 6: Post the Voucher and Release for Payment

Click the **Extended Menu** (three vertical dots on the Form Action Bar) on the voucher. Select **Post Voucher and Release for Payment**. A confirmation window displays the vendor deposit balance available and confirms the application of the deposit against the voucher.

### Step 7: Verify Journal Entries

Click the **AP Journal** tab on the voucher to review the journal entries. The system debits the Vendor Deposit Account (asset) and credits Accounts Payable for the deposit amount.

## What Happens Next

The deposit is recorded as an asset on the vendor's account. When the vendor's final invoice arrives and is vouchered, the deposit balance is available to offset the total amount due. During voucher processing for the final invoice, a confirmation prompt displays the vendor deposit balance and allows you to apply it. The AP Journal tab shows all entries including the deposit application. The deposit appears in the Vendor Deposit subledger report during month-end reconciliation.

## Common Issues

**"Create a Vendor Deposit" option is not available in the extended menu.** Verify you have the VENDDEPOSIT permission. Also confirm the Vendor Deposit Account field is populated on the vendor's Asset tab. Both conditions must be met for the option to appear.

**Vendor Deposit Account is not set on the vendor record.** Open the vendor's Customer/Vendor record, navigate to the Asset tab, and enter the appropriate GL account number for vendor deposits. Save the vendor record, then return to the PO.

**Deposit was posted but the amount is incorrect.** If the deposit voucher has already been posted, you may need to create an adjusting entry. Contact your accounting team to determine the correct approach for correcting the deposit amount.

**Deposit is not being applied to the final invoice.** During final voucher processing, the system prompts you with the available deposit balance. Ensure you select Yes to apply the deposit. If the prompt does not appear, verify the deposit is posted and the vendor number on the final voucher matches the deposit voucher.

**Journal entries do not balance.** Review the Vendor Deposit Account GL number on the vendor record. If it was changed after the deposit was created, the original posting used the account that was configured at the time. Contact accounting to reconcile.
