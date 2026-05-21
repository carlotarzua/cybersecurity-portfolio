# Key Takeaways

## Overview

This lab explored common attack vectors in a controlled training environment. The main lesson was that attackers can target applications, endpoints, networks, availability, and people. Defenders need layered controls that reduce risk before, during, and after an attack.

## Main Takeaways

### 1. Injection attacks come from unsafe input handling

XSS and SQL injection happen when an application accepts input and uses it in a dangerous way. Input should never be trusted automatically.

### 2. XSS affects the browser context

DOM XSS and reflected XSS show how malicious script content can execute in a user's browser context when an application fails to handle input safely.

### 3. SQL injection can expose or alter database information

SQL injection can bypass normal application logic, reveal database errors, or expose records that users should not be able to access.

### 4. Error messages can leak useful information

Detailed server errors can reveal database type, query structure, or application behavior. Production systems should avoid exposing sensitive debugging details.

### 5. Malware often depends on execution

Malware attacks commonly require a user, process, or vulnerability to execute code. Endpoint controls, application allowlisting, and user awareness reduce this risk.

### 6. Reverse connections show why outbound monitoring matters

A system behind a firewall can still be compromised if malicious code initiates an outbound connection. Firewalls should be paired with endpoint monitoring and egress filtering.

### 7. Denial-of-service attacks target availability

DDoS scenarios show how services can become unavailable when resources are exhausted. Availability is part of the CIA triad and must be protected.

### 8. Social engineering targets human behavior

Technical controls are important, but users can still be tricked into clicking links, opening files, or sharing sensitive information.

### 9. Defense requires multiple layers

Prepared statements, output encoding, endpoint protection, backups, filtering, rate limiting, monitoring, training, and phishing-resistant authentication all work together.

## Reflection

This lab helped connect offensive techniques to defensive thinking. The value of the lab is not in repeating attacks, but in understanding how they work so better controls can be designed, tested, and documented.
