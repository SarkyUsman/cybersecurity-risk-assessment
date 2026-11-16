# Cybersecurity Remediation Plan

## 1. Document Information

| Field | Details |
|---|---|
| Document Title | Cybersecurity Remediation Plan |
| Organization | GreenCare Community Hospital |
| Organization Type | Fictional community healthcare facility |
| Estimated Organization Size | Approximately 35 employees |
| Assumed Jurisdiction | Nigeria |
| Document Version | 2.0 |
| Document Status | Proposed Remediation Plan |
| Prepared By | Cybersecurity Portfolio Project |
| Assessment Date | November 2026 |
| Related Document | `risk-assessment-report.md` |
| Related Document | `risk-register.md` |
| Related Document | `security-controls.md` |

> **Important:** GreenCare Community Hospital is a fictional organization created for this educational portfolio project. This remediation plan contains proposed activities, not verified implementation work. No real hospital systems were accessed, modified, scanned, or tested. The document does not represent a formal security audit or completed remediation engagement.

---

## 2. Introduction

A remediation plan defines the actions an organization should take to address identified cybersecurity risks and improve its security posture.

The previous assessment identified eight hypothetical cybersecurity risks affecting seven information assets within the fictional GreenCare Community Hospital.

This document translates the recommended security controls into actionable remediation activities.

Each activity includes:

- A related risk ID.
- The identified vulnerability.
- Recommended security controls.
- A proposed remediation action.
- An accountable owner.
- A priority level.
- A proposed implementation timeline.
- A current status.
- Measurable success criteria.
- Evidence required to verify completion.

The plan is designed to support risk reduction through a structured and measurable approach.

---

## 3. Objectives

The objectives of this remediation plan are to:

1. Address the cybersecurity risks identified in the risk register.
2. Prioritize remediation based on inherent risk ratings.
3. Define practical actions for implementing recommended security controls.
4. Assign responsibility for each remediation activity.
5. Establish realistic proposed implementation timelines.
6. Define measurable acceptance criteria.
7. Identify evidence required to verify implementation.
8. Support residual risk reassessment.
9. Establish a process for tracking outstanding remediation activities.
10. Encourage continuous cybersecurity improvement.

---

## 4. Remediation Scope

This plan addresses the following information assets:

| Asset ID | Asset Name | Criticality |
|---|---|---|
| A-01 | Patient Database | Critical |
| A-02 | Staff Computers | High |
| A-03 | Email System | High |
| A-04 | Hospital Wi-Fi | High |
| A-05 | Public Website | Medium |
| A-06 | File-Sharing System | High |
| A-07 | Network Infrastructure | High |

The remediation activities address the five vulnerability categories identified during the hypothetical assessment.

| Vulnerability ID | Vulnerability | Related Risk IDs |
|---|---|---|
| V-01 | Weak Password Practices | R-006 |
| V-02 | Lack of MFA | R-001 |
| V-03 | Unpatched Systems | R-002, R-005, R-007 |
| V-04 | Poor Network Segmentation | R-003, R-008 |
| V-05 | Excessive Privileges | R-004 |

---

## 5. Remediation Priority Levels

Remediation priorities are based on the inherent risk ratings recorded in `risk-register.md`.

| Priority | Meaning | Expected Attention |
|---|---|---|
| Critical | A risk with potentially severe consequences requiring urgent attention | Immediate |
| High | A significant risk requiring prioritized remediation | High |
| Medium | A risk requiring planned remediation and monitoring | Scheduled |
| Low | A risk that can be managed through routine security activities | Routine |

The priority indicates how urgently the proposed action should be considered. It does not mean that remediation has started or that the risk has been resolved.

---

## 6. Proposed Remediation Timeline

The following timeline provides a planning structure for the fictional organization.

| Timeline | Period | Focus |
|---|---|---|
| Immediate | 0–7 days | Address critical account security weaknesses and establish incident reporting responsibilities |
| Short-term | 8–30 days | Improve password practices, access control, patch management, and backup arrangements |
| Medium-term | 31–60 days | Strengthen network segmentation, endpoint security, and monitoring |
| Longer-term | 61–90 days | Improve website security, validate controls, and conduct security reviews |

These are proposed periods beginning after formal approval of the remediation plan. They are not historical completion dates.

---

## 7. Remediation Status Definitions

The following status values should be used when tracking remediation activities.

| Status | Meaning |
|---|---|
| Not Started | The activity has not started |
| Planned | The activity has been approved and scheduled |
| In Progress | Work has started but is not complete |
| Implemented | The proposed control or activity has been deployed |
| Pending Verification | Implementation is reported complete but evidence has not yet confirmed effectiveness |
| Verified | Evidence confirms that the activity meets its acceptance criteria |
| Blocked | The activity cannot proceed because of an identified dependency or issue |
| Deferred | The activity has been postponed with documented approval |

