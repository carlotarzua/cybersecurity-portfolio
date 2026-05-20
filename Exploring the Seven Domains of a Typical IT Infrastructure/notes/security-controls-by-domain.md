# Security Controls by Domain

## User Domain

### Threats

- Phishing emails
- Malicious attachments
- Credential theft
- Social engineering

### Controls

- External email warning banners
- Attachment filtering
- Security awareness training
- Least privilege access
- Multi-factor authentication

### Lab Connection

The lab included email examples with external sender warnings and blocked attachment behavior, showing how organizations can reduce phishing and malware risk.

---

## Workstation Domain

### Threats

- Malware execution
- Unpatched software
- Disabled antivirus protection
- Unauthorized software installation

### Controls

- Managed Windows Update policies
- Antivirus and real-time protection
- Tamper protection
- Standard user accounts
- Application execution restrictions

### Lab Connection

The lab reviewed sign-in options, update policies, virus and threat protection settings, and executable restrictions.

---

## LAN Domain

### Threats

- Unauthorized internal access
- ARP spoofing
- Lateral movement
- Insecure shared folders

### Controls

- Network segmentation
- Switch monitoring
- File share permissions
- ARP table inspection
- Access control lists

### Lab Connection

The lab used ARP tables, switch forwarding data, and file server access testing to validate LAN behavior and user access limitations.

---

## LAN-to-WAN Domain

### Threats

- Misconfigured firewall rules
- Insecure NAT rules
- Exposed internal services
- Poor DMZ separation

### Controls

- Firewall rules
- NAT policies
- Static routes
- DMZ segmentation
- Port forwarding review

### Lab Connection

The lab reviewed pfSense outbound NAT settings, permissive LAN rules, static routes, port forwarding, and DMZ firewall rules.

---

## WAN Domain

### Threats

- Routing misconfiguration
- Insecure remote connectivity
- Network path exposure
- Inter-site communication failures

### Controls

- Route validation
- Traceroute testing
- Point-to-point route monitoring
- Secure routing configuration

### Lab Connection

The lab tested point-to-point routing, neighbor connectivity, and traceroute behavior across networks.

---

## Remote Access Domain

### Threats

- Insecure VPN configuration
- Split tunneling risk
- Unauthorized remote access
- DNS leakage

### Controls

- VPN authentication
- Full-tunnel routing when appropriate
- DNS validation
- Remote access monitoring
- Least privilege for remote users

### Lab Connection

The lab used VPN connectivity tests, traceroute results, email server access, and reverse DNS lookup to validate remote access behavior.

---

## System/Application Domain

### Threats

- Weak password policy
- Excessive group permissions
- DNS misconfiguration
- Unmonitored services
- Vulnerable web applications

### Controls

- Active Directory group management
- Strong password policy
- DNS record review
- Service status monitoring
- Application security testing

### Lab Connection

The lab reviewed Active Directory group membership, password policy settings, DNS entries, Docker service status, and OWASP Juice Shop availability.

---

## Summary

The strongest security posture comes from combining these controls. Each domain protects a different part of the infrastructure, and each control supports defense-in-depth.
