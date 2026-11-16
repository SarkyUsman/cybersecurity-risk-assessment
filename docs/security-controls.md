# Security Controls

## 1. Document Information

| Field | Details |
|---|---|
| Document Title | Cybersecurity Security Controls |
| Organization | GreenCare Community Hospital |
| Organization Type | Fictional community healthcare facility |
| Estimated Organization Size | Approximately 35 employees |
| Assumed Jurisdiction | Nigeria |
| Document Version | 2.0 |
| Document Status | Proposed Security Controls |
| Prepared By | Cybersecurity Portfolio Project |
| Assessment Date | November 2026 |
| Related Document | `risk-assessment-report.md` |
| Related Document | `risk-register.md` |

> **Important:** GreenCare Community Hospital is a fictional organization created for this educational portfolio project. The controls documented here are recommendations. They have not been deployed, tested, or independently verified in a real environment. This document does not represent a formal security audit.

---

## 2. Introduction

Security controls are safeguards designed to protect an organization's information systems, networks, applications, and data against cybersecurity threats.

They help reduce the likelihood of security incidents, limit their potential impact, detect suspicious activities, and support recovery when incidents occur.

This document identifies recommended security controls for the hypothetical risks identified in the GreenCare Community Hospital cybersecurity risk assessment.

The recommendations focus on protecting patient information, securing user accounts, reducing malware exposure, controlling network access, improving monitoring, and supporting business continuity.

The controls are linked to the existing asset inventory, threat assessment, vulnerability assessment, and risk register.

---

## 3. Objectives

The objectives of this document are to:

1. Identify appropriate security controls for the risks recorded in the risk register.
2. Recommend preventive controls that reduce the likelihood of security incidents.
3. Recommend detective controls that help identify suspicious activities.
4. Recommend corrective and recovery controls that support incident response and service restoration.
5. Map controls to relevant assets, threats, vulnerabilities, and risk IDs.
6. Identify proposed control owners and implementation priorities.
7. Define measurable evidence that could demonstrate successful implementation.
8. Support the remediation plan and future risk reviews.

---

## 4. Scope

The recommended controls cover the following seven information assets:

| Asset ID | Asset Name | Criticality |
|---|---|---|
| A-01 | Patient Database | Critical |
| A-02 | Staff Computers | High |
| A-03 | Email System | High |
| A-04 | Hospital Wi-Fi | High |
| A-05 | Public Website | Medium |
| A-06 | File-Sharing System | High |
| A-07 | Network Infrastructure | High |

The controls address the following security areas:

- Identity and access management.
- Password security.
- Multi-factor authentication.
- Patch and vulnerability management.
- Network security and segmentation.
- Endpoint protection.
- Data protection.
- Backup and recovery.
- Security logging and monitoring.
- Security awareness.
- Incident response.
- Website security.

---

## 5. Security Control Terminology

Security controls can be grouped according to their purpose.

### 5.1 Control Categories

| Control Category | Description | Example |
|---|---|---|
| Preventive | Designed to stop or reduce the likelihood of a security incident | MFA, access restrictions, patch management |
| Detective | Designed to identify suspicious activity or security incidents | Security logs, alerts, monitoring |
| Corrective | Designed to correct security weaknesses or limit the consequences of an incident | Malware removal, account recovery, system remediation |
| Recovery | Designed to restore systems, information, and services after disruption | Backup restoration and disaster recovery |

A single security control may serve more than one purpose.

### 5.2 Security Control Status

The following status descriptions are used throughout this document.

| Status | Meaning |
|---|---|
| Recommended | A proposed control that should be considered for implementation |
| Planned | A control formally scheduled for implementation |
| Implemented | A control that has been deployed |
| Verified | Evidence has been collected to confirm that the control operates as intended |
| Not Applicable | The control does not apply to the assessed environment |

**Current project status:** The controls in this document are recommendations only. None should be described as implemented or verified based on this assessment.

---

## 6. Identified Vulnerabilities and Related Risks

The assessment identified five hypothetical vulnerability areas.

| Vulnerability ID | Vulnerability | Description | Related Risk IDs |
|---|---|---|---|
| V-01 | Weak Password Practices | Weak, reused, or poorly managed passwords may increase the likelihood of account compromise | R-006 |
| V-02 | Lack of MFA | Accounts without multi-factor authentication may be more vulnerable following credential theft | R-001 |
| V-03 | Unpatched Systems | Outdated operating systems, applications, or components may contain known security weaknesses | R-002, R-005, R-007 |
| V-04 | Poor Network Segmentation | Insufficient separation between network environments may allow unauthorized movement between systems | R-003, R-008 |
| V-05 | Excessive Privileges | Users may have more access than necessary for their responsibilities | R-004 |

