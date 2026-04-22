

# 🔍 Projects & Investigations

---

## 🌐 IP Reputation Analysis (Threat Intelligence)

### Objective
Investigate a suspicious IP address using a threat intelligence platform.

### Key Findings
- IP Address: 185.177.72.38  
- Confidence of Abuse: 100%  
- Reports: 4,936  
- Location: France  
- Usage Type: Data Center / Hosting

📸 Evidence:
![AbuseIPDB Result](images/abuseipdb.png)
This screenshot shows the IP flagged with a 100% abuse confidence score, confirming malicious activity.

### Analysis
The IP shows strong indicators of malicious activity based on a high number of abuse reports and infrastructure commonly associated with automated attacks such as scanning and brute force attempts.

### Skills Demonstrated
- Threat Intelligence Analysis  
- IP Reputation Research  
- Risk Assessment  
- Cybersecurity Documentation  

---

## 🧪 SOC Log Analysis & Threat Detection Lab

### Objective
Simulate SOC analyst workflows by detecting suspicious login activity.
Note: All IP addresses and log data shown in this project are part of a simulated lab environment for educational purposes.

### Detection Logic Implemented
- IP repetition detection  
- Threat classification (Normal / Suspicious)  
- Impossible travel detection  
- High-value account monitoring  
- Risk scoring (Low / Medium / High)

📸 Evidence:
![Log Analysis Dashboard](images/log-analysis.png)
This simulated dashboard highlights suspicious login patterns, including repeated failed attempts and high-risk activity.

### Threats Identified
- Brute force attacks  
- Account compromise  
- Suspicious login patterns  
- Privileged account targeting  
- Geographic anomalies  

### Example Detection Logic
Threat Flag → Suspicious if repeated login attempts exceed threshold
Risk Level → Low / Medium / High based on behavior


---

### Skills Demonstrated
- Log Analysis  
- Pattern Recognition  
- Threat Detection  
- Risk Classification  
- SOC-style Alert Triage  
- Behavioral Analysis  
- MITRE ATT&CK Mapping  

---

### MITRE ATT&CK Mapping

| Behavior | Detection Focus | MITRE Mapping |
|----------|---------------|--------------|
| Failed logins | Password guessing | Brute Force |
| Admin targeting | Privilege abuse | Privilege Abuse |
| Success after failures | Credential compromise | Initial Access |
| Location anomalies | Suspicious login behavior | Account Compromise |
| Repeated IP activity | Automated attack patterns | Reconnaissance |

---

## 🚨 Cybersecurity Incident Response Report

📄 Full Report:  
[View Incident Response Report](Projects/incident-response-brute-force-analysis.md)

---

### Incident Title
Suspicious Login Activity and Potential Brute Force Attack

---

### Summary
A pattern of repeated failed login attempts followed by successful access from multiple international IP addresses indicated a likely brute force attack targeting both standard users and privileged accounts.

---

### Indicators of Compromise (IOCs)
- IP: 45.23.11.9 (Russia)  
- IP: 88.21.44.2 (China)  
- Multiple failed login attempts  
- Successful login after repeated failures  
- Admin account targeted  
- Suspicious geographic locations  

---

### Analysis
The behavior observed is consistent with brute force attack techniques:

- High volume of failed authentication attempts  
- Automated login attempts from repeated IP addresses  
- Successful authentication after multiple failures  
- Targeting of high-value accounts  

---

### Impact Assessment
- Potential unauthorized access to user accounts  
- Elevated risk due to admin account involvement  
- Possible exposure of sensitive system data  

---

### Mitigation Recommendations
- Block or blacklist malicious IP addresses  
- Enforce strong password policies  
- Enable Multi-Factor Authentication (MFA)  
- Monitor login behavior for anomalies  
- Implement account lockout policies  

---

### Skills Demonstrated
- Incident Analysis  
- Threat Detection  
- Log Analysis  
- Risk Assessment  
- SOC Workflow Understanding  

---

## 🎥 Project Presentation

Incident Response, Digital Forensics & Counterintelligence (TLT Internship Group Project)

Watch the presentation:

👉 https://youtu.be/14sSrcux18g

---

## 🧠 Key Takeaway
Effective cybersecurity relies on identifying patterns in system activity, correlating multiple indicators of compromise, and responding quickly to prevent escalation of threats.