**Initial project status:** All remediation activities in this document are currently marked `Not Started` because this is a proposed plan for a fictional organization.

---

## 8. Remediation Summary

The following table provides an overview of the eight risks and their proposed remediation priorities.

| Risk ID | Risk Scenario | Vulnerability ID | Inherent Score | Inherent Rating | Priority | Proposed Timeline |
|---|---|---|---:|---|---|---|
| R-001 | Phishing and email account compromise | V-02 | 25 | Critical | Critical | Immediate |
| R-002 | Ransomware affecting patient records | V-03 | 15 | High | High | Short-term |
| R-003 | Unauthorized network access and lateral movement | V-04 | 12 | High | High | Medium-term |
| R-004 | Insider misuse of patient information | V-05 | 15 | High | High | Short-term |
| R-005 | Malware exploitation of unpatched endpoints | V-03 | 12 | High | High | Short-term |
| R-006 | Unauthorized file access through weak passwords | V-01 | 16 | High | High | Short-term |
| R-007 | Public website compromise | V-03 | 9 | Medium | Medium | Longer-term |
| R-008 | Unauthorized wireless access and movement into internal resources | V-04 | 12 | High | High | Medium-term |

---

## 9. Detailed Remediation Activities

### 9.1 R-001: Phishing and Email Account Compromise

**Priority:** Critical

**Proposed Timeline:** Immediate (0–7 days)

| Field | Details |
|---|---|
| Risk ID | R-001 |
| Primary Asset | A-03 Email System |
| Related Threats | T-01 Phishing, T-04 Credential Compromise |
| Vulnerability ID | V-02 Lack of MFA |
| Inherent Likelihood | 5 - Almost Certain |
| Inherent Impact | 5 - Severe |
| Inherent Risk Score | 25 - Critical |
| Proposed Owner | IT Team |
| Supporting Owner | Hospital Management |
| Related Controls | SC-01, SC-02, SC-08, SC-09, SC-11 |
| Current Status | Not Started |

#### Risk Description

An employee could receive a deceptive email and disclose login credentials through a fraudulent website.

An attacker could use the stolen credentials to access the employee's email account and potentially access additional organizational information.

#### Remediation Actions

1. Review all important email accounts.
2. Identify accounts without MFA.
3. Enable MFA for email accounts where supported.
4. Prioritize administrator and privileged accounts.
5. Establish a documented password management policy.
6. Review suspicious email reporting procedures.
7. Provide staff awareness training on phishing.
8. Review available email authentication and security settings.
9. Establish procedures for disabling compromised accounts and resetting credentials.
10. Enable appropriate authentication and account activity logging.

#### Success Metrics and Acceptance Criteria

| Metric | Acceptance Criteria |
|---|---|
| Email MFA coverage | 100% of identified in-scope email accounts have MFA enabled or a documented, approved exception |
| Privileged account protection | All identified privileged email accounts have MFA enabled |
| Password policy | An approved password management policy is documented |
| Staff awareness | All designated staff receive phishing awareness guidance |
| Account monitoring | Relevant authentication events are logged and available for review |
| Incident reporting | A documented process exists for reporting suspected phishing and compromised accounts |

#### Required Evidence

- MFA configuration records.
- Email account inventory.
- Approved password policy.
- Staff awareness materials and attendance records.
- Sample authentication logs with sensitive information removed.
- Documented incident reporting procedure.

#### Expected Outcome

Reduced likelihood of successful account compromise through stolen passwords and improved ability to identify and respond to phishing incidents.

---

### 9.2 R-002: Ransomware Affecting Patient Records

**Priority:** High

**Proposed Timeline:** Short-term (8–30 days)

| Field | Details |
|---|---|
| Risk ID | R-002 |
| Primary Asset | A-01 Patient Database |
| Related Threat | T-03 Ransomware Attack |
| Vulnerability ID | V-03 Unpatched Systems |
| Inherent Likelihood | 3 - Possible |
| Inherent Impact | 5 - Severe |
| Inherent Risk Score | 15 - High |
| Proposed Owner | IT Team |
| Supporting Owner | Database Administrator |
| Related Controls | SC-03, SC-06, SC-07, SC-08, SC-11 |
| Current Status | Not Started |

#### Risk Description

An attacker could exploit an outdated system or another security weakness to introduce ransomware.

The attack could disrupt access to patient records and affect important hospital operations.

#### Remediation Actions