These vulnerability descriptions are scenario assumptions, not technically confirmed findings.

---

## 7. Security Control Mapping

The following table maps each identified risk to the recommended security controls.

| Risk ID | Risk Scenario | Vulnerability | Recommended Controls |
|---|---|---|---|
| R-001 | Phishing and email account compromise | V-02 | SC-01, SC-02, SC-08, SC-09, SC-11 |
| R-002 | Ransomware affecting patient records | V-03 | SC-03, SC-06, SC-07, SC-08, SC-11 |
| R-003 | Unauthorized network access and lateral movement | V-04 | SC-04, SC-08, SC-11 |
| R-004 | Insider misuse of patient information | V-05 | SC-05, SC-08, SC-10, SC-11 |
| R-005 | Malware exploitation of unpatched endpoints | V-03 | SC-03, SC-06, SC-07, SC-08, SC-11 |
| R-006 | Unauthorized file access through weak passwords | V-01 | SC-01, SC-02, SC-05, SC-07, SC-10 |
| R-007 | Public website compromise | V-03 | SC-01, SC-03, SC-08, SC-11, SC-12 |
| R-008 | Unauthorized wireless access and movement into internal resources | V-04 | SC-01, SC-04, SC-08, SC-11 |

---

## 8. Recommended Security Controls

Twelve security controls are proposed to address the identified risks.

### 8.1 Security Control Register

| Control ID | Security Control | Control Category | Related Vulnerabilities | Related Risks | Proposed Owner |
|---|---|---|---|---|---|
| SC-01 | Multi-Factor Authentication | Preventive | V-01, V-02 | R-001, R-006, R-007, R-008 | IT Team |
| SC-02 | Strong Password and Password Management Policy | Preventive | V-01, V-02 | R-001, R-006 | IT Team |
| SC-03 | Patch and Vulnerability Management | Preventive / Corrective | V-03 | R-002, R-005, R-007 | IT Team |
| SC-04 | Network Segmentation and Firewall Restrictions | Preventive | V-04 | R-003, R-008 | Network Administrator |
| SC-05 | Role-Based Access Control and Least Privilege | Preventive | V-05, V-01 | R-004, R-006 | IT Team / Database Administrator |
| SC-06 | Endpoint Protection and Malware Detection | Preventive / Detective | V-03 | R-002, R-005 | IT Team |
| SC-07 | Secure Backup and Recovery | Corrective / Recovery | V-03, V-01 | R-002, R-005, R-006 | IT Team |
| SC-08 | Centralized Logging and Security Monitoring | Detective | V-02, V-03, V-04, V-05 | R-001, R-002, R-003, R-004, R-005, R-007, R-008 | IT Team |
| SC-09 | Phishing Awareness and Staff Security Training | Preventive | V-02 | R-001, R-002 | Hospital Management / IT Team |
| SC-10 | Access Reviews and Account Lifecycle Management | Preventive / Detective | V-05, V-01 | R-004, R-006 | IT Team / Department Heads |
| SC-11 | Incident Response Procedures | Corrective / Recovery | V-01, V-02, V-03, V-04, V-05 | R-001 to R-008 | Hospital Management / IT Team |
| SC-12 | Secure Website Administration and Maintenance | Preventive / Detective | V-03 | R-007 | IT Team / Website Administrator |

---

## 9. Detailed Security Control Recommendations

### 9.1 SC-01: Multi-Factor Authentication

**Control Category:** Preventive

**Related Assets:**
- A-01 Patient Database
- A-03 Email System
- A-04 Hospital Wi-Fi
- A-06 File-Sharing System
- A-05 Public Website

**Related Vulnerabilities:**
- V-01 Weak Password Practices
- V-02 Lack of MFA

**Related Risks:**
- R-001
- R-006
- R-007
- R-008

#### Description

Multi-factor authentication (MFA) requires users to provide more than one form of authentication before accessing an account or system.

It reduces reliance on passwords alone.

For example, a user may enter a password and then confirm their identity using an authenticator application or another approved authentication factor.

#### Recommendations

1. Require MFA for email accounts.
2. Require MFA for administrative and privileged accounts.
3. Enable MFA for access to sensitive systems where supported.
4. Prioritize remote access and accounts that can access patient information.
5. Review MFA enrollment and account recovery procedures.
6. Prefer phishing-resistant authentication methods where technically and operationally feasible.

#### Expected Security Benefit

MFA can reduce the likelihood that stolen passwords alone will result in successful unauthorized account access.

