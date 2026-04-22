# Wireshark Traffic Analysis Lab

## Overview
In this lab, I used Wireshark to capture and analyze live network traffic in a controlled virtual environment. The goal was to understand how different network protocols operate, identify normal communication patterns, and build a foundation for detecting suspicious activity.

This lab focuses on analyzing ICMPv6, DNS, TCP, and HTTP/TLS traffic to simulate how a SOC analyst monitors and interprets network behavior.

---

## Objective
- Capture live network traffic using Wireshark  
- Analyze ICMPv6 communication patterns  
- Observe DNS resolution processes  
- Understand TCP 3-way handshake behavior  
- Examine HTTP and TLS web traffic  
- Identify normal vs expected network behavior  

---

## Environment
- Kali Linux VM  
- Wireshark Network Analyzer  
- Firefox Web Browser  
- Internet connectivity for traffic generation  

---

## Methodology
1. Started packet capture on active interface (eth0)  
2. Generated traffic using ping commands and web browsing  
3. Applied filters to isolate specific protocols  
4. Analyzed packet structure and communication patterns  
5. Identified normal behavior across multiple protocols  

---

## ICMPv6 Analysis

ICMPv6 traffic was generated using ping commands to test connectivity.

### Key Observations:
- Echo Request → system checking connectivity  
- Echo Reply → destination responding successfully  
- Neighbor Solicitation → device asking “who has this IP?”  
- Neighbor Advertisement → device responding with its identity  

### Analysis:
This traffic demonstrates normal network communication and device discovery. ICMPv6 plays a key role in connectivity testing and local network operations.

📸 ICMPv6 Traffic (Ping & Network Discovery)  
![ICMPv6 Analysis](screenshots/icmpv6-analysis.png)

This capture shows ICMPv6 traffic including echo requests and replies (ping), as well as neighbor discovery messages. This type of traffic is used to verify connectivity and allow devices to communicate on IPv6 networks.

---

## DNS Analysis

DNS traffic was captured while browsing websites.

### Key Observations:
- Standard queries for domains (e.g., google.com, mozilla services)  
- DNS responses returning IP addresses  
- Multiple queries generated automatically by browser services  

### Analysis:
DNS is responsible for translating domain names into IP addresses. This step occurs before any web connection is established and is critical in both normal operations and threat detection.

📸 DNS Traffic (Domain Name Resolution)  
![DNS Analysis](screenshots/dns-analysis.png)

This capture shows DNS queries and responses used to resolve domain names into IP addresses. For example, requests to domains such as Mozilla services demonstrate how systems locate servers before establishing connections.

---

## TCP Handshake Analysis

TCP traffic was analyzed to observe connection establishment.

### Key Observations:
- SYN → connection request  
- SYN-ACK → server acknowledgment  
- ACK → connection established  
- TLS Client Hello → beginning of encrypted communication  

### Analysis:
This represents the TCP 3-way handshake, which is used to establish reliable communication between systems. After the handshake, TLS encryption begins, limiting visibility into packet contents.

📸 TCP Handshake (Connection Establishment)  
![TCP Handshake](screenshots/tcp-handshake.png)

This capture also shows encrypted session initiation (TLS Client Hello), indicating the transition from TCP connection establishment to secure communication.

---

## HTTP / Web Traffic Analysis

HTTP traffic was analyzed during web browsing activity.

### Key Observations:
- HTTP GET requests  
- Server responses (200 OK, 301 Redirect, 404 Not Found)  
- OCSP traffic for certificate validation  

### Analysis:
HTTP traffic reveals user activity such as page requests and server responses. While HTTPS encrypts content, metadata such as destination and response behavior remains visible.

📸 HTTP Traffic (Web Requests & Responses)  
![HTTP Traffic](screenshots/http-traffic.png)

This capture shows HTTP requests and responses between the client and web servers. It includes GET requests and server responses such as 200 OK and 404 Not Found, representing normal web browsing activity.

---

## Key Findings
- Network communication follows predictable request/response patterns  
- DNS resolution is required before establishing web connections  
- TCP handshake establishes reliable communication channels  
- Most modern web traffic is encrypted (TLS), limiting payload visibility  
- Background traffic (multicast, neighbor discovery) is normal in active networks

---

## Additional Observations

📸 Initial Traffic Capture (Unfiltered View)  
![Initial Capture](screenshots/initial-capture-overview.png)

This screenshot shows raw network traffic before filtering. Multiple protocols such as ICMPv6 and ARP are visible, demonstrating baseline network communication.

📸 ARP Traffic (Local Network Discovery)  
![ARP Analysis](screenshots/arp-analysis.png)

This capture highlights ARP requests used to map IP addresses to MAC addresses within the local network. This is normal background traffic used for device discovery.

---

## SOC Analyst Relevance
This lab simulates real SOC workflows where analysts monitor network traffic to identify normal and abnormal behavior.

SOC analysts use tools like Wireshark to:
- Investigate suspicious connections  
- Analyze traffic patterns  
- Identify indicators of compromise  
- Correlate network activity with potential threats  

---

## Skills Demonstrated
- Packet capture and filtering  
- Network protocol analysis  
- Traffic pattern recognition  
- Basic threat awareness  
- Wireshark usage  

---

## What I Learned
This lab helped me understand how network communication works across multiple protocols and how to interpret packet-level data. I learned how to identify normal traffic patterns and how analysts rely on behavior and metadata when analyzing encrypted communications.

It reinforced that effective network analysis is not just about capturing data, but understanding how systems communicate and recognizing when something deviates from expected behavior.

---

## Next Steps
Future improvements to this lab will include:
- Simulating abnormal traffic (scanning, brute force attempts)  
- Comparing normal vs suspicious behavior  
- Expanding analysis to include anomaly detection  

---

## Notes
All traffic captured in this lab was generated in a controlled environment for educational purposes.
