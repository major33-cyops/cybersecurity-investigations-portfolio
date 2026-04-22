# Linux Log Analysis Lab

## Author
Sabrina Major

---

## Overview
This lab demonstrates how Linux logs and volatile system data can be used to investigate suspicious activity after a system compromise. The focus of this lab was reviewing authentication logs, login history, running processes, and network information to better understand what happened on the target system.

---

## Objective
- Review Linux log files for signs of suspicious activity
- Analyze authentication events and login history
- Collect volatile data useful for incident response
- Practice investigation steps used in real-world SOC and incident response workflows

---

## Lab Environment
- Attacker System: Kali Linux
- Target System: Ubuntu Server
- Tools Used: Metasploit, Python3 HTTP server, Linux CLI tools

---

## Scenario
In this lab, I simulated a compromise against a Linux server and then shifted into the defender role to investigate the incident. After the target system was compromised, I collected volatile evidence and reviewed important Linux log sources to identify signs of intrusion and account activity.

---

## Investigation Steps

### 1. Initial Compromise Evidence
A reverse shell session was established from the Ubuntu target back to the Kali attacker machine. This demonstrated how an attacker could gain remote access to a system.

![Incident Session](screenshots/incident-session.png)

This screenshot shows evidence of the compromise and confirms that the target system was successfully accessed.

---

### 2. Authentication Log Review
I reviewed the Linux authentication log to identify login-related activity, authentication attempts, and other security-relevant events.

![auth.log Review](screenshots/auth-log-review.png)

The `auth.log` file is important because it can reveal authentication attempts, account usage, and privileged activity.

---

### 3. Failed Login Analysis
I reviewed failed login attempts using the `btmp` history to identify unsuccessful authentication activity.

![Failed Login History](screenshots/failed-login-history.png)

Failed login history is useful for spotting brute-force attempts, invalid credential usage, or suspicious access patterns.

---

### 4. Successful Login History
I reviewed login history using `wtmp` / `last` output to understand which accounts accessed the system and when.

![Login History](screenshots/login-history.png)

This helps build a timeline of account activity during an investigation.

---

### 5. Process Analysis
I collected information about running processes to identify what was active on the system after compromise.

![Process Review](screenshots/process-review.png)

Running processes can reveal suspicious activity, attacker persistence, or unusual commands that may have executed after compromise.

---

### 6. Network and System Details
I documented network interface details and routing information as part of the volatile data collection process.

![Network Details](screenshots/network-details.png)

This information helps responders understand active connections, host configuration, and possible attacker communication paths.

---

### 7. Evidence Documentation
I recorded findings in a report file during the investigation to preserve observations and organize collected evidence.

![Evidence Report](screenshots/evidence-report.png)

Documenting evidence is an important part of incident response because it supports analysis, escalation, and reporting.

---

## Key Findings
- The target system was successfully compromised through a malicious executable.
- Authentication and login records provided useful evidence for reviewing activity on the system.
- Volatile data such as processes, interfaces, and routing information helped capture the state of the machine after compromise.
- Reviewing Linux logs is a critical step in understanding attacker behavior and building an incident timeline.

---

## SOC Analyst Perspective
This lab reflects real SOC and incident response work because analysts often:
- Review authentication logs for suspicious activity
- Check failed and successful login history
- Collect volatile evidence before reboot or shutdown
- Analyze processes and network information during an investigation
- Build a timeline from system artifacts

---

## Skills Demonstrated
- Linux log analysis
- Incident response fundamentals
- Authentication event review
- Volatile data collection
- Process analysis
- Network awareness
- Evidence documentation

---

## Tools Used
- Kali Linux
- Ubuntu Server
- Metasploit
- Python3 HTTP Server
- auth.log
- btmp
- wtmp / last
- Linux command-line utilities

---

## What I Learned
This lab helped me understand how defenders investigate a compromised Linux system by reviewing logs, login history, processes, and network details. It strengthened my understanding of how attackers gain access and how responders collect evidence to understand what happened.

---
