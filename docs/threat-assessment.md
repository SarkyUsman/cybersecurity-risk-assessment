# Threat Assessment

## 1. Document Information

| Field | Details |
|---|---|
| Project | Cybersecurity Risk Assessment |
| Organization | GreenCare Community Hospital |
| Document | Threat Assessment |
| Version | 2.0 |
| Assessment Type | Fictional, Educational Assessment |
| Organization Size | Approximately 35 Employees |
| Jurisdiction Assumption | Nigeria |

## 2. Purpose

This document identifies potential cybersecurity threats that could affect GreenCare Community Hospital.

It examines possible threat actors, their motivations, the assets they may target, and the methods they could use to compromise the organization's systems or information.

The assessment supports the identification of realistic attack scenarios and provides input for the vulnerability assessment and risk register.

**Important:** GreenCare Community Hospital is fictional. No real hospital systems, networks, accounts, or patient records were assessed.

## 3. Threat Assessment Scope

The assessment considers threats affecting the following assets:

- A-01: Patient Database
- A-02: Staff Computers
- A-03: Email System
- A-04: Hospital Wi-Fi
- A-05: Public Website
- A-06: File-Sharing System
- A-07: Network Infrastructure

The assessment focuses on threats that could affect the confidentiality, integrity, and availability of hospital information and services.

## 4. Threat Actor Identification

A threat actor is an individual, group, or entity that can intentionally or unintentionally cause harm to an organization's systems, information, or operations.

The following threat actors are considered relevant to the fictional hospital environment.

| Actor ID | Threat Actor | Possible Motivation | Potential Capability |
|---|---|---|---|
| TA-01 | Cybercriminals | Financial gain, data theft, fraud | Phishing, credential theft, malware |
| TA-02 | Ransomware Operators | Financial extortion and disruption | Ransomware deployment, data encryption, data theft |
| TA-03 | Malicious Insiders | Revenge, financial gain, intentional sabotage | Misuse of legitimate access and unauthorized data access |
| TA-04 | Hacktivists | Political, ideological, or social causes | Website disruption, defacement, unauthorized access |
| TA-05 | Compromised Users | Accounts or devices controlled by an attacker | Unauthorized access through stolen credentials or infected devices |

### 4.1 Threat Actor Analysis

#### TA-01: Cybercriminals

Cybercriminals may target hospital staff through fraudulent emails, fake login pages, or malicious attachments to steal credentials and gain unauthorized access.

**Potential targets:**
- A-03: Email System
- A-02: Staff Computers
- A-01: Patient Database

#### TA-02: Ransomware Operators

Ransomware operators may attempt to gain access to hospital systems, spread malware, encrypt important files, and demand payment to restore access.

**Potential targets:**
- A-01: Patient Database
- A-02: Staff Computers
- A-06: File-Sharing System
- A-07: Network Infrastructure

#### TA-03: Malicious Insiders

A malicious insider could be an employee or contractor who intentionally misuses authorized access to view, copy, alter, or disclose sensitive information.

**Potential targets:**
- A-01: Patient Database
- A-06: File-Sharing System
- A-03: Email System

#### TA-04: Hacktivists

Hacktivists may target the hospital's public-facing website or online services to promote an ideological or political message, disrupt operations, or publish unauthorized information.

**Potential targets:**
- A-05: Public Website
- A-03: Email System
- A-07: Network Infrastructure

#### TA-05: Compromised Users

A legitimate staff account or workstation may become compromised after phishing, malware infection, or password theft. An attacker could then use that account to access systems available to the affected user.

**Potential targets:**
- A-03: Email System
- A-02: Staff Computers
- A-06: File-Sharing System
- A-01: Patient Database, where access permissions allow

## 5. Identified Threats

The following threats were identified based on the hospital's assumed technology environment.

