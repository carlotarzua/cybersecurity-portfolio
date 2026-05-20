# Commands and Wireshark Filters

## Commands Used to Generate Traffic

### Ping

```bash
ping <host-or-ip>
```

Used to generate ICMP Echo Request and Echo Reply traffic.

Example use cases:

```bash
ping default-gateway
ping switch
ping file-server
```

For a public portfolio, avoid committing real internal IP addresses from a school lab.

---

## Wireshark Display Filters

### ICMP

```text
icmp
```

Used to isolate ping traffic and inspect ICMP packet details and payload data.

### FTP

```text
ftp
```

Used to inspect FTP control traffic, passive mode details, and port information.

### SSH

```text
ssh
```

Used to isolate SSH traffic and review SSHv2 encryption and MAC negotiation details.

### Telnet

```text
telnet
```

Used to inspect Telnet traffic and observe why cleartext protocols are risky.

### HTTP

```text
http
```

Used to isolate web traffic during the wireless analysis portion of the lab.

### TCP Port Filtering

```text
tcp.port == 21
tcp.port == 22
tcp.port == 23
tcp.port == 80
```

Useful for filtering traffic by common service ports.

| Port | Protocol |
|---|---|
| 21 | FTP |
| 22 | SSH / SFTP |
| 23 | Telnet |
| 80 | HTTP |

---

## Tools Used

### Wireshark

Used to capture, filter, and analyze packet data.

### PuTTY

Used to generate Telnet and SSH session traffic.

### FileZilla

Used to generate FTP and SFTP file transfer traffic.

### Mininet-WiFi

Used to simulate a wireless network environment.

### Airodump-ng

Used for wireless traffic capture and observation.

### Aireplay-ng

Used in the controlled lab environment to generate deauthentication traffic.

---

## Publishing Notes

Before adding screenshots or capture files to GitHub:

- Remove names and email addresses
- Remove credentials
- Redact internal IP addresses and hostnames
- Avoid uploading raw `.pcap` files if they contain sensitive data
- Avoid publishing instructor-provided lab content
- Use cropped screenshots that show only the skill being demonstrated
