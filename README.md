# cybersecurity-risk-assessment

**Objective**

The objective of this project is to perform a basic cybersecurity risk assessment for a fictional small healthcare organization.

The assessment identifies critical organizational assets, potential threats, vulnerabilities, and associated cybersecurity risks. It also recommends security controls that can reduce the likelihood and impact of those risks.

This project demonstrates practical understanding of:

- Asset identification
- Threat identification
- Vulnerability assessment
- Risk analysis
- Security controls
- Risk mitigation
- Basic security documentation

---

**Organization Overview**

Organization: GreenCare Community Hospital

GreenCare Community Hospital is a fictional small healthcare organization providing outpatient and basic inpatient medical services.

The organization has approximately 35 employees, including doctors, nurses, administrative staff, laboratory personnel, pharmacists, and IT support staff.

**IT Environment**

The hospital's technology environment includes:

- Approximately 25 desktop and laptop computers
- Staff user accounts
- Hospital Wi-Fi network
- Internet connectivity
- Electronic patient database
- Internal email system
- Public-facing hospital website
- Network printer
- Basic file-sharing system
- Administrative systems
- Medical and patient information

**Sensitive Information**

The organization handles sensitive information including:

- Patient names
- Medical histories
- Laboratory results
- Prescriptions
- Contact information
- Staff information
- Administrative and financial records

Because the organization processes sensitive healthcare information, protecting confidentiality, integrity, and availability is particularly important.

---

# Assets

The following assets were identified during the assessment.

| Asset | Importance | Security Concern |
|---|---|---|
| Patient database | Critical | Contains sensitive patient information |
| Staff computers | High | Used to access hospital systems and email |
| Email system | High | May contain sensitive communications |
| Hospital Wi-Fi | High | Provides network access to staff devices |
| Public website | Medium | Public-facing system that may be targeted |
| File-sharing system | High | Stores internal documents and records |
| Network infrastructure | High | Supports connectivity between systems |

**Asset Prioritization**

The patient database is considered the most critical asset because unauthorized disclosure, modification, or loss of patient information could have serious consequences for patients and the organization.

---

**Threats**

The following threats were identified:

1. Phishing

Attackers may send fraudulent emails designed to trick employees into revealing credentials or opening malicious attachments.

2. Malware

Malicious software could infect staff computers through malicious downloads, attachments, compromised websites, or removable media.

3. Ransomware

An attacker could encrypt hospital files and databases, preventing staff from accessing important information and disrupting healthcare operations.

4. Credential Compromise

Usernames and passwords could be stolen through phishing, password reuse, credential stuffing, or other attacks.

5. Insider Threat

A malicious or compromised employee account could be used to access, modify, or disclose sensitive information.

---

**Vulnerabilities**

The assessment identified the following potential vulnerabilities.

1. Weak Password Practices

Employees may use weak, reused, or easily guessed passwords.

2. Lack of Multi-Factor Authentication

Accounts without MFA may be easier to compromise if passwords are stolen.

3. Unpatched Systems

Operating systems and applications may contain known vulnerabilities if security updates are not applied regularly.

4. Poor Network Segmentation

If staff computers, administrative systems, servers, and other devices share the same network, compromise of one device could provide an attacker with greater access to internal resources.

5. Excessive User Privileges

Users may have more permissions than required to perform their jobs, increasing the potential impact of a compromised account.

---

**Risk Assessment**

Risk was evaluated by considering the likelihood of a threat occurring and its potential impact on the organization.

### Risk Rating

| Likelihood | Impact | Risk Level |
|---|---|---|
| Low | Low | Low |
| Low | Medium | Low |
| Medium | Medium | Medium |
| Medium | High | High |
| High | High | Critical |

**Identified Risks**

**Risk 1** — Credential Theft

Threat: Phishing / credential theft

Vulnerability: Lack of MFA and weak password practices

Asset: Staff email accounts

Potential Impact: Unauthorized access to sensitive communications, further compromise of internal systems, and possible data theft.

Likelihood: High

Impact: High

Risk Level: Critical

Recommended Controls:

- Enable MFA
- Enforce strong password policies
- Provide phishing awareness training
- Implement email security controls
- Monitor suspicious login activity

---

**Risk 2** — Ransomware Infection

Threat: Ransomware

Vulnerability: Unpatched systems and insufficient endpoint protection

Asset: Patient database and file-sharing systems

Potential Impact: Loss of access to patient information and disruption of hospital operations.

Likelihood: Medium

Impact: Critical

Risk Level: High

Recommended Controls:

