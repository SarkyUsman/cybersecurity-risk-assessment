# Risk Register

## 1. Document Information

| Field | Details |
|---|---|
| Project | Cybersecurity Risk Assessment |
| Organization | GreenCare Community Hospital |
| Document | Risk Register |
| Version | 2.0 |
| Assessment Type | Fictional, Educational Assessment |
| Organization Size | Approximately 35 Employees |
| Jurisdiction Assumption | Nigeria |
| Risk Assessment Method | Likelihood × Impact |
| Risk Register Status | Initial Assessment |

## 2. Purpose

This document provides a centralized register of the cybersecurity risks identified during the assessment of GreenCare Community Hospital.

It brings together information from the following documents:

- `asset-inventory.md`
- `threat-assessment.md`
- `vulnerability-assessment.md`

The register connects organizational assets, threats, vulnerabilities, and hypothetical attack scenarios to evaluate potential cybersecurity risks.

It also records proposed risk treatments, responsible owners, and estimated residual risks.

The purpose is to help the organization understand which risks require attention and establish a basis for prioritizing security improvements.

**Important:** GreenCare Community Hospital is fictional. The risk scenarios, likelihood ratings, impact ratings, and scores are educational estimates. They are not based on a real hospital investigation, technical testing, or confirmed security incidents.

## 3. Risk Assessment Methodology

The assessment uses a qualitative risk-scoring model based on two factors:

1. Likelihood: How likely a particular risk scenario is to occur.
2. Impact: How severe the consequences could be if the scenario occurs.

The risk score is calculated by multiplying the likelihood score by the impact score.

**Risk Score = Likelihood × Impact**

For this project, the scoring model is adapted as a practical educational method informed by NIST SP 800-30 Revision 1.

The numerical ranges and rating categories below are the project's chosen assessment model. They should not be interpreted as a scoring scale prescribed by NIST.

## 4. Likelihood Scale

Likelihood measures the estimated possibility of a risk scenario occurring.

| Score | Likelihood | Description |
|---|---|---|
| 1 | Rare | Very unlikely to occur. |
| 2 | Unlikely | Could occur but is not expected. |
| 3 | Possible | Could reasonably occur. |
| 4 | Likely | Expected to occur under the assumed conditions. |
| 5 | Almost Certain | Very likely to occur. |

## 5. Impact Scale

Impact measures the potential consequences of a cybersecurity incident on the organization.

The assessment considers confidentiality, integrity, availability, operational disruption, financial consequences, and potential effects on patient information.

| Score | Impact | Description |
|---|---|---|
| 1 | Negligible | Minimal impact on organizational operations or information. |
| 2 | Minor | Limited disruption or limited information exposure. |
| 3 | Moderate | Noticeable operational or security impact requiring corrective action. |
| 4 | Major | Significant operational disruption, data exposure, or recovery effort. |
| 5 | Severe | Critical organizational impact, potentially affecting essential hospital operations or sensitive patient information. |

## 6. Risk Calculation and Rating

The risk score is calculated using:

**Risk Score = Likelihood × Impact**

The resulting score is assigned a risk rating using the following categories.

| Risk Score | Risk Rating | General Interpretation |
|---|---|---|
| 1–4 | Low | Risk is relatively limited but should still be monitored. |
| 5–9 | Medium | Risk requires appropriate security measures and periodic review. |
| 10–16 | High | Risk requires prioritized treatment and management attention. |
| 17–25 | Critical | Risk requires urgent attention and appropriate management action. |

### 6.1 Risk Rating Matrix

The following matrix shows how likelihood and impact combine to produce a risk score.

| Likelihood / Impact | 1 - Negligible | 2 - Minor | 3 - Moderate | 4 - Major | 5 - Severe |
|---|---:|---:|---:|---:|---:|
| 5 - Almost Certain | 5 Medium | 10 High | 15 High | 20 Critical | 25 Critical |
| 4 - Likely | 4 Low | 8 Medium | 12 High | 16 High | 20 Critical |
| 3 - Possible | 3 Low | 6 Medium | 9 Medium | 12 High | 15 High |
| 2 - Unlikely | 2 Low | 4 Low | 6 Medium | 8 Medium | 10 High |
| 1 - Rare | 1 Low | 2 Low | 3 Low | 4 Low | 5 Medium |

## 7. Risk Treatment Options

Risk treatment describes the action selected to address an identified risk.

The assessment considers four treatment options.

