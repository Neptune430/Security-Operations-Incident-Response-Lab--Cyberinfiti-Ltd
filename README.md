# Security Operations & Incident Response Report  
### CyberInfiniti Ltd — Final Sprint (April 2026)

**Report ID:** SOC-TIV-2026-INT-001  
**Author:** John Ofulue  
**Team:** CyberInfiniti SOC Analyst Team 8  
**Classification:** Confidential / Internal Use  

---

## 1. Executive Summary

During this sprint, I actively contributed to multiple security operations workstreams, simulating real-world SOC responsibilities across threat detection, incident response, and vulnerability management.

The engagement involved investigating coordinated phishing attacks, analyzing suspicious authentication activity, conducting malware analysis, engineering detection rules, and assessing vulnerabilities across both enterprise systems and mobile devices.

Key incidents included:

- A phishing campaign targeting multiple users with credential-harvesting links and malicious payloads  
- A confirmed account compromise involving unauthorized access and data exfiltration  
- A malware outbreak involving AsyncRAT and Raccoon Stealer across endpoints  
- Critical vulnerability exposures in mobile devices and Microsoft infrastructure  

All incidents were handled using structured SOC methodologies aligned with industry frameworks, ensuring proper containment, eradication, and recovery.

---

## 2. Scope of Work

This report consolidates all activities completed during the sprint, including:

- Email Threat Investigation  
- Suspicious Login Analysis  
- Malware Analysis  
- Custom Detection Engineering (Microsoft Sentinel)  
- Vulnerability Management (Mobile Devices & Patch Tuesday)  
- Incident Response Playbook Development  

Each workstream was originally documented as a standalone mini-report and is summarized here.

---

## 3. Methodology

A structured SOC workflow was followed throughout:

### Data Collection
- Azure AD Sign-in Logs  
- Email headers and artifacts  
- Endpoint telemetry  
- Threat intelligence sources  

### Analysis
- IOC enrichment using VirusTotal, URLScan, ANY.RUN  
- Behavioral analysis via sandboxing  
- Mapping to MITRE ATT&CK techniques  

### Correlation
- Cross-incident linkage  
- Timeline reconstruction  
- Attack flow analysis  

### Response
- Containment  
- Eradication  
- Recovery  

### Documentation
- Evidence logging  
- Reporting  
- Team collaboration  

---

## 4. Workstream Summary

### 4.1 Email Threat Investigation

Five reported emails were analyzed to determine their legitimacy.

**Key Findings:**
- 3 emails were confirmed malicious (phishing + malware delivery)  
- 1 email was suspicious (social engineering)  
- 1 email was benign  

**Notable Indicators:**
- Malicious domains: `wtools.io`, `contaboserver.net`  
- Payload delivery via `.exe` files and Google Drive links  
- Brand impersonation (e.g., fake Adobe update)

**Actions Taken:**
- Blocked malicious domains and senders  
- Removed emails from affected mailboxes  
- Educated users on phishing risks  

---

### 4.2 Suspicious Login Investigation

Analysis of authentication logs revealed a confirmed account compromise.

**Key Findings:**
- Brute-force attempts from foreign IPs  
- Successful logins from:
  - Bulgaria  
  - China  
  - Thailand  
- Data exfiltration from SharePoint  

**Compromised Assets:**
- Payroll data  
- Internal vulnerability report  

**Response Actions:**
- Password reset and session revocation  
- MFA enforcement  
- Firewall blocking of malicious IPs  
- Enhanced monitoring  

---

### 4.3 Malware Analysis

Two malware samples were analyzed:

- AsyncRAT (Remote Access Trojan)  
- Raccoon Stealer (credential harvesting malware)  

**Behavior Observed:**
- Process injection into `svchost.exe`  
- Registry persistence mechanisms  
- Command & Control (C2) communication  
- Credential theft from browsers  

**Affected Systems:**
- Production servers  
- Executive workstations  

**Response Actions:**
- Endpoint isolation  
- Malware removal  
- System re-imaging  
- Network blocking of C2 infrastructure  

---

### 4.4 Custom Detection Engineering

Four Microsoft Sentinel detection rules were developed:

- Suspicious foreign login activity  
- Malware C2 communication  
- Sensitive data exfiltration  
- Abuse of legitimate Microsoft domains  

**Impact:**
- Transition from reactive to proactive detection  
- Improved SOC visibility  
- Reduced detection time  

---

### 4.5 Vulnerability Management

#### Mobile Device Assessment

- 500-device fleet analyzed  
- 50% outdated devices  
- 3 actively exploited Android vulnerabilities identified  

**Risks:**
- Privilege escalation  
- Remote code execution  
- Data compromise  

**Recommendations:**
- Enforce updates  
- Deploy MDM (Microsoft Intune)  
- Segment outdated devices  

---

#### Microsoft Patch Tuesday Analysis

- 132 vulnerabilities reviewed  
- Multiple critical CVEs identified (CVSS 9.0+)  

**Key Risk:**
- Pre-authentication Remote Code Execution  

**Actions:**
- Prioritized patch deployment  
- Risk-based remediation planning  

---

### 4.6 Incident Response Playbooks

Developed structured playbooks aligned with NIST SP 800-61:

- Malware response workflow  
- Email investigation procedures  

**Phases Covered:**
- Preparation  
- Detection  
- Analysis  
- Containment  
- Eradication  
- Recovery  
- Lessons Learned  

---

## 5. Indicators of Compromise (IoCs)

### Network Indicators
- `79.124.60.6` — Brute-force attacker  
- `150.158.77.170` — Suspicious login  
- `128.24.231.64` — Malware C2  

### Domains
- `wtools.io`  
- `contaboserver.net`  
- `theannoyingsite.com`  

### File Indicators
- AsyncRAT & Raccoon Stealer payload hashes  

---

## 6. Response Actions

### Containment
- Blocked malicious IPs and domains  
- Isolated infected endpoints  
- Disabled compromised accounts  

### Eradication
- Removed malware artifacts  
- Cleared persistence mechanisms  
- Conducted full system scans  

### Recovery
- Enforced MFA  
- Reset credentials  
- Re-imaged systems  
- Deployed monitoring controls  

---

## 7. Key Lessons Learned

- Lack of MFA enabled account compromise  
- Patch management delays increased risk exposure  
- Absence of MDM created mobile security gaps  
- Detection mechanisms were largely reactive  

**What Worked Well:**
- Strong threat analysis and investigation  
- Effective containment procedures  
- Improved detection capabilities through custom rules  

---

## 8. Recommendations

### Immediate
- Enforce MFA organization-wide  
- Patch critical vulnerabilities  
- Complete system re-imaging  

### Short-Term
- Deploy detection rules  
- Conduct account audits  
- Launch mobile update campaign  

### Long-Term
- Implement MDM solution  
- Introduce security awareness training  
- Integrate threat intelligence feeds  

---

## 9. Conclusion

This sprint provided hands-on exposure to real-world SOC operations, covering the full lifecycle of cybersecurity incidents—from detection to recovery.

The experience reinforced the importance of:

- Proactive security controls  
- Structured incident response  
- Continuous monitoring and improvement  

Overall, the sprint significantly strengthened my practical understanding of security operations and prepared me to contribute effectively in a SOC environment.

---

## 10. Appendix

### Mini-Reports
- Email Investigation  
- Suspicious Login Analysis  
- Malware Analysis  
- Custom Alerts  
- Vulnerability Management  
- Mobile Device Security  
- Incident Response Playbooks  


---

## Author

**John Ofulue**  
Cybersecurity Analyst & Instructor 
CyberInfiniti Ltd  

see files above for executive & mini reports.

---
