# Key Takeaways

## Overview

This lab focused on authentication and access controls using Active Directory, Windows permissions, and TrueNAS shared storage. The main lesson was that secure access depends on both verifying user identity and enforcing the correct permissions after login.

## Main Takeaways

### 1. Authentication and authorization are different

Authentication verifies who the user is. Authorization determines what that user can access after authentication succeeds.

### 2. Active Directory centralizes identity management

Active Directory allows administrators to manage users, groups, computers, and permissions from a central location.

### 3. Security groups make permissions scalable

Instead of assigning permissions to each user individually, users can be placed into groups based on role or department. Permissions can then be assigned to the group.

### 4. Role-based access supports least privilege

The lab used role-based access by assigning users to groups such as Developers, Managers, and Human Resources. Each group was allowed to access only the folder needed for its role.

### 5. NTFS permissions protect local folders

Windows Security permissions control what users and groups can do with files and folders, such as read, write, modify, or full control.

### 6. Permission inheritance must be managed carefully

Parent folder permissions can automatically flow down to child folders. Disabling or converting inheritance may be necessary when folders need different permissions.

### 7. Access denied messages are useful evidence

Testing denied access is just as important as testing successful access. Denied access proves that the control is working for unauthorized users.

### 8. PowerShell improves administration

PowerShell cmdlets can create users, create groups, add group members, and force policy updates. This makes identity management faster and more repeatable.

### 9. TrueNAS adds shared storage access control practice

The lab extended access control concepts to SMB shares and TrueNAS datasets, showing that authorization must be enforced across different platforms.

## Reflection

This lab showed how identity, group membership, filesystem permissions, and shared storage access work together. It also reinforced the importance of testing access controls as real users instead of assuming permissions are correct.
