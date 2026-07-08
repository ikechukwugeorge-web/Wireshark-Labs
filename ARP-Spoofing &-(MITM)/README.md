ARP Spoofing & Man-in-the-Middle (MITM) Attack
Overview
---------
Demonstrated network-level Man-in-the-Middle attack using ARP Spoofing to intercept traffic between a victim device and the gateway.
-------------

Tools Used
-----------

Bettercap,
Wireshark,
Kali Linux (Bridged Adapter)

Methodology & Steps
---------------------

Network Discovery
Used nmap -sn 192.168.43.0/24 to identify live hosts on the network.
ARP Spoofing Setup
Enabled IP forwarding:Bashsudo sysctl -w net.ipv4.ip_forward=1
MITM Execution
Launched Bettercap and performed ARP poisoning:textnet.probe on
net.show
set arp.spoof.targets 192.168.43.23
arp.spoof on
Traffic Analysis
Captured traffic in Wireshark on the eth0 interface while the victim device was active.

Key Findings
-------------

Successfully poisoned ARP tables, forcing the victim's traffic through the attacker machine.
Observed DNS queries, HTTP requests, and other network activity from the victim device.

What I Learned
----------------

How ARP protocol works and how it can be abused for MITM attacks.
The importance of network segmentation and ARP inspection (DAI) as defenses.
How to use Bettercap for modern network attacks.
Understanding of network traffic analysis using Wireshark.

Security Takeaways
----------------------

Use static ARP entries or Dynamic ARP Inspection (DAI) on switches.
Implement network segmentation to limit lateral movement.
Educate users about risks of connecting to untrusted networks.
