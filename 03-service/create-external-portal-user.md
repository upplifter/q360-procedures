---
title: Create External Portal User
id: SVC-PORTAL-001
module: Service
screen: User Maintenance
menu_path: Maintenance > User Maintenance
applies_to: System Administrators, Service Managers
prerequisites:
  - User must have access to User Maintenance
  - Customer record must exist in the system
related_procedures:
  - SVC-ADMIN-001
tags:
  - Portal
  - Users
  - Setup
version: 1.0
last_updated: 2026-03-25
---

# Create External Portal User

## What This Procedure Does

This procedure creates an external portal user account so customers can access the self-service customer portal. Portal users can view their service calls, contracts, and block balances online.

## Before You Begin

- Ensure the customer account is already created in the system
- Have the customer's email address
- Have permission to access User Maintenance

## Steps

### Step 1: Open User Maintenance

Go to Maintenance > User Maintenance. Review the list of existing users. Click the Add icon (plus sign) to create a new user.

### Step 2: Set User Type and Basic Information

On the new user form, fill in the following fields:

| Field | What to enter |
|-------|---------------|
| User Type | Select EXTERNAL or PORTAL |
| User ID | Enter a unique identifier for the portal user |
| Name | Enter the customer contact name |
| Email | Enter the customer's email address |
| Password | Enter a secure initial password |
| Customer Link | Link to the customer account this user represents |

### Step 3: Assign Portal Permissions

Configure the user's portal access permissions. Select the modules and reports the user should access through the portal. Portal users typically have read-only access to view calls, contracts, and block balances.

### Step 4: Save the User

Click Save (floppy disk icon). The system creates the user account and sends a welcome notification to the email address provided.

## What Happens Next

The customer can now log into the external portal using their User ID and password. They can view their service calls, active contracts, and remaining block balance amounts. The portal provides a self-service view without requiring internal system access.

## Common Issues

**Customer Cannot Log In**
Verify the User ID and password were entered correctly during creation. Reset the password if needed by opening the user record and updating the password field. Ensure the Customer Link field is populated correctly.

**User Sees No Calls or Contracts**
Confirm the service calls and contracts are linked to the correct customer account. Check that the user's portal permissions include access to the relevant modules and reports.

**Email Notification Not Received**
Review the email address entered in the User record for typos. Check spam folders. Consider resending the welcome message from the user maintenance form if available.
