Cybersecurity Risk Assessment Report

1. Executive Summary

This project presents a cybersecurity risk assessment conducted for GreenCare Community Hospital, a fictional small healthcare organization with approximately 35 employees.

The assessment focuses on identifying important organizational assets, potential threats, security vulnerabilities, associated risks, and appropriate security controls.

The assessment identified several high-priority risks involving credential compromise, ransomware, unauthorized network access, excessive privileges, and exploitation of unpatched systems.

The purpose of the assessment is to demonstrate a practical understanding of cybersecurity risk identification, analysis, prioritization, and treatment.

---

2. Organization Overview

GreenCare Community Hospital is a fictional healthcare organization providing basic medical services to members of its local community.

The organization has approximately 35 employees and relies on technology for:

- patient record management
- staff communication
- email
- internet access
- internal file sharing
- website services
- wireless connectivity
- administrative operations

The organization handles sensitive information, making confidentiality, integrity, and availability important security requirements.

---

3. Assessment Objectives

The objectives of this assessment are to:

1. identify critical organizational assets
2. identify relevant cybersecurity threats
3. identify potential vulnerabilities
4. evaluate cybersecurity risks
5. prioritize identified risks
6. recommend appropriate security controls
7. develop a practical remediation plan

---

4. Assessment Scope

The assessment covers:

- patient information systems
- employee computers
- email systems
- wireless networks
- public-facing website
- internal file-sharing systems
- network infrastructure
- user accounts and access privileges

This is a fictional assessment and does not involve testing or accessing any real organization's systems.

---

5. Overall Findings

The assessment identified five major risks requiring attention:

Risk ID| Risk| Severity
R-01| Credential theft through phishing and lack of MFA| Critical
R-02| Ransomware affecting patient information systems| High
R-03| Unauthorized network access due to poor segmentation| High
R-04| Unauthorized patient data access due to excessive privileges| High
R-05| Exploitation of unpatched systems| High

The most important security improvements are:

- implementing multi-factor authentication
- improving password security
- establishing a patch management process
- implementing network segmentation
- applying least-privilege access
- maintaining secure backups
- improving security awareness
- implementing appropriate logging and monitoring

---

6. Risk Assessment Approach

The assessment follows a basic risk analysis process:

Asset → Threat → Vulnerability → Risk → Control → Remediation

Each identified risk was evaluated using:

- likelihood of occurrence
- potential impact
- overall risk severity

The assessment uses qualitative risk ratings rather than financial risk calculations.

---

7. Conclusion

GreenCare Community Hospital has several cybersecurity risks that could significantly affect its operations and sensitive information if left untreated.

The assessment demonstrates that cybersecurity risk management is not only about identifying technical vulnerabilities. It also requires understanding assets, threats, business impact, access control, security processes, and appropriate risk treatment.

The recommended controls provide a practical starting point for reducing the organization's overall cybersecurity exposure.
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
