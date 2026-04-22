# 🔎 Nmap Reconnaissance & Enumeration Lab

## 👨‍💻 Author

Sabrina Major

---

## 🎯 Objective

The goal of this lab was to perform network reconnaissance against a vulnerable system to identify open ports, running services, and potential security risks.

---

## 🛠 Tools Used

* Kali Linux
* Nmap
* Metasploitable2

---

## 🌐 Lab Environment

* Attacker Machine: Kali Linux
* Target Machine: Metasploitable2
* Network: Local Virtual Network

---

## ⚙️ Methodology

### 1. Connectivity Test

```bash
ping <target-ip>
```

---

### 2. Nmap Scan

```bash
nmap -sC -sV -vv <target-ip>
```

---

### 3. Enumeration

* Identified open ports
* Detected running services
* Collected version information

---

## 🔍 Key Findings

* FTP (Port 21) → Anonymous login enabled
* SSH (Port 22) → Outdated version
* Telnet (Port 23) → Insecure protocol
* HTTP (Port 80) → Apache server
* MySQL (Port 3306) → Database exposed

---

## ⚠️ Security Observations

* Multiple outdated services
* Weak authentication mechanisms
* High attack surface

---

## 🛡️ SOC Analyst Perspective

This type of scan would generate:

* IDS alerts for port scanning
* Firewall logs showing repeated connection attempts
* Suspicious traffic patterns

---

## 📸 Screenshots

(Add your screenshots later)

---

## 📚 Skills Gained

* Network reconnaissance
* Service enumeration
* Vulnerability identification
* Threat awareness

---

## 🧠 What I Learned

This lab showed how attackers can quickly gather valuable information about a system. Even without exploiting anything, identifying open ports and services provides a roadmap for potential attacks.

---
