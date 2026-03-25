---
title: Run the Employee Assignee Detail Forecast Report
id: PROJ-RPT-008
module: Projects
screen: Employee Assignee Detail Forecast Report
menu_path: Main Menu > Projects > Reports > Employee Assignee Detail Forecast
applies_to:
  - Project Manager
  - Operations Manager
  - Resource Manager
prerequisites:
  - Access to the Projects module with resource allocation permissions
  - Understanding of resource assignments and capacity planning
  - Access to employee and task assignment data
related_procedures:
  - PROJ-RPT-007
  - PROJ-RPT-009
  - PROJ-RESOURCE-001
tags:
  - employee assignee
  - detail forecast
  - assigned hours
  - resource forecast
  - employee workload
  - capacity planning
version: "1.0"
last_updated: "2026-03-25"
---

# Run the Employee Assignee Detail Forecast Report

## What This Procedure Does

The Employee Assignee Detail Forecast Report shows assigned hours broken down by individual employee across projects and time periods. For each employee and project task, it displays assignment start and end dates, estimated effort, actual effort, and remaining effort. Use this report to understand individual workloads, identify overallocated or underutilized resources, and plan capacity across your project portfolio.

## Before You Begin

- Have access to the Projects module with resource management permissions
- Identify the time period you want to analyze
- Know which employees or departments you want to focus on
- Understand your organization's resource allocation and utilization targets

## Steps

### Step 1: Navigate to the Employee Assignee Detail Forecast Report

From the main menu, select **Projects > Reports > Employee Assignee Detail Forecast**. The report screen displays with filter options for employee and date selection.

### Step 2: Set Your Filters

Configure the filters to specify which employees and time period to analyze:

| Field | What to enter |
|-------|---------------|
| Company | Select one or more companies, or leave blank for all |
| Branch | Select one or more branches, or leave as ALL for all branches |
| Department | Select one or more departments, or leave as ALL for all departments |
| Employee | Select one or more employees, or leave as ALL to include all employees |
| Date Range | Enter the start and end dates for the analysis period |

### Step 3: Click Run

Click the **Run** button to execute the report.

### Step 4: Review the Report Output

The report displays a detailed grid with one row per employee-project assignment. Columns typically include:

- **Employee Name/ID:** The team member assigned to the task
- **Project Name/ID:** The project to which the employee is assigned
- **Task/Role Description:** The specific task or role (e.g., "Senior Developer," "Project Lead")
- **Assignment Start Date:** When the assignment begins
- **Assignment End Date:** When the assignment is scheduled to end
- **Estimated Effort (Hours):** Total hours budgeted for the assignment
- **Actual Effort (Hours):** Hours already worked or recorded
- **Remaining Effort (Hours):** Forecasted hours still to be expended
- **Utilization %:** Percentage of the employee's available time allocated to this assignment (if configured)

### Step 5: Assess Individual Workloads

Review each employee's total assignments across the date range:

- **High Utilization:** Employees assigned to multiple projects or with total allocated hours exceeding available capacity
- **Low Utilization:** Employees with significant gaps in assignments, indicating available capacity
- **Overallocation:** When an employee's assignments exceed a standard workweek, indicating scheduling conflicts or overload

### Step 6: Identify Capacity Issues

Look for patterns indicating resource constraints:

- **Overallocated Employees:** Team members assigned to more hours than they have available
- **Idle Resources:** Employees with gaps between assignments
- **Skill Bottlenecks:** If the report shows key technical skills assigned to many projects simultaneously

### Step 7: Plan Resource Adjustments

Use the information to:

- Reallocate work among team members to balance capacity
- Identify training or hiring needs to address skill gaps
- Plan resource leveling to eliminate scheduling conflicts
- Adjust project schedules to accommodate resource constraints

### Step 8: Export or Print (Optional)

Use the export or print functions to save the report as Excel, PDF, or hardcopy for resource planning meetings and documentation.

## What Happens Next

After reviewing the Employee Assignee Detail Forecast Report, you may:

- Adjust individual assignments to balance workloads across the team
- Run the Project Labor Forecast Report (PROJ-RPT-009) for a higher-level view of labor demand by project
- Use resource management tools to update assignments and level capacity
- Communicate with employees about their assignments and capacity expectations
- Plan hiring or contractor engagement to fill resource gaps

## Common Issues

**An employee shows zero Estimated or Remaining effort**

This typically occurs when an assignment has not been fully configured or when the assignment end date is in the past. Check the assignment details to verify the dates and effort values are correct. If the assignment is complete, remaining hours will naturally be zero.

**The date range shows assignments outside the selected period**

Some employees may have assignments that span your selected date range. For example, an assignment starting before your date range begin will still appear if it extends into your date range. To see only assignments entirely within your date range, adjust the date boundaries.

**An employee appears over-allocated but I know they have capacity**

Over-allocation calculations may not account for non-project work, administrative tasks, or time off. Verify whether your assignments include buffers or whether they represent pure project time only. Adjust allocations if needed to reflect realistic capacity.

**I don't see all employees in the results**

The report may be filtered by department or branch. Verify your filter selections to ensure all relevant employees are included. If you selected specific employees, confirm their names are in the list. Employees with no assignments during the date range may not appear in the output.

**Remaining effort shows negative hours**

Negative remaining effort indicates an assignment has consumed more hours than originally estimated. This signals an overrun on that task. The project manager should investigate and potentially add time to the assignment or the project budget.

**I need to know who is available for a new assignment**

Review employees with low or zero utilization during your date range. These are candidates for new assignments. Cross-reference with skill requirements to match available resources to project needs.
