# Cybersecurity Risk Assessment Documentation

## Document Information

| Field | Details |
|---|---|
| Document Title | Cybersecurity Risk Assessment |
| Author | Usman Isah Sarki|
| Date Created | September 6, 2026 |
| Project Type | Cybersecurity Portfolio Project |
| Organization | GreenCare Community Hospital (Fictional) |
| Assessment Status | Completed |
| Version | 1.0 |

## 1. Introduction

This document provides the detailed risk assessment methodology used for the fictional GreenCare Community Hospital.

The assessment focuses on identifying important organizational assets, realistic cybersecurity threats, existing vulnerabilities, potential risks, and appropriate security controls.

The assessment follows a simplified risk-analysis approach:

**Asset → Threat → Vulnerability → Risk → Control**

---

## 2. Organization Profile

GreenCare Community Hospital is a fictional healthcare organization with approximately 35 employees.

The organization uses computers, wireless networking, internet connectivity, email, databases, file-sharing systems, and a public website to support its daily operations.

Because the organization processes sensitive patient information, confidentiality, integrity, and availability are important security objectives.

---

## 3. Asset Identification

### Asset 1 — Patient Database

**Classification:** Critical

The patient database contains sensitive medical and personal information.

**Security objectives:**

- Confidentiality
- Integrity
- Availability

**Potential consequences of compromise:**

- Privacy violations
- Data theft
- Unauthorized modification
- Operational disruption
- Reputational damage

---

### Asset 2 — Staff Computers

**Classification:** High

Staff computers provide access to email, hospital systems, files, and other organizational resources.

Compromising one workstation could provide an attacker with an initial foothold inside the organization.

---

### Asset 3 — Email System

**Classification:** High

Email is used for internal and external communication.

Compromised email accounts could be used for:

- Phishing
- Business email compromise
- Credential theft
- Malware distribution
- Unauthorized access to sensitive communications

---

### Asset 4 — Wi-Fi Network

**Classification:** High

The wireless network provides connectivity for staff devices.

Weak authentication, poor configuration, or inadequate segmentation could expose internal systems to unauthorized access.

---

### Asset 5 — Public Website

**Classification:** Medium

The website provides information about the hospital and serves as a public-facing entry point.

A compromised website could result in:

- Defacement
- Malware distribution
- Reputational damage
- Unauthorized access to connected systems

---

## 4. Threat Identification

### 4.1 Phishing

Phishing attempts may target hospital employees through malicious emails or fraudulent login pages.

### 4.2 Malware

Malware may enter the environment through malicious attachments, downloads, compromised websites, or removable media.

### 4.3 Ransomware

Ransomware could encrypt important files and prevent access to critical systems.

### 4.4 Credential Compromise

Attackers may obtain passwords through phishing, password reuse, credential stuffing, or other methods.

### 4.5 Insider Threat

An employee or compromised employee account could intentionally or unintentionally expose sensitive information.

---

## 5. Vulnerability Identification

### 5.1 Weak Password Practices

Weak or reused passwords increase the likelihood of successful credential attacks.

### 5.2 Lack of Multi-Factor Authentication

A stolen password may be sufficient to access an account when MFA is not enabled.

### 5.3 Unpatched Systems

Unpatched software may contain publicly known vulnerabilities that attackers can exploit.

### 5.4 Poor Network Segmentation

Flat networks can allow attackers to move laterally after compromising one system.

### 5.5 Excessive Privileges

Users with unnecessary permissions can cause greater damage if their accounts are compromised.

---

# 6. Risk Analysis

Risk is evaluated using:

**Risk = Likelihood × Impact**

For this assessment, likelihood and impact are categorized as:

- Low
- Medium
- High
- Critical

## 6.1 Risk Rating

| Likelihood | Impact | Risk Level |
|---|---|---|
| Low | Low | Low |
| Low | Medium | Low |
| Medium | Medium | Medium |
| Medium | High | High |
| High | High | Critical |

---

## 6.2 Risk Register

