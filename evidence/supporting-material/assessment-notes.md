# Assessment Notes

## Purpose

This document records the assumptions, methodology, observations, and limitations used during the cybersecurity risk assessment of GreenCare Community Hospital.

The organization is fictional and was created specifically for this portfolio project.

## Organization Assumptions

The assessment assumes that GreenCare Community Hospital has approximately 35 employees and uses common technology resources to support its operations.

The assumed environment includes:

- Staff computers
- Staff user accounts
- Hospital Wi-Fi
- Internet connectivity
- Email services
- A patient database
- A file-sharing system
- A public website
- Basic network infrastructure

The assessment assumes that some systems contain sensitive information and therefore require stronger security controls.

## Assessment Scope

The assessment focuses on the following areas:

| Area | Included |
|---|---|
| Information Assets | Yes |
| Staff Devices | Yes |
| Network Infrastructure | Yes |
| Wi-Fi | Yes |
| Email | Yes |
| Patient Database | Yes |
| File Sharing | Yes |
| Public Website | Yes |
| Human-related Threats | Yes |
| Security Controls | Yes |
| Remediation Planning | Yes |

## Assessment Methodology

The assessment followed this sequence:

```text
1. Define the organization
        ↓
2. Identify assets
        ↓
3. Identify threats
        ↓
4. Identify vulnerabilities
        ↓
5. Connect threats to vulnerabilities
        ↓
6. Identify affected assets
        ↓
7. Assess likelihood and impact
        ↓
8. Assign risk ratings
        ↓
9. Recommend security controls
        ↓
10. Develop remediation priorities

Risk Assessment Model

The primary relationship used during the assessment was:

Threat
   +
Vulnerability
   +
Affected Asset
   +
Potential Impact
   ↓
Risk
   ↓
Security Control
   ↓
Risk Reduction

This approach helped ensure that vulnerabilities were not treated as risks in isolation.

Key Assumptions

The following assumptions were made:

ID| Assumption
A-01| Employees use organizational accounts to access systems and services
A-02| Some systems contain sensitive patient or organizational information
A-03| Employees have access to email and internet services
A-04| Wireless connectivity is available to staff
A-05| Critical systems are connected to the organization's internal network
A-06| Security controls may not be consistently implemented across all systems
A-07| Systems may contain unpatched software or operating systems
A-08| Some users may have more privileges than required for their roles

Key Observations

Observation 1 — Identity Security

Weak password practices and the absence of MFA could increase the likelihood of account compromise.

Recommended focus:

- MFA
- Strong authentication
- Password management
- Security awareness training

Observation 2 — Patch Management

Unpatched systems could provide attackers with opportunities to exploit known vulnerabilities.

Recommended focus:

- Centralized patch management
- Regular vulnerability assessments
- Asset inventory
- Security update monitoring

Observation 3 — Network Segmentation

Poor segmentation could allow an attacker who compromises one device to move toward more sensitive systems.

Recommended focus:

- Network segmentation
- Firewall rules
- Access control
- Network monitoring

Observation 4 — Access Management

Excessive privileges could allow users or compromised accounts to access information beyond their legitimate requirements.

Recommended focus:

- Least privilege
- Role-based access
- Periodic access reviews
- Account lifecycle management

Observation 5 — Recovery Capability

Ransomware or other destructive events could make important systems unavailable.

Recommended focus:

- Secure backups
- Backup testing
- Recovery procedures
- Endpoint protection
- Incident response planning

Evidence Created

The following supporting artifacts were created as part of this assessment:

Evidence| Location| Purpose
Risk Flow Diagram| "evidence/diagrams/risk-flow.md"| Shows the relationship between threat, vulnerability, asset, risk, and control
Network Overview| "evidence/diagrams/network-overview.md"| Demonstrates a proposed segmented network architecture
Risk Matrix| "evidence/supporting-material/risk-matrix.md"| Supports qualitative risk classification
Screenshot Documentation| "evidence/screenshots/README.md"| Documents the project's screenshot evidence policy

Limitations

This assessment has several limitations.

1. Fictional Environment

GreenCare Community Hospital does not represent a real organization.

2. No Technical Testing

No vulnerability scans, penetration tests, configuration reviews, packet captures, log analysis, or system exploitation were performed.

3. Qualitative Risk Ratings

Likelihood and impact ratings are based on reasonable assumptions rather than measured organizational data.

4. Limited Organizational Information

The assessment does not include detailed information about:

- Actual hardware
- Operating systems
- Software versions
- Network topology
- User accounts
- Security policies
- Existing security controls
- Regulatory requirements
- Incident history

5. No Real-World Validation

The proposed controls and remediation actions have not been implemented or validated in a production environment.

Ethical and Legal Considerations

All cybersecurity activities represented in this project are intended for authorized and educational environments.

The project does not involve:

- Unauthorized access
- Credential theft
- Malware deployment
- Exploitation of real systems
- Unauthorized vulnerability scanning
- Collection of real patient information

Any future technical testing should only be conducted against systems where explicit authorization has been provided.

Lessons Learned

This assessment demonstrated several important cybersecurity concepts:

1. Assets must be identified before risks can be properly evaluated.
2. Threats and vulnerabilities are related but are not the same thing.
3. Risk depends on the potential effect of a threat exploiting a vulnerability.
4. Critical assets require stronger protection.
5. Security controls should be prioritized according to risk.
6. Network segmentation can limit lateral movement.
7. Least privilege reduces unnecessary access.
8. MFA can significantly strengthen account security.
9. Secure backups are important for recovery from ransomware and other destructive events.
10. Documentation is an important part of cybersecurity risk management.

Final Assessment Note

The assessment demonstrates a structured approach to identifying cybersecurity risks and developing appropriate controls.

The next stage of development would be to validate these concepts in an authorized laboratory environment through practical exercises such as vulnerability scanning, log analysis, network monitoring, system hardening, and incident investigation.

Evidence Classification

All content in this document is based on a fictional organization and simulated assessment assumptions.

No real organization's security posture is represented.


### Evidence folder is now complete

```text
evidence/
├── diagrams/
│   ├── risk-flow.md
│   └── network-overview.md
├── screenshots/
│   └── README.md
└── supporting-material/
    ├── risk-matrix.md
    └── assessment-notes.md
