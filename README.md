# Wireshark Network Traffic Analysis

## Overview

This repository documents my hands-on learning and practical experience with Wireshark in a controlled cybersecurity lab environment. The objective of this project was to understand how network communication occurs at the packet level and to develop practical network traffic analysis skills used in Security Operations Centers (SOC), Incident Response, Digital Forensics, and Penetration Testing.

Throughout this lab, I captured and analyzed real network traffic generated from web browsing and interactions with the OWASP Juice Shop training application. The focus was on understanding how protocols communicate, how requests and responses are transmitted, and how security analysts investigate network activity.

---

## Lab Environment

* Operating System: Kali Linux
* Network Analysis Tool: Wireshark
* Target Application: OWASP Juice Shop
* Browser: Firefox
* Network Interface: any / eth0 (depending on capture scenario)
* Environment: Controlled local lab

---

## Objectives

* Learn packet-level network analysis.
* Understand protocol encapsulation.
* Analyze client-server communication.
* Capture and inspect HTTP and DNS traffic.
* Understand TCP connection establishment and termination.
* Investigate web application requests and responses.
* Develop foundational skills for SOC analysis and incident response.

---

## Topics Covered

### 1. Introduction to Packet Analysis

* Wireshark interface
* Packet List pane
* Packet Details pane
* Packet Bytes pane
* Frame structure

### 2. Network Protocol Layers

* Ethernet II
* IPv4
* TCP
* UDP
* HTTP
* DNS
* TLS

### 3. TCP Analysis

* Three-way handshake
* Connection termination
* Sequence numbers
* Acknowledgment numbers
* Window size
* TCP flags (SYN, ACK, FIN, RST)

### 4. DNS Analysis

* Standard DNS queries
* A records
* AAAA records
* DNS responses
* Domain resolution

### 5. HTTP Analysis

* HTTP GET requests
* HTTP POST requests
* HTTP response analysis
* HTTP status codes
* Request and response headers

### 6. HTTP Stream Reconstruction

* Reconstructing complete HTTP conversations
* Understanding request/response flow
* Session analysis using Follow HTTP Stream

### 7. Web Application Traffic Analysis

* Login requests
* SQL injection traffic
* File upload requests
* HTTP form-data inspection

### 8. Traffic Filtering

* DNS filters
* HTTP filters
* TCP filters
* IP address filters
* Port-based filtering

### 9. Network Statistics

* Protocol Hierarchy
* Conversations
* Endpoints
* High-level traffic analysis

---

## Skills Demonstrated

* Network traffic analysis
* Packet inspection
* Protocol analysis
* TCP/IP fundamentals
* DNS investigation
* HTTP analysis
* Session reconstruction
* Web application traffic analysis
* Display filtering
* Protocol hierarchy interpretation
* Conversation analysis
* Endpoint analysis
* Basic incident investigation methodology

---

## Repository Evidence

The repository contains screenshots demonstrating practical analysis of:

* Wireshark interface
* Packet analysis
* DNS queries and responses
* TCP three-way handshake
* HTTP GET requests
* HTTP POST requests
* HTTP responses
* HTTP stream reconstruction
* SQL injection traffic
* Display filters

---

## Key Learning Outcomes

This project strengthened my understanding of how data moves across a network, how protocols interact within the TCP/IP stack, and how network analysts investigate communications at the packet level. I learned how to identify normal web traffic, reconstruct HTTP conversations, analyze DNS lookups, inspect TCP sessions, and observe how web application activities such as file uploads and SQL injection attempts appear in captured traffic.

These practical exercises provide a strong foundation for more advanced areas of cybersecurity, including Network Security Monitoring, Security Operations Center (SOC) analysis, Incident Response, Malware Traffic Analysis, Digital Forensics, and Threat Hunting.

---

## Next Steps

This repository is the first stage of my network analysis learning journey.

Upcoming projects include:

* Zeek Network Security Monitoring
* Suricata Intrusion Detection System
* SIEM (Splunk / Elastic)
* Incident Response
* Malware Traffic Analysis
* Digital Forensics
* Threat Hunting
