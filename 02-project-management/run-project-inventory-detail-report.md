---
title: Run the Project Inventory Detail Report
id: PROJ-RPT-022
module: Projects
screen: Project Inventory Detail Report
menu_path: Main Menu > Projects > Reports > Project Inventory Detail
applies_to: Project Manager, Warehouse Manager, Purchasing Manager
prerequisites: null
related_procedures:
  - PROJ-MAT-002
  - PROJ-MAT-001
tags:
  - inventory detail
  - project inventory
  - inventory allocation
  - material detail
  - stock status
  - project materials
version: 1.0
last_updated: 2026-03-25
---

# Run the Project Inventory Detail Report

## What This Procedure Does

This procedure shows you how to run the Project Inventory Detail Report. The report displays materials and inventory items allocated to or used on projects, helping you track material usage, availability, and project inventory status.

## Before You Begin

Ensure you have access to the Projects module and Reports section. You should understand your organization's material allocation practices and which projects you want to review. Have your project and material criteria in mind before starting.

## Steps

### Step 1: Navigate to the Report

From the Main Menu, click **Projects**. In the Projects menu, click **Reports**. Select **Project Inventory Detail** from the report list.

### Step 2: Set Filter Criteria

The report filter panel opens with fields for detailing project inventory. Set the filters using the table below:

| Field | What to enter |
|-------|---------------|
| Project | Select specific projects or leave blank for all |
| Material Type | Choose material types or leave blank for all |
| Status | Select In Stock, Allocated, Used, or All statuses |
| Warehouse | Select a warehouse or leave blank for all |
| Date Range | Enter the period for material activity |

Click **Apply Filters** to update the report with your selections.

### Step 3: Run the Report

Click the **Run** or **Refresh** button to execute the report with your chosen filters.

### Step 4: Review the Report Output

The report displays detailed inventory information by project, including material descriptions, quantities, unit costs, and status. Review material allocations to confirm materials are assigned to the correct projects. Check quantities and availability to ensure adequate stock for active projects.

### Step 5: Export or Print (Optional)

To save the report, click **Export** and choose your format (Excel, PDF, or CSV). To print, click **Print** and follow your printer settings.

## What Happens Next

The project inventory detail data provides visibility into material usage and allocation across projects. Use this information for inventory management, material planning, and cost control. Share the report with warehouse, purchasing, and project management teams for coordination and planning.

## Common Issues

**Report shows more inventory than expected for a project**
Review allocation dates and quantities to confirm materials have been properly assigned. Materials may be allocated for future project phases. Verify that allocated quantities match planned usage with the project manager.

**Inventory appears to be missing from the report**
Confirm that materials have been allocated to the project and that the allocation status is active. Materials in planning stages may not yet be allocated. Check your filter selections to ensure the correct statuses and date ranges are included.

**Quantities and costs do not match purchase orders**
Verify that all purchase receipts have been recorded in the system. Unmatched receipts may show in purchasing records but not in inventory. Confirm that receipt matching and inventory transactions are complete.

**Report shows used materials on projects that have not started**
This may indicate that materials were transferred to a project before active work began, or that material usage is being recorded in advance. Review project schedules and material transaction dates to confirm the activity is intentional.

**Warehouse allocation differs from project records**
Discrepancies may indicate unreconciled inventory transfers or materials that have been reallocated. Review warehouse receipts and project material lists to identify the source of differences. Coordinate with warehouse and project teams to reconcile.
