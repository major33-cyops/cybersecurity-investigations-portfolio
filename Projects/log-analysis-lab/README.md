# SOC Log Analysis & Threat Detection Lab

## Objective
Simulate SOC analyst workflows by detecting suspicious login activity.

**Note:** All data in this project is simulated for educational purposes.

---

## Detection Logic Implemented
- IP repetition detection  
- Threat classification (Normal / Suspicious)  
- Impossible travel detection  
- High-value account monitoring  
- Risk scoring (Low / Medium / High)  

---

## Evidence
![Log Analysis Dashboard](screenshots/log-analysis.png)

This simulated dashboard highlights suspicious login patterns, including repeated failed attempts and high-risk activity.

---

## Threats Identified
- Brute force attacks  
- Account compromise  
- Suspicious login patterns  
- Privileged account targeting  
- Geographic anomalies  

---

## Example Detection Logic
Threat Flag → Suspicious if repeated login attempts exceed threshold  
Risk Level → Low / Medium / High based on behavior  

---

## Skills Demonstrated
- Log Analysis  
- Pattern Recognition  
- Threat Detection  
- Risk Classification  
- SOC-style Alert Triage  
- Behavioral Analysis  
- MITRE ATT&CK Mapping  

---

## MITRE ATT&CK Mapping

| Behavior | Detection Focus | MITRE Mapping |
|----------|---------------|--------------|
| Failed logins | Password guessing | Brute Force |
| Admin targeting | Privilege abuse | Privilege Abuse |
| Success after failures | Credential compromise | Initial Access |
| Location anomalies | Suspicious login behavior | Account Compromise |
| Repeated IP activity | Automated attack patterns | Reconnaissance |