#### Proposed Success Metrics

- Percentage of in-scope accounts protected by MFA.
- Percentage of privileged accounts protected by MFA.
- Number of exceptions documented and approved.
- Results of periodic MFA configuration reviews.

#### Proposed Owner

IT Team.

---

### 9.2 SC-02: Strong Password and Password Management Policy

**Control Category:** Preventive

**Related Assets:**
- A-02 Staff Computers
- A-03 Email System
- A-06 File-Sharing System

**Related Vulnerabilities:**
- V-01 Weak Password Practices
- V-02 Lack of MFA

**Related Risks:**
- R-001
- R-006

#### Description

A password management policy establishes requirements for creating, protecting, and managing user credentials.

Weak or reused passwords may make unauthorized account access easier.

#### Recommendations

1. Establish a documented password policy.
2. Encourage long, unique passwords or passphrases.
3. Prevent the reuse of compromised or commonly known passwords where supported.
4. Discourage password sharing between employees.
5. Use an approved password manager where practical.
6. Change default credentials before systems are placed into service.
7. Establish secure procedures for password resets.
8. Protect privileged credentials with additional safeguards.

#### Expected Security Benefit

Stronger credential management can reduce password-related account compromise and unauthorized access.

#### Proposed Success Metrics

- Approved password policy available.
- Percentage of in-scope accounts reviewed against policy requirements.
- Number of identified default or shared accounts requiring correction.
- Number of password-related incidents reported.

#### Proposed Owner

IT Team.

---

### 9.3 SC-03: Patch and Vulnerability Management

**Control Category:** Preventive / Corrective

**Related Assets:**
- A-01 Patient Database
- A-02 Staff Computers
- A-05 Public Website
- A-06 File-Sharing System

**Related Vulnerability:**
- V-03 Unpatched Systems

**Related Risks:**
- R-002
- R-005
- R-007

#### Description

Patch management is the process of identifying, evaluating, obtaining, testing, and installing updates that address software defects and security vulnerabilities.

Systems that are not updated may remain exposed to known weaknesses.

#### Recommendations

1. Maintain an inventory of operating systems, applications, and software components.
2. Identify available security updates.
3. Prioritize updates according to severity, exposure, and business criticality.
4. Apply security patches through a documented process.
5. Test important updates where practical before wider deployment.
6. Record patch installation dates and exceptions.
7. Review unsupported operating systems and applications.
8. Establish a process for urgent security updates.
9. Verify that critical systems are receiving appropriate updates.

#### Expected Security Benefit

A consistent patch management process can reduce exposure to known software vulnerabilities.

#### Proposed Success Metrics

- Percentage of supported systems covered by patch management.
- Percentage of critical security updates installed within approved timelines.
- Number of overdue critical patches.
- Number of unsupported systems identified.
- Availability of documented patch reports.

#### Proposed Owner

IT Team.

---

### 9.4 SC-04: Network Segmentation and Firewall Restrictions

**Control Category:** Preventive

**Related Assets:**
- A-04 Hospital Wi-Fi
- A-07 Network Infrastructure

**Related Vulnerability:**
- V-04 Poor Network Segmentation

**Related Risks:**
- R-003
- R-008

#### Description

Network segmentation divides a network into separate sections to control communication between systems and reduce unnecessary access.

For a healthcare environment, separation may be appropriate between administrative devices, wireless networks, servers, and sensitive information systems.

#### Recommendations

1. Review the existing network architecture.
2. Separate guest Wi-Fi from internal hospital resources.
3. Restrict access between wireless and sensitive systems.
4. Use firewall rules to allow only required network traffic.
5. Restrict administrative interfaces to authorized management devices or networks.
6. Review network access rules periodically.
7. Document approved network connections.
8. Monitor unusual network traffic where appropriate.

#### Expected Security Benefit

Segmentation can limit unauthorized movement between systems and reduce the potential impact of a compromised device.

#### Proposed Success Metrics

- Approved network segmentation design.
- Number of unnecessary network connections removed.
- Percentage of network access rules reviewed.
- Evidence that guest wireless access is separated from sensitive internal resources.
- Documented network configuration reviews.

#### Proposed Owner

Network Administrator.

---

### 9.5 SC-05: Role-Based Access Control and Least Privilege

**Control Category:** Preventive

**Related Assets:**
- A-01 Patient Database
- A-06 File-Sharing System

**Related Vulnerabilities:**
- V-05 Excessive Privileges
- V-01 Weak Password Practices

**Related Risks:**
- R-004
- R-006

#### Description