| Treatment | Meaning | Example |
|---|---|---|
| Mitigate | Introduce security measures to reduce likelihood or impact. | Implement MFA, patch systems, and improve access controls. |
| Avoid | Stop the activity or remove the condition creating the risk. | Discontinue an unnecessary service that creates unacceptable exposure. |
| Transfer | Shift some financial or contractual consequences to another party. | Use an appropriate cyber insurance policy or contractual risk-sharing arrangement. |
| Accept | Formally acknowledge and retain a risk when it is within approved risk tolerance. | Accept a low-level risk after considering its impact and treatment cost. |

**Important:** Transferring a risk does not eliminate the organization's responsibility to protect sensitive information. Likewise, accepting a risk should involve an informed decision by an authorized person.

## 8. Inherent Risk and Residual Risk

This assessment distinguishes between inherent risk and residual risk.

### 8.1 Inherent Risk

Inherent risk is the estimated level of risk before considering the additional security improvements proposed in this assessment.

It represents the potential exposure under the assumed conditions.

### 8.2 Residual Risk

Residual risk is the estimated level of risk remaining after the proposed security controls have been implemented effectively.

Residual risk is calculated using the same likelihood and impact scales.

**Residual Risk Score = Residual Likelihood × Residual Impact**

Residual scores in this document are projections. They are not evidence that the proposed controls have already been implemented or tested.

## 9. Centralized Risk Register

The following register contains the major hypothetical cybersecurity risks identified for GreenCare Community Hospital.

| Risk ID | Asset | Threat | Vulnerability / Control Gap | Risk Scenario | Likelihood | Impact | Inherent Score | Rating | Treatment | Risk Owner |
|---|---|---|---|---|---:|---:|---:|---|---|---|
| R-001 | A-03 Email System | T-01 Phishing / T-04 Credential Compromise | V-02 Lack of MFA | An employee's credentials are stolen through phishing. An attacker may access the email account and information available to the user. | 5 | 5 | 25 | Critical | Mitigate | IT Team |
| R-002 | A-01 Patient Database | T-03 Ransomware Attack | V-03 Unpatched Systems | Attackers exploit an unpatched system and deploy ransomware, potentially disrupting access to patient information. | 3 | 5 | 15 | High | Mitigate | IT Team / Database Administrator |
| R-003 | A-07 Network Infrastructure | T-02 Malware Infection / T-04 Credential Compromise | V-04 Poor Network Segmentation | An attacker compromises one network device and attempts to reach other internal systems because network separation may be insufficient. | 3 | 4 | 12 | High | Mitigate | Network Administrator |
| R-004 | A-01 Patient Database | T-05 Insider Threat | V-05 Excessive Privileges | An employee or contractor misuses excessive permissions to access, copy, modify, or disclose patient information. | 3 | 5 | 15 | High | Mitigate | IT Team / Database Administrator |
| R-005 | A-02 Staff Computers | T-02 Malware Infection | V-03 Unpatched Systems | An attacker exploits vulnerable endpoint software, potentially compromising a staff workstation and information accessible from it. | 3 | 4 | 12 | High | Mitigate | IT Team |
| R-006 | A-06 File-Sharing System | T-04 Credential Compromise | V-01 Weak Password Practices | An attacker obtains a staff member's weak or reused password and attempts to access shared organizational files. | 4 | 4 | 16 | High | Mitigate | IT Team |
| R-007 | A-05 Public Website | T-02 Malware Infection / T-04 Credential Compromise | V-03 Unpatched Systems | An attacker exploits an unpatched website component or compromised administrator account to alter website content or disrupt public access. | 3 | 3 | 9 | Medium | Mitigate | IT Team / Website Administrator |
| R-008 | A-04 Hospital Wi-Fi | T-02 Malware Infection / T-04 Credential Compromise | V-04 Poor Network Segmentation | An attacker gains access to the wireless network and attempts to reach internal systems that should be separated from wireless users. | 3 | 4 | 12 | High | Mitigate | Network Administrator |

**Scoring note:** The likelihood and impact values are illustrative estimates based on the hypothetical scenarios and assumed asset criticality. They are not measured probabilities or confirmed technical findings.

## 10. Risk Analysis and Treatment Recommendations

### 10.1 R-001: Phishing and Email Account Compromise

**Risk ID:** R-001

**Affected asset:** A-03 Email System

**Related threat IDs:** T-01, T-04

**Related vulnerability ID:** V-02

**Scenario:**

An employee receives a phishing email and enters their credentials on a fraudulent website. An attacker obtains the credentials and attempts to access the employee's email account.

If MFA is not enabled, a valid password may be sufficient to gain access.

