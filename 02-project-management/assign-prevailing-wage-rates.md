---
title: Assign Prevailing Wage Rates to a Project
id: PROJ-WAGE-001
module: Projects
screen: Project Form
menu_path: Main Menu > Projects > Projects
applies_to:
  - Project Manager
  - Payroll Administrator
prerequisites:
  - PROJECT (Edit) permission
  - Prevailing wage rate codes configured in the system
related_procedures:
  - PROJ-RESOURCE-001
  - PROJ-TB-001
  - PROJ-TB-002
tags:
  - prevailing wage
  - wage rates
  - labor class
  - certified payroll
  - prevailing wage code
  - job costing
  - wage type
version: 1.0
last_updated: 2026-03-25
---

# Assign Prevailing Wage Rates to a Project

## What This Procedure Does

This procedure assigns a prevailing wage rate code to a project, establishing the wage schedule that applies to all team members recording time against the project. The prevailing wage code ensures that labor is charged and paid according to the applicable prevailing wage requirements for the project location and type.

## Before You Begin

- Verify you have PROJECT (Edit) permission assigned to your role
- Confirm that prevailing wage rate codes are configured in the system
- Have the appropriate prevailing wage rate code available for the project location and type
- Identify the correct wage schedule that applies to the project

## Steps

### Step 1: Look Up the Project
Navigate to the Projects module and locate the project to which you wish to assign prevailing wage rates.

### Step 2: Enter Edit Mode
Click Edit (pencil icon) to enable editing of the project form.

### Step 3: Locate the Prevailing Wage Rate Code Field
On the Project header tab, locate the Prevailing Wage or PW Rate Code field.

### Step 4: Select the Prevailing Wage Rate Code
Click the dropdown in the Prevailing Wage or PW Rate Code field and select the appropriate prevailing wage rate code. This code links the project to the correct wage schedule for the project location and type.

### Step 5: Save Your Changes
Click Save (floppy disk icon) to record the prevailing wage rate code assignment.

### Step 6: Verify the Assignment
The prevailing wage rate code is now associated with the project and will apply to all time entries recorded against this project.

## What Happens Next

When team members log time against this project, Q360 automatically applies the prevailing wage rate associated with the selected code. The system combines the prevailing wage code with each employee's default PW Labor Class to determine the appropriate wage rate for job costing, payroll processing, and certified payroll reporting. All subsequent time entries will use the assigned prevailing wage schedule.

## Common Issues

**The Prevailing Wage or PW Rate Code field is not visible on the project form.**
The field may not be displayed if your form is configured to hide it. Verify that you are on the Project header tab and refresh your browser to reload the form. If the field remains unavailable, contact your system administrator to verify field visibility settings.

**The prevailing wage rate code dropdown shows no options.**
Prevailing wage rate codes must be configured in your system before they can be assigned to projects. Contact your system administrator to verify that prevailing wage codes have been set up and are available for selection. The system administrator may need to create additional codes if the required code is not available.

**I cannot save the project after selecting a prevailing wage rate code.**
Verify that the prevailing wage rate code you selected is valid and complete. Some codes may have validation requirements. If the save fails with a validation error, retry selecting the code. Contact your system administrator if validation errors persist.

**The prevailing wage rate is not applied to time entries I record.**
Verify that the prevailing wage rate code has been successfully saved to the project by checking the Project header tab after saving. Ensure that team members recording time are using the updated project record. If the rate still does not apply, verify that the employee's PW Labor Class is correctly configured in their user profile.

**I need to change the prevailing wage rate code for an existing project.**
Edit the project and select a different prevailing wage rate code from the Prevailing Wage or PW Rate Code field. The change applies only to new time entries recorded after the change. Time entries recorded under the previous wage code retain their original rate. Save the project to confirm the change.