| ID | Asset | Threat | Vulnerability | Likelihood | Impact | Risk |
|---|---|---|---|---|---|---|
| R-01 | Email system | Credential theft | No MFA | High | High | Critical |
| R-02 | Patient database | Ransomware | Unpatched systems | Medium | Critical | High |
| R-03 | Network | Network attack | Poor segmentation | Medium | High | High |
| R-04 | Patient database | Insider threat | Excessive privileges | Medium | Critical | High |
| R-05 | Staff computers | Exploitation | Unpatched software | Medium | High | High |

---

# 7. Detailed Risk Analysis

## R-01 — Credential Theft

### Risk Description

An attacker obtains an employee's credentials through phishing and gains unauthorized access to the email system.

**Threat:** Phishing / credential theft

**Vulnerability:** Lack of MFA and weak password practices

**Asset:** Staff email accounts

**Likelihood:** High

**Impact:** High

**Risk Level:** Critical

### Potential Impact

- Unauthorized access to sensitive communications
- Data theft
- Further compromise of internal systems
- Account takeover
- Phishing campaigns using compromised accounts

### Recommended Controls

- Enable MFA
- Enforce strong password policies
- Provide phishing awareness training
- Implement email security controls
- Monitor suspicious login activity

### Risk Treatment

**Mitigate**

---

## R-02 — Ransomware Infection

### Risk Description

A ransomware infection could prevent staff from accessing patient information and critical files.

**Threat:** Ransomware

**Vulnerability:** Unpatched systems and insufficient endpoint protection

**Asset:** Patient database and file-sharing systems

**Likelihood:** Medium

**Impact:** Critical

**Risk Level:** High

### Potential Impact

- Loss of access to patient information
- Disruption of hospital operations
- Data loss
- Recovery costs
- Potential data exposure

### Recommended Controls

- Implement regular patch management
- Deploy endpoint protection
- Maintain offline or isolated backups
- Restrict administrative privileges
- Monitor endpoint activity
- Develop an incident response procedure

### Risk Treatment

**Mitigate**

---

## R-03 — Unauthorized Network Access

### Risk Description

An attacker compromises a workstation and uses the internal network to reach additional systems.

**Threat:** Network-based attack

**Vulnerability:** Poor network segmentation

**Asset:** Hospital network and internal systems

**Likelihood:** Medium

**Impact:** High

**Risk Level:** High

### Potential Impact

- Lateral movement
- Unauthorized access to internal systems
- Data theft
- Malware propagation
- Increased incident impact

### Recommended Controls

- Segment the network
- Separate guest Wi-Fi from internal systems
- Use firewalls
- Restrict unnecessary network access
- Monitor network traffic

### Risk Treatment

**Mitigate**

---

## R-04 — Unauthorized Patient Data Access

### Risk Description

A compromised or malicious employee account could access patient records beyond the user's legitimate responsibilities.

**Threat:** Insider threat / compromised account

**Vulnerability:** Excessive user privileges

**Asset:** Patient database

**Likelihood:** Medium

**Impact:** Critical

**Risk Level:** High

### Potential Impact

- Unauthorized disclosure of patient information
- Unauthorized modification of records
- Privacy violations
- Reputational damage
- Regulatory consequences

### Recommended Controls

- Apply least privilege
- Implement role-based access control
- Review user permissions regularly
- Use strong authentication
- Monitor access to sensitive records
- Maintain audit logs

### Risk Treatment

**Mitigate**

---

## R-05 — Exploitation of Unpatched Systems

### Risk Description

Attackers exploit known vulnerabilities in outdated operating systems or applications.

**Threat:** Exploitation of known software vulnerabilities

**Vulnerability:** Poor patch management

**Asset:** Staff computers and servers

**Likelihood:** Medium

**Impact:** High

**Risk Level:** High

### Potential Impact

- System compromise
- Malware infection
- Data theft
- Unauthorized access
- Service disruption

### Recommended Controls

- Establish a patch management process
- Prioritize critical security updates
- Maintain an inventory of systems and software
- Perform regular vulnerability scanning
- Remove unsupported software

### Risk Treatment

**Mitigate**

---

# 8. Security Controls

The following controls are recommended to reduce the identified risks.

