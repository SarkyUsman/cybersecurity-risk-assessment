# Asset Inventory

## 1. Purpose

This document identifies and classifies the information assets and technology resources assumed to exist within GreenCare Community Hospital.

The inventory provides the foundation for identifying threats, vulnerabilities, security risks, and appropriate security controls.

> **Project Note:** GreenCare Community Hospital is a fictional organization created for educational and cybersecurity portfolio purposes. All asset details, owners, dependencies, and classifications are assumed.

## 2. Organization Overview

| Field | Details |
|---|---|
| Organization | GreenCare Community Hospital |
| Industry | Healthcare |
| Organization Size | Approximately 35 employees |
| Location | Nigeria (assumed jurisdiction) |
| Assessment Type | Fictional Cybersecurity Risk Assessment |
| Version | 2.0 |

## 3. Asset Classification Methodology

Assets are evaluated using three information security principles:

| Security Principle | Description |
|---|---|
| Confidentiality | Ensures information is accessible only to authorized individuals |
| Integrity | Ensures information remains accurate, complete, and protected from unauthorized modification |
| Availability | Ensures systems and information are accessible when required |

### Classification Scale

| Rating | Description |
|---|---|
| Low | Limited security or operational importance |
| Medium | Noticeable security or operational importance |
| High | Significant security or operational importance |
| Critical | Essential to the organization's operations or protection of highly sensitive information |

## 4. Asset Inventory

| Asset ID | Asset Name | Description | Owner |
|---|---|---|---|
| A-01 | Patient Database | Stores patient records, medical histories, and other sensitive healthcare information | Health Information Management / IT Team |
| A-02 | Staff Computers | Computers used by employees to access organizational applications and perform daily duties | IT Team |
| A-03 | Email System | Supports internal and external communication and may contain sensitive organizational information | IT Team |
| A-04 | Hospital Wi-Fi | Provides wireless connectivity for authorized staff and other permitted users | Network Administrator |
| A-05 | Public Website | Provides information about the hospital, its services, and contact details | IT Team / Communications |
| A-06 | File-Sharing System | Stores and distributes internal documents and organizational files | IT Team |
| A-07 | Network Infrastructure | Includes routers, switches, firewalls, and related networking equipment | Network Administrator |

## 5. Asset Data and Security Classification

| Asset ID | Asset Name | Data Handled | Confidentiality | Integrity | Availability | Criticality |
|---|---|---|---|---|---|---|
| A-01 | Patient Database | Patient records and medical information | Critical | Critical | Critical | Critical |
| A-02 | Staff Computers | Work documents, user credentials, and locally accessed information | High | High | High | High |
| A-03 | Email System | Internal messages, attachments, and organizational communication | High | High | High | High |
| A-04 | Hospital Wi-Fi | Network authentication information and wireless traffic | High | High | High | High |
| A-05 | Public Website | Public hospital information and service details | Low | High | Medium | Medium |
| A-06 | File-Sharing System | Internal documents and organizational files | High | High | High | High |
| A-07 | Network Infrastructure | Network configurations, traffic information, and access rules | High | High | Critical | High |

## 6. Asset Dependencies

| Asset ID | Asset Name | Dependencies | Potential Effect of Dependency Failure |
|---|---|---|---|
| A-01 | Patient Database | Servers, network infrastructure, authentication, backups, and power | Patient information may become unavailable or inaccessible |
| A-02 | Staff Computers | Operating systems, endpoint protection, network connectivity, and user accounts | Staff productivity and access to services may be disrupted |
| A-03 | Email System | Internet connectivity, email service provider, DNS, and user authentication | Communication may be interrupted or compromised |
| A-04 | Hospital Wi-Fi | Wireless access points, network infrastructure, authentication, and power | Wireless connectivity may become unavailable |
| A-05 | Public Website | Web hosting, DNS, internet connectivity, and website administration | Public access to hospital information may be disrupted |
| A-06 | File-Sharing System | Storage, network infrastructure, authentication, and backups | Internal documents may become unavailable or exposed |
| A-07 | Network Infrastructure | Routers, switches, firewall configuration, power, and network administration | Multiple connected systems may experience disruption |

## 7. Asset Criticality Assessment

### A-01 — Patient Database

**Criticality: Critical**

The patient database contains highly sensitive healthcare information. Unauthorized disclosure, modification, or loss of availability could have serious consequences for patient privacy and hospital operations.

### A-02 — Staff Computers

**Criticality: High**

Staff computers provide access to organizational systems and information. A compromised device could become an entry point for malware, credential theft, or unauthorized network access.

### A-03 — Email System

**Criticality: High**

The email system supports organizational communication and may contain sensitive information. It is also a potential entry point for phishing and business email compromise.

### A-04 — Hospital Wi-Fi

**Criticality: High**

Wireless connectivity supports staff access to organizational resources. Weak wireless security or poor separation of guest and internal networks could increase unauthorized access risks.

### A-05 — Public Website

**Criticality: Medium**

The public website provides information about the hospital and its services. Website compromise could affect public trust, service availability, and the integrity of published information.

### A-06 — File-Sharing System

**Criticality: High**

The file-sharing system contains internal documents and organizational information. Unauthorized access, ransomware, or accidental deletion could affect confidentiality and availability.

### A-07 — Network Infrastructure

**Criticality: High**

Network infrastructure supports communication between organizational systems. Its compromise or failure could affect multiple assets, including critical systems.

## 8. Key Findings

The inventory identifies the patient database as the most critical information asset because of the sensitivity of the information it contains and its importance to healthcare operations.

Other important assets include:

- Staff computers, which may be exposed to malware and phishing.
- Email systems, which are common targets for credential theft.
- Network infrastructure, which supports communication between systems.
- File-sharing systems, which may contain sensitive organizational information.

The dependencies also show that a failure affecting network infrastructure could disrupt several other assets simultaneously.

## 9. Relationship to Risk Assessment

The identified assets will be used in subsequent assessment activities:

| Assessment Activity | Related Document |
|---|---|
| Threat Identification | `docs/threat-assessment.md` |
| Vulnerability Identification | `docs/vulnerability-assessment.md` |
| Risk Evaluation | `docs/risk-register.md` |
| Security Controls | `docs/security-controls.md` |
| Risk Remediation | `docs/remediation-plan.md` |

## 10. Assumptions and Limitations

- All assets are based on a fictional hospital environment.
- Asset owners represent proposed organizational responsibilities, not verified individuals.
- Data classifications are assumed for educational purposes.
- Dependencies represent a proposed environment and have not been technically verified.
- No real systems, databases, networks, or patient records were accessed or assessed.

## 11. Conclusion

A reliable cybersecurity risk assessment begins with understanding the assets that need protection.

This inventory establishes the assumed information assets, their ownership, security requirements, dependencies, and criticality.

These details provide the foundation for identifying realistic threats, analyzing vulnerabilities, evaluating risks, and recommending appropriate security controls.