| Threat ID | Threat | Description | Potentially Affected Assets |
|---|---|---|---|
| T-01 | Phishing | Fraudulent emails or messages designed to trick staff into revealing credentials, opening malicious attachments, or visiting harmful websites. | A-02, A-03 |
| T-02 | Malware Infection | Malicious software introduced through infected attachments, downloads, removable media, or compromised websites. | A-02, A-06, A-07 |
| T-03 | Ransomware Attack | Malware that encrypts files or systems and may involve theft of sensitive information before extortion. | A-01, A-02, A-06, A-07 |
| T-04 | Credential Compromise | Unauthorized acquisition or use of staff login credentials to access organizational systems. | A-02, A-03, A-06, A-01 |
| T-05 | Insider Threat | Intentional or unauthorized misuse of legitimate access by an employee or contractor. | A-01, A-03, A-06 |

## 6. Threat Actor-to-Threat Mapping

This table connects the identified actors to the threats they could cause or exploit.

| Threat Actor | T-01 Phishing | T-02 Malware | T-03 Ransomware | T-04 Credential Compromise | T-05 Insider Threat |
|---|---|---|---|---|---|
| TA-01 Cybercriminals | Yes | Yes | Possible | Yes | No direct association |
| TA-02 Ransomware Operators | Possible | Yes | Yes | Possible | No direct association |
| TA-03 Malicious Insiders | No direct association | Possible | Possible | Possible | Yes |
| TA-04 Hacktivists | Possible | Possible | No direct association | Possible | No direct association |
| TA-05 Compromised Users | Possible | Possible | Possible | Yes | No, unless intentionally misusing access |

*Note: "Possible" indicates a potential relationship, not evidence that an attack has occurred. A compromised user is generally an account holder or device being misused by another actor, rather than necessarily an independent attacker.*

## 7. Attack Scenarios

Attack scenarios describe how a threat could develop into an incident affecting the organization.

The following scenarios are hypothetical and are included to demonstrate possible attack paths.

### Scenario 1: Phishing and Email Account Compromise

**Related threats:** T-01, T-04

**Threat actor:** TA-01 Cybercriminals

**Potentially affected assets:** A-03 Email System, A-02 Staff Computers, A-06 File-Sharing System

**Attack path:**

1. An employee receives a fraudulent email that appears to come from a trusted source.
2. The employee clicks a malicious link and enters their login credentials on a fake website.
3. The attacker obtains the employee's credentials.
4. The attacker attempts to access the employee's email account.
5. If access is successful, the attacker may read confidential messages, send fraudulent emails, or attempt to access other resources available to the account.

**Potential consequences:**
- Unauthorized access to email communications.
- Exposure of sensitive organizational information.
- Fraudulent messages sent using a legitimate account.
- Further compromise of systems accessible through the account.

### Scenario 2: Ransomware Infection

**Related threats:** T-02, T-03

**Threat actor:** TA-02 Ransomware Operators

**Potentially affected assets:** A-02 Staff Computers, A-06 File-Sharing System, A-01 Patient Database

**Attack path:**

1. An employee opens a malicious attachment or downloads an infected file.
2. Malware executes on the employee's workstation.
3. The attacker attempts to establish access and move to other systems.
4. Shared files or accessible systems may become compromised.
5. Ransomware encrypts accessible data and disrupts normal operations.

**Potential consequences:**
- Loss of access to important files.
- Disruption of hospital operations.
- Potential unavailability of patient information.
- Financial and recovery costs.
- Possible exposure of sensitive information if data theft also occurs.

### Scenario 3: Unauthorized Access Through Poor Network Segmentation

**Related threats:** T-02, T-04

**Threat actors:** TA-01 Cybercriminals or TA-05 Compromised Users

**Potentially affected assets:** A-04 Hospital Wi-Fi, A-07 Network Infrastructure, A-01 Patient Database

**Attack path:**

1. An attacker gains access to the hospital's wireless network through compromised credentials or an insecure access point.
2. The attacker identifies devices and services accessible from the wireless network.
3. Weak network separation may allow access attempts against internal systems.
4. The attacker attempts to exploit weaknesses or use compromised credentials.
5. Sensitive systems may be exposed if additional security controls are insufficient.

**Potential consequences:**
- Unauthorized access attempts against internal systems.
- Exposure of sensitive information.
- Increased opportunity for lateral movement.
- Disruption of network services.

### Scenario 4: Insider Misuse of Patient Information

**Related threats:** T-05, T-04

