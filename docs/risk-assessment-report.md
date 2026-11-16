# Cybersecurity Risk Assessment Report

## 1. Document Information

| Field | Details |
|---|---|
| Document Title | Cybersecurity Risk Assessment Report |
| Organization | GreenCare Community Hospital |
| Organization Type | Fictional community healthcare facility |
| Estimated Organization Size | Approximately 35 employees |
| Assumed Jurisdiction | Nigeria |
| Document Version | 2.0 |
| Assessment Type | Hypothetical, educational cybersecurity risk assessment |
| Assessment Status | Documentation and analysis exercise |
| Prepared By | Cybersecurity Portfolio Project |
| Assessment Date | November 2026 |
| Review Status | Proposed for review |

> **Important:** GreenCare Community Hospital is a fictional organization created for this educational portfolio project. This report does not represent an assessment of a real hospital, actual network, production environment, or patient database. No live systems were scanned, accessed, tested, or audited. Findings and risk scores are hypothetical estimates based on the project scenario.

---

## 2. Executive Summary

This report presents a hypothetical cybersecurity risk assessment for GreenCare Community Hospital, a fictional healthcare organization with approximately 35 employees.

Healthcare organizations depend on information systems to support patient care, administrative operations, communication, and record management. These systems may process sensitive patient information and support activities where confidentiality, integrity, and availability are important.

The purpose of this assessment is to identify potential information assets, examine relevant threat actors, identify possible threats and vulnerabilities, evaluate realistic attack scenarios, and recommend security controls to reduce cybersecurity risks.

The assessment identified seven key information assets, five threat categories, and five vulnerability areas. These were used to develop eight hypothetical risk scenarios in a centralized risk register.

### Key assessment results

| Assessment Area | Result |
|---|---:|
| Identified Information Assets | 7 |
| Identified Threat Categories | 5 |
| Identified Vulnerabilities | 5 |
| Documented Risk Scenarios | 8 |
| Critical Inherent Risks | 1 |
| High Inherent Risks | 6 |
| Medium Inherent Risks | 1 |
| Low Inherent Risks | 0 |

The highest-rated hypothetical risk is phishing and email account compromise, with an inherent risk score of 25 (Critical). Other significant risks include ransomware affecting patient records, insider misuse of patient information, poor network segmentation, and weak password practices.

The assessment recommends strengthening identity and access management, implementing multi-factor authentication, improving patch management, reviewing user privileges, strengthening network segmentation, improving backup and recovery arrangements, and establishing security monitoring and incident response procedures.

The proposed controls have not been implemented or tested as part of this project. Residual risk values are projected estimates that assume the recommended controls are implemented effectively.

---

## 3. Introduction

Cybersecurity is important in healthcare because information systems support the storage, processing, transmission, and availability of sensitive information.

A security incident affecting a healthcare organization may result in:

- Unauthorized access to patient information.
- Exposure or theft of sensitive records.
- Disruption of hospital operations.
- Loss or corruption of important data.
- Financial and reputational damage.
- Delays in accessing information needed for healthcare services.

This assessment uses a fictional hospital environment to demonstrate how cybersecurity risks can be identified, analyzed, documented, prioritized, and treated.

The project follows a structured risk assessment approach informed by NIST guidance, particularly NIST Special Publication 800-30 Revision 1 and the NIST Cybersecurity Framework 2.0.

The numerical scoring system used in this project is a tailored educational model. It is not presented as a scoring scale prescribed by NIST.

---

## 4. Assessment Objectives

The main objectives are to:

1. Identify important information assets within the fictional hospital.
2. Identify potential threat actors and cybersecurity threats.
3. Identify vulnerabilities and security control gaps.
4. Develop realistic hypothetical attack scenarios.
5. Assess the likelihood and potential impact of each scenario.
6. Calculate and prioritize inherent cybersecurity risks.
7. Recommend appropriate security controls.
8. Propose risk treatment options.
9. Estimate residual risks after proposed controls.
10. Develop recommendations for remediation and continuous monitoring.

---

## 5. Assessment Scope

### 5.1 In-Scope Assets

The assessment considers the following fictional hospital assets:

| Asset ID | Asset Name | Criticality |
|---|---|---|
| A-01 | Patient Database | Critical |
| A-02 | Staff Computers | High |
| A-03 | Email System | High |
| A-04 | Hospital Wi-Fi | High |
| A-05 | Public Website | Medium |
| A-06 | File-Sharing System | High |
| A-07 | Network Infrastructure | High |

### 5.2 In-Scope Security Areas

The assessment considers:

- Patient information protection.
- User authentication and account security.
- Password management.
- Multi-factor authentication.
- Endpoint security.
- Software updates and patch management.
- Network segmentation.
- User access privileges.
- File storage and sharing.
- Backup and recovery.
- Security monitoring.
- Incident response.

### 5.3 Out of Scope

The following activities were not performed:

- Live network scanning.
- Vulnerability scanning against real systems.
- Penetration testing.
- Exploitation of vulnerabilities.
- Access to actual patient records.
- Inspection of real hospital infrastructure.
- Verification of deployed security controls.
- Formal regulatory compliance auditing.
- Interviews with actual hospital employees.

