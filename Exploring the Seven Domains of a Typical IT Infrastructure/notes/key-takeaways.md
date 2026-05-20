# Key Takeaways

## Overview

This lab demonstrated how security controls work across the seven domains of a typical IT infrastructure. The most important lesson was that infrastructure security is not handled by one tool or one setting. It depends on layered controls across users, endpoints, networks, remote access paths, and critical systems.

## Main Takeaways

### 1. Security controls should be layered

No single control is enough. Endpoint protections, access control, firewall rules, VPN routing, DNS, and system monitoring all work together to reduce risk.

### 2. Least privilege reduces impact

User accounts should only have the permissions required for their role. In the lab, access testing showed how a user could access authorized folders while being blocked from unauthorized folders.

### 3. Endpoint hardening matters

Managed update policies, antivirus settings, tamper protection, and blocked executable behavior help prevent users or attackers from weakening workstation security.

### 4. Email security protects the User Domain

External email warnings and blocked attachments help reduce phishing and malware risk before a user can accidentally run malicious content.

### 5. Network visibility is essential

Commands such as `ipconfig`, `arp`, `ping`, and `tracert` help security analysts understand network configuration, host reachability, routing paths, and local communication behavior.

### 6. Firewall and NAT rules define network boundaries

pfSense rules, NAT settings, static routes, port forwarding, and DMZ rules determine which traffic can move between internal, external, and segmented network zones.

### 7. VPN routing affects remote-user security

Traceroute results can show whether VPN traffic is routed through the organization or allowed to exit through the local network.

### 8. System/Application security includes identity, services, and records

Active Directory groups, password policies, DNS entries, Docker services, and web application availability all contribute to the overall security posture.

## Reflection

This lab helped connect cybersecurity concepts to real infrastructure tasks. Instead of only reading about defense-in-depth, least privilege, segmentation, and remote access security, I practiced validating those controls in a simulated enterprise environment.
