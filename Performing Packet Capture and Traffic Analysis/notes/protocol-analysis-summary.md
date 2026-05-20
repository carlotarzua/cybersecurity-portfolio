# Protocol Analysis Summary

## ICMP

ICMP was used to test network reachability with ping. In Wireshark, ICMP packets showed Echo Request and Echo Reply behavior, packet details, and payload bytes.

### Security relevance

ICMP is useful for troubleshooting, but it can also be used during reconnaissance to identify live hosts.

---

## Telnet

Telnet was used to create a remote terminal session. Because Telnet is not encrypted, its packet data can reveal readable session information in Wireshark.

### Security relevance

Telnet should be avoided for administrative access. SSH is preferred because it encrypts the session.

---

## SSH

SSH was used to create an encrypted remote session. Wireshark showed SSHv2 negotiation details such as encryption and MAC selections. The packet bytes were not readable like Telnet traffic.

### Security relevance

SSH protects confidentiality and integrity for remote administration.

---

## FTP

FTP was used to transfer a file. Wireshark analysis included FTP control details such as passive mode and port information.

### Security relevance

FTP is insecure because it does not encrypt credentials or transferred data. It should be replaced with SFTP, FTPS, or another secure file transfer method.

---

## SFTP

SFTP was used to perform a secure file transfer over SSH.

### Security relevance

SFTP encrypts file transfer traffic, making it safer than FTP for sensitive or untrusted networks.

---

## HTTP

HTTP appeared in the wireless traffic analysis portion of the lab.

### Security relevance

HTTP is unencrypted and can expose web traffic. HTTPS should be used whenever possible.

---

## Wireless Traffic

Wireless analysis included SSID and channel information, ICMP and HTTP packet details, four-way handshake information, and deauthentication-related traffic.

### Security relevance

Wireless networks require strong encryption, secure authentication, and monitoring for suspicious management frames such as deauthentication packets.

---

## Cleartext vs. Encrypted Traffic

| Protocol | Encrypted? | Risk |
|---|---:|---|
| Telnet | No | Can expose session data |
| FTP | No | Can expose credentials and files |
| HTTP | No | Can expose web traffic |
| SSH | Yes | Protects remote sessions |
| SFTP | Yes | Protects file transfers |

## Summary

This lab showed that packet captures can reveal sensitive information when insecure protocols are used. It also showed how encrypted protocols change what analysts can see in packet bytes, while still allowing metadata and protocol behavior to be inspected.