All scenarios and findings are hypothetical.

---

## 6. Assessment Methodology

The assessment follows a structured process informed by NIST SP 800-30 Rev. 1.

The process connects information assets to threats, vulnerabilities, attack scenarios, likelihood, impact, risk ratings, security controls, and treatment recommendations.

### 6.1 Assessment Workflow

| Step | Assessment Activity | Purpose |
|---|---|---|
| 1 | Asset Identification | Identify important information assets |
| 2 | Threat Identification | Identify potential cybersecurity threats |
| 3 | Threat Actor Analysis | Identify possible individuals or groups behind threats |
| 4 | Vulnerability Analysis | Identify weaknesses and security control gaps |
| 5 | Attack Scenario Development | Describe how threats could exploit vulnerabilities |
| 6 | Likelihood Assessment | Estimate how likely each scenario could occur |
| 7 | Impact Assessment | Estimate the potential consequences |
| 8 | Risk Calculation | Calculate risk scores |
| 9 | Risk Register Development | Record and prioritize identified risks |
| 10 | Security Control Recommendations | Identify safeguards to reduce risks |
| 11 | Risk Treatment | Recommend appropriate treatment options |
| 12 | Residual Risk Assessment | Estimate remaining risks after proposed controls |
| 13 | Remediation Planning | Assign owners, priorities, timelines, and success metrics |
| 14 | Continuous Monitoring | Recommend ongoing review and improvement |

### 6.2 Risk Assessment Terminology

The following terms are used throughout this report:

| Term | Meaning |
|---|---|
| Asset | Something valuable to the organization that requires protection |
| Threat | A potential event or action that could cause harm |
| Threat Actor | An individual or group capable of carrying out a threat |
| Vulnerability | A weakness that could be exploited |
| Control Gap | A missing, inadequate, or ineffective security safeguard |
| Attack Scenario | A description of how a threat could exploit a vulnerability and affect an asset |
| Risk | The possibility of harm resulting from a threat exploiting a vulnerability |
| Security Control | A safeguard designed to prevent, detect, or reduce security incidents |
| Inherent Risk | The estimated risk before considering additional recommended controls |
| Residual Risk | The estimated risk remaining after controls are implemented and operating effectively |

---

## 7. Asset Identification and Classification

Seven information assets were identified for the fictional hospital scenario.

The assets were classified according to their importance and the potential consequences of losing confidentiality, integrity, or availability.

### 7.1 Asset Inventory Summary

| Asset ID | Asset Name | Data or Information Handled | Owner | Criticality |
|---|---|---|---|---|
| A-01 | Patient Database | Patient records, medical histories, and sensitive healthcare information | Health Information Management / IT Team | Critical |
| A-02 | Staff Computers | Work documents, credentials, and locally accessed information | IT Team | High |
| A-03 | Email System | Messages, attachments, and organizational communications | IT Team | High |
| A-04 | Hospital Wi-Fi | Network authentication information and wireless traffic | Network Administrator | High |
| A-05 | Public Website | Public hospital information and services | IT Team / Communications | Medium |
| A-06 | File-Sharing System | Internal documents and organizational files | IT Team | High |
| A-07 | Network Infrastructure | Network configurations, traffic information, and access rules | Network Administrator | High |

### 7.2 CIA Triad Considerations

The assessment uses the Confidentiality, Integrity, and Availability (CIA) triad.

| Security Principle | Meaning | Healthcare Example |
|---|---|---|
| Confidentiality | Information is accessible only to authorized individuals | Preventing unauthorized access to patient records |
| Integrity | Information remains accurate and is not improperly modified | Preventing unauthorized changes to patient medical records |
| Availability | Information and systems remain accessible when needed | Ensuring authorized staff can access patient information when required |

The patient database is considered critical because unauthorized disclosure, alteration, or unavailability could have serious consequences.

The complete asset details, ownership, dependencies, and CIA classifications are documented in `asset-inventory.md`.

---

## 8. Threat Actor Analysis

Threat actors are individuals or groups that may intentionally or unintentionally cause harm to an organization's systems or information.

Five hypothetical threat actor categories were identified.

### 8.1 Identified Threat Actors

| Threat Actor ID | Threat Actor | Description | Potential Motivation |
|---|---|---|---|
| TA-01 | Cybercriminals | Individuals or groups seeking unauthorized access to systems or information | Financial gain, data theft, fraud |
| TA-02 | Ransomware Operators | Attackers who deploy ransomware to disrupt systems or demand payment | Extortion and financial gain |
| TA-03 | Malicious Insiders | Employees or trusted individuals who intentionally misuse authorized access | Personal benefit, revenge, data theft |
| TA-04 | Hacktivists | Individuals or groups targeting organizations for ideological or political reasons | Publicity, disruption, protest |
| TA-05 | Compromised Users | Legitimate users whose accounts or devices have been taken over | May be exploited by external attackers |

### 8.2 Threat Actor Considerations

The assessment considers that:

- Cybercriminals could use phishing to steal employee credentials.
- Ransomware operators could exploit weak security practices to disrupt access to important files.
- Malicious insiders could misuse legitimate access to view or disclose patient information.
- Hacktivists could target publicly accessible services or organizational infrastructure.
- Compromised users could unintentionally provide attackers with access to internal resources.