1. Identify systems supporting the patient database.
2. Review operating systems and database software versions.
3. Establish a patch management process.
4. Prioritize critical security updates.
5. Deploy appropriate endpoint protection.
6. Restrict unnecessary access to database systems.
7. Establish scheduled backups.
8. Protect backup copies against unauthorized modification.
9. Maintain isolated or immutable backup copies where feasible.
10. Document and test database restoration procedures.
11. Establish ransomware incident response procedures.

#### Success Metrics and Acceptance Criteria

| Metric | Acceptance Criteria |
|---|---|
| Asset coverage | All identified patient database supporting systems are documented |
| Patch management | Critical supported components are covered by a documented patch process |
| Endpoint protection | All supported in-scope endpoints have approved protection deployed |
| Backup coverage | The patient database has a documented backup schedule |
| Backup protection | Backup access is restricted to authorized accounts |
| Recovery testing | At least one documented restoration test is completed successfully |
| Incident response | A documented ransomware response procedure is available |

#### Required Evidence

- Patient database supporting asset inventory.
- Patch reports.
- Endpoint protection deployment records.
- Backup schedules and job logs.
- Backup access permissions.
- Restoration test report.
- Ransomware incident response procedure.

#### Expected Outcome

Improved protection of patient information and better ability to restore important records following a ransomware incident or data loss event.

---

### 9.3 R-003: Unauthorized Network Access and Lateral Movement

**Priority:** High

**Proposed Timeline:** Medium-term (31–60 days)

| Field | Details |
|---|---|
| Risk ID | R-003 |
| Primary Asset | A-07 Network Infrastructure |
| Related Threats | T-02 Malware Infection, T-04 Credential Compromise |
| Vulnerability ID | V-04 Poor Network Segmentation |
| Inherent Likelihood | 3 - Possible |
| Inherent Impact | 4 - Major |
| Inherent Risk Score | 12 - High |
| Proposed Owner | Network Administrator |
| Supporting Owner | IT Team |
| Related Controls | SC-04, SC-08, SC-11 |
| Current Status | Not Started |

#### Risk Description

An attacker could gain access to one part of the network and exploit insufficient network separation to reach additional internal resources.

This could increase the impact of a compromised device or account.

#### Remediation Actions

1. Document the existing network architecture.
2. Identify important network segments.
3. Separate guest wireless access from internal resources.
4. Review communication between user devices and sensitive systems.
5. Apply firewall restrictions between network segments.
6. Restrict access to administrative interfaces.
7. Remove unnecessary network access rules.
8. Document approved network communication paths.
9. Enable appropriate network logging.
10. Review network access rules periodically.

#### Success Metrics and Acceptance Criteria

| Metric | Acceptance Criteria |
|---|---|
| Network documentation | An approved network overview and segmentation design are available |
| Guest network separation | Guest wireless access is separated from sensitive internal resources |
| Firewall rules | Network access rules have been reviewed and documented |
| Administrative access | Administrative interfaces are restricted to authorized access paths |
| Network monitoring | Relevant network security events are available for review |
| Configuration review | A documented network security review is completed |

#### Required Evidence

- Network architecture diagram.
- Network segmentation documentation.
- Firewall rule review records.
- Approved network configuration records.
- Relevant network logs.
- Documented review results.

#### Expected Outcome

Reduced opportunities for unauthorized movement between network environments and improved visibility into network activity.

---

### 9.4 R-004: Insider Misuse of Patient Information

**Priority:** High

**Proposed Timeline:** Short-term (8–30 days)

| Field | Details |
|---|---|
| Risk ID | R-004 |
| Primary Asset | A-01 Patient Database |
| Related Threat | T-05 Insider Threat |
| Vulnerability ID | V-05 Excessive Privileges |
| Inherent Likelihood | 3 - Possible |
| Inherent Impact | 5 - Severe |
| Inherent Risk Score | 15 - High |
| Proposed Owner | IT Team / Database Administrator |
| Supporting Owner | Hospital Management / Department Heads |
| Related Controls | SC-05, SC-08, SC-10, SC-11 |
| Current Status | Not Started |

#### Risk Description

An employee with excessive access privileges could view, copy, modify, or disclose patient information without an authorized purpose.

This could result in privacy violations, data exposure, and reputational damage.

#### Remediation Actions

1. Identify users with access to patient records.
2. Review existing database permissions.
3. Define access roles according to job responsibilities.
4. Apply least-privilege access.
5. Separate standard and privileged accounts.
6. Require approval for access to sensitive information.
7. Review user access periodically.
8. Disable unnecessary or inactive accounts.
9. Enable appropriate audit logging.
10. Establish procedures for investigating suspicious access to patient information.

#### Success Metrics and Acceptance Criteria

