# 🎯 Common Attack Vectors Lab

![Cybersecurity](https://img.shields.io/badge/Cybersecurity-0A66C2?style=for-the-badge&logo=securityscorecard&logoColor=white)
![OWASP](https://img.shields.io/badge/OWASP-000000?style=for-the-badge&logo=owasp&logoColor=white)
![Kali Linux](https://img.shields.io/badge/Kali%20Linux-557C94?style=for-the-badge&logo=kalilinux&logoColor=white)
![Metasploit](https://img.shields.io/badge/Metasploit-2596CD?style=for-the-badge&logo=metasploit&logoColor=white)
![Web Security](https://img.shields.io/badge/Web%20Security-FF6F00?style=for-the-badge&logo=firefoxbrowser&logoColor=white)

A hands-on cybersecurity lab focused on **common attack vectors, vulnerable web applications, malware behavior, denial-of-service concepts, and social engineering awareness**.

This lab demonstrates how attackers abuse weak input validation, insecure application logic, user trust, and availability limits. It also connects each attack vector to defensive controls such as input validation, prepared statements, output encoding, endpoint protection, backups, rate limiting, filtering, security awareness, and phishing-resistant authentication.

---

## ✨ Features

- 🧪 **Injection Attack Review** — Explored DOM XSS, reflected XSS, and SQL injection behavior in a vulnerable web application
- 🛒 **OWASP Juice Shop Testing** — Used a deliberately vulnerable training app to observe web application security issues
- 🔎 **Browser Developer Tools** — Inspected HTTP requests, responses, JSON output, and error behavior
- 🧬 **Malware Behavior Demonstration** — Observed how reverse-shell style behavior can establish unauthorized access in a controlled lab
- 🖥️ **Post-Compromise Enumeration** — Reviewed system information after a simulated compromise
- 🌊 **DDoS Availability Impact** — Observed how recruited hosts can overwhelm a web service and trigger connection failures
- 🎣 **Social Engineering Awareness** — Reviewed phishing-style workflow concepts in a lab environment
- 🛡️ **Defensive Measures** — Documented mitigations for injection, malware, denial-of-service, social engineering, and credential attacks

---

## 🚀 Demo

> The lab follows a controlled attacker-perspective workflow to understand how common attack vectors work and how defenders can reduce risk.

```text
Recon / Input Testing
        │
        ▼
 Web Injection Testing
        │
        ▼
 Malware Behavior Observation
        │
        ▼
 Availability Attack Simulation
        │
        ▼
 Social Engineering Scenario
        │
        ▼
 Defensive Measures & Lessons Learned
```

> Note: This repository is for defensive education and portfolio documentation only. Do not publish executable payloads, exploit commands, phishing templates, target details, credentials, or screenshots containing sensitive lab identifiers.

---

## 🛠️ Tech Stack

| Component | Technology |
|---|---|
| **Vulnerable Web App** | OWASP Juice Shop |
| **Browser Analysis** | Firefox Web Developer Tools |
| **Security Testing Platform** | Kali Linux |
| **Exploit Framework Exposure** | Metasploit Framework |
| **Payload Generation Exposure** | msfvenom |
| **DDoS / Botnet Simulation** | Irssi-based lab workflow |
| **Social Engineering Lab Tool** | Social Engineering Toolkit |
| **Email Client** | Thunderbird |
| **Operating Systems** | Windows Server, Kali Linux, Ubuntu Linux, Debian Linux, Raspberry Pi OS, FreeBSD / pfSense |

---

## 🧠 How It Works

```text
Vulnerable Application
        │
        ▼
  Injection Testing  ─────────── DOM XSS, reflected XSS, SQL injection behavior
        │
        ▼
  Response Analysis  ─────────── Browser developer tools, HTTP status codes, JSON data
        │
        ▼
  Malware Scenario  ──────────── Controlled payload execution and system enumeration
        │
        ▼
  Availability Scenario  ─────── DDoS traffic simulation and failed web connection
        │
        ▼
  Social Engineering Scenario ── Phishing-style user deception workflow
        │
        ▼
  Defensive Controls  ────────── Mitigation research and security recommendations
```

1. **Tested web application input handling** using OWASP Juice Shop
2. **Observed DOM XSS and reflected XSS behavior** in a controlled vulnerable application
3. **Reviewed SQL injection behavior** through login bypass and database response analysis
4. **Inspected web requests and responses** using Firefox Developer Tools
5. **Observed malware attack workflow concepts** in a closed lab environment
6. **Reviewed post-compromise system information** to understand attacker objectives
7. **Simulated distributed denial-of-service impact** against a lab web service
8. **Reviewed social engineering workflow concepts** and phishing-style data collection risk
9. **Documented defensive measures** for each attack vector

---

## 📂 Project Structure

```text
common-attack-vectors-lab/
├── README.md
└── notes/
    ├── key-takeaways.md
    ├── defensive-measures.md
    └── attack-vector-summary.md
```

---

## ⚙️ Lab Summary

### Objective

Understand how common cyberattacks are performed in a controlled lab environment and identify practical defensive measures that reduce the likelihood or impact of those attacks.

### Main Activities

| Area | What Was Practiced |
|---|---|
| **Injection Attacks** | DOM XSS, reflected XSS, SQL injection, vulnerable input handling |
| **Web App Analysis** | Browser developer tools, HTTP requests/responses, JSON inspection |
| **Malware Scenario** | Payload behavior, reverse shell concept, system information gathering |
| **DDoS Scenario** | Recruited hosts, availability disruption, connection timeout behavior |
| **Social Engineering** | Phishing-style workflow and user deception risks |
| **Defensive Research** | Mitigations for injection, malware, denial-of-service, social engineering, and credential attacks |

---

## 🔐 Security Concepts Demonstrated

- **Attack Vectors** — Paths attackers use to compromise confidentiality, integrity, or availability
- **Cross-Site Scripting** — Injection of script content into a browser context
- **SQL Injection** — Manipulation of database queries through unsafe input handling
- **Reverse Shell Concept** — Outbound connection behavior used to bypass inbound firewall restrictions
- **Denial of Service** — Overwhelming a service so legitimate users cannot access it
- **Social Engineering** — Manipulating people into taking unsafe actions
- **Defense-in-Depth** — Combining technical controls, monitoring, user training, and response planning
- **Secure Coding** — Preventing injection through prepared statements, validation, and encoding
- **Endpoint Defense** — Blocking or detecting malicious execution
- **Availability Protection** — Using filtering, rate limiting, scaling, and DDoS response controls

---

## 📸 Suggested Screenshots to Include Later

From the submitted lab report, the strongest portfolio screenshots would be:

| Screenshot | Why It Is Useful |
|---|---|
| **DOM XSS dialog box** | Shows web injection testing in OWASP Juice Shop |
| **Successful admin login** | Shows SQL injection impact in a vulnerable app |
| **Successful reflected XSS injection** | Shows reflected XSS behavior |
| **User with @owasp.org email** | Shows database information exposure from SQL injection |
| **msfvenom output** | Shows malware generation concept in a controlled lab; redact sensitive details |
| **Opening malware payload dialog** | Shows user-execution risk and social engineering relevance |
| **sysinfo output** | Shows post-compromise enumeration concept; redact host/user details |
| **Newly recruited hosts** | Shows DDoS/botnet simulation concept |
| **drisst.org before and failed connection after** | Shows availability impact |
| **PF states limit reached** | Shows infrastructure-level resource exhaustion evidence |
| **SET phishing email composition** | Shows social engineering workflow; redact payload links and targets |
| **transaction.php page** | Shows phishing landing-page risk; redact sensitive fields |

---

## 🧩 Key Takeaways

- Injection attacks happen when applications treat untrusted input as executable code or database logic.
- DOM XSS, reflected XSS, and SQL injection demonstrate why input handling must be designed carefully.
- Browser developer tools are useful for understanding web requests, responses, errors, and exposed data.
- Malware often relies on user execution, unsafe downloads, weak endpoint controls, or social engineering.
- Reverse-shell behavior helps explain why outbound traffic monitoring matters.
- Denial-of-service attacks target availability, not just confidentiality or integrity.
- Social engineering attacks target people and processes, not only technology.
- Defensive security requires secure coding, endpoint protection, monitoring, backups, user awareness, and incident response planning.
- Labs involving offensive tools should be documented carefully and sanitized before being added to a public portfolio.

---

## 🌱 Future Improvements

- [ ] Add sanitized screenshots from OWASP Juice Shop injection testing
- [ ] Add a defensive controls matrix for each attack vector
- [ ] Add a short OWASP Top 10 mapping section
- [ ] Add a safe incident response checklist for malware and phishing scenarios
- [ ] Add a reflection on ethical hacking rules of engagement

---

## 👩‍💻 About Me

Built by **Carlota Arzúa** — a cybersecurity student and developer interested in web application security, infrastructure defense, threat analysis, and applied defensive security.

- 💼 [LinkedIn](https://www.linkedin.com/in/carlota-a-53a75b206/)
- 🌐 [Portfolio]()
- 📧 carlotaarzua@gmail.com

---

## 📄 License

This repository is for educational and defensive portfolio purposes.

Do not redistribute instructor-provided lab manuals, answer keys, exploit commands, executable payloads, phishing templates, credentials, private lab details, or copyrighted course material without permission.
