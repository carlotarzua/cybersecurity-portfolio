# Key Takeaways

## Overview

This lab focused on using Wireshark to capture and analyze network traffic. The main lesson was that packet captures can reveal how systems communicate, what protocols are being used, whether traffic is encrypted, and what information may be exposed on the network.

## Main Takeaways

### 1. Packet capture is essential for network visibility

Most network communication is invisible to users. Wireshark allows analysts to inspect that communication and understand what is happening at the packet level.

### 2. Filters make analysis practical

A capture file can contain hundreds or thousands of packets. Display filters such as `icmp`, `ftp`, `ssh`, `telnet`, and `http` make it easier to isolate relevant traffic.

### 3. ICMP is useful for basic connectivity analysis

Ping traffic creates ICMP Echo Request and Echo Reply packets. These packets are useful for confirming reachability and learning how packet fields and payloads appear in Wireshark.

### 4. Cleartext protocols create security risk

Telnet and FTP can expose session information, credentials, commands, and transferred data because they do not encrypt traffic. This makes them risky on untrusted or poorly segmented networks.

### 5. Encrypted protocols protect sensitive data

SSH and SFTP protect traffic with encryption and integrity checks. In Wireshark, encrypted payloads appear unreadable compared with cleartext protocol data.

### 6. Packet details show layered communication

Wireshark makes it possible to inspect frame information, Ethernet details, IP addressing, transport-layer ports, and application-layer protocol information.

### 7. FTP uses separate control and data behavior

FTP analysis showed details such as passive mode and destination port values. This helps explain why FTP can be more complex to secure and monitor than simpler protocols.

### 8. Wireless traffic has additional fields and risks

Wireless analysis includes SSIDs, channels, management frames, ICMP/HTTP traffic, and handshake-related information. Wireless traffic analysis is important for understanding Wi-Fi security.

### 9. Deauthentication and handshake traffic matter for wireless security

The lab included wireless security concepts such as deauthentication traffic and four-way handshake packets, which are important when studying Wi-Fi attack and defense techniques.

## Reflection

This lab connected basic networking concepts to real packet evidence. It showed why secure protocols matter and why analysts need hands-on experience reading packet captures instead of only relying on high-level network summaries.