| Metric | Acceptance Criteria |
|---|---|
| Access inventory | All identified patient database accounts are documented |
| Role definition | Approved access roles are documented |
| Permission review | All identified patient database accounts are reviewed |
| Excessive privileges | Unnecessary privileges identified during the review are removed or formally approved as exceptions |
| Access approval | New sensitive access requests have documented authorization |
| Audit logging | Relevant patient database access events are logged where supported |
| Account lifecycle | A documented process exists for changing and removing user access |

#### Required Evidence

- User account inventory.
- Database permission review records.
- Approved role definitions.
- Access approval records.
- Audit log samples with sensitive information removed.
- Account removal and modification records.

#### Expected Outcome

Reduced unauthorized access to patient information and improved accountability for user activity.

---

### 9.5 R-005: Malware Exploitation of Unpatched Endpoints

**Priority:** High

**Proposed Timeline:** Short-term (8–30 days)

| Field | Details |
|---|---|
| Risk ID | R-005 |
| Primary Asset | A-02 Staff Computers |
| Related Threat | T-02 Malware Infection |
| Vulnerability ID | V-03 Unpatched Systems |
| Inherent Likelihood | 3 - Possible |
| Inherent Impact | 4 - Major |
| Inherent Risk Score | 12 - High |
| Proposed Owner | IT Team |
| Supporting Owner | Department Heads |
| Related Controls | SC-03, SC-06, SC-07, SC-08, SC-11 |
| Current Status | Not Started |

#### Risk Description

An attacker could exploit an outdated endpoint or introduce malicious software through a deceptive attachment or unsafe download.

A compromised endpoint could expose information or provide a route to additional systems.

#### Remediation Actions

1. Maintain an inventory of staff computers.
2. Identify operating systems and installed applications.
3. Establish regular security update procedures.
4. Remove unsupported software where possible.
5. Deploy endpoint protection.
6. Restrict unnecessary software installation.
7. Review local administrator privileges.
8. Enable appropriate endpoint security logging.
9. Establish procedures for isolating compromised devices.
10. Include important endpoint data in the backup strategy where appropriate.

#### Success Metrics and Acceptance Criteria

| Metric | Acceptance Criteria |
|---|---|
| Endpoint inventory | All identified staff computers are recorded |
| Patch coverage | Supported endpoints are covered by a documented update process |
| Critical updates | Critical security updates are tracked and addressed within approved timelines |
| Endpoint protection | All supported in-scope endpoints have approved protection deployed |
| Local privileges | Unnecessary local administrator privileges are removed or documented as approved exceptions |
| Incident handling | A documented process exists for isolating compromised endpoints |

#### Required Evidence

- Endpoint inventory.
- Operating system and software inventory.
- Patch compliance reports.
- Endpoint protection reports.
- Local administrator review records.
- Endpoint incident handling procedure.

#### Expected Outcome

Reduced exposure to known endpoint vulnerabilities and improved ability to detect and contain malware infections.

---

### 9.6 R-006: Unauthorized File Access Through Weak Passwords

**Priority:** High

**Proposed Timeline:** Short-term (8–30 days)

| Field | Details |
|---|---|
| Risk ID | R-006 |
| Primary Asset | A-06 File-Sharing System |
| Related Threat | T-04 Credential Compromise |
| Vulnerability ID | V-01 Weak Password Practices |
| Inherent Likelihood | 4 - Likely |
| Inherent Impact | 4 - Major |
| Inherent Risk Score | 16 - High |
| Proposed Owner | IT Team |
| Supporting Owner | Department Heads |
| Related Controls | SC-01, SC-02, SC-05, SC-07, SC-10 |
| Current Status | Not Started |

#### Risk Description

Weak or reused passwords could allow an unauthorized person to access the file-sharing system.

Sensitive organizational files could be exposed, modified, copied, or deleted.

#### Remediation Actions

1. Review accounts with access to the file-sharing system.
2. Establish strong password requirements.
3. Encourage unique passwords for each account.
4. Implement MFA where supported.
5. Review shared folder permissions.
6. Remove unnecessary access privileges.
7. Restrict access to sensitive folders.
8. Disable inactive accounts.
9. Maintain appropriate backups.
10. Review file access activity where logging is available.

#### Success Metrics and Acceptance Criteria

| Metric | Acceptance Criteria |
|---|---|
| Account inventory | All identified file-sharing accounts are documented |
| Password policy | An approved password management policy is available |
| MFA coverage | All identified in-scope accounts support MFA or have documented exceptions |
| Folder permissions | Sensitive shared folders have documented access permissions |
| Inactive accounts | Inactive accounts identified during the review are disabled or formally justified |
| Backup coverage | Important shared files are included in the approved backup process |
| Access reviews | A documented access review is completed |

#### Required Evidence