**Potential consequences:**

- Unauthorized access to email communications.
- Exposure of confidential organizational information.
- Fraudulent messages sent from a legitimate account.
- Further compromise of services accessible through the account.

**Recommended treatment: Mitigate**

- Enable MFA for organizational email accounts.
- Prioritize privileged and administrative accounts.
- Provide phishing awareness training.
- Monitor unusual login attempts and account activity.
- Establish a secure account recovery process.

**Risk owner:** IT Team.

### 10.2 R-002: Ransomware Affecting the Patient Database

**Risk ID:** R-002

**Affected asset:** A-01 Patient Database

**Related threat ID:** T-03

**Related vulnerability ID:** V-03

**Scenario:**

An attacker exploits an unpatched system or compromises an endpoint connected to the hospital environment. Ransomware may then affect accessible systems or shared data, potentially disrupting access to patient information.

**Potential consequences:**

- Loss of access to patient records.
- Disruption of hospital operations.
- Data recovery expenses.
- Potential exposure of sensitive information if data theft occurs.

**Recommended treatment: Mitigate**

- Establish a documented patch management process.
- Maintain regular backups of important information.
- Keep protected backup copies isolated from ordinary user access.
- Test backup restoration periodically.
- Deploy endpoint protection and monitoring.
- Develop an incident response and recovery procedure.

**Risk owner:** IT Team / Database Administrator.

### 10.3 R-003: Network Compromise Through Poor Segmentation

**Risk ID:** R-003

**Affected asset:** A-07 Network Infrastructure

**Related threat IDs:** T-02, T-04

**Related vulnerability ID:** V-04

**Scenario:**

An attacker gains initial access to a device connected to the hospital network. Insufficient network separation may allow the attacker to identify and attempt access to additional internal systems.

**Potential consequences:**

- Unauthorized access attempts against internal systems.
- Increased opportunity for lateral movement.
- Wider malware impact.
- Exposure of sensitive organizational information.

**Recommended treatment: Mitigate**

- Separate guest wireless access from internal hospital networks.
- Implement network segmentation where appropriate.
- Restrict communication between network segments.
- Review firewall and access rules.
- Monitor unusual network traffic.

**Risk owner:** Network Administrator.

### 10.4 R-004: Insider Misuse of Patient Information

**Risk ID:** R-004

**Affected asset:** A-01 Patient Database

**Related threat ID:** T-05

**Related vulnerability ID:** V-05

**Scenario:**

An employee or contractor has permissions beyond their job requirements and intentionally accesses or discloses patient information outside their authorized responsibilities.

**Potential consequences:**

- Unauthorized disclosure of patient information.
- Privacy violations.
- Loss of trust.
- Legal and reputational consequences.

**Recommended treatment: Mitigate**

- Apply the principle of least privilege.
- Implement role-based access control where appropriate.
- Review user permissions regularly.
- Remove unnecessary access rights.
- Monitor privileged activity.
- Maintain records of access approvals and changes.

**Risk owner:** IT Team / Database Administrator.

### 10.5 R-005: Endpoint Compromise Through Unpatched Software

**Risk ID:** R-005

**Affected asset:** A-02 Staff Computers

**Related threat ID:** T-02

**Related vulnerability ID:** V-03

**Scenario:**

A staff computer runs software containing a known security vulnerability. An attacker attempts to exploit the weakness to execute malicious software or gain unauthorized access.

**Potential consequences:**

- Malware infection.
- Unauthorized access to workstation data.
- Credential theft.
- Potential access to connected organizational resources.

**Recommended treatment: Mitigate**

- Maintain an endpoint inventory.
- Apply security updates regularly.
- Remove unsupported software.
- Use endpoint protection.
- Restrict unnecessary administrative privileges.
- Monitor endpoint security alerts.

**Risk owner:** IT Team.

### 10.6 R-006: Unauthorized Access to Shared Files

**Risk ID:** R-006

**Affected asset:** A-06 File-Sharing System

**Related threat ID:** T-04

**Related vulnerability ID:** V-01

**Scenario:**

An attacker obtains a staff member's weak or reused password and attempts to access the file-sharing system using the compromised account.

**Potential consequences:**

- Unauthorized access to organizational documents.
- Exposure of sensitive information.
- Unauthorized modification or deletion of files.
- Further compromise of connected accounts.

**Recommended treatment: Mitigate**

- Establish strong password practices.
- Encourage unique passwords for organizational accounts.
- Implement MFA where supported.
- Review file-sharing permissions.
- Monitor unusual file access and downloads.
- Provide staff security awareness training.