Role-Based Access Control (RBAC) assigns permissions according to a user's job responsibilities.

The principle of least privilege means users should receive only the access necessary to perform their authorized duties.

#### Recommendations

1. Define access roles for different job responsibilities.
2. Restrict patient record access to authorized personnel.
3. Separate normal user accounts from administrative accounts.
4. Review access permissions periodically.
5. Remove unnecessary privileges.
6. Disable accounts when employees leave the organization.
7. Review temporary and third-party access.
8. Require approval before granting access to sensitive information.
9. Maintain records of important access changes.

#### Expected Security Benefit

RBAC and least privilege can reduce unauthorized access and limit the potential consequences of compromised or misused accounts.

#### Proposed Success Metrics

- Documented access roles.
- Percentage of sensitive accounts reviewed.
- Number of unnecessary privileges removed.
- Number of inactive accounts disabled.
- Percentage of access requests with documented approval.

#### Proposed Owner

IT Team / Database Administrator.

---

### 9.6 SC-06: Endpoint Protection and Malware Detection

**Control Category:** Preventive / Detective

**Related Assets:**
- A-02 Staff Computers
- A-01 Patient Database
- A-06 File-Sharing System

**Related Vulnerability:**
- V-03 Unpatched Systems

**Related Risks:**
- R-002
- R-005

#### Description

Endpoint protection helps secure computers and other devices against malware, suspicious activity, and unauthorized changes.

Endpoint security should be supported by regular updates, secure configuration, and monitoring.

#### Recommendations

1. Deploy reputable endpoint protection on supported devices.
2. Enable real-time malware protection where available.
3. Keep endpoint security software updated.
4. Restrict unnecessary software installation.
5. Apply secure configuration baselines.
6. Restrict local administrator privileges.
7. Investigate security alerts.
8. Establish procedures for isolating compromised devices.
9. Review endpoint protection coverage periodically.

#### Expected Security Benefit

Endpoint protection can help prevent, detect, and contain malware infections.

#### Proposed Success Metrics

- Percentage of supported endpoints covered by endpoint protection.
- Percentage of endpoint protection agents reporting healthy status.
- Number of unresolved high-priority endpoint alerts.
- Time taken to investigate significant endpoint alerts.
- Availability of endpoint security reports.

#### Proposed Owner

IT Team.

---

### 9.7 SC-07: Secure Backup and Recovery

**Control Category:** Corrective / Recovery

**Related Assets:**
- A-01 Patient Database
- A-02 Staff Computers
- A-06 File-Sharing System

**Related Vulnerabilities:**
- V-03 Unpatched Systems
- V-01 Weak Password Practices

**Related Risks:**
- R-002
- R-005
- R-006

#### Description

Backups provide copies of important information that can be used to restore data after accidental deletion, system failure, corruption, or a cybersecurity incident.

Backups should be protected against unauthorized access and modification.

#### Recommendations

1. Identify critical information requiring backup.
2. Establish a documented backup schedule.
3. Protect backup access using appropriate authentication and permissions.
4. Maintain offline or immutable backup copies where feasible.
5. Separate backup administration from ordinary user accounts.
6. Monitor backup jobs and investigate failures.
7. Test restoration procedures periodically.
8. Document recovery responsibilities.
9. Establish recovery priorities for important systems.

#### Expected Security Benefit

Reliable and protected backups can support recovery after ransomware, data loss, or system disruption.

#### Proposed Success Metrics

- Percentage of critical systems covered by backups.
- Percentage of scheduled backup jobs completed successfully.
- Number of backup failures unresolved.
- Date and result of the latest restoration test.
- Documented recovery procedures for critical assets.

#### Proposed Owner

IT Team.

---

### 9.8 SC-08: Centralized Logging and Security Monitoring

**Control Category:** Detective

**Related Assets:**
- A-01 Patient Database
- A-02 Staff Computers
- A-03 Email System
- A-04 Hospital Wi-Fi
- A-05 Public Website
- A-06 File-Sharing System
- A-07 Network Infrastructure

**Related Vulnerabilities:**
- V-02 Lack of MFA
- V-03 Unpatched Systems
- V-04 Poor Network Segmentation
- V-05 Excessive Privileges

**Related Risks:**
- R-001
- R-002
- R-003
- R-004
- R-005
- R-007
- R-008

#### Description

Security logging records activities performed on systems, applications, and networks.

Security monitoring helps identify suspicious events that may indicate unauthorized access, malware activity, or misuse of information.

#### Recommendations

