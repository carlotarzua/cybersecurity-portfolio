# Commands Used

This file summarizes commands and tools practiced during the lab. Exact outputs and sensitive values should not be committed publicly.

## Windows Networking

### View network configuration

```bash
ipconfig /all
```

Used to inspect network adapters, IP address configuration, DNS settings, MAC addresses, and default gateway information.

### View ARP table

```bash
arp -a
```

Used to inspect IP-to-MAC address mappings learned by the workstation.

### Test host reachability

```bash
ping <host-or-ip>
```

Used to confirm whether hosts on the LAN or across routed networks were reachable.

### Trace network path

```bash
tracert <host-or-ip>
```

Used on Windows to view the route traffic takes to reach a destination.

## Linux / Network Device Commands

### Trace network path

```bash
traceroute <host-or-ip>
```

Used on Linux/Unix-based systems to inspect routing paths.

### DNS lookup

```bash
nslookup <host-or-ip>
```

Used to test forward or reverse DNS resolution.

### Current user context

```bash
whoami
```

Used to verify the current authenticated user or security context.

## Security and Administration Tools

### Windows Security

Used to review antivirus, threat protection, tamper protection, and managed security settings.

### Group Policy Management

Used to inspect security policy settings such as password policy.

### Active Directory

Used to inspect user and group membership.

### pfSense

Used to review firewall rules, NAT configuration, static routes, port forwarding, and DMZ rules.

### PuTTY

Used to remotely connect to network or server systems.

### OpenVPN

Used to test remote access behavior and routing.

### Docker

Used to verify containerized service status.

### OWASP Juice Shop

Used as a sample web application for system/application domain review.

## Public Portfolio Note

Before publishing screenshots or command outputs, remove or blur:

- Student name and email
- Platform watermarks
- Credentials
- Private/internal IP addresses
- Hostnames that belong to a school-provided lab
- Any answer-key style content