| Control | Purpose |
|---|---|
| Multi-Factor Authentication | Reduce account compromise |
| Strong password policy | Improve credential security |
| Network segmentation | Limit lateral movement |
| Regular patching | Reduce exploitable vulnerabilities |
| Endpoint protection | Detect and prevent malware |
| Least privilege | Reduce unauthorized access |
| Regular backups | Support recovery from ransomware |
| Security awareness training | Reduce phishing success |
| Access reviews | Identify excessive permissions |
| Logging and monitoring | Detect suspicious activity |

---

# 9. Security Control Mapping

| Risk | Primary Control | Expected Benefit |
|---|---|---|
| R-01 Credential theft | MFA | Reduce unauthorized account access |
| R-02 Ransomware | Backups + patch management | Reduce likelihood and impact of ransomware |
| R-03 Network compromise | Network segmentation | Limit lateral movement |
| R-04 Unauthorized data access | Least privilege + RBAC | Restrict access to sensitive information |
| R-05 Unpatched systems | Patch management | Reduce exposure to known vulnerabilities |

---

# 10. Recommended Security Priorities

The organization should prioritize controls based on potential risk reduction.

## Immediate Priorities

1. Enable MFA for critical accounts.
2. Patch critical and high-risk vulnerabilities.
3. Implement protected backups.
4. Remove unnecessary administrative privileges.
5. Separate guest Wi-Fi from internal systems.

## Medium-Term Priorities

1. Establish vulnerability management.
2. Improve centralized logging.
3. Conduct security awareness training.
4. Implement formal access reviews.
5. Develop an incident response plan.

## Long-Term Priorities

1. Develop a formal security program.
2. Conduct periodic risk assessments.
3. Perform regular security testing.
4. Improve security monitoring capabilities.
5. Establish documented security policies and procedures.

---

# 11. Risk Treatment Strategy

The primary risk treatment strategy for the identified risks is **risk mitigation**.

The organization should reduce cybersecurity risk by implementing preventive, detective, and corrective controls.

### Preventive Controls

Examples include:

- MFA
- Strong passwords
- Network segmentation
- Least privilege
- Security awareness training
- Patch management

### Detective Controls

Examples include:

- Security logging
- Login monitoring
- Network monitoring
- Endpoint monitoring
- Access auditing

### Corrective Controls

Examples include:

- Backups
- Incident response procedures
- System recovery procedures
- Malware removal
- Account recovery procedures

---

# 12. Conclusion

The assessment demonstrates that a small organization can face significant cybersecurity risks even without a large or complex IT environment.

For GreenCare Community Hospital, the highest-priority areas are identity security, patch management, network segmentation, access control, and data recovery.

Implementing these controls would reduce the likelihood and potential impact of several major cybersecurity incidents.

The assessment also demonstrates the importance of approaching cybersecurity from a risk perspective rather than focusing only on individual vulnerabilities.

A vulnerability matters because of what it could allow an attacker to do, which assets could be affected, and how severe the resulting consequences could be.

The overall assessment process can therefore be summarized as:

**Asset → Threat → Vulnerability → Risk → Control → Risk Reduction**

---

# 13. Lessons Learned

This project demonstrated the importance of understanding the relationship between assets, threats, vulnerabilities, and risks.

Key lessons include:

- Cybersecurity risk assessment starts with identifying what needs to be protected.
- Not every vulnerability represents the same level of risk.
- Risk depends on both likelihood and potential impact.
- Critical assets require stronger protection.
- Security controls should be selected based on the risks they address.
- Documentation is an important part of cybersecurity work.
- Risk assessment helps organizations prioritize limited security resources.

---

# 14. Limitations

This assessment is based on a fictional organization and does not represent an actual security assessment of a real hospital.

The assessment does not include:

- Live vulnerability scanning
- Penetration testing
- Real network traffic analysis
- Actual security logs
- Real user interviews
- Configuration reviews
- Physical security assessment
- Regulatory compliance audit

The risks and controls presented are therefore theoretical and intended for educational and portfolio purposes.

---

# 15. References

- National Institute of Standards and Technology (NIST)
- NIST Special Publication 800-30 — Guide for Conducting Risk Assessments
- NIST Cybersecurity Framework
- NIST Risk Management Framework
- Open Worldwide Application Security Project (OWASP)
- MITRE ATT&CK
- Cybersecurity and Infrastructure Security Agency (CISA)