These are possible scenarios, not confirmed incidents involving the fictional organization.

---

## 9. Threat Identification

Five main threat categories were identified.

### 9.1 Threat Register Summary

| Threat ID | Threat Name | Description | Potentially Affected Assets |
|---|---|---|---|
| T-01 | Phishing | Deceptive messages designed to trick users into revealing credentials or opening malicious content | A-02, A-03, A-06 |
| T-02 | Malware Infection | Malicious software that may compromise devices, disrupt operations, or steal information | A-02, A-05, A-07 |
| T-03 | Ransomware Attack | Malicious software that may encrypt or otherwise deny access to important information | A-01, A-02, A-06 |
| T-04 | Credential Compromise | Unauthorized access resulting from stolen, exposed, or misused login credentials | A-01, A-03, A-04, A-06 |
| T-05 | Insider Threat | Misuse of authorized access by an employee or trusted individual | A-01, A-06 |

### 9.2 Threat-to-Actor Mapping

| Threat ID | Threat | Potential Threat Actors |
|---|---|---|
| T-01 | Phishing | TA-01, TA-02 |
| T-02 | Malware Infection | TA-01, TA-02, TA-04 |
| T-03 | Ransomware Attack | TA-02 |
| T-04 | Credential Compromise | TA-01, TA-02, TA-05 |
| T-05 | Insider Threat | TA-03 |

Threat actor and threat analysis is documented in `threat-assessment.md`.

---

## 10. Vulnerability and Control Gap Assessment

The assessment identified five hypothetical vulnerability areas that could increase the hospital's exposure to cybersecurity threats.

These are potential weaknesses in the fictional scenario. They have not been confirmed through technical testing.

### 10.1 Identified Vulnerabilities

| Vulnerability ID | Vulnerability | Description | Related Assets |
|---|---|---|---|
| V-01 | Weak Password Practices | Weak, reused, or poorly managed passwords may increase the likelihood of account compromise | A-02, A-03, A-06 |
| V-02 | Lack of MFA | Accounts without multi-factor authentication may be more vulnerable to unauthorized access following credential theft | A-01, A-03, A-06 |
| V-03 | Unpatched Systems | Outdated operating systems, applications, or components may contain known security weaknesses | A-02, A-05, A-06 |
| V-04 | Poor Network Segmentation | Insufficient separation between network environments may allow unauthorized movement between systems | A-04, A-07 |
| V-05 | Excessive Privileges | Users may have more access than necessary for their responsibilities | A-01, A-06 |

### 10.2 Vulnerability Assessment Considerations

The potential consequences include:

- Unauthorized account access.
- Increased exposure to phishing and credential theft.
- Exploitation of known software weaknesses.
- Lateral movement between network resources.
- Unauthorized access to sensitive patient information.
- Increased impact of malicious insider activity.

### 10.3 Important Assessment Limitation

No vulnerability scanner, penetration testing tool, or configuration review was used against a real environment.

The vulnerabilities are scenario assumptions used to demonstrate risk assessment methodology.

The detailed analysis is available in `vulnerability-assessment.md`.

---

## 11. Attack Scenario Analysis

Attack scenarios describe how a threat actor could exploit a vulnerability or control gap and affect an information asset.

Five hypothetical scenarios were developed.

### 11.1 Scenario 1: Phishing and Email Account Compromise

| Field | Details |
|---|---|
| Scenario ID | AS-01 |
| Related Risk ID | R-001 |
| Threat Actor | TA-01 Cybercriminals |
| Threat | T-01 Phishing |
| Related Vulnerability | V-02 Lack of MFA |
| Primary Asset | A-03 Email System |
| Attack Description | An employee receives a deceptive email and enters their credentials into a fraudulent login page. An attacker may then use the stolen credentials to access the employee's email account. |
| Potential Impact | Unauthorized access to organizational communications, exposure of sensitive information, and possible further compromise of internal accounts. |
| Recommended Controls | MFA, email security, phishing awareness training, account monitoring, and incident response procedures. |

### 11.2 Scenario 2: Ransomware Infection

| Field | Details |
|---|---|
| Scenario ID | AS-02 |
| Related Risk ID | R-002 |
| Threat Actor | TA-02 Ransomware Operators |
| Threat | T-03 Ransomware Attack |
| Related Vulnerability | V-03 Unpatched Systems |
| Primary Asset | A-01 Patient Database |
| Attack Description | An attacker exploits an outdated system or another security weakness to introduce ransomware into the environment. The attack could affect access to patient records and connected resources. |
| Potential Impact | Disruption of access to patient information, operational delays, data recovery costs, and possible data exposure. |
| Recommended Controls | Patch management, endpoint protection, network segmentation, secure backups, and incident response planning. |

### 11.3 Scenario 3: Unauthorized Access Through Poor Network Segmentation