1. Enable appropriate security logging on important systems.
2. Record authentication successes and failures.
3. Monitor privileged account activities.
4. Monitor important changes to user permissions.
5. Review suspicious access to patient information.
6. Centralize logs where practical.
7. Protect logs against unauthorized modification or deletion.
8. Establish alerting for important security events.
9. Define who is responsible for reviewing alerts.
10. Retain logs according to operational, legal, and privacy requirements.

#### Expected Security Benefit

Logging and monitoring can improve visibility into system activity and support earlier detection and investigation of security incidents.

#### Proposed Success Metrics

- Percentage of critical systems producing relevant security logs.
- Percentage of privileged accounts covered by activity logging.
- Number of unresolved high-priority alerts.
- Time taken to review and escalate significant alerts.
- Availability of documented log review records.

#### Proposed Owner

IT Team.

---

### 9.9 SC-09: Phishing Awareness and Staff Security Training

**Control Category:** Preventive

**Related Assets:**
- A-02 Staff Computers
- A-03 Email System

**Related Vulnerability:**
- V-02 Lack of MFA

**Related Risks:**
- R-001
- R-002

#### Description

Security awareness training helps employees recognize common cybersecurity threats and understand how to respond appropriately.

Phishing remains an important concern because attackers may use deceptive messages to obtain credentials or encourage users to open malicious attachments.

#### Recommendations

1. Provide security awareness training during employee onboarding.
2. Teach employees how to identify suspicious emails.
3. Explain the risks of opening unexpected attachments.
4. Teach staff to verify unusual payment or account requests.
5. Establish a clear method for reporting suspicious messages.
6. Explain why passwords and MFA codes must not be shared.
7. Provide periodic reminders about safe information handling.
8. Conduct controlled phishing awareness exercises only when properly authorized and designed.

#### Expected Security Benefit

Security awareness can reduce unsafe user behavior and improve early reporting of suspicious activity.

#### Proposed Success Metrics

- Percentage of employees completing awareness training.
- Number of employees trained during onboarding.
- Number of suspicious messages reported through the approved process.
- Training assessment results.
- Trends in phishing exercise results, if authorized exercises are conducted.

#### Proposed Owner

Hospital Management / IT Team.

---

### 9.10 SC-10: Access Reviews and Account Lifecycle Management

**Control Category:** Preventive / Detective

**Related Assets:**
- A-01 Patient Database
- A-06 File-Sharing System

**Related Vulnerabilities:**
- V-05 Excessive Privileges
- V-01 Weak Password Practices

**Related Risks:**
- R-004
- R-006

#### Description

Account lifecycle management covers the creation, modification, review, and removal of user accounts.

Regular access reviews help identify accounts that are inactive, unnecessary, or assigned excessive permissions.

#### Recommendations

1. Establish an account creation and approval process.
2. Require authorization before granting access to sensitive information.
3. Review user permissions regularly.
4. Disable accounts promptly when access is no longer required.
5. Remove access when employees change roles.
6. Review third-party and temporary accounts.
7. Maintain an inventory of privileged accounts.
8. Document access reviews and corrective actions.

#### Expected Security Benefit

Account lifecycle management can reduce unnecessary access and help detect permission-related security weaknesses.

#### Proposed Success Metrics

- Percentage of user accounts reviewed each quarter.
- Number of inactive accounts disabled.
- Number of excessive permissions corrected.
- Percentage of access changes with documented approval.
- Percentage of departing employees whose access is removed according to approved procedures.

#### Proposed Owner

IT Team / Department Heads.

---

### 9.11 SC-11: Incident Response Procedures

**Control Category:** Corrective / Recovery

**Related Assets:**
- A-01 Patient Database
- A-02 Staff Computers
- A-03 Email System
- A-04 Hospital Wi-Fi
- A-05 Public Website
- A-06 File-Sharing System
- A-07 Network Infrastructure

**Related Vulnerabilities:**
- V-01
- V-02
- V-03
- V-04
- V-05

**Related Risks:**
- R-001
- R-002
- R-003
- R-004
- R-005
- R-006
- R-007
- R-008

#### Description

Incident response is the organized process of preparing for, identifying, containing, investigating, and recovering from cybersecurity incidents.

A documented response process helps reduce confusion and improve coordination during security events.

#### Recommendations

1. Develop a documented incident response procedure.
2. Assign incident response responsibilities.
3. Establish a process for employees to report suspected incidents.
4. Define incident severity and escalation criteria.
5. Establish procedures for isolating affected devices.
6. Preserve relevant logs and evidence.
7. Define communication and notification responsibilities.
8. Establish recovery and restoration procedures.
9. Document lessons learned after incidents.
10. Review and update the response procedure periodically.

#### Suggested Incident Response Stages

