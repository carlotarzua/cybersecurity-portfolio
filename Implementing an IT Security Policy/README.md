# 🎯 IT Security Policy Implementation Lab

![Cybersecurity](https://img.shields.io/badge/Cybersecurity-0A66C2?style=for-the-badge&logo=securityscorecard&logoColor=white)
![Group Policy](https://img.shields.io/badge/Group%20Policy-0078D4?style=for-the-badge&logo=microsoft&logoColor=white)
![Windows Server](https://img.shields.io/badge/Windows%20Server-0078D6?style=for-the-badge&logo=windows&logoColor=white)
![Microsoft Defender](https://img.shields.io/badge/Microsoft%20Defender-00A4EF?style=for-the-badge&logo=microsoft&logoColor=white)
![Android Security](https://img.shields.io/badge/Android%20Security-3DDC84?style=for-the-badge&logo=android&logoColor=white)

A hands-on cybersecurity lab focused on **implementing IT security policies using Active Directory Group Policy, Windows Defender Antivirus controls, Microsoft security baselines, and mobile device security settings**.

This lab demonstrates how organizations translate security policies into enforceable technical controls, including password requirements, account lockout settings, centrally managed antivirus protection, Windows security baselines, mobile device updates, lock screens, device encryption, and Find My Device configuration.

---

## ✨ Features

- 🔐 **Password Policy Enforcement** — Configured domain password history, maximum age, minimum length, and complexity requirements
- 👤 **User Password Validation** — Tested password policy enforcement by resetting a domain user password
- 🛡️ **Centralized Antivirus Policy** — Used Group Policy to enforce Microsoft Defender real-time protection settings
- 🚫 **Local Override Prevention** — Verified that endpoint security settings were grayed out and centrally managed
- 📋 **Windows Security Baseline Review** — Reviewed Microsoft-recommended password and account lockout policy settings
- 🧱 **GPO Baseline Deployment** — Linked a Microsoft domain security baseline object to the domain
- 📱 **Mobile Device Security** — Reviewed Android Play Protect, system updates, lock screen, encryption, and Find My Device
- 📄 **Policy Research** — Researched acceptable use policy and privacy policy best practices

---

## 🚀 Demo

> The lab shows how written security policy requirements can be converted into technical controls and enforced across domain-joined systems and mobile devices.

```text
Security Policy Requirements
        │
        ▼
 Group Policy Configuration
        │
        ▼
 Password + Antivirus Enforcement
        │
        ▼
 Security Baseline Application
        │
        ▼
 Mobile Device Controls
        │
        ▼
 Policy Validation & Documentation
```

> Note: Before publishing screenshots, remove or blur names, email addresses, timestamps, platform watermarks, internal domain names, private IP addresses, and any lab-specific credentials.

---

## 🛠️ Tech Stack

| Component | Technology |
|---|---|
| **Directory / Policy Management** | Active Directory, Group Policy Management Console |
| **User Management** | Active Directory Users and Computers |
| **Endpoint Protection** | Microsoft Defender Antivirus / Windows Security |
| **Security Baselines** | Microsoft Security Compliance Toolkit |
| **Command Line** | Windows PowerShell |
| **Mobile Security** | Android Play Protect, Android system updates, lock screen, device encryption, Find My Device |
| **Operating Systems** | Windows Server, Android OS, FreeBSD / pfSense, Debian Linux |

---

## 🧠 How It Works

```text
Policy Goal
        │
        ▼
  Domain Password Policy  ────── History, age, length, complexity
        │
        ▼
  User Validation  ───────────── Reset password and test policy enforcement
        │
        ▼
  Defender Policy  ───────────── Enforce real-time protection through GPO
        │
        ▼
  Baseline Policy  ───────────── Apply Microsoft security baseline recommendations
        │
        ▼
  Mobile Controls  ───────────── Play Protect, updates, lock screen, encryption, location
        │
        ▼
  Documentation  ─────────────── AUP and privacy policy research
```

1. **Configured password policy settings** in the Default Domain Policy
2. **Forced Group Policy updates** to apply domain policy changes
3. **Tested password enforcement** by attempting both non-compliant and compliant password resets
4. **Logged in as a domain user** to validate successful policy application
5. **Configured Microsoft Defender real-time protection settings** through Group Policy
6. **Verified endpoint settings were centrally managed** by checking grayed-out real-time protection controls
7. **Reviewed Microsoft security baseline recommendations** for password and account lockout policies
8. **Linked a security baseline GPO** to the domain
9. **Reviewed mobile device security controls** including Play Protect, system updates, lock screen, encryption, and Find My Device
10. **Researched acceptable use and privacy policy statements** and documented their significance

---

## 📂 Project Structure

```text
it-security-policy-lab/
├── README.md
└── notes/
    ├── key-takeaways.md
    ├── policy-controls-summary.md
    └── acceptable-use-and-privacy-notes.md
```

---

## ⚙️ Lab Summary

### Objective

Implement and validate IT security policies using centrally managed technical controls, Windows security baselines, and mobile device security settings.

### Main Activities

| Area | What Was Practiced |
|---|---|
| **Password Protection Policy** | Configured password history, maximum age, minimum length, and complexity settings |
| **Policy Validation** | Tested failed and successful password changes |
| **Antivirus Policy** | Enforced Microsoft Defender real-time protection through Group Policy |
| **Central Management** | Verified that users could not override managed security settings |
| **Security Baseline** | Reviewed and linked a Microsoft Windows Server 2019 domain security baseline |
| **Account Lockout Review** | Reviewed recommended lockout threshold, duration, and reset settings |
| **Mobile Device Security** | Checked Play Protect, updates, lock screen, encryption setup, and Find My Device |
| **Policy Research** | Identified common acceptable use and privacy policy statements |

---

## 🧪 Tools & Controls Practiced

### Group Policy Management

```text
Computer Configuration
└── Policies
    └── Windows Settings
        └── Security Settings
            └── Account Policies
                └── Password Policy
```

Used to configure domain password policy settings.

### Microsoft Defender Antivirus Policy

```text
Computer Configuration
└── Policies
    └── Administrative Templates
        └── Windows Components
            └── Microsoft Defender Antivirus
                └── Real-time Protection
```

Used to centrally enforce endpoint protection settings.

### PowerShell

```powershell
gpupdate /force
```

Used to force Group Policy updates after configuration changes.

---

## 🔐 Security Concepts Demonstrated

- **Security Policy Implementation** — Translating written policy into technical controls
- **Group Policy Objects** — Centrally managing domain-wide security settings
- **Password Policy** — Enforcing password length, complexity, age, and history requirements
- **Account Lockout Policy** — Reducing brute-force password attack risk
- **Endpoint Protection** — Ensuring antivirus and real-time protection remain enabled
- **Security Baselines** — Applying recommended secure configuration sets
- **Mobile Device Security** — Protecting BYOD/mobile devices through scans, updates, locks, encryption, and location controls
- **Acceptable Use Policy** — Defining allowed and prohibited use of organizational technology
- **Privacy Policy** — Explaining how user data is collected, used, stored, shared, and protected
- **Centralized Administration** — Reducing reliance on individual users to maintain security settings

---

## 📸 Suggested Screenshots to Include Later

From the submitted lab report, the strongest portfolio screenshots would be:

| Screenshot | Why It Is Useful |
|---|---|
| **Newly configured Domain Password Policy settings** | Shows domain-level password policy enforcement |
| **Successful password change message** | Shows policy validation through user password reset |
| **Logged on user account** | Shows successful authentication after policy application |
| **Domain Real-time protection Policy settings** | Shows centralized antivirus configuration |
| **Grayed-out real-time threat protection settings** | Shows users cannot override managed security controls |
| **Microsoft recommended Password and Account Lockout settings** | Shows security baseline review |
| **Linked MSDomainSecurity2019 object** | Shows baseline GPO deployment |
| **Password and Account Lockout policy settings** | Shows applied baseline verification |
| **Google Play Protect scan results** | Shows mobile malware protection review |
| **Android system update timestamp** | Shows patch/update validation |
| **Android lock screen** | Shows mobile access control |
| **Encryption setup explanation** | Shows mobile data-at-rest protection |
| **Find My Device settings** | Shows mobile device recovery/loss controls |

---

## 🧩 Key Takeaways

- Security policies are only effective when they are implemented through enforceable controls.
- Group Policy allows administrators to manage password and endpoint protection settings centrally.
- Password policies should include more than complexity; length, history, expiration, and lockout behavior also matter.
- Centralized antivirus policy helps prevent users from disabling key protections.
- Security baselines reduce manual configuration effort and help align systems with recommended settings.
- Mobile security policies should include malware scanning, updates, lock screens, encryption, and device location/recovery controls.
- Acceptable use policies define how users may use organizational systems.
- Privacy policies define how organizations collect, use, protect, and share personal information.
- Documentation and validation are essential parts of policy implementation.

---

## 🌱 Future Improvements

- [ ] Add sanitized screenshots of Group Policy settings
- [ ] Add a policy-to-control mapping table
- [ ] Add a password policy vs. account lockout policy comparison
- [ ] Add a mobile device security checklist
- [ ] Add a short reflection on balancing usability and security

---

## 👩‍💻 About Me

Built by **Carlota Arzúa** — a cybersecurity student and developer interested in governance, risk, compliance, endpoint security, identity management, and applied defensive security.

- 💼 [LinkedIn](https://www.linkedin.com/in/carlota-a-53a75b206/)
- 🌐 [Portfolio]()
- 📧 carlotaarzua@gmail.com

---

## 📄 License

This repository is for educational and portfolio purposes.

Do not redistribute instructor-provided lab manuals, answer keys, screenshots with sensitive information, credentials, internal domain details, or copyrighted course material without permission.
