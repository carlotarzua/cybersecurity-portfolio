# Defensive Measures

## Injection Attacks

### Risks

- Cross-site scripting
- SQL injection
- Data exposure
- Authentication bypass
- Application logic abuse

### Defensive Measures

- Use prepared statements and parameterized queries
- Validate input on the server side
- Encode output before rendering it in the browser
- Use content security policy headers
- Avoid exposing detailed database errors to users
- Perform secure code review and dynamic application testing

---

## Malware Attacks

### Risks

- Unauthorized shell access
- Data theft
- Persistence
- Lateral movement
- Ransomware-style impact

### Defensive Measures

- Use endpoint detection and response tools
- Enable antivirus and real-time protection
- Use application allowlisting
- Block unknown executables where possible
- Keep operating systems and applications patched
- Monitor outbound connections
- Maintain tested backups
- Train users not to run untrusted downloads

---

## Denial-of-Service Attacks

### Risks

- Service outage
- Resource exhaustion
- Firewall state table exhaustion
- Business disruption
- Reduced customer trust

### Defensive Measures

- Use rate limiting and traffic filtering
- Deploy DDoS protection services
- Monitor abnormal traffic volume
- Configure firewall state limits appropriately
- Use load balancing and scaling
- Prepare an incident response plan for availability events
- Coordinate with ISP or upstream providers during large attacks

---

## Social Engineering Attacks

### Risks

- Credential theft
- Financial fraud
- Malware delivery
- Sensitive information disclosure
- Unauthorized account access

### Defensive Measures

- Conduct security awareness training
- Use phishing-resistant multi-factor authentication
- Verify financial requests through a second channel
- Mark external emails clearly
- Disable or sandbox dangerous attachments
- Report and analyze phishing attempts
- Use email authentication controls such as SPF, DKIM, and DMARC

---

## Credential Attacks

### Risks

- Account takeover
- Privilege escalation
- Unauthorized access to data
- Reuse of compromised passwords

### Defensive Measures

- Enforce strong password policies
- Use multi-factor authentication
- Detect impossible travel and suspicious logins
- Lock or throttle repeated failed login attempts
- Disable unused accounts
- Apply least privilege
- Monitor privileged accounts closely

---

## Portfolio Safety Notes

Do not publish:

- Exploit commands
- Working malware payloads
- Phishing templates
- Target IP addresses or domains from a private lab
- Credentials
- Internal hostnames
- Unredacted system information
- Instructor-provided answer-key material
