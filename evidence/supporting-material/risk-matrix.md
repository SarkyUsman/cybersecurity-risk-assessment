# Risk Matrix

## Purpose

This risk matrix supports the risk assessment for GreenCare Community Hospital.

It provides a simple method for evaluating risk based on two factors:

- **Likelihood** — how likely the event is to occur.
- **Impact** — how severe the consequences would be if the event occurred.

> **Important:** The ratings in this matrix are qualitative estimates created for this fictional portfolio project. They are not measurements from a real organization.

## Risk Rating Method

The assessment uses three likelihood levels:

| Likelihood | Description |
|---|---|
| Low | The event is unlikely to occur under the assumed conditions |
| Medium | The event is possible and could reasonably occur |
| High | The event is likely to occur under the assumed conditions |

Impact is assessed using four levels:

| Impact | Description |
|---|---|
| Low | Limited effect on systems, information, or operations |
| Medium | Noticeable effect on operations or security |
| High | Significant effect on systems, information, or operations |
| Critical | Severe effect on sensitive information or essential operations |

## Risk Matrix

| Likelihood \ Impact | Low | Medium | High | Critical |
|---|---|---|---|---|
| **High** | Medium | High | Critical | Critical |
| **Medium** | Low | Medium | High | High |
| **Low** | Low | Low | Medium | High |

## Risk Classification

| Risk Rating | Meaning | Recommended Response |
|---|---|---|
| Low | Limited risk | Monitor and manage |
| Medium | Moderate risk | Implement appropriate controls |
| High | Significant risk | Prioritize remediation |
| Critical | Severe risk | Immediate attention and remediation |

## Project Risk Mapping

| Risk ID | Risk | Likelihood | Impact | Risk Rating |
|---|---|---|---|---|
| R-01 | Credential Theft | High | High | Critical |
| R-02 | Ransomware | Medium | Critical | High |
| R-03 | Unauthorized Network Access | Medium | High | High |
| R-04 | Unauthorized Data Access | Medium | Critical | High |
| R-05 | Exploitation of Known Vulnerabilities | Medium | High | High |

## Risk Prioritization

Based on the assessment, the risks should be addressed in the following order:

| Priority | Risk ID | Risk | Rating | Primary Treatment |
|---|---|---|---|---|
| 1 | R-01 | Credential Theft | Critical | Implement MFA and security awareness training |
| 2 | R-02 | Ransomware | High | Patch management, secure backups, endpoint protection |
| 3 | R-03 | Unauthorized Network Access | High | Network segmentation and firewall controls |
| 4 | R-04 | Unauthorized Data Access | High | Least privilege and access reviews |
| 5 | R-05 | Exploitation of Known Vulnerabilities | High | Patch management and vulnerability monitoring |

## Risk Treatment Approach

The primary treatment strategy for the identified risks is **risk reduction**.

Risk reduction involves implementing security controls that decrease the likelihood of a successful attack, reduce the potential impact, or both.

Examples include:

```text
MFA
 ↓
Reduces account takeover risk

Patch Management
 ↓
Reduces exposure to known vulnerabilities

Network Segmentation
 ↓
Limits lateral movement

Least Privilege
 ↓
Limits unauthorized access

Secure Backups
 ↓
Improves recovery from ransomware and data loss

Relationship to the Risk Register

This matrix complements the project's:

- "docs/risk-register.md"
- "docs/security-controls.md"
- "docs/remediation-plan.md"

The risk register records the individual risks, while this matrix provides the overall framework used to classify their severity.

Evidence Classification

This is a qualitative risk matrix created for a fictional cybersecurity assessment.

No real organization's risk levels, security posture, or infrastructure were assessed.

Key Takeaway

Risk prioritization helps an organization focus limited security resources on the threats that could have the greatest consequences.

For GreenCare Community Hospital, credential theft is the highest-priority risk, followed by ransomware and other risks affecting critical systems and sensitive information.


### Evidence structure now

```text
evidence/
├── diagrams/
│   ├── risk-flow.md
│   └── network-overview.md
├── screenshots/
│   └── README.md
└── supporting-material/
    └── risk-matrix.md

Done: "risk-matrix.md" ✅

Next: "evidence/supporting-material/assessment-notes.md" — the final supporting artifact.
