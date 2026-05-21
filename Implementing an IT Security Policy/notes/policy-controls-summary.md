# Policy Controls Summary

## Password Protection Policy

### Controls Implemented

- Enforce password history
- Maximum password age
- Minimum password length
- Password complexity requirements

### Security Value

These settings reduce weak password use and make password reuse harder.

---

## Account Lockout Policy

### Controls Reviewed

- Account lockout duration
- Account lockout threshold
- Reset account lockout counter after a defined time

### Security Value

Account lockout policies reduce the effectiveness of brute-force and password guessing attacks.

---

## Antivirus Policy

### Controls Implemented

- Real-time protection enforced through Group Policy
- Local override disabled
- User-facing settings grayed out after policy application

### Security Value

Centrally managed antivirus protection helps ensure endpoint defenses remain enabled and consistent across the organization.

---

## Windows Security Baseline

### Controls Reviewed

- Microsoft recommended password settings
- Microsoft recommended account lockout settings
- Domain security baseline GPO
- Linked security baseline object

### Security Value

Security baselines provide recommended configuration sets that help harden systems and reduce manual configuration errors.

---

## Mobile Device Security Policy

### Controls Reviewed

- Google Play Protect scan
- System update check
- Lock screen
- Device encryption setup
- Find My Device settings

### Security Value

Mobile device controls help protect organizational data on BYOD or managed devices, especially when devices are lost, stolen, or exposed to malicious apps.

---

## Policy Implementation Workflow

```text
Define Policy Requirement
        │
        ▼
Map Requirement to Technical Control
        │
        ▼
Configure Control
        │
        ▼
Force / Wait for Policy Application
        │
        ▼
Test as User or Device
        │
        ▼
Document Evidence
```

## Portfolio Safety Notes

Do not publish:

- Real credentials
- Internal domain names
- Private IP addresses
- Student emails
- Platform watermarks
- Instructor-provided answer content
- Unredacted mobile device identifiers
