---
title: Create Schedule of Values (SOV)
id: PROJ-SOV-001
module: Projects
screen: Project Form > SOV Tab
menu_path: Main Menu > Projects > Projects
applies_to:
  - Project Manager
  - Accounts Receivable
prerequisites:
  - PROJECT (Edit) permission
  - PROJECTSOV permission
  - PROJECTSOV configuration set to ON
  - Project has approved line items
related_procedures:
  - PROJ-SOV-002
  - PROJ-INV-001
  - PROJ-GROUP-001
tags:
  - schedule of values
  - SOV
  - progress billing
  - create SOV
  - tax master
  - SOV-TAXABLE
  - SOV-NONTAXABLE
version: 1.0
last_updated: 2026-03-25
---

# Create Schedule of Values (SOV)

## What This Procedure Does

This procedure enables you to create a Schedule of Values (SOV) from your project's approved line items. An SOV organizes project deliverables for progress billing and revenue recognition. Before invoicing using the SOV, you must assign tax applicability codes to determine which items are subject to sales tax.

## Before You Begin

- Verify you have PROJECT (Edit) and PROJECTSOV permissions
- Confirm PROJECTSOV configuration is enabled in your system
- Ensure the project has approved line items ready for the SOV
- Consider updating project line item grouping first for optimal SOV structure (see PROJ-GROUP-001)

## Steps

### Step 1: Navigate to the SOV Tab
Look up the project in the Projects module. Click on the SOV tab to access the Schedule of Values section.

### Step 2: Initiate SOV Creation
Click Create SOV. Q360 displays available creation shortcut options.

### Step 3: Choose an SOV Creation Method
Select one of the available SOV creation shortcut options based on your project structure and grouping requirements. For best automatic results, update the grouping of project line items before creating the SOV (see PROJ-GROUP-001).

### Step 4: Assign Tax Applicability Codes
Before you can invoice using the SOV, assign tax applicability codes to SOV items:

a. Select all sales tax-applicable SOV lines.

b. Click the Items grid Extended Menu (3 vertical dots) and select Set Master for Selected Items.

c. Choose a miscellaneous M-type master configured for taxation (for example, SOV-TAXABLE).

d. Repeat the process for non-taxable line items, selecting a master configured for non-taxation (for example, SOV-NONTAXABLE).

### Step 5: Review and Customize the SOV
You have full control of the SOV once created. Review the structure and make any necessary adjustments to ensure accurate progress billing and revenue recognition.

## What Happens Next

The SOV is now established on your project and ready for use in invoicing. The assigned tax codes determine how each SOV item is treated during billing and revenue recognition processes. You can update SOV progress as work advances (see PROJ-SOV-002).

## Common Issues

**SOV creation appears to have no shortcut options available.**
If no shortcut options display when you initiate SOV creation, verify that the PROJECTSOV configuration is enabled in your system. Contact your system administrator if this setting appears disabled. Additionally, confirm that your project has at least one approved line item to create an SOV from.

**Tax applicability codes are not available in the Master dropdown.**
The miscellaneous M-type masters displayed in the dropdown must be configured for taxation or non-taxation in your system. Work with your system administrator to create or enable the appropriate masters (such as SOV-TAXABLE and SOV-NONTAXABLE) before proceeding with tax code assignment.

**Selected SOV line items do not appear after selecting them.**
Ensure you have selected SOV items in the Items grid before clicking the Extended Menu. The selection may be cleared if you navigate away from the grid. Re-select the desired items and immediately proceed to the Extended Menu.

**The SOV tab does not appear on the project form.**
Verify that PROJECTSOV permission is assigned to your user role and that the PROJECTSOV configuration is enabled in your system. If you have the required permission and configuration is enabled, refresh your browser to reload the project form.

**SOV creation fails with a validation error.**
Verify that all line items in the project are in an approved status before creating the SOV. Unapproved or draft line items may prevent SOV creation. Review and approve all project line items before attempting to create the SOV again.
