# Access Control Summary

## Lab Access Model

The lab implemented role-based access control using Active Directory security groups and folder permissions.

## Groups

| Group | Purpose |
|---|---|
| Developers | Access to developer files |
| Managers | Access to manager files |
| HumanResources | Access to HR files |

## Folders

| Folder | Intended Access |
|---|---|
| `HRfiles` | HumanResources group |
| `MGRfiles` | Managers group |
| `DEVfiles` | Developers group |

## User Access Examples

| User | Group Membership | Expected Access |
|---|---|---|
| scarpenter | Developers | DEVfiles only |
| lcasado | HumanResources | HRfiles only |
| cprince | Developers, Managers | DEVfiles and MGRfiles |

## What Was Tested

### Successful access

Users were expected to create files in folders that matched their group membership.

Examples:

- Developer user creates a file in `DEVfiles`
- HR user creates a file in `HRfiles`
- Manager/Developer user creates files in `MGRfiles` and `DEVfiles`

### Denied access

Users were expected to receive access denied messages when opening folders outside their assigned role.

Examples:

- Developer user denied from `HRfiles` and `MGRfiles`
- HR user denied from `MGRfiles` and `DEVfiles`
- Manager/Developer user denied from `HRfiles`

## TrueNAS / SMB Share Extension

The lab extended the access control model to TrueNAS datasets and SMB shares.

### What this demonstrated

- Shared storage also needs role-based permissions
- Fileserver access should match Active Directory group membership
- Users should only see or access the shared folders they are authorized to use

## Key Security Principles

### Principle of Least Privilege

Users should only have the access required to perform their work.

### Role-Based Access Control

Permissions are easier to manage when they are based on groups and roles instead of individual users.

### Separation of Duties

Different departments or job roles should have separate access boundaries.

### Permission Validation

Access controls should be tested using real user accounts to confirm both allowed and denied behavior.

## Public Portfolio Note

Do not publish screenshots or notes that reveal:

- Real student email addresses
- Lab credentials
- Internal hostnames
- Private IP addresses
- Platform watermarks
- Course answer-key content
