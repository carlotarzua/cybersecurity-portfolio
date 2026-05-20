# 🎯 Vulnerability Assessment Lab

![Cybersecurity](https://img.shields.io/badge/Cybersecurity-0A66C2?style=for-the-badge&logo=securityscorecard&logoColor=white)
![Nmap](https://img.shields.io/badge/Nmap-00457C?style=for-the-badge&logoColor=white)
![Nessus](https://img.shields.io/badge/Nessus-00A5B5?style=for-the-badge&logo=tenable&logoColor=white)
![OpenVAS](https://img.shields.io/badge/OpenVAS-4CAF50?style=for-the-badge&logoColor=white)
![Kali Linux](https://img.shields.io/badge/Kali%20Linux-557C94?style=for-the-badge&logo=kalilinux&logoColor=white)

A hands-on cybersecurity lab focused on performing a **vulnerability assessment** using Nmap/Zenmap, Nessus, and OpenVAS. The lab demonstrates how to discover hosts, enumerate ports and services, review vulnerability scanner results, assess risk, and recommend mitigations.

This project is written as a portfolio-safe summary of the work completed in a controlled lab environment.

---

## ✨ Features

- 🔎 **Host Discovery** — Identified live hosts in a target network using Nmap/Zenmap
- 🚪 **Port Scanning** — Used SYN scanning to identify open TCP ports on target systems
- 🧬 **OS Detection** — Used Nmap OS detection to infer target operating systems
- 🧾 **Service Enumeration** — Identified running services and service versions with Nmap service scans
- 🛡️ **Nessus Vulnerability Assessment** — Ran internal vulnerability scans and reviewed risk summaries
- 🟢 **OpenVAS / Greenbone Scanning** — Reviewed detailed external vulnerability scan results
- 🧪 **Penetration Test Reporting** — Summarized scope, findings, severity, risk, and remediation steps
- 🔐 **Mitigation Planning** — Recommended fixes for weak passwords, vulnerable services, insecure encryption, and exposed services

---

## 🚀 Demo

> The lab follows a vulnerability management workflow: discover assets, enumerate services, scan for vulnerabilities, analyze risk, and recommend remediation.

![Vulnerability Assessment Summary](assets/vulnerability-assessment-summary.png)

Selected sanitized screenshots are included in the `screenshots/` folder.

---

## 🛠️ Tech Stack

| Component | Technology |
|---|---|
| **Operating System** | Windows Server lab workstation, Kali Linux |
| **Port Scanner** | Nmap / Zenmap |
| **Vulnerability Scanner** | Nessus Essentials |
| **External Scanner** | OpenVAS / Greenbone Security Manager |
| **Network Tools** | `ping`, `traceroute`, Nmap OS detection, Nmap service scan |
| **Reporting** | Vulnerability summary, penetration test report, mitigation notes |

---

## 🧠 How It Works

```text
Target Network
      │
      ▼
Host Discovery  ──────────────── Identify live systems
      │
      ▼
Port Scanning  ───────────────── Find open TCP ports
      │
      ▼
Service Enumeration  ─────────── Identify services and versions
      │
      ▼
Vulnerability Scanning  ──────── Nessus / OpenVAS results
      │
      ▼
Risk Review  ─────────────────── Severity, CVSS, likelihood, impact
      │
      ▼
Mitigation Plan  ─────────────── Patch, reconfigure, restrict, monitor
      │
      ▼
Report  ──────────────────────── Findings, scope, evidence, remediation
```

1. **Scanned the internal network** using Zenmap/Nmap to identify hosts and exposed services
2. **Performed a SYN scan** to identify open ports while minimizing full TCP connection activity
3. **Used OS detection** to identify likely operating systems on target hosts
4. **Ran service detection** to collect service names and version information
5. **Used Nessus** to perform an internal vulnerability assessment and review host-level risk
6. **Used OpenVAS** to review detailed external scan findings from an auditor-style perspective
7. **Prepared findings** with severity, CVSS scores, risk descriptions, and remediation steps

---

## 📂 Project Structure

```text
vulnerability-assessment-lab/
├── README.md
├── assets/
│   └── vulnerability-assessment-summary.png
├── notes/
│   ├── commands-used.md
│   ├── key-findings.md
│   └── remediation-plan.md
└── screenshots/
    ├── zenmap-nmap/
    │   ├── 01-zenmap-syn-scan-ports-hosts.png
    │   ├── 02-zenmap-os-detection-host-details.png
    │   ├── 03-zenmap-service-scan-versions.png
    │   └── 08-domain-controller-targeted-port-scan.png
    ├── nessus/
    │   ├── 04-nessus-vulnerability-summary.png
    │   └── 09-domain-controller-nessus-summary.png
    ├── openvas/
    │   └── 07-openvas-detailed-scan-results.png
    └── penetration-test/
        ├── 05-kali-traceroute-results.png
        └── 06-nmap-os-detection-external-scan.png
```

---

## 📸 Screenshots Used

| Screenshot | Why It Is Useful |
|---|---|
| `01-zenmap-syn-scan-ports-hosts.png` | Shows open-port discovery during the SYN scan |
| `02-zenmap-os-detection-host-details.png` | Shows OS detection and host fingerprinting |
| `03-zenmap-service-scan-versions.png` | Shows service enumeration and version discovery |
| `04-nessus-vulnerability-summary.png` | Shows internal vulnerability scan results and severity distribution |
| `05-kali-traceroute-results.png` | Shows external network path testing from Kali |
| `06-nmap-os-detection-external-scan.png` | Shows auditor-style external Nmap OS detection |
| `07-openvas-detailed-scan-results.png` | Shows detailed OpenVAS findings and high-risk issues |
| `08-domain-controller-targeted-port-scan.png` | Shows targeted scanning against a domain controller |
| `09-domain-controller-nessus-summary.png` | Shows vulnerability summary for the domain controller |

---

## 🧪 Commands & Techniques Practiced

```bash
nmap -sS <target>
nmap -O <target>
nmap -sV <target>
traceroute <target>
```

Additional tools used:

```text
Zenmap
Nessus Essentials
OpenVAS / Greenbone Security Manager
Kali Linux terminal
Vulnerability report review
CVSS-based risk analysis
```

---

## 🔐 Security Concepts Demonstrated

- **Vulnerability Management Lifecycle** — Identify, assess, remediate, and validate
- **Scanning and Enumeration** — Discover systems, ports, services, and versions
- **Risk Prioritization** — Focus first on high and critical findings
- **CVSS-Based Assessment** — Use risk scores to communicate severity
- **Service Exposure Review** — Identify risky services and unnecessary open ports
- **Credential Hardening** — Recommend stronger passwords and reduced remote access
- **Patch Management** — Remove or update vulnerable software
- **Secure Configuration** — Disable weak encryption, restrict services, and enforce safer defaults

---

## 🧩 Key Findings

### SNMP GETBULK Reflection DDoS

The internal vulnerability assessment identified an SNMP `GETBULK` reflection DDoS issue on a file server. The finding had a **CVSS v2 score of 5.0**, rated Medium. Recommended mitigation included disabling SNMP if not required, restricting SNMP access to trusted management hosts, replacing default community strings, and monitoring SNMP traffic.

### Weak MySQL Password

The external scan identified a weak MySQL/MariaDB password issue. The recommended remediation was to enforce strong passwords, disable remote root login, and review database access controls.

### vsftpd Backdoor

The external OpenVAS results identified a vulnerable vsftpd service associated with **CVE-2011-2523**. Recommended remediation included removing or updating the vulnerable FTP service and closing unnecessary exposed ports.

### Weak SSL Encryption

The domain controller assessment identified weak SSL encryption related to **SWEET32 / CVE-2016-2183**. Recommended remediation included disabling weak ciphers and enforcing TLS 1.2 or higher.

---

## 🌱 Future Improvements

- [ ] Add a formal executive summary section
- [ ] Add a severity matrix for critical, high, medium, low, and informational findings
- [ ] Include a remediation tracking table
- [ ] Add a before/after validation scan workflow
- [ ] Create a one-page vulnerability management checklist
- [ ] Add more labs covering authenticated scanning and patch validation

---

## 👩‍💻 About Me

Built by **Carlota Arzúa** — a cybersecurity student and developer interested in vulnerability management, infrastructure security, networking, and defensive security.

- 💼 [LinkedIn](https://www.linkedin.com/in/carlota-a-53a75b206/)
- 🌐 [Portfolio]()
- 📧 carlotaarzua@gmail.com

---

## 📄 License

This repository is for educational and portfolio purposes.

Do not redistribute instructor-provided lab manuals, answer keys, platform screenshots with sensitive information, credentials, or copyrighted course material without permission.
