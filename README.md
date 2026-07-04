Wireshark Network Traffic Analysis

This repository documents my hands-on learning in network traffic analysis using Wireshark in a controlled lab environment. The focus is on understanding how network communication works at the packet level.

-------
What I Have Covered So Far
1. Introduction to Packet Analysis
Understanding how data is broken into packets
Interpreting Wireshark interface (packet list, details, and bytes view)
Identifying frame structure (Ethernet, IP, TCP layers)
2. TCP Fundamentals
TCP three-way handshake (SYN, SYN-ACK, ACK)
TCP connection termination (FIN, ACK, RST)
Sequence and acknowledgment numbers
Window size and flow control
3. Network Addressing
MAC addresses and Ethernet communication
IPv4 addressing and routing behavior
Source vs destination communication flow
4. Ports and Communication
Ephemeral ports vs server ports (e.g. 50402 → 443)
How multiple connections are handled by the OS
5. Protocol Identification
DNS traffic identification and resolution flow
HTTP vs HTTPS behavior
TLS encrypted traffic observation
6. Packet Inspection
Understanding packet size and frame structure
Reading raw hex data and decoded protocol layers
Identifying control packets (SYN, ACK, FIN, RST)
What I Learned

Through this lab, I developed an understanding of how:

Network communication is structured in layers (Ethernet → IP → TCP → Application)
A single web request generates multiple packets across different protocols
TCP ensures reliable delivery using sequence and acknowledgment numbers
Modern web traffic is mostly encrypted using TLS, limiting visibility of payload data
Network analysis requires interpreting relationships between packets, not just individual frames