| Field | Details |
|---|---|
| Scenario ID | AS-03 |
| Related Risk ID | R-003 |
| Threat Actor | TA-01 Cybercriminals |
| Threat | T-02 Malware Infection / T-04 Credential Compromise |
| Related Vulnerability | V-04 Poor Network Segmentation |
| Primary Asset | A-07 Network Infrastructure |
| Attack Description | An attacker gains access to one part of the hospital network and takes advantage of insufficient network separation to reach additional resources. |
| Potential Impact | Unauthorized access to internal systems, wider malware distribution, and increased exposure of sensitive information. |
| Recommended Controls | Network segmentation, firewall rules, access restrictions, network monitoring, and secure configuration management. |

### 11.4 Scenario 4: Insider Misuse of Patient Information

| Field | Details |
|---|---|
| Scenario ID | AS-04 |
| Related Risk ID | R-004 |
| Threat Actor | TA-03 Malicious Insiders |
| Threat | T-05 Insider Threat |
| Related Vulnerability | V-05 Excessive Privileges |
| Primary Asset | A-01 Patient Database |
| Attack Description | An employee with excessive access privileges views, copies, changes, or discloses patient information without an authorized business or healthcare purpose. |
| Potential Impact | Privacy violations, unauthorized disclosure of sensitive information, reputational damage, and possible legal or regulatory consequences. |
| Recommended Controls | Least-privilege access, role-based access control, access reviews, audit logging, and appropriate staff procedures. |

### 11.5 Scenario 5: Public Website Compromise

| Field | Details |
|---|---|
| Scenario ID | AS-05 |
| Related Risk ID | R-007 |
| Threat Actor | TA-01 Cybercriminals / TA-04 Hacktivists |
| Threat | T-02 Malware Infection / T-04 Credential Compromise |
| Related Vulnerability | V-03 Unpatched Systems |
| Primary Asset | A-05 Public Website |
| Attack Description | An attacker exploits an outdated website component or compromises an administrative account to modify or disrupt the public website. |
| Potential Impact | Website defacement, service disruption, reputational damage, or unauthorized access to website administration. |
| Recommended Controls | Timely patching, secure administration, MFA, web application protection, and website monitoring. |

---

## 12. Risk Assessment Methodology

Risk is evaluated using two factors:

- Likelihood: How likely a hypothetical threat scenario is to occur.
- Impact: How serious the consequences could be if the scenario occurs.

### 12.1 Likelihood Scale

| Score | Rating | Description |
|---|---|---|
| 1 | Rare | Very unlikely |
| 2 | Unlikely | Could occur but is not expected |
| 3 | Possible | Could reasonably occur |
| 4 | Likely | Expected to occur |
| 5 | Almost Certain | Very likely to occur |

### 12.2 Impact Scale

| Score | Rating | Description |
|---|---|---|
| 1 | Negligible | Minimal impact |
| 2 | Minor | Limited impact |
| 3 | Moderate | Noticeable operational or security impact |
| 4 | Major | Significant operational or security impact |
| 5 | Severe | Critical organizational impact |

### 12.3 Risk Calculation

The project uses the following formula:

**Risk Score = Likelihood × Impact**

For example:

If the likelihood of a scenario is rated 5 and its impact is rated 5:

Risk Score = 5 × 5 = 25

The resulting score is classified as Critical.

### 12.4 Risk Rating Bands

| Risk Score | Risk Rating |
|---|---|
| 1–4 | Low |
| 5–9 | Medium |
| 10–16 | High |
| 17–25 | Critical |

### 12.5 Risk Matrix

| Likelihood / Impact | 1 - Negligible | 2 - Minor | 3 - Moderate | 4 - Major | 5 - Severe |
|---|---:|---:|---:|---:|---:|
| 5 - Almost Certain | 5 Medium | 10 High | 15 High | 20 Critical | 25 Critical |
| 4 - Likely | 4 Low | 8 Medium | 12 High | 16 High | 20 Critical |
| 3 - Possible | 3 Low | 6 Medium | 9 Medium | 12 High | 15 High |
| 2 - Unlikely | 2 Low | 4 Low | 6 Medium | 8 Medium | 10 High |
| 1 - Rare | 1 Low | 2 Low | 3 Low | 4 Low | 5 Medium |

> The likelihood and impact values are hypothetical estimates for this educational scenario. They are not based on measured incident frequency or verified technical findings.

---

## 13. Risk Register Summary

Eight hypothetical risk scenarios were evaluated and recorded.

### 13.1 Inherent Risk Register

| Risk ID | Asset | Threat | Vulnerability | Risk Scenario | Likelihood | Impact | Score | Rating | Treatment |
|---|---|---|---|---|---:|---:|---:|---|---|
| R-001 | A-03 Email System | T-01 / T-04 | V-02 | Phishing and email account compromise | 5 | 5 | 25 | Critical | Mitigate |
| R-002 | A-01 Patient Database | T-03 | V-03 | Ransomware affecting patient records | 3 | 5 | 15 | High | Mitigate |
| R-003 | A-07 Network Infrastructure | T-02 / T-04 | V-04 | Unauthorized network access and lateral movement | 3 | 4 | 12 | High | Mitigate |
| R-004 | A-01 Patient Database | T-05 | V-05 | Insider misuse of patient information | 3 | 5 | 15 | High | Mitigate |
| R-005 | A-02 Staff Computers | T-02 | V-03 | Malware exploitation of unpatched endpoints | 3 | 4 | 12 | High | Mitigate |
| R-006 | A-06 File-Sharing System | T-04 | V-01 | Unauthorized file access through weak or reused passwords | 4 | 4 | 16 | High | Mitigate |
| R-007 | A-05 Public Website | T-02 / T-04 | V-03 | Public website compromise | 3 | 3 | 9 | Medium | Mitigate |
| R-008 | A-04 Hospital Wi-Fi | T-02 / T-04 | V-04 | Unauthorized wireless access and movement into internal resources | 3 | 4 | 12 | High | Mitigate |

