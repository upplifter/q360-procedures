---
title: Create a Quote
id: SALES-QUOTE-001
module: Sales
screen: Quote Form
menu_path: Main Menu > Sales > Quotes
applies_to:
  - Sales Rep
  - Engineer
prerequisites:
  - QUOTE (Create) permission assigned to your user or group
  - A customer or prospect record exists (see SALES-PROSPECT-001)
  - For opportunity-linked quotes, an opportunity exists (see SALES-OPP-001)
related_procedures:
  - SALES-OPP-001
  - SALES-QUOTE-002
  - SALES-QUOTE-003
  - SALES-QUOTE-007
tags: quote, create quote, new quote, estimate, proposal, line items, sections, find product, quick list, quote builder, pricing
version: 1.0
last_updated: 2026-03-25
---

# Create a Quote

## What This Procedure Does

Builds a new sales quote including header information, sections, and line items. Quotes can be created from an opportunity or directly from a customer record. The completed quote flows through the confirmation, authorization, and submission process before customer approval generates an order.

## Before You Begin

- You have QUOTE (Create) permission.
- The customer or prospect record exists in Q360 (see SALES-PROSPECT-001).
- If linking to an opportunity, the opportunity already exists (see SALES-OPP-001).
- You have your bill of materials, labor estimates, and pricing ready.

## Steps

### Step 1: Start the Quote

**Scenario A - From an opportunity:** Look up the opportunity. Click the **Quotes** tab. Click the **Grid Add Row** button (plus icon) on the Quotes grid.

**Scenario B - From a customer record:** Look up the customer. Click the **Quotes** tab. Click the **Grid Add Row** button (plus icon) on the Quotes grid.

A new Quote form opens.

### Step 2: Fill In the Header

Click the **Header** tab on the Quote form and fill in the following fields.

| Field | What to enter |
|---|---|
| Title | A descriptive name for the quote. |
| Sale Type | Select the type of sale (e.g., Project, Service, Install). |
| Site | Select the customer site this quote applies to. |
| Contact | Select the customer contact for this quote. |
| Branch | Defaults from the company. Change if needed. |
| Department | Select the department. |
| Sales Rep | Defaults from the company. Change if needed. |

To link an existing quote to an opportunity after creation, click the opportunity **Link** button on the Header tab.

### Step 3: Set Up Sections (If Needed)

Click the **Sections** panel on the left side of the Line Items tab.

1. To add a section (e.g., a room, floor, or system), click the **Add** button in the Sections panel. Type the section name and click **Ok**.
2. To add a subsection, right-click an existing section and select **Add Sub Section**. Type the subsection name and click **Ok**.
3. To duplicate a section, right-click the section and choose **Duplicate Section**.
4. To rename a section, find the section header row in the Line Items grid and double-click the description column. Update the title and press **Enter**.
5. To reorder or nest sections, click and drag sections in the Sections panel.

### Step 4: Add Line Items

**From masters (catalog items):**

1. To add items within a specific section, double-click the section name in the Sections panel first. Otherwise, items are added to the UNASSIGNED section.
2. Click the **Find Product** panel on the left.
3. Type a search term (part number, description, or manufacturer) and press **Enter**. Use Advanced Search for more specific criteria, including master profiles (e.g., GPO price lists).
4. Click the **Add** button next to the desired item to add it to the quote.

**From Quick Lists (pre-built item sets):**

1. Select the target section in the Sections panel.
2. Click the **Quick List** panel on the left.
3. Click the plus button next to the quick list to add.
4. Choose whether to keep the parent costs and prices or use current dynamic pricing from masters.
5. Click **Add**. Q360 prompts to add the quick list as a subsection.

**Manual line items (non-catalog):**

1. Close any open left-side panel by clicking the panel name.
2. Click the **Grid Add Row** button (plus icon) on the Line Items grid.
3. Fill in the description, unit cost, unit price, vendor part number, and manufacturer columns.

To delete line items, select them and click the Line Items grid **Delete** button (trash can icon).

### Step 5: Adjust Line Items

With items added, you can adjust values in any editable column (indicated by a pencil icon in the column header).

- Update **Quantity** on a section row to act as a section multiplier.
- Select multiple cells vertically in one column, right-click, and choose **Set Value** to batch-update.
- Use the Line Items grid **Extended Menu** (three vertical dots) for additional batch update commands.
- Check the **Optional** checkbox on line items to exclude them from the quote total while still showing them to the customer.
- To reorder items, click the Line Items grid **grouping mode button**, drag items, then click the button again to exit.

### Step 6: Set Line Item Groupings (If Needed)

Groupings carry forward to downstream records (projects, warehouse) while sections do not.

1. In the Sections panel, double-click **ALL** to show all sections.
2. In the Line Items grid, click the expand button (+) to show all items.
3. Select all line items using the select all button.
4. Click the Line Items grid **Extended Menu** and select **Update Group Fields by Section**.
5. Leave the option to dynamically update groups based on sections and click **Confirm**.

### Step 7: Save and Confirm the Quote

1. Click the **Save Record** button (floppy disk icon) to save your work.
2. When the quote is complete and ready for internal review, click the **Process Actions** button (gear icon) on the form action bar, then click **Confirm**.

## What Happens Next

The quote status changes to CONFIRMED and appears in the **Confirmed Quotes** bucket in the Sales Overview workflow. A sales manager or authorized user can now review and authorize the quote (see SALES-QUOTE-003).

Before authorization, you can manage revisions to preserve a snapshot of the current quote state (see SALES-QUOTE-002). If the quote was copied from an older quote, refresh line item pricing to current catalog values (see SALES-QUOTE-007).

## Common Issues

**The Find Product panel returns no results.**
Broaden your search by using fewer characters. Check for typos in the search term. You can also adjust category and subcategory filters in Advanced Search mode.

**Line items are added to the UNASSIGNED section.**
Double-click the target section name in the Sections panel before adding items. If items were added to the wrong section, use grouping mode to drag them to the correct section.

**The quote total does not match expectations.**
Check for items marked as Optional - these are excluded from the total. Also verify the section multiplier quantities are correct.

**The Confirm action fails or is not available.**
Ensure the quote has at least one line item and that all fields expected by your system configuration are filled in. Check the Process Actions menu for available actions based on the quote's current status.

**You cannot see the Sections panel.**
Click the **Grid Sections Toggle** button (list icon with horizontal lines) on the Line Items grid toolbar to show or hide the Sections panel.
