---
title: Manage Secure Access Records
id: SVC-SECACCESS-001
module: Service
screen: Site / Product > Access Info Tab
menu_path: Service > Service Call > Call Tab (lock icon)
applies_to: Service Managers, System Administrators, Technicians with ACCESSINFO permission
prerequisites:
  - ACCESSINFO permission enabled for user
  - Access to Site or Product record, or service call
  - ACCINFOCAT and ACCINFOSUB general codes configured
related_procedures:
  - SVC-ADMIN-001
tags:
  - Secure Access
  - Security
  - Sensitive Data
  - Credentials
version: 1.0
last_updated: 2026-03-25
---

# Manage Secure Access Records

## What This Procedure Does

This procedure manages secure access information such as network details, VPN credentials, and server information. Access Info records are restricted and audited. Users must have the ACCESSINFO permission to view sensitive data.

## Before You Begin

- User must have ACCESSINFO permission in their role
- Site or Product record must already exist
- Identify who needs access to this sensitive information
- Prepare the sensitive information (credentials, network details, etc.)

## Steps

### Step 1: Open Site or Product Access Info Tab

Open a Site or Product record. Click the Access Info tab to view existing secure access records. Alternatively, open a service call, click the Call tab, and click the lock icon next to the Site or Product field to access the Access Info interface.

### Step 2: Add Access Information

Click the Add icon (plus sign) to create a new access information record. Fill in the following information:

| Field | What to enter |
|-------|---------------|
| Category | Select the category using ACCINFOCAT general codes |
| Subcategory | Select the subcategory using ACCINFOSUB general codes |
| Information | Enter the sensitive data (VPN address, username, server name, network details, etc.) |

### Step 3: Configure Access Settings

Set the access permissions for this record. Use the following options:

| Field | What to enter |
|-------|---------------|
| Public Flag | Check if all users with ACCESSINFO permission should see this record |

If not using the Public Flag, configure granular access using the Permissions tab.

### Step 4: Configure Granular Permissions (if needed)

Click the Permissions tab to limit access to specific users or groups. Click Add and specify which users or user groups can view this access information record. This restricts the record to only those individuals.

### Step 5: Save the Record

Click Save (floppy disk icon). The access information is now stored and protected.

### Step 6: Review History

To audit changes to access information, click the History tab. The history shows the Date, User ID, Action (Created, Modified, Viewed), Field Name, and From/To values for all changes. This provides a complete audit trail.

## What Happens Next

The secure access information is stored in the system and restricted by permissions. Only users with ACCESSINFO permission and appropriate access rights can view the information. When technicians need the information during a service call, they can access it through the lock icon on the Call tab. All access is logged in the History tab for security auditing.

## Common Issues

**User Cannot View Access Information**
Verify the user has ACCESSINFO permission in their role. If using the Public Flag, check it is enabled. If using granular permissions, ensure the user is added to the Permissions tab. Check the History tab to confirm the record was created correctly.

**Need to Revoke Access for a User**
Open the Access Info record, click the Permissions tab, and delete the user or group from the access list. Save the record. The user will no longer see this information.

**Access Information Changed or Needs Update**
Open the Access Info record, click Edit icon (pencil), update the Information field with new credentials or details, and Save. All changes are tracked in the History tab with the user ID and timestamp.
