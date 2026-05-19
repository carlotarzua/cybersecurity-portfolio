# 🎯 Seven Domains of IT Infrastructure Lab

![Cybersecurity](https://img.shields.io/badge/Cybersecurity-0A66C2?style=for-the-badge&logo=securityscorecard&logoColor=white)
![Networking](https://img.shields.io/badge/Networking-00599C?style=for-the-badge&logo=cisco&logoColor=white)
![Windows Server](https://img.shields.io/badge/Windows%20Server-0078D6?style=for-the-badge&logo=windows&logoColor=white)
![pfSense](https://img.shields.io/badge/pfSense-212121?style=for-the-badge&logo=pfsense&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)

A hands-on cybersecurity lab focused on exploring the **seven domains of a typical IT infrastructure** and identifying security controls across workstations, LAN devices, perimeter firewalls, WAN routing, remote access, and system/application services.

This lab demonstrates foundational blue-team and infrastructure security skills, including endpoint hardening, least privilege, ARP analysis, firewall rule review, NAT configuration, VPN routing validation, DNS lookups, Active Directory inspection, and service verification.

---

## ✨ Features

- 🖥️ **Workstation Security Review** — Verified Windows sign-in controls, update policies, antivirus settings, and execution restrictions
- 🔐 **Least Privilege Validation** — Confirmed standard user limitations and restricted access to unauthorized folders
- 🌐 **LAN Analysis** — Inspected ARP tables, switch forwarding behavior, and local network connectivity
- 🔥 **Firewall & NAT Review** — Reviewed pfSense outbound NAT, port forwarding, static routes, LAN rules, and DMZ firewall rules
- 🛜 **WAN & Remote Access Testing** — Validated routing paths, VPN behavior, traceroute results, and remote service access
- 🧩 **System/Application Domain Review** — Checked Active Directory group membership, password policy, DNS entries, Docker service status, and web application availability
- 📝 **Security Documentation** — Captured evidence, documented findings, and summarized security takeaways

---

## 🚀 Demo

> The lab walks through a simulated enterprise environment and validates how security controls are applied across multiple infrastructure domains.

![Lab Demo](assets/demo-screenshot.png)

> Note: Screenshots in this repository should be sanitized before publishing. Do not include student email addresses, platform watermarks, credentials, private IP details, or instructor-provided lab content.

---

## 🛠️ Tech Stack

| Component | Technology |
|---|---|
| **Operating Systems** | Windows Server, Debian Linux, Ubuntu Linux, FreeBSD, Kali Linux |
| **Endpoint Security** | Windows Security, Microsoft Defender, Group Policy-managed settings |
| **Networking Tools** | `ipconfig`, `arp`, `ping`, `tracert`, `traceroute`, `nslookup` |
| **Remote Access** | OpenVPN |
| **Firewall / Router** | pfSense |
| **Remote Shell** | PuTTY |
| **Directory Services** | Active Directory, Group Policy Management |
| **Web Application** | OWASP Juice Shop |
| **Containers / Services** | Docker |
| **Documentation** | Lab report, screenshots, technical notes |

---

## 🧠 How It Works

```text
Enterprise Lab Environment
        │
        ▼
  Workstation Domain  ─────────── Endpoint controls, updates, antivirus, least privilege
        │
        ▼
  LAN Domain  ─────────────────── ARP tables, switch forwarding, file server access
        │
        ▼
  LAN-to-WAN Domain  ──────────── pfSense firewall rules, NAT, static routes, DMZ rules
        │
        ▼
  WAN Domain  ─────────────────── Point-to-point routing, BGP neighbor testing, traceroute
        │
        ▼
  Remote Access Domain  ───────── VPN routing, email server access, reverse DNS lookup
        │
        ▼
  System/Application Domain  ──── AD groups, password policy, DNS, Docker, web services
        │
        ▼
  Security Findings  ──────────── Documented controls, screenshots, and key takeaways
```

1. **Reviewed workstation security controls** by checking sign-in options, update policies, antivirus protections, and blocked executable behavior
2. **Validated least privilege** by confirming user access was limited to authorized personal and department folders
3. **Inspected LAN communication** using ARP tables, ping tests, switch forwarding tables, and file server directory access
4. **Reviewed perimeter security** by examining pfSense NAT settings, LAN rules, static routes, port forwarding, and DMZ firewall rules
5. **Tested WAN and remote access behavior** using ping, traceroute, VPN routing checks, email server connectivity, and reverse DNS lookup
6. **Explored system/application services** by checking Active Directory group membership, password policy settings, DNS entries, Docker status, and OWASP Juice Shop availability
7. **Documented findings** with sanitized screenshots and security-focused explanations

---

## 📂 Project Structure

```text
seven-domains-it-infrastructure-lab/
├── README.md
├── sanitized-report.pdf              # Optional: sanitized version of submitted lab report
├── notes/
│   ├── key-takeaways.md
│   ├── commands-used.md
│   └── security-controls-by-domain.md
├── assets/
│   ├── demo-screenshot.png           # Sanitized screenshot or summary graphic
│   └── network-diagram-redacted.png  # Redacted/simplified diagram, if allowed
└── screenshots/
    ├── workstation-security/
    ├── lan-analysis/
    ├── firewall-nat/
    ├── remote-access/
    └── system-application/
```

---

## ⚙️ Lab Summary

### Objective

Explore the seven domains of a typical IT infrastructure and identify how security controls protect users, workstations, networks, remote access paths, and critical systems.

### Domains Covered

| Domain | What Was Reviewed |
|---|---|
| **User Domain** | Phishing-related email warnings, blocked attachments, user access limitations |
| **Workstation Domain** | Sign-in options, Windows Update policies, antivirus settings, executable restrictions |
| **LAN Domain** | ARP tables, switch forwarding table, file server connectivity |
| **LAN-to-WAN Domain** | pfSense NAT, firewall rules, static routes, port forwarding, DMZ rules |
| **WAN Domain** | Point-to-point routes, routing tests, traceroute results |
| **Remote Access Domain** | VPN routing behavior, email server access, reverse DNS lookup |
| **System/Application Domain** | Active Directory groups, password policy, DNS records, Docker, web services |

---

## 🧪 Commands & Tools Practiced

```bash
ipconfig /all
arp -a
ping
tracert
traceroute
nslookup
whoami
```

Additional tools and platforms used:

```text
Windows Security
PuTTY
pfSense
OpenVPN
Active Directory
Group Policy Management Console
Docker
OWASP Juice Shop
```

---

## 🔐 Security Concepts Demonstrated

- **Defense-in-Depth** — Multiple security controls across different layers of the infrastructure
- **Principle of Least Privilege** — Users only receive the access required for their role
- **Endpoint Hardening** — Updates, antivirus, and controlled security settings reduce workstation risk
- **Network Segmentation** — LAN, DMZ, WAN, and remote access areas are separated by routing and firewall controls
- **Firewall Rule Review** — Rules define which traffic is allowed between network zones
- **VPN Routing Validation** — Traceroute results help determine whether VPN traffic is split tunnel or full tunnel
- **Access Control Testing** — Shared folder permissions confirm whether users can only access authorized resources
- **Monitoring & Verification** — CLI tools help validate configuration, connectivity, and service availability

---

## 📸 Evidence Collected

The lab report included screenshots showing:

- Sign-in options and managed account settings
- Windows Update policies
- Virus & threat protection settings
- Blocked executable behavior
- Blocked email attachment message
- Successful and failed folder access attempts
- Original and updated ARP tables
- Switch forwarding table
- pfSense outbound NAT settings
- LAN firewall rules
- Static route configuration
- Port forwarding rules
- DMZ firewall rules
- VPN and traceroute results
- Reverse DNS lookup
- Active Directory group membership
- Password policy settings
- DNS entries
- Docker service status
- OWASP Juice Shop web page
- Storage volume information

---

## 🧩 Key Takeaways

- Workstation security controls reduce the risk created by phishing, malware, and user mistakes.
- Managed update policies help ensure systems receive security patches consistently.
- Antivirus and tamper protection settings are more effective when users cannot disable them.
- Least privilege limits the damage an attacker can cause after compromising a user account.
- ARP tables and switch forwarding tables are useful for understanding local network communication.
- Firewall, NAT, static route, and DMZ configurations are essential for controlling traffic between network zones.
- VPN traceroute results help determine how remote user traffic is routed and protected.
- Active Directory, DNS, Docker, and web service checks are important parts of system/application security validation.

---

## 🌱 Future Improvements

- [ ] Replace all raw screenshots with redacted, portfolio-safe versions
- [ ] Add a simplified custom network diagram
- [ ] Create a one-page summary of security controls by domain
- [ ] Add a `commands-used.md` reference sheet
- [ ] Include a short reflection for each lab section
- [ ] Add links to related labs as the cybersecurity course progresses

---

## 👩‍💻 About Me

Built by **Carlota Arzúa** — a cybersecurity student and developer interested in infrastructure security, networking, cloud security, and applied defensive security.

- 💼 [LinkedIn](https://www.linkedin.com/in/carlota-a-53a75b206/)
- 🌐 [Portfolio]()
- 📧 carlotaarzua@gmail.com

---

## 📄 License

This repository is for educational and portfolio purposes.

Do not redistribute instructor-provided lab manuals, answer keys, platform screenshots with sensitive information, or any copyrighted course material without permission.