**Risk owner:** IT Team.

### 10.7 R-007: Public Website Compromise

**Risk ID:** R-007

**Affected asset:** A-05 Public Website

**Related threat IDs:** T-02, T-04

**Related vulnerability ID:** V-03

**Scenario:**

An attacker exploits an unpatched website component or compromises an administrator account to gain unauthorized access to website management functions.

**Potential consequences:**

- Website defacement.
- Disruption of public information services.
- Publication of misleading information.
- Reputational damage.

**Recommended treatment: Mitigate**

- Keep website software and components updated.
- Secure administrator accounts with MFA.
- Restrict administrative access.
- Maintain website backups.
- Monitor website changes and suspicious activity.
- Establish a recovery procedure.

**Risk owner:** IT Team / Website Administrator.

### 10.8 R-008: Unauthorized Access Through Hospital Wi-Fi

**Risk ID:** R-008

**Affected asset:** A-04 Hospital Wi-Fi

**Related threat IDs:** T-02, T-04

**Related vulnerability ID:** V-04

**Scenario:**

An attacker gains access to the hospital's wireless network through compromised credentials or an insecure access point. If network separation is insufficient, the attacker may attempt to reach internal systems.

**Potential consequences:**

- Unauthorized network access.
- Exposure of internal services.
- Increased opportunity for lateral movement.
- Potential disruption of hospital network services.

**Recommended treatment: Mitigate**

- Use secure wireless authentication.
- Separate guest Wi-Fi from internal networks.
- Review wireless access permissions.
- Change default administrative credentials on network equipment.
- Monitor connected devices.
- Review wireless network configurations regularly.

**Risk owner:** Network Administrator.

## 11. Residual Risk Assessment

Residual risk represents the estimated risk remaining after the proposed security controls have been implemented effectively.

The following values are projected estimates for educational purposes. They must be reassessed after implementation and testing.

| Risk ID | Inherent Likelihood | Inherent Impact | Inherent Score | Inherent Rating | Proposed Control Effect | Residual Likelihood | Residual Impact | Residual Score | Residual Rating |
|---|---:|---:|---:|---|---|---:|---:|---:|---|
| R-001 | 5 | 5 | 25 | Critical | MFA, phishing awareness, login monitoring | 2 | 5 | 10 | High |
| R-002 | 3 | 5 | 15 | High | Patch management, protected backups, recovery testing | 2 | 3 | 6 | Medium |
| R-003 | 3 | 4 | 12 | High | Network segmentation, firewall rules, traffic monitoring | 2 | 4 | 8 | Medium |
| R-004 | 3 | 5 | 15 | High | Least privilege, access reviews, activity monitoring | 2 | 5 | 10 | High |
| R-005 | 3 | 4 | 12 | High | Security patching, endpoint protection, monitoring | 2 | 3 | 6 | Medium |
| R-006 | 4 | 4 | 16 | High | Strong passwords, MFA, file access reviews | 2 | 4 | 8 | Medium |
| R-007 | 3 | 3 | 9 | Medium | Website patching, administrator MFA, backups | 2 | 3 | 6 | Medium |
| R-008 | 3 | 4 | 12 | High | Secure wireless access, network separation, monitoring | 2 | 4 | 8 | Medium |

### 11.1 Residual Risk Interpretation

The projected residual risk ratings show that implementing security controls may reduce the likelihood or impact of several scenarios.

However, some risks may remain High even after the proposed improvements.

For example:

- R-001 may still have a High residual rating because successful compromise of an email account could expose sensitive information even when MFA is enabled.
- R-004 may remain High because authorized users can still misuse legitimate access, even when permissions are restricted.
- R-002 may reduce to Medium if patching, protected backups, and recovery procedures are implemented and tested effectively.

Residual risk should not automatically be accepted simply because security controls have been introduced.

Management should review remaining risks and determine whether further treatment is necessary.

## 12. Risk Prioritization

The following order is based on the initial inherent risk scores.

| Priority | Risk ID | Risk Description | Inherent Score | Rating |
|---|---|---|---:|---|
| 1 | R-001 | Phishing and Email Account Compromise | 25 | Critical |
| 2 | R-006 | Unauthorized Access to Shared Files | 16 | High |
| 3 | R-002 | Ransomware Affecting the Patient Database | 15 | High |
| 4 | R-004 | Insider Misuse of Patient Information | 15 | High |
| 5 | R-003 | Network Compromise Through Poor Segmentation | 12 | High |
| 6 | R-005 | Endpoint Compromise Through Unpatched Software | 12 | High |
| 7 | R-008 | Unauthorized Access Through Hospital Wi-Fi | 12 | High |
| 8 | R-007 | Public Website Compromise | 9 | Medium |