### 13.2 Risk Distribution

| Risk Rating | Number of Risks |
|---|---:|
| Critical | 1 |
| High | 6 |
| Medium | 1 |
| Low | 0 |
| **Total** | **8** |

### 13.3 Risk Prioritization

The risks are prioritized according to their calculated inherent risk scores.

| Priority | Risk ID | Risk Scenario | Score | Rating |
|---|---|---|---:|---|
| 1 | R-001 | Phishing and email account compromise | 25 | Critical |
| 2 | R-006 | Unauthorized file access through weak passwords | 16 | High |
| 3 | R-002 | Ransomware affecting patient records | 15 | High |
| 4 | R-004 | Insider misuse of patient information | 15 | High |
| 5 | R-003 | Unauthorized network access and lateral movement | 12 | High |
| 6 | R-005 | Malware exploitation of unpatched endpoints | 12 | High |
| 7 | R-008 | Unauthorized wireless access | 12 | High |
| 8 | R-007 | Public website compromise | 9 | Medium |

The highest priority should be given to R-001 because of its Critical rating and potential to provide an attacker with access to organizational communications and additional resources.

R-002 and R-004 also require strong attention because they involve the patient database, which is classified as a critical asset.

---

## 14. Recommended Security Controls

The following controls are proposed to reduce the identified risks.

They are recommendations, not confirmed existing controls.

### 14.1 Control Recommendations

| Control ID | Recommended Security Control | Control Type | Related Risks | Purpose |
|---|---|---|---|---|
| SC-01 | Multi-factor authentication | Preventive | R-001, R-006, R-007, R-008 | Reduce unauthorized access resulting from stolen credentials |
| SC-02 | Strong password and password management policy | Preventive | R-001, R-006 | Reduce password-related account compromise |
| SC-03 | Regular patch and vulnerability management | Preventive | R-002, R-005, R-007 | Reduce exposure to known software weaknesses |
| SC-04 | Network segmentation and firewall restrictions | Preventive | R-003, R-008 | Limit unauthorized movement between network environments |
| SC-05 | Role-based access control and least privilege | Preventive | R-004, R-006 | Restrict access to information according to job responsibilities |
| SC-06 | Endpoint protection and malware detection | Preventive / Detective | R-002, R-005 | Reduce and detect malicious software activity |
| SC-07 | Secure, tested, and isolated backups | Corrective / Recovery | R-002, R-005, R-006 | Support restoration after data loss or ransomware incidents |
| SC-08 | Centralized logging and security monitoring | Detective | R-001, R-003, R-004, R-007, R-008 | Identify suspicious activity and support investigations |
| SC-09 | Phishing awareness and staff security training | Preventive | R-001, R-002 | Improve employee awareness of common attack techniques |
| SC-10 | Access reviews and account lifecycle management | Preventive / Detective | R-004, R-006 | Identify excessive privileges and remove unnecessary access |
| SC-11 | Incident response procedures | Corrective | R-001, R-002, R-003, R-004, R-005, R-007, R-008 | Improve response and containment during security incidents |
| SC-12 | Secure website administration and maintenance | Preventive / Detective | R-007 | Reduce website compromise risks |

### 14.2 Control Implementation Principles

Recommended controls should be implemented according to risk priority and operational requirements.

Important principles include:

- Apply least privilege to user accounts.
- Require MFA for important systems and remote access where supported.
- Remove unnecessary or inactive accounts.
- Apply security updates through a documented patch management process.
- Separate wireless, administrative, and sensitive system environments where appropriate.
- Maintain protected backups and test restoration procedures.
- Monitor important systems and investigate suspicious activity.
- Train employees to recognize phishing and report suspicious messages.
- Document incident response responsibilities and escalation procedures.

Detailed recommendations are available in `security-controls.md`.

---

## 15. Risk Treatment Strategy

The assessment uses four recognized risk treatment options.

| Treatment Option | Meaning | Example |
|---|---|---|
| Mitigate | Introduce controls to reduce likelihood or impact | Implement MFA to reduce account compromise risk |
| Avoid | Stop the activity that creates the risk | Disable an unnecessary exposed service |
| Transfer | Shift some financial consequences to another party | Consider appropriate cyber insurance |
| Accept | Formally acknowledge and retain a risk | Accept a low-level risk when further treatment is not justified |

### 15.1 Proposed Risk Treatment

