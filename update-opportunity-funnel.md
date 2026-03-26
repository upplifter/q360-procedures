---
title: Update Opportunity Funnel Position
id: SALES-OPP-003
module: Sales
screen: Opportunity Form
menu_path: Main Menu > Sales > Opportunities
applies_to:
  - Sales Rep
  - Sales Manager
prerequisites:
  - OPPORTUNITY (Edit) permission assigned to your user or group
  - An opportunity record exists with a funnel definition assigned (see SALES-OPP-001)
related_procedures:
  - SALES-OPP-001
  - SALES-OPP-002
  - SALES-RPT-002
  - SALES-RPT-003
tags: funnel, funnel steps, funnel position, mark complete, sales process, pipeline stage, opportunity funnel, advance opportunity
version: 1.0
last_updated: 2026-03-25
---

# Update Opportunity Funnel Position

## What This Procedure Does

Marks one or more funnel steps as complete on a sales opportunity. Completing funnel steps advances the opportunity through the defined sales process phases (e.g., Qualify, Discovery, Proposal) and can automatically update the opportunity probability. Funnel position feeds into the Funnel Forecast and View Funnel reports.

## Before You Begin

- You have OPPORTUNITY (Edit) permission.
- The opportunity exists and has a funnel definition assigned.
- You know which funnel steps have been completed.

## Steps

### Step 1: Look Up the Opportunity

Navigate to **Main Menu > Sales > Opportunities**. Type part of the opportunity title or number in the **Form Quick Search** field and press **Enter**. Select the correct opportunity.

### Step 2: Locate the Funnel Grid

On the Opportunity form, locate the funnel steps grid. This grid lists the steps defined in the opportunity's funnel definition, showing their current completion status.

### Step 3: Mark Steps as Complete

Ensure you are **not** in edit mode. Select the step or steps that have been completed. Click the funnel grid **Extended Menu** (three vertical dots) and select **Mark as Complete**.

Q360 updates the selected steps to show a completed status and recalculates the opportunity's funnel phase position.

### Step 4: Verify the Updated Probability

If the funnel definition assigns probability values to each phase, check the opportunity's Probability field. It updates automatically based on the highest completed phase. If you need to override this value, click **Edit Record** (pencil icon), update the Probability manually, and click **Save Record** (floppy disk icon).

## What Happens Next

The opportunity's funnel position moves forward to reflect the newly completed steps. This affects:

- The **Funnel Forecast** quick view, which groups opportunities by their current funnel phase and shows the total value per phase (see SALES-RPT-002).
- The **View Funnel** quick view, which displays a visual funnel chart of active opportunities across phases (see SALES-RPT-003).
- The opportunity's Probability field, if the funnel definition has probability values configured per phase.
- The **Sales Score Card** report, which includes a Funnel Score metric based on completed funnel steps (see SALES-RPT-010).

Continue marking steps as complete as the deal progresses through each phase of the sales process.

## Common Issues

**The Mark as Complete option is not available in the extended menu.**
Ensure you are not in edit mode. The Mark as Complete command is only available when the form is in view mode.

**Completing a funnel step does not change the probability.**
The funnel definition may not have probability values assigned to each phase. In this case, update the probability manually on the opportunity (see SALES-OPP-002).

**The funnel grid shows no steps.**
The opportunity may not have a funnel definition assigned. Click Edit Record and select a Funnel Definition from the dropdown, then save. Steps populate based on the selected definition.

**You want to undo a completed funnel step.**
Funnel step completion is typically not reversible from the grid. Contact your administrator if you need to revert a step to incomplete status.

**Funnel steps appear out of order.**
The funnel step sequence is determined by the funnel definition configuration. If the order seems incorrect, contact your administrator to review the funnel definition setup in the system configuration.
