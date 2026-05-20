# 🎯 Packet Capture & Traffic Analysis Lab

![Cybersecurity](https://img.shields.io/badge/Cybersecurity-0A66C2?style=for-the-badge&logo=securityscorecard&logoColor=white)
![Wireshark](https://img.shields.io/badge/Wireshark-1679A7?style=for-the-badge&logo=wireshark&logoColor=white)
![Networking](https://img.shields.io/badge/Networking-00599C?style=for-the-badge&logo=cisco&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![Wireless Security](https://img.shields.io/badge/Wireless%20Security-6A5ACD?style=for-the-badge&logo=wifi&logoColor=white)

A hands-on cybersecurity lab focused on **packet capture, protocol analysis, traffic filtering, and wireless traffic inspection** using Wireshark and supporting network tools.

This lab demonstrates foundational network security analysis skills, including capturing live traffic, comparing encrypted and unencrypted protocols, inspecting packet headers and payloads, analyzing ICMP/FTP/SSH traffic, and reviewing wireless frames and WPA-style handshake behavior.

---

## ✨ Features

- 🦈 **Live Packet Capture** — Captured network traffic using Wireshark on a selected network interface
- 📦 **Packet-Level Inspection** — Reviewed packet list, packet details, and packet bytes panes
- 🌐 **Protocol Analysis** — Analyzed ICMP, Telnet, SSH, FTP, SFTP, HTTP, and wireless traffic
- 🔍 **Display Filtering** — Used Wireshark filters to isolate specific protocol traffic
- 🔐 **Encrypted vs. Cleartext Traffic Comparison** — Compared insecure protocols like FTP/Telnet with encrypted protocols like SSH/SFTP
- 📡 **Wireless Traffic Review** — Analyzed wireless network details including SSID, channel, ICMP/HTTP packets, and handshake information
- 🛡️ **Security Takeaways** — Identified why encryption, secure authentication, and traffic visibility matter in defensive security

---

## 🚀 Demo

> The lab captures live traffic, generates multiple types of network activity, and uses Wireshark to inspect how protocols appear at the packet level.

```text
Generate Traffic
        │
        ▼
 Capture with Wireshark
        │
        ▼
 Apply Display Filters
        │
        ▼
 Inspect Packet Details
        │
        ▼
 Compare Cleartext vs. Encrypted Traffic
        │
        ▼
 Document Security Findings
```

> Note: Before publishing screenshots, remove or blur names, student email addresses, timestamps, platform watermarks, private IP addresses, credentials, and any course-provided lab identifiers.

---

## 🛠️ Tech Stack

| Component | Technology |
|---|---|
| **Packet Capture** | Wireshark |
| **Remote Access / Sessions** | PuTTY, Telnet, SSH |
| **File Transfer** | FileZilla, FTP, SFTP |
| **Network Testing** | `ping`, ICMP |
| **Wireless Lab Environment** | Mininet-WiFi |
| **Wireless Analysis Tools** | Airodump-ng, Aireplay-ng |
| **Operating Systems** | Windows Server, Linux, FreeBSD |
| **Traffic Types Reviewed** | ICMP, Telnet, SSHv2, FTP, SFTP, HTTP, 802.11 wireless traffic |

---

## 🧠 How It Works

```text
User Activity
        │
        ▼
  Traffic Generation  ─────────── Ping, Telnet, SSH, FTP, SFTP, HTTP, wireless activity
        │
        ▼
  Packet Capture  ─────────────── Wireshark captures frames from the selected interface
        │
        ▼
  Traffic Filtering  ──────────── Display filters isolate protocols such as ICMP, FTP, SSH, HTTP
        │
        ▼
  Packet Inspection  ──────────── Packet List, Packet Details, and Packet Bytes panes are reviewed
        │
        ▼
  Security Analysis  ──────────── Cleartext vs. encrypted traffic is compared
        │
        ▼
  Findings  ───────────────────── Key risks and defensive lessons are documented
```

1. **Started a Wireshark capture session** on the lab workstation network interface
2. **Generated traffic** using ping, Telnet, SSH, FTP, SFTP, and wireless lab activity
3. **Filtered captured packets** to isolate specific protocols
4. **Inspected packet layers** including frame, Ethernet, IP, transport, and application-layer details
5. **Reviewed ICMP payload data** to understand how packet bytes are represented
6. **Compared insecure protocols** such as Telnet and FTP against encrypted protocols such as SSH and SFTP
7. **Analyzed wireless traffic** including SSID/channel information, ICMP/HTTP details, and four-way handshake information
8. **Documented security lessons** related to encryption, packet visibility, and traffic analysis

---

## 📂 Project Structure

```text
packet-capture-traffic-analysis-lab/
├── README.md
└── notes/
    ├── key-takeaways.md
    ├── commands-and-filters.md
    └── protocol-analysis-summary.md
```

---

## ⚙️ Lab Summary

### Objective

Use Wireshark to capture and analyze network traffic, identify information at different layers of the TCP/IP protocol stack, apply filters, and compare wired and wireless packet behavior.

### Main Activities

| Area | What Was Practiced |
|---|---|
| **Packet Capture** | Started and stopped a Wireshark capture session |
| **Traffic Generation** | Created ICMP, Telnet, SSH, FTP, SFTP, HTTP, and wireless traffic |
| **Packet Analysis** | Reviewed packet list, packet details, and packet bytes panes |
| **ICMP Review** | Inspected ICMP payload data |
| **Telnet Review** | Observed how cleartext session data can appear in captures |
| **SSH Review** | Identified SSHv2 encryption and MAC selections |
| **FTP Review** | Reviewed passive port and destination port details |
| **SFTP Review** | Compared encrypted file transfer behavior against FTP |
| **Wireless Review** | Inspected SSID, channel, ICMP/HTTP wireless packets, and handshake details |

---

## 🧪 Commands, Filters & Tools Practiced

### Network Traffic Generation

```bash
ping <host-or-ip>
```

Used to generate ICMP Echo Request and Echo Reply traffic.

### Wireshark Display Filters

```text
icmp
ftp
ssh
telnet
http
```

Used to isolate protocol-specific packets for analysis.

### Tools Used

```text
Wireshark
PuTTY
FileZilla
Mininet-WiFi
Airodump-ng
Aireplay-ng
```

---

## 🔐 Security Concepts Demonstrated

- **Packet Capture** — Collecting network traffic for troubleshooting and security analysis
- **Protocol Analysis** — Understanding how different protocols appear in packet captures
- **Encapsulation** — Observing how frames, IP packets, and protocol data are layered
- **Cleartext Risk** — Seeing why Telnet and FTP can expose sensitive information
- **Encryption Benefits** — Understanding how SSH and SFTP protect session and file transfer data
- **Display Filtering** — Narrowing large packet captures to relevant traffic
- **Wireless Security Analysis** — Reviewing wireless frames, SSID/channel details, and handshake-related traffic
- **Traffic Baseline Awareness** — Learning why analysts need to understand normal traffic before identifying suspicious activity

---

## 📸 Suggested Screenshots to Include Later

From the submitted lab report, the strongest portfolio screenshots would be:

| Screenshot | Why It Is Useful |
|---|---|
| **Successful FTP and SFTP transfers** | Shows hands-on file transfer testing and comparison of secure vs. insecure protocols |
| **ICMP payload** | Demonstrates packet byte-level analysis in Wireshark |
| **Telnet Last Login / cleartext packet details** | Shows why unencrypted protocols are risky |
| **SSHv2 encryption and MAC selections** | Shows encrypted session negotiation |
| **Encrypted SSH packet bytes** | Demonstrates that encrypted traffic is not readable like cleartext traffic |
| **FTP passive port details** | Shows protocol-level packet inspection |
| **Destination port field value** | Demonstrates transport-layer analysis |
| **SSID and channel details** | Shows wireless packet inspection |
| **Four-way handshake information** | Shows wireless security analysis skills |
| **Deauthentication packet output** | Shows wireless attack/defense awareness in a controlled lab |

---

## 🧩 Key Takeaways

- Wireshark is useful for both troubleshooting and cybersecurity analysis.
- Packet captures make it possible to inspect traffic across multiple layers of the network stack.
- Display filters are essential for finding relevant packets in large captures.
- ICMP traffic is useful for testing reachability and reviewing packet structure.
- Telnet and FTP can expose sensitive information because they do not encrypt traffic.
- SSH and SFTP protect session data through encryption and integrity checks.
- Packet bytes can reveal cleartext information when insecure protocols are used.
- Wireless traffic analysis requires attention to SSIDs, channels, management frames, and handshake packets.
- Security analysts need to understand normal traffic before they can reliably identify suspicious or malicious traffic.

---

## 🌱 Future Improvements

- [ ] Add sanitized screenshots from the Wireshark packet analysis
- [ ] Add a mini cheat sheet of Wireshark filters
- [ ] Add a comparison table for FTP vs. SFTP and Telnet vs. SSH
- [ ] Add a short reflection on cleartext protocol risk
- [ ] Add a wireless security section with handshake and deauthentication notes

---

## 👩‍💻 About Me

Built by **Carlota Arzúa** — a cybersecurity student and developer interested in network security, traffic analysis, infrastructure security, and applied defensive security.

- 💼 [LinkedIn](https://www.linkedin.com/in/carlota-a-53a75b206/)
- 🌐 [Portfolio]()
- 📧 carlotaarzua@gmail.com

---

## 📄 License

This repository is for educational and portfolio purposes.

Do not redistribute instructor-provided lab manuals, answer keys, platform screenshots with sensitive information, packet captures containing credentials, or any copyrighted course material without permission.
