# Attack Vector Summary

## Injection Attacks

Injection attacks occur when an application processes untrusted input as code, query logic, or executable content.

### Lab examples

- DOM XSS
- Reflected XSS
- SQL injection
- JSON/API data exposure

### Defensive focus

Secure coding, input validation, output encoding, prepared statements, and safe error handling.

---

## Malware Attacks

Malware attacks use harmful code to perform unauthorized actions on a system.

### Lab concepts

- Payload delivery
- User execution
- Reverse-shell behavior
- System information gathering after compromise

### Defensive focus

Endpoint protection, application allowlisting, patching, outbound monitoring, backups, and user awareness.

---

## Denial-of-Service Attacks

Denial-of-service attacks attempt to make a service unavailable to legitimate users.

### Lab concepts

- Recruited hosts
- Web service unavailability
- Connection timeouts
- Firewall state exhaustion

### Defensive focus

Rate limiting, filtering, DDoS protection, monitoring, scaling, and response planning.

---

## Social Engineering Attacks

Social engineering attacks manipulate people into taking unsafe actions.

### Lab concepts

- Phishing-style email composition
- Fake transaction page
- Sensitive information collection risk

### Defensive focus

Training, reporting, multi-factor authentication, email security, and out-of-band verification.

---

## Misconfiguration and Information Exposure

Misconfiguration attacks take advantage of unsafe defaults, exposed functionality, verbose errors, or abandoned features.

### Lab-related examples

- Detailed server error messages
- Exposed API-style JSON data
- Publicly reachable vulnerable services

### Defensive focus

Hardening, least privilege, secure deployment, error handling, access control, and regular configuration review.

---

## Ethical Use

The techniques studied in this lab should only be used in authorized environments, such as class labs, capture-the-flag systems, internal security testing with written permission, or approved penetration tests.
