---
title: Monitor Materials Status
id: PROJ-MAT-002
module: Projects
screen: Project Form > Materials Tab
menu_path: Main Menu > Projects > Projects
applies_to: Project Manager
prerequisites: PROJECT (View) permission, Project has materials with PO Release dates set (see PROJ-MAT-001)
related_procedures:
  - PROJ-MAT-001
  - PROJ-PRODUCT-001
tags:
  - materials status
  - PO status
  - ETA
  - received
  - shipped
  - staging location
  - tracking
  - project materials
  - procurement
  - purchasing
version: 1.0
last_updated: 2026-03-25
---

# Monitor Materials Status

## What This Procedure Does

This procedure tracks PO status, ETA dates, received dates, and staging locations of project line items from the Materials tab. Monitoring material status ensures materials arrive on schedule and helps coordinate delivery and installation timelines with project work.

## Before You Begin

Ensure you have PROJECT (View) permission. The project must have materials on the Materials tab with PO Release dates set (refer to PROJ-MAT-001 to set release dates if needed).

## Steps

### Step 1: Open the Project

Navigate to Main Menu > Projects > Projects. Search for and open the desired project to monitor.

### Step 2: Navigate to Materials Tab

Click the Materials tab on the project form. The grid displays all line items and their current procurement status.

### Step 3: Identify Line Items to Check

Locate the specific line items you want to monitor. Review the columns described below to understand material status at a glance.

### Step 4: Check PO Status Column

Examine the PO Status column for each line item. Understand the following status values:

- **DATAENTRY**: The item is on a purchase order but the order has not yet been confirmed or sent to the vendor. Note the PO ETA Date column to see the expected delivery date.
- **RECEIVED**: The item has been received at the warehouse or facility. Note the PO Received Date column to see when it arrived.

When an item status shows RECEIVED, the corresponding order line-item status should typically read PICKED (see Step 5 below).

### Step 5: Check Order Line-Item Status Column

Review the status of the order line item itself (distinct from the PO status). Understand the following status values:

- **DATAENTRY**: The line item has not yet been picked from stock or shipped to the project site.
- **PICKED**: The corresponding PO item was received at the warehouse or the item was physically picked from stock and staged for shipment.
- **SHIPPED**: The line item has been physically shipped to the project site. Note the Courier and Waybill columns for inbound tracking information.

### Step 6: Track Drop-Ship Items

For items arriving via drop-ship (vendor ships directly to project site), note the PO Courier and PO Waybill columns. These provide tracking information for the inbound shipment. Monitor these details to know when drop-ship items will arrive.

### Step 7: Monitor ETA Dates

Review the PO ETA Date column for items that have not yet been received. This date indicates when the vendor is expected to deliver the material. Compare the ETA to your project schedule to identify any potential delays.

### Step 8: Monitor Received Dates

Review the PO Received Date column for items that have been received. This date shows when the material arrived at the warehouse. Use this information to confirm materials are in stock and available for picking.

### Step 9: Note Staging Location

Review the Staging Location column to see where each material is currently stored. This helps coordinate material availability with project installation timelines. Materials in the correct staging location are ready for pickup or delivery to the project site.

### Step 10: Update Staging Locations

If you need to change the staging location for one or more materials (e.g., move items to a loading dock for delivery), select those items in the grid and click the Materials grid Extended Menu (3 vertical dots). Choose the option to update or set staging location. Select the new location and apply the change.

## Monitor Project Buckets for Material Issues

### Step 1: Access Projects Overview

Click Workflow > Projects Overview. This workflow view shows project status buckets and material-related alerts.

### Step 2: Review Material Status Buckets

Watch for dedicated buckets that flag material issues:
- Equipment Availability: Shows materials ready for use
- Items with No ETA: Shows materials without delivery date information
- Overdue ETA: Shows materials that should have arrived but have not
- ETA Past Request Date: Shows materials with delivery dates later than the requested delivery date

### Step 3: Take Action on Alerts

Projects appearing in negative material status buckets need immediate attention. Review the Materials tab for these projects and contact vendors or purchasing to expedite deliveries or resolve delays.

## What Happens Next

You have reviewed material status and identified any potential delays or issues. Continue to monitor materials regularly as your project progresses. Update staging locations and monitor ETAs to ensure materials arrive when needed for project work. Coordinate with the purchasing and warehouse teams when issues arise.

## Common Issues

**PO Status Shows DATAENTRY But Expected Delivery Is Soon**
DATAENTRY status means the purchase order has not yet been sent to the vendor. Contact the purchasing department to confirm the order was placed. There may be a system lag before PO status updates to reflect the confirmed order.

**Item Shows SHIPPED But Has Not Arrived at Project Site**
Check the Courier and Waybill columns for tracking information. Use the waybill number to track the shipment with the delivery company. Confirm the correct delivery address was provided on the purchase order.

**Staging Location Is Incorrect or Needs to Change**
Select the line item(s) and use the Materials grid Extended Menu (3 vertical dots) to update the staging location. This allows you to move materials to a new location as project needs change.

**ETA Date Is in the Past**
If the ETA has passed and status is still DATAENTRY or not yet RECEIVED, the material is overdue. Contact the vendor immediately to determine the revised delivery date. The material may have been delayed in transit.

**Multiple Items Missing ETAs in PO ETA Date Column**
Items without ETA dates cannot be reliably scheduled into project work. Contact purchasing or the vendor to obtain confirmed ETAs. Update the PO ETA Date once the vendor provides delivery information.

**Cannot See All Materials Tab Columns**
The Materials tab grid may require horizontal scrolling to view all columns. Use the horizontal scroll bar at the bottom of the grid to navigate left and right across columns like Courier, Waybill, and Staging Location.
