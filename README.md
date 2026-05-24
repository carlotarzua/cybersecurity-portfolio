# 🛡️ Cybersecurity Lab Portfolio

![Cybersecurity](https://img.shields.io/badge/Cybersecurity-0A66C2?style=for-the-badge&logo=securityscorecard&logoColor=white)
![Networking](https://img.shields.io/badge/Networking-00599C?style=for-the-badge&logo=cisco&logoColor=white)
![Windows Server](https://img.shields.io/badge/Windows%20Server-0078D6?style=for-the-badge&logo=windows&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![Kali Linux](https://img.shields.io/badge/Kali%20Linux-557C94?style=for-the-badge&logo=kalilinux&logoColor=white)
![Wireshark](https://img.shields.io/badge/Wireshark-1679A7?style=for-the-badge&logo=wireshark&logoColor=white)
![OWASP](https://img.shields.io/badge/OWASP-000000?style=for-the-badge&logo=owasp&logoColor=white)

A portfolio of hands-on cybersecurity labs focused on **infrastructure security, vulnerability assessment, packet analysis, identity and access management, cryptography, attack vector analysis, and security policy implementation**.

These labs were completed in controlled training environments and rewritten as professional, portfolio-safe project summaries. The goal of this repository is to document practical cybersecurity skills, tools used, key concepts learned, and defensive takeaways.

---

## 📌 Portfolio Focus

This repository demonstrates hands-on experience across several cybersecurity domains:

- 🏢 **Infrastructure Security** — endpoint hardening, network segmentation, firewall/NAT review, VPN routing, DNS, Active Directory, and Docker service validation
- 🔎 **Vulnerability Assessment** — host discovery, port scanning, service enumeration, Nessus/OpenVAS review, CVSS risk analysis, and remediation planning
- 🦈 **Network Traffic Analysis** — Wireshark packet capture, protocol filtering, cleartext vs. encrypted traffic comparison, and wireless traffic inspection
- 👤 **Identity & Access Management** — Active Directory users/groups, NTFS permissions, role-based access control, SMB shares, and least privilege testing
- 🔐 **Cryptography** — GPG/Kleopatra key pairs, public key exchange, digital signatures, OpenSSL, symmetric encryption, and hybrid cryptography
- 🧪 **Attack Vector Awareness** — XSS, SQL injection, malware behavior, DDoS concepts, social engineering risks, and defensive controls
- 📋 **Security Policy Implementation** — Group Policy, password policies, Microsoft Defender controls, security baselines, and mobile device security

---

## 🧭 Lab Index

| # | Lab | Focus Area | Key Tools |
|---:|---|---|---|
| 01 | [Seven Domains of IT Infrastructure](./seven-domains-it-infrastructure-lab/) | Infrastructure security and layered controls | Windows Security, pfSense, OpenVPN, Active Directory, Docker |
| 02 | [Vulnerability Assessment](./vulnerability-assessment-lab/) | Scanning, enumeration, risk review, remediation | Nmap, Zenmap, Nessus, OpenVAS, Kali Linux |
| 03 | [Packet Capture & Traffic Analysis](./packet-capture-traffic-analysis-lab/) | Packet analysis and protocol inspection | Wireshark, PuTTY, FileZilla, Mininet-WiFi |
| 04 | [User Authentication & Access Controls](./user-authentication-access-controls-lab/) | IAM, RBAC, NTFS permissions, SMB shares | Active Directory, PowerShell, TrueNAS |
| 05 | [Encryption for Confidentiality & Integrity](./encryption-confidentiality-integrity-lab/) | Cryptography, signing, encryption, hybrid crypto | Kleopatra, GPG, OpenSSL, Linux |
| 06 | [Common Attack Vectors](./common-attack-vectors-lab/) | Web attacks, malware concepts, DDoS, social engineering | OWASP Juice Shop, Firefox DevTools, Kali, Metasploit, SET |
| 07 | [IT Security Policy Implementation](./it-security-policy-lab/) | Security governance and technical enforcement | Group Policy, Microsoft Defender, Security Compliance Toolkit, Android |

---

## 🧰 Tools & Technologies

| Category | Tools / Technologies |
|---|---|
| **Operating Systems** | Windows Server, Ubuntu Linux, Debian Linux, Kali Linux, FreeBSD / pfSense, Android OS |
| **Networking** | `ping`, `ipconfig`, `arp`, `tracert`, `traceroute`, `nslookup`, OpenVPN |
| **Firewall / Routing** | pfSense, NAT rules, static routes, DMZ rules, firewall policies |
| **Directory Services** | Active Directory, Active Directory Users and Computers, Group Policy Management Console |
| **Vulnerability Assessment** | Nmap, Zenmap, Nessus Essentials, OpenVAS / Greenbone |
| **Packet Analysis** | Wireshark, display filters, ICMP, FTP, SFTP, SSH, HTTP, wireless frames |
| **Cryptography** | Kleopatra, GPG4Win, GPG, OpenSSL, RSA, AES-256-CBC |
| **Web Security** | OWASP Juice Shop, Firefox Web Developer Tools, JSON/API inspection |
| **Security Policy** | Microsoft Defender Antivirus, Microsoft Security Compliance Toolkit, Android security settings |
| **Storage / Access Control** | TrueNAS, SMB shares, NTFS permissions, ACLs |

---

## 🧠 Skills Demonstrated

### Infrastructure & Network Security

- Reviewed endpoint security settings and managed update policies
- Validated firewall, NAT, static route, and DMZ configurations
- Tested VPN routing behavior and remote access paths
- Inspected ARP tables, switch forwarding behavior, DNS records, and service status

### Vulnerability Management

- Performed host discovery and port scanning
- Enumerated services and operating system details
- Reviewed vulnerability scan output from Nessus and OpenVAS
- Prioritized findings by severity, impact, and remediation effort
- Recommended mitigations for exposed services, weak passwords, and vulnerable software

### Traffic Analysis

- Captured and inspected packets with Wireshark
- Used display filters to isolate protocol traffic
- Compared cleartext protocols such as FTP/Telnet with encrypted protocols such as SSH/SFTP
- Reviewed packet details, payload bytes, ports, and session behavior
- Explored wireless traffic, SSIDs, channels, and handshake-related data

### Identity & Access Management

- Created and managed Active Directory users and security groups
- Applied role-based access control through group membership
- Configured NTFS folder permissions and tested access outcomes
- Validated least privilege through successful and denied access tests
- Extended access control concepts to SMB shares and TrueNAS datasets

### Cryptography

- Generated public/private key pairs
- Exchanged and certified public keys
- Signed, encrypted, decrypted, and verified messages
- Used symmetric and asymmetric encryption workflows
- Practiced hybrid cryptography using OpenSSL

### Web & Attack Vector Awareness

- Observed DOM XSS, reflected XSS, and SQL injection behavior in a controlled vulnerable app
- Used browser developer tools to inspect requests, responses, and exposed data
- Reviewed malware behavior and reverse-shell concepts in a lab environment
- Observed DDoS availability impact and social engineering workflow risks
- Connected offensive techniques to defensive controls

### Security Governance

- Implemented password policy settings through Group Policy
- Enforced Microsoft Defender real-time protection controls
- Reviewed Microsoft security baseline recommendations
- Validated Android mobile security controls
- Researched Acceptable Use Policy and Privacy Policy best practices

---

## 📂 Suggested Repository Structure

```text
cybersecurity-lab-portfolio/
├── README.md
├── seven-domains-it-infrastructure-lab/
│   ├── README.md
│   └── notes/
├── vulnerability-assessment-lab/
│   ├── README.md
│   ├── assets/
│   ├── notes/
│   └── screenshots/
├── packet-capture-traffic-analysis-lab/
│   ├── README.md
│   └── notes/
├── user-authentication-access-controls-lab/
│   ├── README.md
│   └── notes/
├── encryption-confidentiality-integrity-lab/
│   ├── README.md
│   └── notes/
├── common-attack-vectors-lab/
│   ├── README.md
│   └── notes/
└── it-security-policy-lab/
    ├── README.md
    └── notes/
```

---

## 📚 Lab Summaries

### 01 — Seven Domains of IT Infrastructure

A foundational infrastructure security lab exploring how security controls apply across the user, workstation, LAN, LAN-to-WAN, WAN, remote access, and system/application domains.

**Highlights**

- Reviewed Windows Security, update policies, and endpoint protection
- Validated least privilege and restricted folder access
- Inspected ARP tables and switch forwarding behavior
- Reviewed pfSense NAT, firewall, static route, port forwarding, and DMZ rules
- Tested VPN routing, DNS, Active Directory groups, Docker status, and web service availability

**Key Concepts**

`Defense-in-Depth` `Network Segmentation` `Endpoint Hardening` `VPN Routing` `Firewall Rules` `Least Privilege`

---

### 02 — Vulnerability Assessment

A vulnerability management lab focused on discovering hosts, identifying open ports, enumerating services, reviewing scanner findings, and recommending remediation.

**Highlights**

- Used Nmap/Zenmap for host discovery, SYN scanning, OS detection, and service enumeration
- Reviewed Nessus internal vulnerability assessment results
- Reviewed OpenVAS external scan findings
- Documented risk using severity, CVSS, likelihood, impact, and remediation steps
- Recommended mitigations for weak credentials, vulnerable services, weak SSL/TLS encryption, and unnecessary exposed ports

**Key Concepts**

`Host Discovery` `Port Scanning` `Service Enumeration` `Vulnerability Management` `CVSS` `Remediation Planning`

---

### 03 — Packet Capture & Traffic Analysis

A network security analysis lab using Wireshark to capture traffic, inspect packet contents, filter protocols, and compare cleartext and encrypted communication.

**Highlights**

- Captured ICMP, Telnet, SSH, FTP, SFTP, HTTP, and wireless traffic
- Used Wireshark display filters to isolate protocol activity
- Compared cleartext protocols with encrypted protocols
- Reviewed packet details, payload bytes, ports, and session behavior
- Explored wireless traffic, SSIDs, channels, and handshake-related data

**Key Concepts**

`Packet Capture` `Protocol Analysis` `Wireshark Filters` `Cleartext Risk` `Encryption` `Wireless Security`

---

### 04 — User Authentication & Access Controls

An identity and access management lab focused on Active Directory users, security groups, NTFS permissions, SMB shares, and least privilege validation.

**Highlights**

- Created users and security groups in Active Directory
- Used PowerShell to create AD objects and manage group membership
- Configured folder-level NTFS permissions for HR, manager, and developer folders
- Tested allowed and denied access as different users
- Created TrueNAS datasets and SMB shares for role-based access control

**Key Concepts**

`Authentication` `Authorization` `RBAC` `NTFS Permissions` `ACLs` `SMB Shares` `Least Privilege`

---

### 05 — Encryption for Confidentiality & Integrity

A cryptography lab focused on protecting confidentiality and integrity using GPG/Kleopatra, OpenSSL, digital signatures, symmetric encryption, asymmetric encryption, and hybrid cryptography.

**Highlights**

- Generated public/private key pairs
- Exchanged and certified public keys
- Signed and encrypted files using public-key cryptography
- Decrypted files and verified digital signatures
- Used OpenSSL to generate RSA keys and encrypt files with AES-256-CBC
- Practiced hybrid cryptography by protecting a symmetric key with asymmetric encryption

**Key Concepts**

`Confidentiality` `Integrity` `Digital Signatures` `Public Key Cryptography` `Symmetric Encryption` `Hybrid Cryptography`

---

### 06 — Common Attack Vectors

A security awareness and defensive analysis lab exploring common attack vectors in a controlled environment, including injection attacks, malware concepts, DDoS, and social engineering.

**Highlights**

- Tested DOM XSS, reflected XSS, and SQL injection behavior in OWASP Juice Shop
- Used Firefox Developer Tools to inspect requests, responses, errors, and JSON data
- Observed malware behavior and system enumeration after compromise in a controlled lab
- Simulated availability disruption with recruited hosts and failed web connections
- Reviewed phishing-style social engineering workflow risks
- Documented defensive measures for injection, malware, DDoS, social engineering, and credential attacks

**Key Concepts**

`XSS` `SQL Injection` `Malware Behavior` `DDoS` `Social Engineering` `Secure Coding` `Defense-in-Depth`

---

### 07 — IT Security Policy Implementation

A governance and technical enforcement lab focused on converting security policies into enforceable controls using Group Policy, Microsoft Defender, Microsoft security baselines, and Android security settings.

**Highlights**

- Configured domain password policy settings
- Tested password reset enforcement
- Enforced Microsoft Defender real-time protection through Group Policy
- Verified endpoint security settings were centrally managed
- Reviewed and linked a Microsoft Windows Server security baseline
- Checked Android Play Protect, system updates, lock screen, encryption, and Find My Device settings
- Researched acceptable use and privacy policy statements

**Key Concepts**

`Security Policy` `Group Policy` `Password Policy` `Microsoft Defender` `Security Baselines` `Mobile Security` `Governance`

---

## 🧪 Commands & Filters Practiced

```bash
ipconfig /all
arp -a
ping <host-or-ip>
tracert <host-or-ip>
traceroute <host-or-ip>
nslookup <host-or-ip>
nmap -sS <target>
nmap -O <target>
nmap -sV <target>
```

```powershell
gpupdate /force
New-ADGroup -Name HumanResources -GroupScope Global -GroupCategory Security
Add-ADGroupMember -Identity HumanResources -Members <user>
```

```bash
openssl genrsa -aes256 -out private.key 8192
openssl rsa -in private.key -pubout -out public.key
openssl enc -aes-256-cbc -pbkdf2 -salt -a -e -in plaintext.txt -out ciphertext.txt
```

```text
Wireshark filters:
icmp
ftp
ssh
telnet
http
```

---

## 🔐 Security Concepts Covered

| Concept | Where Practiced |
|---|---|
| **Defense-in-Depth** | Infrastructure, endpoint security, firewall review, security policy |
| **Least Privilege** | Folder permissions, AD groups, TrueNAS shares |
| **Network Segmentation** | LAN, WAN, DMZ, firewall, NAT, VPN routing |
| **Vulnerability Management** | Nmap, Nessus, OpenVAS, remediation planning |
| **Packet Analysis** | Wireshark, protocol filters, cleartext/encrypted comparison |
| **Identity & Access Management** | AD users/groups, RBAC, ACLs, SMB shares |
| **Cryptography** | GPG, Kleopatra, OpenSSL, signatures, hybrid encryption |
| **Web Application Security** | XSS, SQL injection, OWASP Juice Shop |
| **Endpoint Protection** | Microsoft Defender, antivirus policy, mobile security |
| **Governance, Risk & Compliance** | IT security policy, AUP, privacy policy, baselines |

---

## 🧼 Portfolio Safety Notes

This repository is sanitized for portfolio use.

Do **not** commit:

- Raw instructor lab manuals
- Answer keys or full course-provided instructions
- Credentials, passwords, passphrases, private keys, or API keys
- Raw packet captures containing sensitive data
- Executable malware payloads or exploit artifacts
- Phishing templates or working social engineering pages
- Private IP addresses, internal hostnames, or platform-specific identifiers
- Screenshots containing student email, names, timestamps, watermarks, or lab system details

Use cropped/redacted screenshots that show the skill being demonstrated without exposing sensitive information.

---

## 🌱 Future Improvements

- [ ] Add sanitized screenshots for each lab
- [ ] Add a one-page skills matrix
- [ ] Add a glossary of cybersecurity terms practiced
- [ ] Add executive summaries for each lab
- [ ] Add remediation checklists for vulnerability and policy labs
- [ ] Add diagrams for network segmentation, IAM flow, and cryptography workflows
- [ ] Add links to related projects, scripts, or write-ups

---

## 👩‍💻 About Me

Built by **Carlota Arzúa** — a cybersecurity student and developer interested in infrastructure security, identity and access management, vulnerability management, network security, cryptography, and applied defensive security.

- 💼 [LinkedIn](https://www.linkedin.com/in/carlota-a-53a75b206/)
- 🌐 [Portfolio]()
- 📧 carlotaarzua@gmail.com

---

## 📄 License

This repository is for educational and portfolio purposes.

Do not redistribute instructor-provided lab manuals, answer keys, platform screenshots with sensitive information, exploit artifacts, credentials, private keys, or copyrighted course material without permission.