- File-sharing account inventory.
- Password policy.
- MFA configuration records.
- Shared folder permission reports.
- Inactive account review records.
- Backup records.
- Access review documentation.

#### Expected Outcome

Reduced risk of unauthorized file access through weak credentials and unnecessary permissions.

---

### 9.7 R-007: Public Website Compromise

**Priority:** Medium

**Proposed Timeline:** Longer-term (61–90 days)

| Field | Details |
|---|---|
| Risk ID | R-007 |
| Primary Asset | A-05 Public Website |
| Related Threats | T-02 Malware Infection, T-04 Credential Compromise |
| Vulnerability ID | V-03 Unpatched Systems |
| Inherent Likelihood | 3 - Possible |
| Inherent Impact | 3 - Moderate |
| Inherent Risk Score | 9 - Medium |
| Proposed Owner | IT Team / Website Administrator |
| Supporting Owner | Communications Team |
| Related Controls | SC-01, SC-03, SC-08, SC-11, SC-12 |
| Current Status | Not Started |

#### Risk Description

An attacker could exploit outdated website components or compromise an administrative account to modify or disrupt the public website.

This could affect the organization's reputation and public access to information.

#### Remediation Actions

1. Document the website platform and components.
2. Identify outdated or unsupported website components.
3. Apply supported security updates.
4. Enable MFA for website administrator accounts.
5. Remove unused plugins and components.
6. Restrict administrative access.
7. Ensure HTTPS is correctly configured.
8. Maintain website backups.
9. Monitor important administrative changes.
10. Document website recovery procedures.

#### Success Metrics and Acceptance Criteria

| Metric | Acceptance Criteria |
|---|---|
| Website inventory | Website platform and components are documented |
| Patch status | Supported website components are covered by an update process |
| Administrator protection | All identified website administrator accounts have MFA or documented exceptions |
| Component management | Unnecessary and unsupported components are removed or formally addressed |
| HTTPS | The website uses a valid HTTPS configuration |
| Backup coverage | A documented website backup process exists |
| Monitoring | Important website administration events are logged where supported |

#### Required Evidence

- Website component inventory.
- Website update records.
- Administrator account review.
- MFA configuration records.
- HTTPS configuration evidence.
- Backup records.
- Website monitoring records.

#### Expected Outcome

Reduced exposure to website vulnerabilities and improved ability to detect and recover from website compromise.

---

### 9.8 R-008: Unauthorized Wireless Access and Movement Into Internal Resources

**Priority:** High

**Proposed Timeline:** Medium-term (31–60 days)

| Field | Details |
|---|---|
| Risk ID | R-008 |
| Primary Asset | A-04 Hospital Wi-Fi |
| Related Threats | T-02 Malware Infection, T-04 Credential Compromise |
| Vulnerability ID | V-04 Poor Network Segmentation |
| Inherent Likelihood | 3 - Possible |
| Inherent Impact | 4 - Major |
| Inherent Risk Score | 12 - High |
| Proposed Owner | Network Administrator |
| Supporting Owner | IT Team |
| Related Controls | SC-01, SC-04, SC-08, SC-11 |
| Current Status | Not Started |

#### Risk Description

Weak wireless security or insufficient separation between wireless and internal networks could allow unauthorized devices to reach resources that should be restricted.

#### Remediation Actions

1. Document wireless network configurations.
2. Review wireless authentication settings.
3. Use strong, supported wireless security configurations.
4. Separate guest wireless access from internal hospital resources.
5. Restrict wireless access to sensitive systems.
6. Review authorized wireless users and devices.
7. Change default administrative credentials on wireless equipment.
8. Restrict access to wireless administration interfaces.
9. Monitor relevant wireless security events.
10. Review wireless access controls periodically.

#### Success Metrics and Acceptance Criteria

| Metric | Acceptance Criteria |
|---|---|
| Wireless inventory | Wireless access points and network configurations are documented |
| Authentication | Approved wireless authentication settings are configured |
| Guest network separation | Guest wireless access is separated from sensitive internal resources |
| Administrative access | Wireless administration interfaces are restricted to authorized personnel |
| Default credentials | Default administrative credentials are changed |
| Monitoring | Relevant wireless access events are available for review |
| Configuration review | A documented wireless security review is completed |

#### Required Evidence

- Wireless network inventory.
- Wireless security configuration records.
- Network segmentation documentation.
- Administrative access review.
- Wireless monitoring records.
- Configuration review report.

#### Expected Outcome

Reduced risk of unauthorized wireless access and improved separation between wireless users and sensitive internal resources.

---

## 10. Consolidated Remediation Action Tracker

The following table provides a central view of the proposed activities.

It can be updated as implementation progresses.