| Risk ID | Risk Rating | Proposed Treatment | Reason |
|---|---|---|---|
| R-001 | Critical | Mitigate | Email compromise could provide access to organizational communications and additional resources |
| R-002 | High | Mitigate | Ransomware could disrupt access to critical patient information |
| R-003 | High | Mitigate | Poor segmentation could increase the impact of a network compromise |
| R-004 | High | Mitigate | Excessive privileges could expose sensitive patient information |
| R-005 | High | Mitigate | Unpatched endpoints could provide opportunities for malware infection |
| R-006 | High | Mitigate | Weak passwords could allow unauthorized access to internal files |
| R-007 | Medium | Mitigate | Website compromise could affect public services and organizational reputation |
| R-008 | High | Mitigate | Weak wireless separation could expose internal network resources |

The proposed approach prioritizes mitigation for all eight risks.

The organization should review treatment decisions according to operational requirements, available resources, and its formal risk acceptance authority.

---

## 16. Residual Risk Assessment

Residual risk represents the risk expected to remain after recommended controls have been implemented and are operating effectively.

The values below are projected estimates. They are not verified post-implementation results.

### 16.1 Projected Residual Risk Register

| Risk ID | Inherent Likelihood | Inherent Impact | Inherent Score | Inherent Rating | Projected Residual Likelihood | Projected Residual Impact | Residual Score | Residual Rating |
|---|---:|---:|---:|---|---:|---:|---:|---|
| R-001 | 5 | 5 | 25 | Critical | 2 | 5 | 10 | High |
| R-002 | 3 | 5 | 15 | High | 2 | 3 | 6 | Medium |
| R-003 | 3 | 4 | 12 | High | 2 | 4 | 8 | Medium |
| R-004 | 3 | 5 | 15 | High | 2 | 5 | 10 | High |
| R-005 | 3 | 4 | 12 | High | 2 | 3 | 6 | Medium |
| R-006 | 4 | 4 | 16 | High | 2 | 4 | 8 | Medium |
| R-007 | 3 | 3 | 9 | Medium | 2 | 3 | 6 | Medium |
| R-008 | 3 | 4 | 12 | High | 2 | 4 | 8 | Medium |

### 16.2 Residual Risk Interpretation

The projected residual scores indicate that recommended controls could reduce the likelihood of several scenarios.

However, some risks remain significant because their potential impact could still be severe even after preventive controls are introduced.

For example:

- R-001 remains High because a successful compromise of email accounts could still have serious consequences.
- R-004 remains High because authorized users may still misuse access despite access restrictions and monitoring.
- R-002 is projected to reduce to Medium if patching, endpoint protection, and reliable recovery controls operate effectively.

### 16.3 Residual Risk Limitations

Residual risk estimates must be reassessed after control implementation.

A real organization should not treat these projected values as evidence that risks have been reduced.

Validation should include:

- Reviewing implemented configurations.
- Checking MFA coverage.
- Reviewing access permissions.
- Confirming patch compliance.
- Testing backup restoration.
- Reviewing security logs.
- Conducting appropriate security assessments.
- Recording control failures and corrective actions.

---

## 17. Remediation Priorities

The following priorities are proposed for addressing the identified risks.

### 17.1 Remediation Priority Overview

| Priority | Risk IDs | Recommended Focus |
|---|---|---|
| Critical | R-001 | Strengthen email account security and phishing protection |
| High | R-002, R-003, R-004, R-005, R-006, R-008 | Improve patient data protection, access control, patching, network security, and backups |
| Medium | R-007 | Improve public website security and administration |

### 17.2 Proposed Remediation Timeline

| Timeline | Priority | Recommended Activities |
|---|---|---|
| Immediate: 0–7 days | Critical | Review important accounts, prioritize MFA, identify unnecessary access, and establish incident escalation procedures |
| Short-term: 8–30 days | High | Improve password practices, begin access reviews, review patching processes, and verify backup arrangements |
| Medium-term: 31–60 days | High | Improve network segmentation, strengthen endpoint protection, and establish centralized security monitoring |
| Longer-term: 61–90 days | Medium | Improve website security, conduct control reviews, test recovery procedures, and refine security awareness activities |

These are proposed planning periods for the fictional scenario, not actual completion dates.

### 17.3 Remediation Accountability

| Activity | Proposed Owner | Expected Evidence of Completion |
|---|---|---|
| MFA implementation | IT Team | MFA configuration records and coverage report |
| Password policy improvement | IT Team | Approved password policy and implementation records |
| Patch management | IT Team | Patch reports and documented update records |
| Network segmentation | Network Administrator | Approved network design and configuration evidence |
| Privileged access review | IT Team / Database Administrator | Access review records and approved permissions |
| Endpoint protection | IT Team | Endpoint protection deployment and monitoring reports |
| Backup and recovery | IT Team | Backup logs and successful restoration test records |
| Security monitoring | IT Team | Monitoring configuration and incident review records |
| Staff awareness | Hospital Management / IT Team | Training materials and attendance records |
| Incident response | Hospital Management / IT Team | Approved incident response procedure and exercise records |

The complete remediation plan is documented in `remediation-plan.md`.

---

## 18. Governance and Security Responsibilities

Cybersecurity risk management requires clear ownership and accountability.

The following responsibilities are proposed for the fictional organization.

