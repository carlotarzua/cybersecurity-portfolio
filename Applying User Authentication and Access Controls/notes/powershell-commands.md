# PowerShell Commands

This file summarizes the PowerShell commands practiced in the lab. Sensitive values are sanitized for portfolio use.

## Create an Active Directory Security Group

```powershell
New-ADGroup -Name HumanResources -GroupScope Global -GroupCategory Security
```

### Purpose

Creates a new Active Directory security group.

### Key parameters

| Parameter | Meaning |
|---|---|
| `-Name` | Name of the group |
| `-GroupScope` | Scope of the group, such as Global |
| `-GroupCategory` | Type of group, such as Security |

---

## Create an Active Directory User

```powershell
New-ADUser -Name lcasado `
  -UserPrincipalName lcasado@domain.example `
  -AccountPassword (ConvertTo-SecureString -AsPlainText "REDACTED" -Force) `
  -GivenName Laura `
  -Surname Casado `
  -Enabled $true
```

### Purpose

Creates a new Active Directory user account and enables it.

### Key parameters

| Parameter | Meaning |
|---|---|
| `-Name` | AD object name |
| `-UserPrincipalName` | User logon name |
| `-AccountPassword` | Password assigned to the account |
| `-GivenName` | User first name |
| `-Surname` | User last name |
| `-Enabled` | Enables the account when set to `$true` |

### Portfolio note

Do not publish real passwords. Replace them with `REDACTED` or use example values.

---

## Add a User to a Group

```powershell
Add-ADGroupMember -Identity HumanResources -Members lcasado
```

### Purpose

Adds a user to an Active Directory security group.

### Key parameters

| Parameter | Meaning |
|---|---|
| `-Identity` | Target group |
| `-Members` | User or users to add |

---

## Force a Group Policy Update

```powershell
gpupdate /force
```

### Purpose

Forces the system to immediately refresh Group Policy settings.

---

## Skills Demonstrated

- Creating AD security groups
- Creating AD users
- Assigning users to groups
- Using PowerShell for identity administration
- Applying repeatable administrative commands
- Sanitizing sensitive information before public documentation