| Action ID | Risk ID | Recommended Action | Related Controls | Proposed Owner | Priority | Timeline | Status |
|---|---|---|---|---|---|---|---|
| RA-001 | R-001 | Enable MFA for important email accounts and review account security | SC-01, SC-02 | IT Team | Critical | 0–7 days | Not Started |
| RA-002 | R-001 | Deliver phishing awareness training and establish reporting procedures | SC-09, SC-11 | Hospital Management / IT Team | Critical | 0–7 days | Not Started |
| RA-003 | R-002 | Establish patch management and review patient database supporting systems | SC-03 | IT Team | High | 8–30 days | Not Started |
| RA-004 | R-002 | Protect backups and conduct a restoration test | SC-07 | IT Team / Database Administrator | High | 8–30 days | Not Started |
| RA-005 | R-003 | Document network architecture and implement segmentation improvements | SC-04 | Network Administrator | High | 31–60 days | Not Started |
| RA-006 | R-003 | Improve network logging and review access rules | SC-08 | Network Administrator / IT Team | High | 31–60 days | Not Started |
| RA-007 | R-004 | Review patient database permissions and implement least privilege | SC-05 | IT Team / Database Administrator | High | 8–30 days | Not Started |
| RA-008 | R-004 | Establish regular access reviews and relevant audit logging | SC-08, SC-10 | IT Team / Department Heads | High | 8–30 days | Not Started |
| RA-009 | R-005 | Inventory endpoints and establish patch management | SC-03 | IT Team | High | 8–30 days | Not Started |
| RA-010 | R-005 | Deploy endpoint protection and document isolation procedures | SC-06, SC-11 | IT Team | High | 8–30 days | Not Started |
| RA-011 | R-006 | Establish password management and MFA requirements | SC-01, SC-02 | IT Team | High | 8–30 days | Not Started |
| RA-012 | R-006 | Review file-sharing permissions and inactive accounts | SC-05, SC-10 | IT Team / Department Heads | High | 8–30 days | Not Started |
| RA-013 | R-007 | Review website components, updates, and administrator access | SC-03, SC-12 | Website Administrator | Medium | 61–90 days | Not Started |
| RA-014 | R-007 | Improve website logging, backups, and incident procedures | SC-08, SC-11, SC-12 | IT Team / Website Administrator | Medium | 61–90 days | Not Started |
| RA-015 | R-008 | Review wireless security and implement guest network separation | SC-04 | Network Administrator | High | 31–60 days | Not Started |
| RA-016 | R-008 | Review wireless access and monitoring arrangements | SC-01, SC-08 | Network Administrator / IT Team | High | 31–60 days | Not Started |

---

## 11. Remediation Dependencies

Some remediation activities depend on other activities being completed first.

The following dependencies should be considered during implementation.

| Action ID | Dependency | Explanation |
|---|---|---|
| RA-001 | Email account inventory | Accounts must be identified before MFA coverage can be measured |
| RA-003 | System inventory | Systems must be identified before patch status can be reviewed |
| RA-004 | Backup scope and access review | Critical data and backup permissions must be identified before recovery arrangements can be evaluated |
| RA-005 | Network documentation | Existing network connections must be understood before segmentation changes are planned |
| RA-007 | User and permission inventory | Existing database access must be reviewed before permissions can be adjusted |
| RA-009 | Endpoint inventory | Devices must be identified before patch coverage can be measured |
| RA-011 | File-sharing account inventory | Relevant accounts must be identified before password and MFA coverage can be reviewed |
| RA-013 | Website component inventory | Website software and components must be identified before updates can be planned |
| RA-015 | Wireless network documentation | Wireless networks must be documented before segmentation improvements are implemented |

Dependencies should be reviewed before assigning final implementation dates.

---

## 12. Remediation Verification

Completing a task does not automatically mean that the associated risk has been reduced.

Each remediation activity should be supported by evidence.

### 12.1 Verification Process

| Step | Activity | Expected Result |
|---|---|---|
| 1 | Review the remediation requirement | The intended security improvement is clearly defined |
| 2 | Confirm the responsible owner | Accountability is assigned |
| 3 | Implement the recommended control | The control is deployed according to the approved plan |
| 4 | Collect supporting evidence | Implementation records are available |
| 5 | Test or inspect the control | Evidence shows whether the control operates as intended |
| 6 | Compare results against acceptance criteria | Completion requirements are evaluated |
| 7 | Update remediation status | Status accurately reflects progress |
| 8 | Reassess the related risk | Likelihood, impact, and residual risk are reviewed |
| 9 | Record remaining issues | Exceptions and outstanding actions are documented |
| 10 | Obtain appropriate approval | Relevant owners approve closure or risk acceptance |

