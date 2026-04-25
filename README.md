# Security-Operations-Incident-Response-Lab---Cyberinfiti-Ltd.
 A hands-on simulation of real-world Security Operations Center (SOC) activities including threat detection, incident response, malware analysis, and vulnerability management.

---

## 📌 Overview

This project documents my final sprint during a SOC-focused cybersecurity internship, where I performed end-to-end security operations across multiple incident scenarios.

The work simulates a real enterprise environment using Azure AD, SIEM tools, and threat intelligence platforms, focusing on detection, investigation, and response.

---

## 🎯 Objectives

- Investigate real-world phishing and email-based threats  
- Analyze suspicious authentication activity  
- Perform malware analysis using sandbox environments  
- Engineer detection rules in a SIEM (Microsoft Sentinel)  
- Identify and remediate system vulnerabilities  
- Develop structured incident response playbooks  

---

## 🧠 Skills Demonstrated

- Security Operations (SOC)  
- Incident Response & Threat Hunting  
- Log Analysis (Azure AD, Sign-in Logs)  
- Malware Analysis (Static & Dynamic)  
- Threat Intelligence & IOC Enrichment  
- SIEM Engineering (Microsoft Sentinel, KQL)  
- Vulnerability Assessment & Risk Prioritization  

---

## 🛠️ Tools & Technologies

- Microsoft Sentinel (SIEM)  
- Azure Active Directory (Entra ID)  
- VirusTotal  
- ANY.RUN Sandbox  
- URLScan  
- Hybrid Analysis  
- Splunk (log correlation concepts)  

---

## 🔍 Project Workstreams

### 1. 📧 Email Threat Investigation
- Analyzed 5 reported emails  
- Identified phishing, malware delivery, and social engineering attempts  
- Extracted and enriched Indicators of Compromise (IoCs)  

📄 [View Report](./reports/email-investigation.md)

---

### 2. 🔐 Suspicious Login Investigation
- Investigated anomalous login patterns  
- Identified brute-force attack and account compromise  
- Confirmed data exfiltration activity  

📄 [View Report](./reports/suspicious-login.md)

---

### 3. 🦠 Malware Analysis
- Analyzed AsyncRAT and Raccoon Stealer samples  
- Observed persistence, C2 communication, and credential theft  
- Mapped behavior to MITRE ATT&CK  

📄 [View Report](./reports/malware-analysis.md)

---

### 4. 🚨 Custom SIEM Detection Rules
- Built 4 Microsoft Sentinel detection rules  
- Covered authentication anomalies, C2 traffic, and data exfiltration  

📄 [View Report](./reports/custom-alerts.md)

---

### 5. 🛡️ Vulnerability Management

#### Mobile Devices
- Assessed 500-device fleet  
- Identified actively exploited Android vulnerabilities  

#### Patch Management
- Analyzed Microsoft Patch Tuesday vulnerabilities  
- Prioritized critical CVEs (CVSS 9.0+)  

📄 [View Report](./reports/vulnerability-management.md)

---

### 6. 📘 Incident Response Playbooks
- Developed structured response workflows  
- Aligned with NIST SP 800-61  

📄 [View Report](./reports/playbooks.md)

---

## ⚠️ Key Findings

- Phishing was the primary attack vector across incidents  
- Lack of MFA enabled account compromise  
- Malware established persistence and C2 communication  
- Sensitive data (payroll) was successfully exfiltrated  
- Critical vulnerabilities remained unpatched  

---

## 🧩 Indicators of Compromise (Sample)

### IPs:
- 79.124.60.6
- 150.158.77.170
- 128.24.231.64

### Domains:
- wtools.io
- contaboserver.net
- theannoyingsite.com



---

## 🚑 Incident Response Actions

- Blocked malicious IPs and domains  
- Isolated infected endpoints  
- Reset compromised credentials  
- Enforced Multi-Factor Authentication (MFA)  
- Removed malware and persistence mechanisms  
- Deployed detection rules for future prevention  

---

## 📈 Lessons Learned

- MFA is critical for preventing account compromise  
- Patch management must be prioritized  
- Detection should be proactive, not reactive  
- Mobile devices are often overlooked attack surfaces  

---

## 🚀 Recommendations

### Immediate
- Enforce MFA across all accounts  
- Patch critical vulnerabilities  
- Re-image infected systems  

### Long-Term
- Deploy Mobile Device Management (MDM)  
- Implement user security awareness training  
- Integrate threat intelligence feeds  
- Automate response with SOAR  

---

## 📂 Repository Structure


├── README.md
├── reports/
│ ├── email-investigation.md
│ ├── suspicious-login.md
│ ├── malware-analysis.md
│ ├── custom-alerts.md
│ ├── vulnerability-management.md
│ └── playbooks.md
├── evidence/
│ ├── screenshots/
│ └── logs/


---

## 👤 Author

**John Ofulue**  
Cybersecurity Analyst & Instructor 

---

## 📬 Contact

- LinkedIn: (https://linkedin.com/in/john-ofulue)  
- GitHub: (https://github.com/neptune430)  

---

## ⭐ Final Note

This project reflects my ability to think like a security analyst — not just identifying threats, but understanding their impact and responding effectively.

---