| Stage | Description | Example Activity |
|---|---|---|
| Preparation | Establish the people, processes, and resources needed to respond | Assign responsibilities and prepare response procedures |
| Detection and Analysis | Identify and assess suspicious activity | Review alerts, logs, and reported incidents |
| Containment | Limit the spread or impact of an incident | Isolate a suspected compromised endpoint |
| Eradication | Remove the cause of the incident | Remove malware and address the exploited weakness |
| Recovery | Restore affected systems and services | Restore clean backups and verify system operation |
| Lessons Learned | Review the incident and improve security | Document findings and update controls |

#### Expected Security Benefit

Incident response procedures can improve containment, reduce operational disruption, and support recovery.

#### Proposed Success Metrics

- Approved incident response procedure.
- Assigned incident response responsibilities.
- Percentage of relevant staff aware of reporting procedures.
- Results of periodic tabletop exercises.
- Number of corrective actions completed after exercises or incidents.

#### Proposed Owner

Hospital Management / IT Team.

---

### 9.12 SC-12: Secure Website Administration and Maintenance

**Control Category:** Preventive / Detective

**Related Asset:**
- A-05 Public Website

**Related Vulnerability:**
- V-03 Unpatched Systems

**Related Risk:**
- R-007

#### Description

A public website may be exposed to internet-based threats.

Secure website administration and maintenance help reduce the likelihood of unauthorized changes, exploitation of outdated components, and service disruption.

#### Recommendations

1. Keep the website platform and components updated.
2. Protect administrator accounts with MFA.
3. Use unique administrative credentials.
4. Restrict administrative access to authorized personnel.
5. Remove unused plugins, themes, and components.
6. Use HTTPS with valid TLS configuration.
7. Maintain website backups.
8. Monitor important website changes.
9. Review website permissions and administrative accounts.
10. Establish a process for responding to website security alerts.

#### Expected Security Benefit

These controls can reduce the likelihood of website compromise and support detection and recovery if an incident occurs.

#### Proposed Success Metrics

- Percentage of website components receiving supported security updates.
- Number of unnecessary plugins or components removed.
- Percentage of administrator accounts protected by MFA.
- Availability of current website backups.
- Documented website security reviews.

#### Proposed Owner

IT Team / Website Administrator.

---

## 10. Control Mapping to Security Principles

The controls support different elements of the CIA triad.

| Control ID | Security Control | Confidentiality | Integrity | Availability |
|---|---|---|---|---|
| SC-01 | Multi-Factor Authentication | Yes | Yes | Yes |
| SC-02 | Password Management | Yes | Yes | Yes |
| SC-03 | Patch Management | Yes | Yes | Yes |
| SC-04 | Network Segmentation | Yes | Yes | Yes |
| SC-05 | Role-Based Access Control | Yes | Yes | Yes |
| SC-06 | Endpoint Protection | Yes | Yes | Yes |
| SC-07 | Backup and Recovery | Yes | Yes | Yes |
| SC-08 | Logging and Monitoring | Yes | Yes | Yes |
| SC-09 | Security Awareness Training | Yes | Yes | Yes |
| SC-10 | Access Reviews | Yes | Yes | Yes |
| SC-11 | Incident Response | Yes | Yes | Yes |
| SC-12 | Website Security | Yes | Yes | Yes |

The CIA mappings indicate potential support for the security principles. They do not mean every control provides equal protection across all three principles.

---

## 11. Control Mapping to NIST CSF 2.0

The following mapping shows how the proposed controls relate to the six NIST Cybersecurity Framework 2.0 functions.

| Control ID | Security Control | Govern | Identify | Protect | Detect | Respond | Recover |
|---|---|---|---|---|---|---|---|
| SC-01 | Multi-Factor Authentication |  |  | Yes |  |  |  |
| SC-02 | Password Management |  |  | Yes |  |  |  |
| SC-03 | Patch Management |  | Yes | Yes |  |  |  |
| SC-04 | Network Segmentation |  | Yes | Yes |  |  |  |
| SC-05 | Role-Based Access Control | Yes |  | Yes |  |  |  |
| SC-06 | Endpoint Protection |  |  | Yes | Yes |  |  |
| SC-07 | Backup and Recovery |  |  |  |  |  | Yes |
| SC-08 | Logging and Monitoring |  |  |  | Yes |  |  |
| SC-09 | Security Awareness Training | Yes |  | Yes |  |  |  |
| SC-10 | Access Reviews | Yes | Yes | Yes | Yes |  |  |
| SC-11 | Incident Response | Yes |  |  | Yes | Yes | Yes |
| SC-12 | Website Security |  | Yes | Yes | Yes |  |  |