### 12.2 Evidence Quality

Evidence should be:

- Relevant to the specific remediation activity.
- Genuine and traceable.
- Dated where appropriate.
- Protected against unauthorized disclosure.
- Free of unnecessary sensitive information.
- Sufficient to support the stated completion status.

Examples include configuration records, access review reports, patch reports, backup logs, restoration test reports, and approved security procedures.

Screenshots should only be used when they genuinely demonstrate the relevant configuration or result.

---

## 13. Residual Risk Reassessment

After remediation activities are completed and verified, the organization should reassess each related risk.

The projected residual risk scores in the risk register should not be treated as confirmed outcomes.

### 13.1 Projected Residual Risk Summary

| Risk ID | Inherent Score | Inherent Rating | Projected Residual Score | Projected Residual Rating |
|---|---:|---|---:|---|
| R-001 | 25 | Critical | 10 | High |
| R-002 | 15 | High | 6 | Medium |
| R-003 | 12 | High | 8 | Medium |
| R-004 | 15 | High | 10 | High |
| R-005 | 12 | High | 6 | Medium |
| R-006 | 16 | High | 8 | Medium |
| R-007 | 9 | Medium | 6 | Medium |
| R-008 | 12 | High | 8 | Medium |

### 13.2 Residual Risk Review Requirements

For each risk, the responsible owner should:

1. Confirm that the relevant controls have been implemented.
2. Review supporting implementation evidence.
3. Verify that controls operate as intended.
4. Reassess likelihood based on the effectiveness of the controls.
5. Reassess impact where appropriate.
6. Recalculate the risk score.
7. Record the new risk rating.
8. Document any remaining control gaps.
9. Obtain approval for any risk that is formally accepted.

A risk should not be marked as reduced solely because a remediation activity has been reported as complete.

---

## 14. Risk Acceptance and Exception Management

Some risks may remain after remediation.

Where additional treatment is not practical or justified, the organization may consider formal risk acceptance.

Risk acceptance should be documented and approved by an authorized decision-maker.

### 14.1 Risk Exception Record

| Field | Required Information |
|---|---|
| Risk ID | Identifier from the central risk register |
| Risk Description | Explanation of the remaining risk |
| Current Risk Rating | Current assessed rating |
| Reason for Exception | Why the recommended control cannot be implemented or completed |
| Compensating Controls | Alternative safeguards currently in place |
| Business Justification | Reason for accepting the remaining risk |
| Risk Owner | Person responsible for the risk |
| Approval Authority | Authorized decision-maker |
| Review Date | Date for reviewing the exception |
| Expiry Date | Date when the exception must be reconsidered |

No risk acceptance is assumed or recorded as approved in this educational project.

---

## 15. Remediation Governance and Responsibilities

The following roles are proposed for the fictional hospital.

| Role | Responsibility |
|---|---|
| Hospital Management | Approve remediation priorities, provide resources, and oversee risk acceptance |
| IT Team | Coordinate account security, patching, endpoint protection, backups, and monitoring |
| Network Administrator | Manage network segmentation, wireless security, and firewall restrictions |
| Database Administrator | Support patient database security, access reviews, and recovery |
| Website Administrator | Maintain website security and administrative access |
| Department Heads | Support staff access reviews and security awareness |
| All Employees | Follow security procedures and report suspicious activities |

The proposed owners should provide regular progress updates to the appropriate management representative.

---

## 16. Remediation Progress Reporting

Progress should be reviewed regularly to identify delays, dependencies, and unresolved security weaknesses.

### 16.1 Recommended Reporting Frequency

| Reporting Activity | Recommended Frequency | Responsible Role |
|---|---|---|
| Critical risk remediation review | Weekly until addressed | IT Team / Hospital Management |
| High-risk remediation review | Biweekly | IT Team / Relevant Owners |
| Medium-risk remediation review | Monthly | IT Team / Relevant Owners |
| Remediation evidence review | At each verification milestone | Assigned Reviewer |
| Risk register update | After significant remediation changes | IT Team / Risk Owners |
| Management progress review | Monthly | Hospital Management |

### 16.2 Suggested Progress Indicators

| Indicator | Measurement |
|---|---|
| Total remediation actions | Number of actions in the tracker |
| Completed actions | Actions verified against acceptance criteria |
| In-progress actions | Actions currently being implemented |
| Blocked actions | Actions delayed by dependencies or other issues |
| Overdue actions | Actions past their approved target date |
| Critical open risks | Critical risks without verified treatment |
| High open risks | High risks without verified treatment |
| Evidence completion | Percentage of completed actions with supporting evidence |

Progress reports should reflect actual implementation records. No completion percentages should be reported until real tracking data is available.

