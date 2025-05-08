# SOC-Playbook-and-Automation-Lab

## Incident Response Plan For Apex Capital with Scenarios for Privileged Account Compromise. 

## OVERVIEW
Maintaining trust and meeting regulatory requirements is crucial to protect confidential information and systems against cyber-attacks. Apex Capital incident response plan aims to quickly and effectively contain cyber threats while ensuring normal business operations. This involves protecting privileged accounts and requires the collaboration of various departments. The plan will be updated regularly to reflect organizational changes, compliance culture and new technologies, and regular testing will be conducted to ensure preparedness.

## Objective
This plan provides a comprehensive approach to respond to a privileged account compromise, addressing different methods of attack, and ensuring thorough detection, containment, and remediation processes.

![image](https://github.com/user-attachments/assets/eb852df3-d08c-4eb8-83a9-2ca4f6f299d6)

## 1.  PREPARATION: 
These preparation steps are crucial to establishing an effective Cybersecurity Incident Response Team and ensuring that Apex Capital is ready to respond promptly and effectively to security incidents. Preparation must be completed before an incident.

1. Determine the Members of the Cybersecurity Incident Response Team (CSIRT)
## Core CSIRT Member
Composition: The core CSIRT includes members from Information Technology roles and a few roles from various departments for support, this helps maintain confidentiality and efficiency.


| **Role**                          | **Responsibility** | **Contact** |
|----------------------------------|--------------------|-------------|
| **Information Security**<br>Chief Information Security Officer | Develops incident response criteria and communicates with the executive team and Board. | Seun Matthew<br>📞 09051120975<br>📧 seunmatthew@apex-capital.org |
| **Incident Response Team**<br>Lead and Team Members | Maintains the IR plan, conducts checks, identifies and evaluates incidents. | Ese Brume<br>📞 08054768572<br>📧 brumeese@apex-capital.org |
| **Identity and Access Management**<br>Team Lead and Members | Manages privilege audits, monitors activity, and responds to account compromises. | Paul Ike<br>📞 08143304076<br>📧 paulike@apex-capital.org |
| **IT Operations and Support** | Manages system access and software updates. | Micheal Nwokeke<br>📞 08036713523<br>📧 michealnwokeke@apex-capital.org |
| **Legal Counsel** | Confirms breach notification requirements, checks law enforcement involvement. | Kemi Oshinowo<br>📞 07074696452<br>📧 kemioshinowo@apex-capital.org |
| **Audit & Compliance** | Manages regulatory reporting. | Sydney Biose<br>📞 08067534219<br>📧 sydneybiose@apex-capital.org |
| **Human Resources** | Communicates breach info to employees. | Adenike Ola<br>📞 08185697166<br>📧 adenikeola@apex-capital.org |
| **Regulatory Contact** | Manages breach info to regulators. | Chioma Aniekwe<br>📞 08156723489<br>📧 chiomaaniekwe@apex-capital.org |

#### Communications Team

| **Role**                          | **Responsibility** | **Contact** |
|----------------------------------|--------------------|-------------|
| **Marketing & PR Lead** | Handles external communications and crisis messaging. | Chukwuemeka Anthony<br>📞 07056432134<br>📧 anthonyemeka@apex-capital.org |
| **Web & Social Media Lead** | Publishes updates on web/social channels, monitors feedback. | Sodiq Isah<br>📞 08045792236<br>📧 sodiqisah@apex-capital.com |
| **Technical Support (Internal)** | Provides internal guidance and bulletins. | Amos Oghenetega<br>📞 09024657688<br>📧 amosoghenetega@apex-capital.org |
| **Technical Support (External)** | Supports external users during a breach. | Akpan Okon<br>📞 08123567890<br>📧 akpanokon@gmail.com |

---

### 1.2 Escalation Paths

- Define when and how incidents escalate.
- Ensure low-impact events that evolve are appropriately handled.
- Create clear documentation and response flows.

### 1.3 Logging Configuration

- **Login System Logging:** Maintain logs (Active Directory, VPN, etc.) for minimum 90 days.
- **Secure Log Storage:** Use SIEM systems to store logs and prevent tampering.

---

## 2. Detection and Analysis

- Analyze logs for suspicious activity (e.g., excessive logins, malware indicators).
- Identify entry points, attack vectors, and compromised data.
- Investigate using:
  - Endpoint and app behavior
  - Email system queries
  - Network and access anomalies
- Review behavior and access to sensitive systems like OneDrive, Google Drive, SharePoint, etc.

### Sample Incident Scenarios

#### Incident 1 – Brute Force / Credential Harvesting

| **CIA Category** | **Compromise Type** | **Business Impact** | **Risk Level** |
|------------------|----------------------|----------------------|----------------|
| C, I             | Privileged Account   | Yes                  | High           |

Evidence: Repeated failed login attempts and logins from various IPs using different passwords.

---

#### Incident 2 – Insider Threat

| **CIA Category** | **Compromise Type** | **Business Impact** | **Risk Level** |
|------------------|----------------------|----------------------|----------------|
| C, I             | Privileged Account   | Yes                  | Medium         |

Evidence: Abnormal employee behavior, large file transfers, visiting malicious sites.

---

#### Incident 3 – Phishing

| **CIA Category** | **Compromise Type** | **Business Impact** | **Risk Level** |
|------------------|----------------------|----------------------|----------------|
| C                | Privileged Account   | Yes                  | High           |

Evidence: Suspicious email with phishing links, spelling errors, and odd addresses.

---

## 3. Containment, Eradication, and Recovery

### Containment
These steps in containment should be followed cautiously and carried out based on the kind of attack and the response that best handles the compromise.
**Immediate Actions:**
- Lock compromised accounts, reset passwords, enforce MFA.
- Block phishing sources and suspicious domains.
- Disable unauthorized accounts.
- Preserve evidence: logs, screenshots, files.

**Long-Term Actions:**
- Use forensic tools for deeper analysis.
- Monitor activity via IDS/SIEM.
- Analyze malware with tools like VirusTotal, Hybrid-Analysis.

### Eradication

- Identify the root cause of the malware; phishing,
- Remove the malicious files and processes identified on the infected systems.
- Use antivirus and anti-malware tools to scan and clean the affected
  endpoints.
- Update all software and apply necessary patches to address vulnerabilities
 exploited by the attackers.
- Ensure the latest security updates are installed on all systems.
# Credential Reset:
- Reset passwords for compromised accounts and ensure multi-factor
  authentication (MFA) is enforced.
- Monitor for any suspicious account activities post-incident.
- Disable the compromised account and isolate affected systems.
- Scan and clean affected systems using antivirus and anti-malware tools.
- Close firewall ports and network connections that were used during the attack.


### Recovery

- Apply the latest security patches and software updates to address vulnerabilities exploited by the attackers.
- Return any systems that were taken offline to production.
-  Close network access previously used by the attackers and reset passwords for affected accounts.
- Download and apply the latest security patches to address any vulnerabilities exploited during the incident.
- Conduct a vulnerability analysis to ensure that all identified issues have been resolved.
- Inform employees about the recovery process and any changes made.
- Share recovery information externally through appropriate channels
- Continue to monitor for any signs of malicious activity related to the incident to ensure that the threat has been fully eradicated.



## 4. Post-Incident Activities

- Evaluate incident costs and outcomes.
- Evaluate the cost of the incident.
- Discuss the following questions and document the information for future reference.
   what went well during the investigation?
- Identify areas that did not go well during the investigation.
- Determine any vulnerabilities or gaps in the organization’s security and how to address them.
- Explore additional steps or actions that could have helped prevent the incident.
- Consider whether modifications must be made to existing protocols or procedures.
- Update the incident response plan.
- Maintain robust application security Operating System and Application patching procedures
- Employee, IT, or CSIRT Training
- Create and distribute an incident report to relevant parties
- Document all information and more technical reports for the CSIRT.
- Document and present an executive summary of the incident to the management team.