This is a high-level educational mapping to the NIST CSF 2.0 functions, not a complete CSF implementation assessment or claim of compliance.

---

## 12. Recommended Implementation Priorities

Not all controls need to be implemented at the same time.

The proposed order considers the inherent risk ratings and the importance of protecting critical healthcare information.

| Priority | Control IDs | Recommended Focus | Reason |
|---|---|---|---|
| Critical | SC-01, SC-02, SC-09 | Account protection and phishing risk reduction | Addresses R-001, the highest-rated risk |
| High | SC-03, SC-05, SC-06, SC-07 | Patch management, access control, endpoint protection, and recovery | Addresses patient information, malware, and unauthorized access risks |
| High | SC-04, SC-08, SC-10, SC-11 | Network security, monitoring, account reviews, and incident response | Reduces attack movement and improves detection and response |
| Medium | SC-12 | Public website security | Addresses R-007 |

These are proposed priorities. Actual scheduling should consider system dependencies, available resources, operational requirements, and risk ownership.

---

## 13. Control Ownership and Accountability

Clear ownership helps ensure that security controls are implemented, maintained, and reviewed.

| Role | Responsibility |
|---|---|
| Hospital Management | Approve security policies, support implementation, and oversee risk treatment |
| IT Team | Coordinate account security, patch management, endpoint protection, backups, and monitoring |
| Network Administrator | Manage network segmentation, firewall rules, wireless security, and network monitoring |
| Database Administrator | Support patient database access controls, database maintenance, and recovery |
| Website Administrator | Maintain website security, administrative access, and updates |
| Department Heads | Review staff access and support security awareness |
| All Employees | Follow security procedures, protect credentials, and report suspicious activities |

The roles are proposed for the fictional organization and have not been verified as actual appointments.

---

## 14. Control Monitoring and Review

Security controls should be reviewed periodically to confirm that they remain appropriate and effective.

### 14.1 Recommended Review Schedule

| Control Area | Recommended Review Frequency | Responsible Role |
|---|---|---|
| MFA coverage | Monthly | IT Team |
| Password policy | Annually and after significant security changes | IT Team |
| Patch management | Monthly | IT Team |
| Network segmentation | Quarterly and after network changes | Network Administrator |
| User access permissions | Quarterly | IT Team / Department Heads |
| Endpoint protection | Monthly | IT Team |
| Backup status | Daily | IT Team |
| Backup restoration | Quarterly | IT Team |
| Security logs and alerts | Daily or continuously where supported | IT Team |
| Staff awareness | At onboarding and periodically | Hospital Management / IT Team |
| Account lifecycle | Monthly | IT Team |
| Incident response procedures | Annually and after significant incidents | Hospital Management / IT Team |
| Website security | Monthly and after significant changes | Website Administrator |

These frequencies are recommendations for the fictional scenario. A real organization should define review intervals based on its risk exposure and operational requirements.

### 14.2 Events Requiring Control Review

Controls should be reviewed when:

- A cybersecurity incident occurs.
- A new system or application is introduced.
- A critical vulnerability is identified.
- A major network change takes place.
- An employee changes roles or leaves the organization.
- A security control fails.
- A new external service provider is introduced.
- Applicable legal or regulatory requirements change.

---

## 15. Evidence Required to Verify Controls

A control should not be considered effective simply because it has been recommended or documented.

Evidence should be collected to confirm implementation and operation.

| Control ID | Evidence That Could Be Collected |
|---|---|
| SC-01 | MFA configuration records and account coverage reports |
| SC-02 | Approved password policy and account security review records |
| SC-03 | Patch reports, update records, and documented exceptions |
| SC-04 | Network diagrams, firewall rules, and segmentation review records |
| SC-05 | Approved access roles and permission review records |
| SC-06 | Endpoint protection reports and security alert records |
| SC-07 | Backup logs and successful restoration test records |
| SC-08 | Security log samples, monitoring configuration, and alert review records |
| SC-09 | Training materials, attendance records, and assessment results |
| SC-10 | Account inventory, access review records, and account removal records |
| SC-11 | Approved incident response procedure and exercise reports |
| SC-12 | Website update records, administrator access reviews, and backup records |

Any screenshots or evidence added to this portfolio should be genuine and should not expose passwords, patient information, private network details, or other sensitive data.

---

## 16. Relationship to Residual Risk

The recommended controls are intended to reduce the likelihood or impact of the eight risks recorded in `risk-register.md`.

The residual risk values below are projections from the risk register, not verified outcomes.