**Priority note:** Risks with the same score may require different treatment timelines depending on asset criticality, operational consequences, and available resources.

## 13. Risk Ownership and Accountability

Risk owners are responsible for coordinating the treatment and monitoring of assigned risks.

The following roles are assumed for this fictional organization.

| Role | Main Responsibility |
|---|---|
| IT Team | Coordinates account security, endpoint protection, patch management, and information security improvements. |
| Network Administrator | Oversees network infrastructure, wireless security, segmentation, and network monitoring. |
| Database Administrator | Oversees database access, database security, backup coordination, and data protection. |
| Website Administrator | Coordinates website maintenance, administrator access, updates, and website recovery. |
| Hospital Management | Reviews major risks, approves resources, and makes formal risk acceptance decisions. |

**Note:** These are assumed organizational roles. Actual responsibility assignments would need to be confirmed in a real organization.

## 14. Risk Monitoring and Review

The risk register should be reviewed periodically and whenever significant changes occur.

Suggested review activities include:

| Monitoring Activity | Purpose | Suggested Frequency |
|---|---|---|
| Review user access permissions | Identify unnecessary or excessive privileges. | Quarterly |
| Review MFA coverage | Confirm that sensitive accounts use additional authentication. | Monthly |
| Review patch status | Identify systems with outstanding security updates. | Monthly |
| Review backup status | Confirm that important data is backed up. | Weekly |
| Test backup restoration | Confirm that backups can be restored successfully. | Quarterly |
| Review network access rules | Identify unnecessary communication between network segments. | Quarterly |
| Review security incidents | Identify new threats and reassess existing risks. | After each significant incident |
| Review the risk register | Update likelihood, impact, treatment, and residual risk. | Quarterly |

These frequencies are proposed planning targets, not verified existing organizational practices.

### 14.1 Events That Should Trigger a Risk Review

The risk register should also be reviewed when:

- A new system or application is introduced.
- A major software vulnerability is disclosed.
- A cybersecurity incident occurs.
- An employee changes roles or leaves the organization.
- Network architecture changes.
- Sensitive information is moved to a new platform.
- A security control fails or becomes ineffective.
- New legal or regulatory requirements affect the organization.

## 15. Relationship to Other Assessment Documents

| Document | Relationship |
|---|---|
| `asset-inventory.md` | Provides asset IDs, ownership, data classification, and criticality. |
| `threat-assessment.md` | Provides threat IDs, threat actors, and hypothetical attack scenarios. |
| `vulnerability-assessment.md` | Provides vulnerability IDs and potential security control gaps. |
| `security-controls.md` | Documents safeguards intended to reduce the identified risks. |
| `remediation-plan.md` | Converts risk treatment recommendations into assigned actions and timelines. |
| `risk-assessment-report.md` | Summarizes the overall assessment methodology, findings, and conclusions. |

## 16. Limitations and Assumptions

- GreenCare Community Hospital is fictional.
- All risk scenarios are hypothetical.
- Likelihood and impact scores are illustrative estimates.
- No real hospital systems, networks, or patient records were assessed.
- No vulnerability scanning or penetration testing was performed.
- No actual security incidents or threat intelligence records were reviewed.
- Proposed security controls have not been implemented or tested as part of this project.
- Residual risk scores are projections, not verified post-treatment measurements.
- Risk owners and organizational responsibilities are assumed.
- This document is not a formal compliance audit or certification.

A real-world assessment would require validation through technical evidence, stakeholder interviews, system configuration reviews, and ongoing risk monitoring.

## 17. Conclusion

This risk register consolidates the assets, threats, vulnerabilities, and hypothetical attack scenarios identified in the GreenCare Community Hospital assessment.

Eight major risks were documented and evaluated using the likelihood and impact scoring model.

The initial assessment identifies:

- One Critical risk.
- Six High risks.
- One Medium risk.

The register also proposes risk treatment measures, assigns assumed risk owners, and estimates residual risk after the proposed controls.

The next stage is to document the security controls required to address these risks and establish a practical remediation plan.

Risk management should remain an ongoing activity. Risks should be reviewed and updated as systems, threats, vulnerabilities, and organizational requirements change.

---

**Document Status:** Updated

**Version:** 2.0

**Project:** Cybersecurity Risk Assessment — GreenCare Community Hospital