**Threat actor:** TA-03 Malicious Insiders

**Potentially affected assets:** A-01 Patient Database, A-06 File-Sharing System

**Attack path:**

1. An employee or contractor has legitimate access to hospital information systems.
2. The individual intentionally accesses records outside their authorized work responsibilities.
3. Sensitive patient information is copied, disclosed, or shared without authorization.
4. The unauthorized activity may remain unnoticed if access logging and monitoring are inadequate.

**Potential consequences:**
- Unauthorized disclosure of patient information.
- Privacy violations.
- Loss of trust.
- Legal, regulatory, and reputational consequences.

### Scenario 5: Public Website Compromise

**Related threats:** T-02, T-04

**Threat actors:** TA-01 Cybercriminals or TA-04 Hacktivists

**Potentially affected assets:** A-05 Public Website, A-07 Network Infrastructure

**Attack path:**

1. An attacker identifies a weakness in the public-facing website or its administration process.
2. The attacker attempts to exploit the weakness or obtain administrator credentials.
3. If successful, the attacker gains unauthorized access to website management functions.
4. The attacker may alter website content, disrupt services, or attempt further access.

**Potential consequences:**
- Website defacement.
- Loss of public access to hospital information.
- Publication of misleading information.
- Reputational damage.
- Potential exposure of information if the website is connected to other systems.

## 8. Threat-to-Asset Relationship

| Threat ID | Threat | Threat Actor | Target Asset | Potential Security Impact |
|---|---|---|---|---|
| T-01 | Phishing | TA-01 | A-03 Email System | Credential theft and unauthorized email access |
| T-02 | Malware Infection | TA-01 / TA-02 | A-02 Staff Computers | System compromise and malware execution |
| T-03 | Ransomware Attack | TA-02 | A-01 Patient Database | Loss of data availability |
| T-04 | Credential Compromise | TA-01 / TA-05 | A-03 Email System | Unauthorized account access |
| T-05 | Insider Threat | TA-03 | A-01 Patient Database | Unauthorized access or disclosure of patient information |

## 9. Key Findings

The assessment identifies several important threat concerns:

1. **Email-based attacks:** Phishing could provide attackers with an opportunity to steal staff credentials and gain access to organizational accounts.
2. **Ransomware exposure:** Malware and ransomware could affect important hospital systems and disrupt access to operational information.
3. **Insider misuse:** Employees or contractors with excessive access may expose sensitive information intentionally or without authorization.
4. **Network exposure:** Weak network segmentation could increase the potential for unauthorized movement between connected systems.
5. **Public-facing services:** Weaknesses in website security could affect the availability and integrity of public hospital information.

These findings identify potential attack paths. They do not establish that the fictional organization has experienced any of these incidents.

## 10. Relationship to Other Assessment Documents

| Document | Relationship |
|---|---|
| `asset-inventory.md` | Identifies the assets that may be targeted by threats. |
| `vulnerability-assessment.md` | Examines weaknesses and control gaps that could allow threats to succeed. |
| `risk-register.md` | Combines assets, threats, vulnerabilities, and attack scenarios to evaluate risk. |
| `security-controls.md` | Documents safeguards that can reduce the likelihood or impact of threats. |
| `remediation-plan.md` | Defines actions for addressing identified security weaknesses. |

## 11. Limitations

- The organization and its technology environment are fictional.
- Threat actors and attack scenarios are hypothetical.
- No penetration testing, vulnerability scanning, or live network investigation was conducted.
- No actual threat intelligence or incident records were collected.
- The assessment does not confirm that any identified threat has occurred.
- Threat likelihood and impact will be evaluated in the centralized risk register.

## 12. Conclusion

This threat assessment identifies five major threat categories and five relevant threat actor groups that could affect GreenCare Community Hospital.

The attack scenarios demonstrate how phishing, malware, ransomware, credential compromise, insider misuse, and weaknesses in public-facing services could affect hospital assets.

The next stage is to examine the vulnerabilities and control gaps that could make these scenarios possible.

---

**Document Status:** Updated

**Version:** 2.0

**Project:** Cybersecurity Risk Assessment — GreenCare Community Hospital