- Implement regular patch management
- Deploy endpoint protection
- Maintain offline or isolated backups
- Restrict administrative privileges
- Monitor endpoint activity
- Develop an incident response procedure

---

**Risk 3** — Unauthorized Network Access

Threat: Network-based attack

Vulnerability: Poor network segmentation

Asset: Hospital network and internal systems

Potential Impact: An attacker compromising one device may gain access to additional systems.

Likelihood: Medium

Impact: High

Risk Level: High

Recommended Controls:

- Segment the network
- Separate guest Wi-Fi from internal systems
- Use firewalls
- Restrict unnecessary network access
- Monitor network traffic

---

**Risk 4** — Unauthorized Access to Patient Data

Threat: Insider threat / compromised account

Vulnerability: Excessive user privileges

Asset: Patient database

Potential Impact: Unauthorized disclosure or modification of patient information.

Likelihood: Medium

Impact: Critical

Risk Level: High

Recommended Controls:

- Apply least privilege
- Implement role-based access control
- Review user permissions regularly
- Monitor access to sensitive records
- Disable accounts immediately when employees leave

---

**Risk 5** — Exploitation of Unpatched Systems

Threat: Exploitation of known software vulnerabilities

Vulnerability: Poor patch management

Asset: Staff computers and servers

Potential Impact: System compromise, malware infection, data theft, or service disruption.

Likelihood: Medium

Impact: High

Risk Level: High

Recommended Controls:

- Establish a patch management process
- Prioritize critical security updates
- Maintain an inventory of systems and software
- Perform regular vulnerability scanning
- Remove unsupported software

---

# Security Controls

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

**Recommendations**

Based on the assessment, GreenCare Community Hospital should prioritize the following actions.

**Priority 1** — Implement MFA

Enable MFA for:

- Email accounts
- Administrative accounts
- Remote access
- Critical applications

**Priority 2** — Improve Patch Management

Establish a documented process for identifying, testing, and deploying security updates.

Critical vulnerabilities should receive priority treatment.

**Priority 3** — Implement Network Segmentation

Separate:

- Staff network
- Guest Wi-Fi
- Servers
- Administrative systems
- Other sensitive systems

This can reduce the ability of attackers to move between systems after an initial compromise.

**Priority 4** — Strengthen Access Control

Implement least privilege and role-based access control.

Users should only have access to the information and systems necessary for their responsibilities.

**Priority 5** — Establish Secure Backups

Maintain regular backups of critical data and ensure that backups are protected from unauthorized access and ransomware.

**Priority 6** — Security Awareness Training

Provide regular training covering:

- Phishing
- Password security
- Social engineering
- Malware
- Safe browsing
- Reporting suspicious activity

**Priority 7** — Logging and Monitoring

Centralize and review security logs where possible.

Important events to monitor include:

- Failed login attempts
- Unusual login locations
- Privilege changes
- Suspicious network activity
- Access to sensitive data

---

**Key Findings**

The assessment identified several areas that could significantly increase cybersecurity risk.

The most important findings are:

1. Lack of MFA could make compromised credentials significantly more dangerous.
2. Weak password practices could increase the probability of account compromise.
3. Poor network segmentation could allow attackers to move between compromised systems.
4. Unpatched systems could expose the organization to known vulnerabilities.
5. Excessive privileges could increase the impact of compromised or malicious accounts.
6. Insufficient backup protection could make ransomware incidents more damaging.

The assessment indicates that identity security, patch management, network segmentation, access control, and backup protection should be among the organization's highest priorities.

---

**Lessons Learned**

This assessment demonstrated that cybersecurity risk is not determined by a vulnerability alone.

A vulnerability becomes more significant when it can be exploited by a realistic threat and affects an important organizational asset.

The assessment also demonstrated the importance of connecting:

Asset → Threat → Vulnerability → Risk → Control

For example:

Patient Database
↓
Ransomware
↓
Unpatched Systems
↓
Loss of access to critical patient information
↓
Patch management + endpoint protection + protected backups

This approach provides a structured way to understand and prioritize cybersecurity risks.

---

**Limitations**

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

**References**

- NIST Cybersecurity Framework
- NIST Risk Management Framework
- NIST Special Publication 800-30 — Guide for Conducting Risk Assessments
- OWASP — Open Worldwide Application Security Project
- MITRE ATT&CK
- CISA — Cybersecurity and Infrastructure Security Agency

---

**Project Status**

Completed — Cybersecurity Fundamentals / Risk Assessment

This project was created as part of my practical cybersecurity learning journey to demonstrate foundational skills in cybersecurity risk identification, assessment, and mitigation.
