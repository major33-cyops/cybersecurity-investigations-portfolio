# AI Prompt Firewall & Security Controls Analysis

## Overview
In this project, I developed a simple “prompt firewall” to demonstrate how security controls can be used to detect and block malicious or unsafe input before it reaches a system. The goal was to simulate how modern security tools enforce rules, filter input, and generate alerts in a controlled environment.

This project combines secure coding, input validation, logging, and alerting to reflect how real-world systems reduce risk and support security operations.

---

## Objective
- Implement input validation as a security control  
- Detect and block suspicious or malicious user input  
- Create logging for monitoring system activity  
- Simulate alerting based on repeated suspicious behavior  
- Understand how controls support SOC workflows  

---

## Environment
- Ubuntu Virtual Machine  
- Python-based firewall logic  
- Command-line interface  
- Local log file monitoring  

---

## Methodology
- Built a filtering system to inspect user input  
- Defined a blacklist of suspicious keywords  
- Implemented input length restrictions  
- Logged all user activity (allowed and blocked)  
- Triggered alerts after repeated suspicious attempts  

---

## Security Controls Implemented

### Input Validation (Preventive Control)
- Blocks high-risk keywords such as:
  - bypass  
  - ignore  
  - password  
- Prevents unauthorized or unsafe input from being processed  

### Length Restriction (Preventive Control)
- Blocks unusually long inputs that may indicate abuse or injection attempts  

### Logging (Detective Control)
- Records:
  - Allowed inputs  
  - Blocked inputs  
  - Alert-triggering activity  
- Provides visibility into system behavior  

### Alerting (Detective Control)
- Triggers alerts after repeated suspicious inputs  
- Simulates escalation conditions used in real security environments  

---

## Example Detection Logic
- If input contains restricted keywords → BLOCK  
- If input exceeds defined length → BLOCK  
- If repeated suspicious input occurs → ALERT triggered  

---

## Example Scenario
A user attempts to bypass system restrictions:

1. User enters restricted keyword (e.g., "bypass")  
2. System detects keyword match  
3. Input is immediately blocked  
4. Event is logged  
5. After multiple attempts, an alert is triggered  

---

## Key Findings
- Simple controls can significantly reduce system risk  
- Input validation is a critical first layer of defense  
- Logging enables visibility into potentially malicious behavior  
- Repeated activity patterns can indicate malicious intent  

---

## SOC Analyst Relevance
This project directly reflects how SOC teams monitor and defend systems.

SOC analysts must:
- Review logs for suspicious patterns  
- Identify repeated malicious behavior  
- Respond to alerts triggered by detection systems  
- Understand how security controls reduce attack surface  

### Example SOC Impact
- Blocked input → potential attack attempt  
- Repeated violations → possible malicious actor  
- Log entries → evidence for investigation  

---

## Skills Demonstrated
- Security control implementation  
- Input validation techniques  
- Threat detection logic  
- Log analysis  
- Alerting and monitoring concepts  
- Secure coding fundamentals  

---

## Screenshots

### Firewall Blocking Suspicious Input
![Firewall Block](screenshots/firewall-block.png)

### Firewall Detection Logic (Code)
![Firewall Code](screenshots/firewall-code.png)

### Firewall Running in Ubuntu Environment
![Ubuntu Firewall](screenshots/ubuntu-firewall-run.png)

### Log Output and Alert Detection
![Log Output](screenshots/log-analysis-output.png)

---

## What I Learned
This project showed that effective security is not only about detecting attacks, but preventing them before they happen. Even simple controls like input filtering, logging, and alerting can significantly reduce risk when applied correctly.

It also reinforced how security controls support SOC operations by providing visibility, detection, and response capabilities.

---

## Notes
All configurations and scenarios in this project are based on a simulated environment for educational purposes.