| Risk ID | Main Recommended Controls | Inherent Score | Projected Residual Score | Projected Residual Rating |
|---|---|---:|---:|---|
| R-001 | SC-01, SC-02, SC-08, SC-09, SC-11 | 25 | 10 | High |
| R-002 | SC-03, SC-06, SC-07, SC-08, SC-11 | 15 | 6 | Medium |
| R-003 | SC-04, SC-08, SC-11 | 12 | 8 | Medium |
| R-004 | SC-05, SC-08, SC-10, SC-11 | 15 | 10 | High |
| R-005 | SC-03, SC-06, SC-07, SC-08, SC-11 | 12 | 6 | Medium |
| R-006 | SC-01, SC-02, SC-05, SC-07, SC-10 | 16 | 8 | Medium |
| R-007 | SC-01, SC-03, SC-08, SC-11, SC-12 | 9 | 6 | Medium |
| R-008 | SC-01, SC-04, SC-08, SC-11 | 12 | 8 | Medium |

### 16.1 Residual Risk Considerations

Even after controls are implemented, some risks may remain.

For example:

- MFA reduces the risk of password-only account compromise but does not eliminate every account takeover technique.
- Access restrictions reduce unnecessary access but cannot guarantee that an authorized user will never misuse information.
- Backups support recovery but do not prevent every ransomware incident.
- Network segmentation limits movement but does not eliminate all network threats.
- Security monitoring improves visibility but depends on correct configuration, review, and response.

Residual risks should be reassessed using actual evidence after implementation.

---

## 17. Assumptions and Limitations

This document has the following limitations:

1. GreenCare Community Hospital is fictional.
2. The identified vulnerabilities are hypothetical.
3. The proposed controls have not been deployed.
4. No system configurations were inspected.
5. No network security tests were performed.
6. No MFA deployment was verified.
7. No endpoint protection deployment was verified.
8. No backup restoration test was performed.
9. No security monitoring platform was inspected.
10. Control effectiveness has not been measured.
11. The control owners are proposed roles, not confirmed appointments.
12. The recommendations do not constitute a formal security audit or compliance certification.

The purpose is to demonstrate how security controls can be selected and mapped to identified cybersecurity risks.

---

## 18. Conclusion

Security controls are an important part of cybersecurity risk management.

This document proposes twelve controls to address the vulnerabilities and risks identified in the fictional GreenCare Community Hospital assessment.

The recommendations cover identity and access management, password security, patch management, network segmentation, endpoint protection, backup and recovery, security monitoring, staff awareness, account reviews, incident response, and website security.

The controls are mapped to the existing risk register to maintain consistency across the project documentation.

The next step is to convert these recommendations into a practical remediation plan with assigned owners, priorities, proposed timelines, implementation status, and measurable success criteria.

All recommendations remain proposed until implementation and verification evidence is available.

---

## 19. Related Project Documents

| File | Purpose |
|---|---|
| `README.md` | Project overview and repository navigation |
| `docs/risk-assessment-report.md` | Main cybersecurity risk assessment report |
| `docs/asset-inventory.md` | Identified information assets and classifications |
| `docs/threat-assessment.md` | Threat actors, threats, and attack scenarios |
| `docs/vulnerability-assessment.md` | Identified vulnerabilities and control gaps |
| `docs/risk-register.md` | Risk scores, ratings, treatment, and residual risk |
| `docs/remediation-plan.md` | Proposed implementation activities and timelines |
| `references/references.md` | Supporting frameworks and reference materials |

---

## 20. References

### NIST Cybersecurity Framework 2.0

**Organization:** National Institute of Standards and Technology (NIST)

**URL:** https://nvlpubs.nist.gov/nistpubs/CSWP/NIST.CSWP.29.pdf

**Application:** Used as a reference for organizing security recommendations around Govern, Identify, Protect, Detect, Respond, and Recover.

### NIST Special Publication 800-30 Revision 1

**Title:** Guide for Conducting Risk Assessments

**Organization:** National Institute of Standards and Technology (NIST)

**URL:** https://csrc.nist.gov/pubs/sp/800/30/r1/final

**Application:** Informed the risk-based approach used to connect threats, vulnerabilities, likelihood, impact, and risk treatment.

### Nigeria Data Protection Commission

**Organization:** Nigeria Data Protection Commission (NDPC)

**URL:** https://ndpc.gov.ng/

**Application:** Provides a reference point for considering personal data protection obligations in the assumed Nigerian healthcare context.

> These references inform the educational recommendations. Their inclusion does not establish that the fictional organization complies with any framework or legislation.

---

**End of Document**