---

## 17. Continuous Improvement

Remediation is not a one-time activity.

Cybersecurity controls should be reviewed and improved as threats, technology, systems, and organizational requirements change.

Recommended continuous improvement activities include:

- Reviewing the risk register quarterly.
- Reviewing access permissions regularly.
- Monitoring patch compliance.
- Testing backup restoration.
- Reviewing endpoint security alerts.
- Updating incident response procedures.
- Providing periodic staff security awareness training.
- Reviewing network access rules.
- Recording lessons learned from security incidents.
- Reassessing risks after major system changes.

The remediation plan should be updated whenever new risks or significant control gaps are identified.

---

## 18. Assumptions and Limitations

This remediation plan has the following limitations:

1. GreenCare Community Hospital is fictional.
2. All identified risks are hypothetical.
3. The proposed remediation activities have not been implemented.
4. No actual system configurations were reviewed.
5. No real patient records or organizational data were accessed.
6. No technical security testing was performed.
7. No remediation evidence has been collected.
8. No controls have been verified.
9. The proposed owners are roles, not confirmed appointments.
10. The proposed timelines are planning estimates.
11. The projected residual risk values are not measured outcomes.
12. The document does not constitute a formal audit, certification, or compliance assessment.

The purpose of this document is to demonstrate how cybersecurity findings can be translated into structured, measurable remediation activities.

---

## 19. Conclusion

This remediation plan converts the eight hypothetical risks identified in the GreenCare Community Hospital cybersecurity risk assessment into proposed security improvement activities.

The plan prioritizes phishing and email account compromise because it received the highest inherent risk score.

Other important remediation areas include patient database protection, ransomware resilience, access management, endpoint security, network segmentation, password management, and wireless security.

Each proposed activity has an assigned owner, priority, timeline, status, and measurable acceptance criteria.

The plan also establishes requirements for evidence collection, verification, residual risk reassessment, and progress reporting.

The next step for a real organization would be to approve the proposed activities, assign accountable individuals, allocate appropriate resources, implement the recommended controls, and verify their effectiveness.

Until implementation and verification evidence exists, all remediation activities must remain classified as proposed or not started.

---

## 20. Related Project Documents

| File | Purpose |
|---|---|
| `README.md` | Project overview, objectives, and repository navigation |
| `docs/risk-assessment-report.md` | Main cybersecurity risk assessment report |
| `docs/asset-inventory.md` | Information asset identification and classification |
| `docs/threat-assessment.md` | Threat actors, threats, and attack scenarios |
| `docs/vulnerability-assessment.md` | Vulnerability analysis and control gaps |
| `docs/risk-register.md` | Risk scoring, ratings, treatment, and residual risk |
| `docs/security-controls.md` | Recommended preventive, detective, and corrective security controls |
| `references/references.md` | Supporting frameworks and reference materials |

---

## 21. References

### NIST Special Publication 800-30 Revision 1

**Title:** Guide for Conducting Risk Assessments

**Organization:** National Institute of Standards and Technology (NIST)

**URL:** https://csrc.nist.gov/pubs/sp/800/30/r1/final

**Application:** Informed the risk assessment approach used to identify, analyze, and prioritize cybersecurity risks.

### NIST Cybersecurity Framework 2.0

**Title:** The NIST Cybersecurity Framework (CSF) 2.0

**Organization:** National Institute of Standards and Technology (NIST)

**URL:** https://nvlpubs.nist.gov/nistpubs/CSWP/NIST.CSWP.29.pdf

**Application:** Informed the security improvement approach across Govern, Identify, Protect, Detect, Respond, and Recover.

### Nigeria Data Protection Commission

**Organization:** Nigeria Data Protection Commission (NDPC)

**URL:** https://ndpc.gov.ng/

**Application:** Provides a reference point for considering personal data protection obligations in the assumed Nigerian healthcare context.

> These references support the educational methodology and recommendations. Their inclusion does not establish compliance by the fictional organization.

---

## 22. Document Review Checklist

| Review Item | Status |
|---|---|
| Remediation objectives documented | Included |
| Scope and affected assets identified | Included |
| Vulnerabilities mapped to risks | Included |
| Remediation priorities defined | Included |
| Proposed timelines defined | Included |
| Responsible owners assigned | Included |
| Remediation actions documented | Included |
| Measurable success criteria defined | Included |
| Required evidence identified | Included |
| Remediation status definitions documented | Included |
| Dependencies identified | Included |
| Verification process documented | Included |
| Residual risk review process documented | Included |
| Risk acceptance process documented | Included |
| Progress reporting process documented | Included |
| Continuous improvement recommendations included | Included |
| Assumptions and limitations documented | Included |

---

**End of Document**