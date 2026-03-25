---
title: Print Call Report
id: SVC-CALL-019
module: Service
screen: Service Call
menu_path: Service > Service Calls
applies_to: Technicians, CSRs, Service Managers
prerequisites:
  - Service call is open or closed
  - Call has associated data (customer, location, work details)
related_procedures:
  - SVC-CALL-018
  - SVC-CALL-021
tags:
  - reports
  - call documentation
  - printing
  - pdf export
version: 1.0
last_updated: 2026-03-25
---

# Print Call Report

## What This Procedure Does

Generate and print a service call report. Select from available report templates, choose output destination (screen, printer, email), select output format (PDF, Excel), and configure display options. The call report can include customer signature, parts list, labor details, and other call information.

## Before You Begin

- The service call must be open or closed
- The call must contain the data you want to include in the report
- Your system must have report templates configured
- For email delivery, the customer must have a valid email address on record

## Steps

### Step 1: Open the Service Call

Open the service call for which you want to print a report.

### Step 2: Click Print Report

Click Print Report (printer icon) on the action bar. The Print Report dialog opens.

### Step 3: Select Report Template

The Print Report dialog displays available templates:

| Template Option | Content Included |
|-----------------|-----------------|
| Standard Call Report | Customer, site, problem, solution, parts, labor |
| Work Order | Problem description and work instructions |
| Invoice Report | Billing details, amounts, payment terms |
| Summary Report | Call overview without detailed line items |

Select the template that best fits your reporting need. Review the template name to ensure it matches your intent.

### Step 4: Set Output Destination

Select where the report should be delivered:

| Destination | Use Case |
|-------------|----------|
| Screen | View before printing or saving |
| Printer | Send directly to a connected printer |
| Email | Send report as attachment to customer email |
| File | Save report to system or network location |

### Step 5: Set Output Format

Select the format for the output:

| Format | Best For |
|--------|----------|
| PDF | Professional appearance, email distribution, archive |
| Excel | Data analysis, spreadsheet integration, manipulation |
| HTML | Web viewing, email without attachments |

### Step 6: Configure Display Options

Check or uncheck options to control report content:

| Option | Effect |
|--------|--------|
| Save Record | Saves a copy in call documents |
| Include Signature | Adds customer signature if captured |
| Include Parts Detail | Lists all parts with costs |
| Include Labor Detail | Lists all time entries with technician names |
| Include Photos | Includes any photos attached to call |
| Include Comments | Includes internal notes and communications |

Select options appropriate for your audience (customer-facing vs. internal).

### Step 7: Click Print or Generate

Click Print, Generate, or OK (depending on your interface) to create the report. The system generates the report in the selected format.

### Step 8: Review and Deliver

If the destination is Screen, review the report for accuracy before printing. For Printer, the report prints automatically to the selected printer. For Email, enter the recipient email address and send. For File, the system saves the report to the designated location.

## What Happens Next

The report is generated in the selected format and delivered to the chosen destination. Screen-view reports remain open for review or can be printed from your browser. Printer-sent reports appear at the designated printer. Email-delivered reports are sent as attachments. File-saved reports are archived in the call's documents or a central repository. The report can be printed again at any time by reopening the call.

## Common Issues

**Print Report button does not appear on action bar**

Verify the call is open in the system. Some read-only views may not show the Print Report option. Click Edit (pencil icon) to enter edit mode and try again. If the option still does not appear, contact your system administrator to verify report generation is enabled.

**Selected report template shows as blank or missing data**

Verify the call has the data the template expects (problem description, solution, parts, labor). If a field is blank, the template may not display that section. Try selecting a different template. If all templates appear blank, the call may be newly created or missing critical data. Save the call and try again.

**Email delivery fails or does not send**

Verify the customer has a valid email address entered on the call. Check that your system has email integration configured. If the email bounces back, verify the address is correct. Contact your system administrator if email delivery is not working.

**Report output shows incorrect or incomplete data**

Verify the selected template includes the data you want. Check that the call record has been saved with all current information (refresh the call before printing). If data is still missing, the call may need updates. Edit the call, add missing information, and save before printing again.
