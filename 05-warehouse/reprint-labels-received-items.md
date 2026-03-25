---
title: Re-print Labels for Received Items
id: WH-LABEL-001
module: Warehouse
screen: Purchase Order Form > Line Items tab
menu_path: Purchasing > Purchase Orders > [select PO] > Line Items tab
applies_to:
  - Warehouse Staff
prerequisites:
  - PO items have been received (see WH-RECEIVE-001)
  - Label printer is configured and connected to your workstation
related_procedures:
  - WH-RECEIVE-001
tags: label, reprint, receiving, PO, barcode
version: 1.0
last_updated: 2026-03-25
---

# Re-print Labels for Received Items

## What This Procedure Does

Reprint PO receiving labels from the Purchase Order Line Items tab using the extended grid menu. Labels are reprinted when original labels are damaged, lost, or need to be duplicated for warehouse organization purposes.

## Before You Begin

- The purchase order has been fully or partially received (items show received quantities)
- You know which PO line items need label reprints
- A label printer is connected and configured to your workstation
- You have Warehouse Staff role or equivalent permissions

## Steps

### Step 1: Search and Open the Purchase Order

Navigate to **Purchasing > Purchase Orders**. Search for the PO by PO number, vendor name, or date range.

Click on the PO in the search results to open the Purchase Order form.

### Step 2: Navigate to Line Items Tab

On the Purchase Order form, click the **Line Items Tab**. The tab displays all line items on the PO, including:

- Line number
- Item/Master description
- Ordered quantity
- Received quantity
- Unit price
- Extended amount

### Step 3: Select Line Items to Reprint

Click on the line item rows you want to reprint labels for. You can:

- Click a single row to select one line item
- Click the checkbox at the top of the grid to select all line items
- Hold **Ctrl** (Windows) or **Cmd** (Mac) and click multiple rows to select multiple specific items

For reprinting, typically select the line items that have been received (Received Qty > 0).

### Step 4: Access Grid Extended Menu

On the Line Items grid toolbar, click the **Grid Extended Menu** button (three vertical dots on the grid toolbar). A menu appears with options for the selected line items.

### Step 5: Select Reprint Labels

From the Grid Extended Menu, click **Reprint Labels**. The label reprint dialog opens.

The dialog displays:

- List of selected line items
- Quantity to reprint (defaulting to received quantity)
- Printer selection dropdown
- Label format options (if available)

### Step 6: Verify Line Items and Quantities

Review the list of line items to reprint. Verify:

- The correct line items are listed
- The quantities match the received quantities
- No unintended items are included

If you need to adjust the quantity to print for a specific line item, edit the quantity field in the dialog (some systems allow this, others use the received quantity automatically).

### Step 7: Select Printer

From the Printer dropdown, select the label printer you want to print to. The dropdown shows all configured printers on your network.

If your label printer is not listed:

- Verify the printer is powered on and connected to the network
- Check printer configuration in your system settings
- Contact your IT support if the printer is not available

### Step 8: Print Labels

Click the **Print** button to send the labels to the selected printer. The system generates the labels based on:

- PO number
- Line item description
- Received quantity
- Receiving date
- Any other data configured for labels

Labels print to your selected printer. Verify that labels printed correctly and match the line items you selected.

### Step 9: Apply Labels to Received Items

Take the printed labels and attach them to the corresponding received items in the warehouse. Labels should be:

- Affixed to the package or bin where items are stored
- Positioned where they are easily visible and scannable
- Protected from damage or moisture (if applicable to your warehouse environment)

Labels provide barcode scanning reference during put-away and subsequent inventory operations.

## What Happens Next

The reprinted labels are now applied to received items in the warehouse. The labels:

- Support barcode scanning during put-away operations
- Remain on items as they are stored and allocated to orders
- Are reference points for warehouse location and item verification
- May be used in future receiving operations if items are returned or reworked

## Common Issues

**Selected line items do not appear in the reprint dialog**

Verify that line items are actually selected on the grid. Click on the line item rows to select them, then access the Grid Extended Menu again. If items still do not appear:

- Some systems may not allow reprinting for certain line item statuses
- Items may need to have received quantities > 0 to be eligible for reprinting
- Contact your system administrator if reprinting is restricted

**Label printer does not appear in the printer list**

Verify the printer is configured on your workstation:

- Check your computer's printer settings to confirm the label printer is installed
- Restart the Q360 application and try again
- Test the printer by printing a test page from your operating system printer settings

If the printer still does not appear, it may not be connected to the network. Contact your IT support to verify printer connectivity.

**Labels print but contain incomplete or incorrect information**

The label template may be configured incorrectly. Verify that:

- PO number, item description, and quantities are visible on the printed labels
- Date and receiving information is correct
- Barcode (if included) scans properly

If label content is incorrect, contact your system administrator to review label template settings.

**Cannot print to the specific printer I need**

If the printer is connected but not showing in the dropdown:

- Check that you have permission to print to that printer
- Verify the printer is on the network and not in offline/error status
- Try selecting a different printer as a test
- Contact your IT support for printer access issues

**Quantities printed do not match what I selected**

The system may use fixed quantities (e.g., received quantity) rather than custom quantities. If you need to print specific quantities:

- Print the labels as is, and mark extras for disposal
- Contact your Warehouse Manager about label quantity requirements
- Verify with your system administrator if quantity customization is available

**Labels jam or fail to print from the printer**

Check the printer for:

- Paper jams or obstructions
- Low or empty label stock
- Printer error lights or messages

Clear any jams, refill label stock, and retry printing. If the printer continues to fail, contact your IT support or printer vendor.
