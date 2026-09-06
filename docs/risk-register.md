Risk Register

1. Purpose

The purpose of this Risk Register is to document, evaluate, and prioritize the cybersecurity risks identified during the assessment.

The register connects each Threat → Vulnerability → Asset → Risk to help determine appropriate security treatment.

---

2. Risk Rating Methodology

Risk ratings are based on two factors:

- Likelihood — How likely the risk is to occur
- Impact — How serious the consequences would be if the risk occurred

| Rating | Likelihood | Description |
|---|---|---|
| Low | Low | Unlikely to occur under current conditions |
| Medium | Medium | Possible to occur |
| High | High | Likely to occur |

| Rating | Impact | Description |
|---|---|---|
| Low | Low | Limited effect on operations or information |
| Medium | Medium | Noticeable operational or security impact |
| High | High | Significant effect on systems or operations |
| Critical | Critical | Severe effect on sensitive information or essential operations |

---

3. Risk Register

| Risk ID | Threat | Vulnerability | Asset | Likelihood | Impact | Risk Rating |
|---|---|---|---|---|---|---|
| R-01 | Credential Theft | Lack of MFA | Email System | High | High | Critical |
| R-02 | Ransomware | Unpatched Systems | Patient Database | Medium | Critical | High |
| R-03 | Unauthorized Network Access | Poor Network Segmentation | Network Infrastructure | Medium | High | High |
| R-04 | Unauthorized Data Access | Excessive Privileges | Patient Database | Medium | Critical | High |
| R-05 | Exploitation of Known Vulnerabilities | Unpatched Systems | Staff Computers | Medium | High | High |

---

4. Risk Analysis

R-01 — Credential Theft

Threat: Phishing or credential theft

Vulnerability: Lack of MFA

Asset: Email System

Risk: An attacker could obtain a user's password and access the organization's email environment.

Potential Impact:

- Account takeover
- Sensitive information exposure
- Further compromise of internal systems

Recommended Treatment: Implement MFA and improve phishing awareness.

---

R-02 — Ransomware

Threat: Ransomware

Vulnerability: Unpatched Systems

Asset: Patient Database

Risk: A ransomware infection could make important patient information unavailable and disrupt hospital operations.

Potential Impact:

- Patient service disruption
- Data unavailability
- Recovery costs
- Potential data loss

Recommended Treatment: Improve patch management, endpoint protection, backups, and recovery procedures.

---

R-03 — Unauthorized Network Access

Threat: Unauthorized Network Access

Vulnerability: Poor Network Segmentation

Asset: Network Infrastructure

Risk: A compromised device could provide an attacker with an opportunity to move toward sensitive systems.

Potential Impact:

- Lateral movement
- Unauthorized access to sensitive systems
- Wider network compromise

Recommended Treatment: Implement network segmentation and restrictive firewall rules.

---

R-04 — Unauthorized Patient Data Access

Threat: Insider Threat or Compromised Account

Vulnerability: Excessive Privileges

Asset: Patient Database

Risk: Users may access sensitive patient information beyond what is necessary for their roles.

Potential Impact:

- Unauthorized disclosure
- Privacy violations
- Data misuse

Recommended Treatment: Apply Least Privilege and conduct regular access reviews.

---

R-05 — Exploitation of Known Vulnerabilities

Threat: Exploitation of Known Vulnerabilities

Vulnerability: Unpatched Systems

Asset: Staff Computers

Risk: Attackers could exploit known software vulnerabilities to compromise endpoints.

Potential Impact:

- Malware infection
- Unauthorized access
- Data compromise
- Operational disruption

Recommended Treatment: Establish a formal patch management process and prioritize critical security updates.

---

5. Risk Prioritization

| Priority | Risk ID | Risk | Rating | Recommended Focus |
|---|---|---|---|---|
| 1 | R-01 | Credential Theft | Critical | Implement MFA |
| 2 | R-02 | Ransomware | High | Patch management, backups, endpoint protection |
| 3 | R-03 | Unauthorized Network Access | High | Network segmentation |
| 4 | R-04 | Unauthorized Data Access | High | Least privilege and access reviews |
| 5 | R-05 | Exploitation of Known Vulnerabilities | High | Patch management |

---

6. Risk Treatment

The recommended approach is primarily Risk Reduction through the implementation of appropriate security controls.

The organization should prioritize Critical and High risks first while continuously monitoring residual risk.

---

7. Key Observation

The highest-priority risk is credential theft because compromised credentials could provide attackers with an entry point into organizational systems.

However, the risks are interconnected. Addressing MFA, patch management, network segmentation, least privilege, backups, and monitoring together provides a stronger overall security posture.