| Role | Proposed Responsibility |
|---|---|
| Hospital Management | Approve security priorities, provide oversight, and support risk treatment decisions |
| IT Team | Coordinate system security, account management, patching, endpoint protection, and security documentation |
| Network Administrator | Manage network infrastructure, segmentation, wireless security, and network monitoring |
| Database Administrator | Support patient database security, permissions, backups, and database maintenance |
| Health Information Management | Support appropriate handling and protection of patient information |
| Department Heads | Ensure staff follow approved security procedures |
| All Employees | Protect credentials, follow security policies, and report suspicious activity |

These roles are proposed for the fictional assessment and are not verified organizational appointments.

---

## 19. Regulatory and Framework Considerations

Because the fictional organization is assumed to operate in Nigeria and may process sensitive health information, data protection and healthcare information security obligations should be considered.

### 19.1 Nigeria Data Protection Considerations

The Nigeria Data Protection Act 2023 provides a legal framework for the processing and protection of personal data in Nigeria.

A real healthcare organization should assess its obligations concerning:

- Lawful processing of personal data.
- Protection of sensitive personal information.
- Appropriate technical and organizational security measures.
- Access to personal data.
- Personal data breaches.
- Data subject rights.
- Applicable breach reporting and accountability requirements.

This project does not determine whether a real organization complies with the Act.

### 19.2 NIST Cybersecurity Framework 2.0

The NIST Cybersecurity Framework 2.0 provides a structured approach to managing cybersecurity risks.

Its six core functions are:

| Function | Purpose | Example Application in This Project |
|---|---|---|
| Govern | Establish cybersecurity strategy, responsibilities, and oversight | Define risk ownership and security responsibilities |
| Identify | Understand assets and cybersecurity risks | Develop the asset inventory and risk register |
| Protect | Implement safeguards | Recommend MFA, access control, patching, and backups |
| Detect | Identify possible cybersecurity incidents | Recommend logging, monitoring, and suspicious activity detection |
| Respond | Take action during cybersecurity incidents | Recommend incident response procedures |
| Recover | Restore services and operations | Recommend backup and recovery planning |

### 19.3 NIST SP 800-30 Revision 1

NIST SP 800-30 Revision 1 provides guidance for conducting risk assessments.

This project uses its risk assessment concepts to structure:

- Threat identification.
- Vulnerability identification.
- Likelihood assessment.
- Impact assessment.
- Risk determination.
- Risk documentation.

The project's specific 1–5 scoring scale and risk rating bands are tailored educational choices.

### 19.4 Compliance Limitation

The frameworks and legislation referenced here provide guidance for the assessment.

This report is not a legal opinion, formal compliance assessment, certification, or independent audit.

A real organization should seek appropriate legal, privacy, and cybersecurity expertise to determine its specific obligations.

---

## 20. Continuous Monitoring and Review

Cybersecurity risks change as systems, users, technologies, and threats change.

The fictional hospital should establish a regular process for reviewing its cybersecurity risk register and security controls.

### 20.1 Recommended Monitoring Activities

| Monitoring Activity | Recommended Frequency | Responsible Role |
|---|---|---|
| Review user access privileges | Quarterly | IT Team / Department Heads |
| Review privileged accounts | Monthly | IT Team |
| Review patch status | Monthly | IT Team |
| Review security alerts and logs | Daily or continuously where supported | IT Team |
| Review backup status | Daily | IT Team |
| Conduct backup restoration tests | Quarterly | IT Team |
| Review firewall and network access rules | Quarterly | Network Administrator |
| Review incident response procedures | Annually and after significant incidents | Hospital Management / IT Team |
| Conduct staff security awareness activities | At onboarding and periodically | Hospital Management / IT Team |
| Review the risk register | Quarterly and after significant changes | Risk Owners / IT Team |

These frequencies are proposed recommendations and should be adjusted according to organizational resources and risk exposure.

### 20.2 Events That Should Trigger a Risk Review

A new assessment or risk register review should be considered when:

- A significant security incident occurs.
- A new information system is introduced.
- A major network change takes place.
- New vulnerabilities are identified.
- Employees change roles or leave the organization.
- Access privileges change significantly.
- New regulatory requirements apply.
- A security control fails or becomes ineffective.
- The organization begins using a new external service provider.

---

## 21. Key Findings

The assessment produced the following key observations.

### Finding 1: Email Account Security Requires Priority Attention

Phishing and credential compromise represent a significant hypothetical risk.

MFA, stronger authentication practices, email security, and employee awareness should be prioritized.

### Finding 2: Patient Information Requires Strong Protection

The patient database is classified as a critical asset.

Access control, monitoring, backup protection, and secure system maintenance are important safeguards.

### Finding 3: Patch Management Is an Important Security Activity

Outdated systems may expose an organization to known vulnerabilities.

A documented patch management process should be established, including prioritization and verification.

### Finding 4: Network Segmentation Can Limit Attack Impact

Insufficient separation between network environments may allow an attacker to move from one compromised system to other resources.

Network access restrictions and segmentation should be reviewed.

### Finding 5: Excessive Privileges Increase Insider Risk

Users should only have access to the information and systems required for their responsibilities.

Regular access reviews and audit logging can help reduce and detect misuse.

### Finding 6: Backup and Recovery Planning Is Essential

Backups should be protected against unauthorized modification and ransomware.

Restoration should be tested regularly rather than assuming that successful backup jobs guarantee recoverability.

