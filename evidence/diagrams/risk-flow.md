Risk Flow Diagram

Purpose

This diagram shows how a cybersecurity threat can exploit a vulnerability, affect an organizational asset, create a risk, and require a security control.

Risk Relationship

┌──────────────────────┐
│        THREAT        │
│                      │
│      Phishing        │
└──────────┬───────────┘
           │
           ▼
┌──────────────────────┐
│    VULNERABILITY     │
│                      │
│ Lack of MFA          │
└──────────┬───────────┘
           │
           ▼
┌──────────────────────┐
│        ASSET         │
│                      │
│   Email System       │
└──────────┬───────────┘
           │
           ▼
┌──────────────────────┐
│         RISK         │
│                      │
│ Credential Theft     │
│                      │
│ Risk Rating:         │
│ Critical             │
└──────────┬───────────┘
           │
           ▼
┌──────────────────────┐
│       CONTROL        │
│                      │
│ Multi-Factor         │
│ Authentication       │
│                      │
│ Security Awareness   │
│ Training             │
└──────────────────────┘

Example Risk Chain

Stage| Description
Threat| An attacker sends a phishing email to a hospital employee
Vulnerability| The employee's account does not use MFA
Asset| Hospital email system
Risk| The attacker may gain unauthorized access to the account
Impact| Sensitive information may be exposed or used for further attacks
Control| MFA, security awareness training, email security controls
Risk Treatment| Risk reduction

Additional Risk Relationships

R-02 — Ransomware

Ransomware
     ↓
Unpatched Systems
     ↓
Patient Database
     ↓
Data Encryption / System Unavailability
     ↓
Patch Management + Secure Backups + Endpoint Protection

R-03 — Unauthorized Network Access

Unauthorized Network Access
     ↓
Poor Network Segmentation
     ↓
Network Infrastructure
     ↓
Lateral Movement / Unauthorized Access
     ↓
Network Segmentation + Firewall Rules

R-04 — Unauthorized Data Access

Insider Threat
     ↓
Excessive Privileges
     ↓
Patient Database
     ↓
Unauthorized Patient Data Access
     ↓
Least Privilege + Access Reviews

R-05 — Exploitation of Known Vulnerabilities

Exploitation of Known Vulnerabilities
     ↓
Unpatched Systems
     ↓
Staff Computers
     ↓
System Compromise
     ↓
Patch Management + Vulnerability Monitoring

Assessment Model

The assessment follows this general model:

Threat
  ↓
Vulnerability
  ↓
Affected Asset
  ↓
Potential Impact
  ↓
Risk
  ↓
Security Control
  ↓
Remediation
  ↓
Residual Risk

Evidence Classification

This diagram is simulated documentation created for a cybersecurity portfolio project.

No real hospital systems, networks, accounts, databases, or infrastructure were accessed, scanned, exploited, or tested.

Key Takeaway

A vulnerability does not automatically represent a complete risk.

A meaningful risk assessment considers the relationship between the threat, vulnerability, affected asset, likelihood, and potential impact, then identifies appropriate controls to reduce the risk.
