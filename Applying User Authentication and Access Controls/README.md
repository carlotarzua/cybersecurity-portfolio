# 🎯 User Authentication & Access Controls Lab

![Cybersecurity](https://img.shields.io/badge/Cybersecurity-0A66C2?style=for-the-badge&logo=securityscorecard&logoColor=white)
![Active Directory](https://img.shields.io/badge/Active%20Directory-0078D4?style=for-the-badge&logo=microsoft&logoColor=white)
![Windows Server](https://img.shields.io/badge/Windows%20Server-0078D6?style=for-the-badge&logo=windows&logoColor=white)
![PowerShell](https://img.shields.io/badge/PowerShell-5391FE?style=for-the-badge&logo=powershell&logoColor=white)
![TrueNAS](https://img.shields.io/badge/TrueNAS-0095D5?style=for-the-badge&logo=truenas&logoColor=white)

A hands-on cybersecurity lab focused on **user authentication, Active Directory security groups, NTFS permissions, SMB shares, and access control validation**.

This lab demonstrates identity and access management skills by creating users and groups, assigning role-based permissions, configuring protected folders, building TrueNAS datasets, and testing whether users can access only the resources required for their role.

---

## ✨ Features

- 👤 **Active Directory User Management** — Created and managed domain users in Active Directory
- 👥 **Security Group Configuration** — Built role-based security groups for Developers, Managers, and Human Resources
- ⚙️ **PowerShell Administration** — Used PowerShell cmdlets to create AD users/groups and update group membership
- 📁 **NTFS Permission Configuration** — Configured folder-level security permissions for HR, manager, and developer folders
- 🔐 **Least Privilege Validation** — Tested successful and denied access for multiple user roles
- 🗄️ **TrueNAS Dataset Configuration** — Created SMB datasets and shared folders for department-based access
- 🧪 **Access Control Testing** — Verified authentication and authorization by logging in as different users
- 📝 **Security Documentation** — Documented access control behavior, folder permissions, and role-based access outcomes

---

## 🚀 Demo

> The lab builds a role-based access control model and verifies that users can only access folders assigned to their security group.

```text
Create AD Users & Groups
        │
        ▼
 Assign Users to Security Groups
        │
        ▼
 Create Department Folders
        │
        ▼
 Configure NTFS / ACL Permissions
        │
        ▼
 Test Access as Each User
        │
        ▼
 Validate Least Privilege
```

> Note: Before publishing screenshots, remove or blur student names, email addresses, timestamps, platform watermarks, internal hostnames, private IPs, and any credentials.

---

## 🛠️ Tech Stack

| Component | Technology |
|---|---|
| **Directory Services** | Microsoft Active Directory Domain Services |
| **Identity Management** | Active Directory Users and Computers |
| **Automation / CLI** | Windows PowerShell |
| **File Permissions** | Windows NTFS Security Permissions |
| **Shared Storage** | TrueNAS |
| **File Sharing** | SMB Shares |
| **Operating Systems** | Windows Server, FreeBSD / TrueNAS |
| **Security Concepts** | Authentication, authorization, least privilege, RBAC, ACLs |

---

## 🧠 How It Works

```text
Identity Setup
        │
        ▼
  Active Directory  ───────────── Create users and security groups
        │
        ▼
  Group Membership  ───────────── Assign users to role-based groups
        │
        ▼
  Folder Structure  ───────────── Create HRfiles, MGRfiles, and DEVfiles
        │
        ▼
  Access Controls  ────────────── Apply NTFS permissions and ACLs
        │
        ▼
  TrueNAS Shares  ─────────────── Create SMB datasets and shared folders
        │
        ▼
  Validation  ─────────────────── Log in as each user and test access
        │
        ▼
  Findings  ───────────────────── Confirm least privilege and role-based access
```

1. **Created Active Directory security groups** for Developers, Managers, and Human Resources
2. **Created domain user accounts** using Active Directory Users and Computers and PowerShell
3. **Assigned users to groups** based on department and job role
4. **Created protected folders** for HR, manager, and developer files
5. **Configured NTFS permissions** so each folder was restricted to the correct security group
6. **Tested access control behavior** by logging in as each user and attempting to access each folder
7. **Configured TrueNAS datasets and SMB shares** for remote file server access
8. **Validated remote access controls** through the Employees shared folder
9. **Completed challenge tasks** by creating additional users, group memberships, datasets, and access tests

---

## 📂 Project Structure

```text
user-authentication-access-controls-lab/
├── README.md
└── notes/
    ├── key-takeaways.md
    ├── powershell-commands.md
    └── access-control-summary.md
```

---

## ⚙️ Lab Summary

### Objective

Use Active Directory and file system permissions to implement authentication and access controls, then verify that users can only access resources authorized by their group membership.

### Main Activities

| Area | What Was Practiced |
|---|---|
| **User Creation** | Created new domain user accounts |
| **Group Creation** | Created security groups for Developers, Managers, and Human Resources |
| **Group Membership** | Added users to role-based security groups |
| **PowerShell Administration** | Used AD cmdlets for group/user management |
| **Folder Permissions** | Configured NTFS permissions for HRfiles, MGRfiles, and DEVfiles |
| **Access Testing** | Verified successful and denied folder access |
| **SMB Sharing** | Created TrueNAS datasets and shared folders |
| **Remote File Access** | Tested Employees folder visibility for different users |
| **Challenge Work** | Created additional users, datasets, and group-based access controls |

---

## 🧪 PowerShell Commands Practiced

```powershell
New-ADGroup -Name HumanResources -GroupScope Global -GroupCategory Security
```

Created a new global security group in Active Directory.

```powershell
New-ADUser -Name lcasado `
  -UserPrincipalName lcasado@domain.example `
  -AccountPassword (ConvertTo-SecureString -AsPlainText "REDACTED" -Force) `
  -GivenName Laura `
  -Surname Casado `
  -Enabled $true
```

Created a new Active Directory user account.

```powershell
Add-ADGroupMember -Identity HumanResources -Members lcasado
```

Added a user account to an Active Directory security group.

```powershell
gpupdate /force
```

Forced a Group Policy update.

> Public portfolio note: replace real lab domains, usernames, and passwords with sanitized examples before publishing.

---

## 🔐 Security Concepts Demonstrated

- **Authentication** — Verifying a user’s identity before granting access
- **Authorization** — Deciding what an authenticated user is allowed to access
- **Role-Based Access Control** — Assigning permissions based on job role or department
- **Principle of Least Privilege** — Giving users only the access required for their work
- **Security Groups** — Managing access through group membership instead of individual user permissions
- **NTFS Permissions** — Applying file and folder permissions in Windows
- **ACLs** — Using access control lists to allow or deny access to protected resources
- **SMB Share Access** — Controlling access to shared network folders
- **Permission Validation** — Testing access from the perspective of different users

---

## 📸 Suggested Screenshots to Include Later

From the submitted lab report, the strongest portfolio screenshots would be:

| Screenshot | Why It Is Useful |
|---|---|
| **New users and groups in Active Directory** | Shows identity and group management |
| **HRfiles / MGRfiles / DEVfiles security permissions** | Shows NTFS permission configuration |
| **Three folders inside LabFiles** | Shows the protected folder structure |
| **Access denied errors for unauthorized users** | Demonstrates least privilege validation |
| **File properties created by authorized users** | Shows successful authorized access |
| **TrueNAS Employees dataset** | Shows storage/share administration |
| **Three new TrueNAS datasets** | Shows ACL-ready shared folder structure |
| **Employees folder as different users** | Shows user-specific access outcomes |
| **Member Of tab for challenge users** | Shows group membership validation |
| **GG Studios TrueNAS datasets** | Shows independent challenge/application work |

---

## 🧩 Key Takeaways

- Authentication confirms identity, but access control determines what a user can do after logging in.
- Active Directory makes it easier to centrally manage users, groups, and permissions.
- Security groups are more scalable than assigning permissions to individual users one by one.
- NTFS permissions protect files and folders at the Windows filesystem level.
- Inheritance must be understood carefully because parent folder permissions can flow down to child folders.
- The Principle of Least Privilege is validated by testing both successful access and denied access.
- PowerShell helps automate repetitive identity and access management tasks.
- TrueNAS and SMB shares can integrate with role-based access models for shared storage.
- Access control testing should be performed from the perspective of real users, not only administrators.

---

## 🌱 Future Improvements

- [ ] Add sanitized screenshots of AD users and groups
- [ ] Add a permission matrix showing each user and folder access result
- [ ] Add a short explanation of NTFS permissions vs. share permissions
- [ ] Add a TrueNAS ACL summary section
- [ ] Add a diagram showing user → group → folder access flow

---

## 👩‍💻 About Me

Built by **Carlota Arzúa** — a cybersecurity student and developer interested in identity and access management, infrastructure security, and applied defensive security.

- 💼 [LinkedIn](https://www.linkedin.com/in/carlota-a-53a75b206/)
- 🌐 [Portfolio]()
- 📧 carlotaarzua@gmail.com

---

## 📄 License

This repository is for educational and portfolio purposes.

Do not redistribute instructor-provided lab manuals, answer keys, screenshots with sensitive information, credentials, or copyrighted course material without permission.
