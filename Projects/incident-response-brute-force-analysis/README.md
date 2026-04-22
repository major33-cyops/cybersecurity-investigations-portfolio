# Incident Response Report – Brute Force Attack

## Overview
In this project, I analyzed a simulated security incident involving suspicious login activity consistent with a brute force attack. The goal was to investigate indicators of compromise, assess impact, and recommend mitigation strategies using a structured incident response approach.

---

## Key Takeaway (SOC Perspective)

This project demonstrates how SOC analysts identify attack patterns, correlate multiple indicators of compromise, and respond to unauthorized access attempts before they escalate.

---

## Incident Title
Suspicious Login Activity and Potential Brute Force Attack

---

## Incident Summary
A series of suspicious login attempts were detected involving repeated failed authentication attempts followed by successful logins. The activity originated from multiple international IP addresses and targeted both standard users and high-value administrative accounts.

This behavior strongly indicates a brute force attack that may have resulted in unauthorized access.

---

## Indicators of Compromise (IOCs)
- IP Address: 45.23.11.9 (Russia)  
- IP Address: 88.21.44.2 (China)  
- Multiple failed login attempts  
- Successful login after repeated failures  
- Targeting of admin account  
- Suspicious geographic login locations  

---

## Timeline of Events
1. Multiple failed login attempts detected  
2. Repeated attempts from same IP addresses  
3. Successful login after multiple failures  
4. Admin account accessed from suspicious location  
5. Continued login activity observed  

---

## Analysis
The behavior observed is consistent with a brute force attack, where an attacker attempts multiple password combinations to gain access.

Key indicators include:
- High volume of failed authentication attempts  
- Successful login after repeated failures  
- Repeated IP usage indicating automation  
- Targeting of privileged accounts  

Geographic anomalies further suggest possible account compromise or unauthorized access.

---

## Impact Assessment
- Potential unauthorized access to user accounts  
- Elevated risk due to admin account involvement  
- Possible exposure of sensitive data  
- Increased risk of further system compromise  

---

## Response Actions
- Identified suspicious login patterns  
- Flagged high-risk IP addresses  
- Classified threat severity  
- Highlighted critical activity involving admin accounts  

---

## Mitigation Recommendations
- Block or blacklist malicious IP addresses  
- Enforce strong password policies  
- Enable Multi-Factor Authentication (MFA)  
- Monitor login behavior for anomalies  
- Implement account lockout policies  

---

## SOC Analyst Relevance
This project reflects real SOC responsibilities, including:

- Investigating suspicious login activity  
- Identifying brute force attack patterns  
- Correlating multiple indicators of compromise  
- Assessing risk and escalation needs  

### Example SOC Impact
- Failed login patterns → brute force detection  
- Successful login after failures → account compromise risk  
- Admin targeting → high-severity incident  

---

## Skills Demonstrated
- Incident analysis  
- Threat detection  
- Log analysis  
- Risk assessment  
- SOC workflow understanding  

---

## What I Learned
This project reinforced the importance of identifying behavioral patterns in login activity. Repeated failed attempts, combined with geographic anomalies and eventual success, provide strong indicators of compromise.

It also demonstrated how structured incident response processes help analysts detect, investigate, and respond to threats efficiently.

---

## Notes
All scenarios and data in this project are based on a simulated environment for educational purposes.
