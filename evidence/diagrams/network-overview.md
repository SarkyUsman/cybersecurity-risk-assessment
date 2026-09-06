# Network Overview Diagram

## Purpose

This diagram provides a simplified view of the fictional GreenCare Community Hospital network used in this cybersecurity risk assessment.

The purpose is to demonstrate how organizational assets could be logically separated into different network segments to reduce unauthorized access and lateral movement.

> **Important:** This is a fictional network design created for educational and portfolio purposes. It does not represent the actual infrastructure of a real hospital.

## Simplified Network Architecture

```text
                         INTERNET
                             │
                             ▼
                    ┌─────────────────┐
                    │    FIREWALL     │
                    │                 │
                    │ Traffic Control │
                    └────────┬────────┘
                             │
                             ▼
                    ┌─────────────────┐
                    │ CORE NETWORK    │
                    │     SWITCH      │
                    └───────┬─────────┘
                            │
             ┌──────────────┼──────────────┐
             │              │              │
             ▼              ▼              ▼
      ┌────────────┐ ┌────────────┐ ┌──────────────┐
      │ STAFF      │ │ SERVER /   │ │ GUEST        │
      │ NETWORK    │ │ DATA       │ │ NETWORK      │
      │            │ │ NETWORK    │ │              │
      │ Computers  │ │ Patient DB │ │ Guest Wi-Fi  │
      │ Email      │ │ File Share │ │ Internet     │
      └────────────┘ └────────────┘ └──────────────┘
             │              │
             │              │
             ▼              ▼
      ┌────────────┐ ┌──────────────┐
      │ STAFF      │ │ RESTRICTED   │
      │ WI-FI      │ │ SYSTEMS      │
      │            │ │              │
      │ Authorized │ │ Sensitive    │
      │ Employees  │ │ Information  │
      └────────────┘ └──────────────┘

Network Segments

| Segment | Purpose | Example Assets | Security Consideration |
|---|---|---|---|
| Internet | External connectivity | Public website, external services | Firewall and traffic filtering |
| Staff Network | Normal employee operations | Staff computers, email access | Authentication and endpoint protection |
| Server/Data Network | Hosts critical systems | Patient database, file-sharing system | Restricted access and monitoring |
| Staff Wi-Fi | Wireless access for employees | Authorized staff devices | Strong authentication and encryption |
| Guest Network | Internet access for visitors | Guest devices | Isolated from internal systems |

Security Controls

| Control | Purpose |
|---|---|
| Firewall | Controls traffic between networks and the internet |
| Network Segmentation | Separates systems according to their security requirements |
| Access Controls | Restricts users and devices to authorized resources |
| MFA | Provides additional protection for user accounts |
| Endpoint Protection | Helps detect and prevent malicious activity |
| Logging and Monitoring | Supports detection and investigation |
| Secure Wi-Fi Configuration | Reduces unauthorized wireless access |
| Least Privilege | Limits access to only what users require |
Relationship to Risk R-03

The assessment identified the following risk chain:

Threat
   ↓
Unauthorized Network Access
   ↓
Vulnerability
   ↓
Poor Network Segmentation
   ↓
Potential Attack Path
   ↓
Unauthorized Lateral Movement
   ↓
Critical Systems
   ↓
Patient Database / File-Sharing System

Network segmentation helps reduce this risk by creating boundaries between less-trusted and more-sensitive systems.

For example:

Guest Wi-Fi
    X
    │
    │  Blocked / Restricted
    ▼
Staff Network
    │
    │  Controlled Access
    ▼
Server/Data Network
    │
    ▼
Patient Database

The goal is not to assume that segmentation makes the environment completely secure. Instead, it adds another security layer that can limit the scope of a compromise.

Recommended Segmentation Principles

1. Separate guest devices from internal systems.
2. Separate staff devices from critical servers.
3. Restrict access to the patient database based on job responsibilities.
4. Apply firewall rules between network segments.
5. Monitor traffic between sensitive network zones.
6. Review network access rules periodically.
7. Prevent unnecessary direct communication between network segments.

Security Architecture Principle

The proposed design follows a defense-in-depth approach.

Internet
   ↓
Firewall
   ↓
Network Segmentation
   ↓
Access Controls
   ↓
Endpoint Protection
   ↓
Authentication
   ↓
Logging & Monitoring
   ↓
Secure Data

Each layer provides additional protection if another layer is bypassed.

Evidence Classification

This is a simulated network architecture diagram created specifically for this portfolio project.

No real hospital network was accessed, scanned, mapped, or tested.

Key Takeaway

Network segmentation reduces the potential impact of a compromised device by limiting what that device can directly access.

For GreenCare Community Hospital, separating guest, staff, and sensitive server networks would provide an important layer of protection for critical systems such as the patient database.