### Finding 7: Security Monitoring and Incident Response Need Attention

Preventive controls alone cannot eliminate cybersecurity risk.

Monitoring, incident reporting, containment, and recovery procedures are also necessary.

---

## 22. Assessment Limitations

This project has important limitations.

1. GreenCare Community Hospital is fictional.
2. The organization size and operating environment are assumptions.
3. No real information assets were inspected.
4. No real network or application was scanned.
5. No penetration testing was performed.
6. Vulnerabilities were not technically verified.
7. Likelihood and impact scores are hypothetical estimates.
8. Security controls were recommended but not implemented or tested.
9. Residual risk scores are projections rather than measured outcomes.
10. The assessment does not constitute a formal audit or compliance certification.

The findings should therefore be interpreted as an educational demonstration of cybersecurity risk assessment practices.

---

## 23. Conclusion

This cybersecurity risk assessment demonstrates how an organization can identify information assets, analyze threats and vulnerabilities, develop attack scenarios, calculate risk scores, and recommend appropriate security controls.

The fictional GreenCare Community Hospital scenario identified eight hypothetical risks across seven information assets.

The highest-rated risk was phishing and email account compromise, followed by risks involving weak password practices, ransomware, insider misuse, and network security weaknesses.

The assessment recommends prioritizing identity and access management, MFA, patch management, network segmentation, endpoint protection, backup and recovery, security monitoring, and incident response.

The projected residual risk analysis demonstrates how recommended safeguards may reduce risk, while also recognizing that significant residual risks can remain.

A real organization would need to validate its assets, vulnerabilities, controls, and risk ratings through appropriate evidence collection, technical assessment, stakeholder consultation, and continuous monitoring.

This project is intended to demonstrate a structured, evidence-conscious approach to cybersecurity risk assessment and documentation.

---

## 24. Supporting Project Documents

The following documents provide additional details supporting this report.

| File | Description |
|---|---|
| `README.md` | Project overview, objectives, scope, and repository navigation |
| `docs/asset-inventory.md` | Detailed information asset inventory and classification |
| `docs/threat-assessment.md` | Threat actor analysis, threats, and attack scenarios |
| `docs/vulnerability-assessment.md` | Vulnerability analysis and identified control gaps |
| `docs/risk-register.md` | Centralized risk register, scoring methodology, and residual risk estimates |
| `docs/security-controls.md` | Recommended preventive, detective, and corrective security controls |
| `docs/remediation-plan.md` | Proposed remediation activities, priorities, owners, and success metrics |
| `evidence/diagrams/risk-flow.md` | Risk assessment process diagram |
| `evidence/diagrams/network-overview.md` | Fictional network overview |
| `evidence/screenshots/README.md` | Description of the evidence directory and screenshot limitations |
| `evidence/supporting-material/risk-matrix.md` | Supporting risk matrix |
| `evidence/supporting-material/assessment-notes.md` | Assessment assumptions and supporting notes |
| `references/references.md` | External frameworks, standards, and reference materials |

---

## 25. References

The following sources informed the assessment methodology and framework considerations.

### 25.1 NIST Special Publication 800-30 Revision 1

**Title:** Guide for Conducting Risk Assessments

**Organization:** National Institute of Standards and Technology (NIST)

**URL:** https://csrc.nist.gov/pubs/sp/800/30/r1/final

**Application in this project:** Informed the risk assessment approach, including threat identification, vulnerability consideration, likelihood, impact, and risk determination.

### 25.2 NIST Cybersecurity Framework 2.0

**Title:** The NIST Cybersecurity Framework (CSF) 2.0

**Organization:** National Institute of Standards and Technology (NIST)

**URL:** https://nvlpubs.nist.gov/nistpubs/CSWP/NIST.CSWP.29.pdf

**Application in this project:** Informed the organization of cybersecurity recommendations around Govern, Identify, Protect, Detect, Respond, and Recover.

### 25.3 Nigeria Data Protection Act 2023

**Title:** Nigeria Data Protection Act 2023

**Organization:** Federal Republic of Nigeria

**Application in this project:** Provides jurisdictional context for considering the protection and lawful processing of personal data in the fictional Nigerian healthcare scenario.

**Reference:** https://ndpc.gov.ng/

> The references support the educational methodology and contextual considerations. They do not establish that the fictional organization has achieved compliance with any framework or law.

---

## 26. Document Review

| Review Item | Status |
|---|---|
| Fictional organization and assessment scope documented | Included |
| Assessment objectives documented | Included |
| Asset identification documented | Included |
| Threat actor analysis documented | Included |
| Threat identification documented | Included |
| Vulnerability analysis documented | Included |
| Attack scenarios documented | Included |
| Likelihood and impact scales defined | Included |
| Risk calculation methodology defined | Included |
| Risk register summarized | Included |
| Security controls recommended | Included |
| Risk treatment options documented | Included |
| Residual risk estimates documented | Included |
| Remediation priorities documented | Included |
| Governance responsibilities proposed | Included |
| Regulatory and framework considerations documented | Included |
| Continuous monitoring recommendations documented | Included |
| Limitations clearly stated | Included |
| Supporting documents referenced | Included |

---

**End of Report**