Security Controls

1. Purpose

This document maps the identified cybersecurity risks to recommended security controls.

The objective is to reduce the likelihood and/or impact of the identified risks.

---

2. Control Mapping

| Risk ID | Risk | Recommended Control | Purpose |
|---|---|---|---|
| R-01 | Credential Theft | Multi-Factor Authentication (MFA) | Reduce account takeover risk |
| R-01 | Credential Theft | Security Awareness Training | Reduce successful phishing attempts |
| R-02 | Ransomware | Patch Management | Reduce exposure to known vulnerabilities |
| R-02 | Ransomware | Endpoint Protection | Detect and prevent malicious activity |
| R-02 | Ransomware | Secure Backups | Support recovery after data loss |
| R-03 | Unauthorized Network Access | Network Segmentation | Limit lateral movement |
| R-03 | Unauthorized Network Access | Firewall Rules | Restrict unnecessary network traffic |
| R-04 | Unauthorized Data Access | Least Privilege | Restrict unnecessary access |
| R-04 | Unauthorized Data Access | Access Reviews | Identify inappropriate permissions |
| R-05 | Exploitation of Known Vulnerabilities | Patch Management | Reduce exposure to known vulnerabilities |
| R-05 | Exploitation of Known Vulnerabilities | Vulnerability Monitoring | Identify systems requiring remediation |

---

3. Recommended Security Controls

3.1 Multi-Factor Authentication

MFA should be implemented for:

- Email accounts
- Administrative accounts
- Critical applications
- Systems containing sensitive information

MFA provides an additional layer of protection if a password is compromised.

---

3.2 Strong Password Policy

The organization should establish appropriate password requirements and discourage password reuse.

Recommended measures include:

- Strong password requirements
- Password managers where appropriate
- Protection against commonly used passwords
- MFA for important accounts

---

3.3 Patch Management

The organization should establish a documented process for identifying, prioritizing, and deploying security updates.

Critical vulnerabilities should receive higher priority based on their severity and exposure.

---

3.4 Network Segmentation

Critical systems should be separated from general-purpose user networks.

Possible segmentation areas include:

- Staff network
- Guest Wi-Fi
- Administrative systems
- Patient information systems
- Network management systems

Firewall rules should restrict unnecessary communication between segments.

---

3.5 Endpoint Protection

Staff computers should use appropriate endpoint security controls to help detect and prevent malicious activity.

Controls may include:

- Endpoint Protection Platform (EPP)
- Endpoint Detection and Response (EDR)
- Malware protection
- Host-based firewall
- Application control

---

3.6 Least Privilege

Users should receive only the permissions required to perform their assigned responsibilities.

Administrative privileges should be restricted and reviewed regularly.

---

3.7 Secure Backups

Important systems and data should be backed up regularly.

Backups should be:

- Protected from unauthorized access
- Regularly tested
- Recoverable
- Appropriately separated from production systems
- Protected against unauthorized modification or deletion

---

3.8 Security Awareness Training

Employees should receive regular security awareness training covering:

- Phishing
- Password security
- Suspicious attachments
- Social engineering
- Safe browsing
- Reporting security incidents

---

3.9 Logging and Monitoring

Important systems should generate security-relevant logs.

Where practical, logs should be centrally collected and reviewed for suspicious activity.

Examples include:

- Authentication events
- Failed login attempts
- Privilege changes
- System alerts
- Security events

---

4. Defense-in-Depth Strategy

The organization should avoid relying on a single security control.

A layered approach should combine:

| Security Layer | Example Control |
|---|---|
| Identity | MFA and strong authentication |
| Endpoint | EPP / EDR |
| Network | Segmentation and firewalls |
| Data | Access controls and backups |
| People | Security awareness training |
| Monitoring | Logging and security monitoring |
| Recovery | Backup and recovery procedures |

---

5. Control Prioritization

| Priority | Control | Reason |
|---|---|---|
| 1 | Multi-Factor Authentication | Reduces account takeover risk |
| 2 | Patch Management | Reduces exposure to known vulnerabilities |
| 3 | Network Segmentation | Limits attacker movement |
| 4 | Least Privilege | Reduces unauthorized access |
| 5 | Secure Backups | Improves recovery from ransomware and data loss |
| 6 | Endpoint Protection | Helps detect and prevent malware |
| 7 | Security Awareness Training | Reduces human-related security risks |
| 8 | Logging and Monitoring | Improves detection and investigation |

---

6. Key Observation

Effective cybersecurity requires multiple layers of protection.

For example:

MFA + Strong Passwords + Security Awareness + Monitoring

provides stronger protection against credential-based attacks than relying on any single control alone.
