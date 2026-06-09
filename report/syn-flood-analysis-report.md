# TCP SYN Traffic Analysis Lab Report

## Executive Summary

This report documents a controlled cybersecurity lab focused on network traffic analysis and TCP communication monitoring. The primary objective was to observe TCP connection behavior, analyze packet captures, and gain hands-on experience with network monitoring tools in an isolated environment.

The lab provided practical exposure to network discovery, packet inspection, and traffic analysis techniques commonly used by cybersecurity professionals and Security Operations Center (SOC) analysts.

---

# Objectives

The objectives of this lab were to:

* Understand the TCP/IP communication process.
* Analyze the TCP three-way handshake.
* Perform host discovery within a local network.
* Capture and inspect network traffic.
* Develop practical experience using Wireshark and Nmap.
* Document observations and findings.

---

# Lab Environment

| Component               | Description              |
| ----------------------- | ------------------------ |
| Operating System        | Kali Linux               |
| Virtualization Platform | VirtualBox               |
| Network Analysis Tool   | Wireshark                |
| Network Discovery Tool  | Nmap                     |
| Network Type            | Isolated Lab Environment |

---

# Methodology

## Phase 1: Network Discovery

Host discovery techniques were used to identify active devices within the network.

### Command Used

```bash
nmap -sn 10.20.30.0/24
```

### Purpose

* Identify active hosts
* Establish network visibility
* Create a baseline inventory of devices

---

## Phase 2: Service Enumeration

Network services were identified to understand the communication capabilities of discovered systems.

### Command Used

```bash
nmap -sV <target-ip>
```

### Purpose

* Identify open ports
* Detect running services
* Understand network exposure

---

## Phase 3: Traffic Capture

Wireshark was used to capture network traffic generated during testing.

### Activities Performed

* Packet capture initiation
* TCP traffic monitoring
* Traffic filtering
* Packet inspection

### Filter Example

```text
tcp
```

---

## Phase 4: Traffic Analysis

Captured traffic was analyzed to identify communication patterns and protocol behavior.

The analysis focused on:

* Source and destination hosts
* TCP SYN packets
* TCP ACK packets
* Connection establishment behavior
* Communication timing

---

# Observations

## Host Discovery

* Active systems were successfully identified within the subnet.
* Network visibility was established prior to traffic analysis.
* Devices responded as expected during discovery operations.

## TCP Communication

* TCP SYN packets were observed during connection establishment.
* Communication flows followed expected TCP behavior.
* Source and destination addressing information was visible in packet captures.

## Packet Analysis

* Packet captures provided detailed visibility into network activity.
* Traffic flows could be correlated to specific hosts.
* Wireshark enabled detailed inspection of protocol behavior.

## Monitoring Capabilities

* Network monitoring tools provided real-time visibility into traffic patterns.
* Endpoint communication could be identified and analyzed.
* Traffic filtering improved investigation efficiency.

---

# Findings

### Finding 1

TCP traffic patterns can be effectively analyzed using packet capture tools to understand communication behavior and network activity.

### Finding 2

Host discovery techniques provide valuable visibility into network assets and active devices.

### Finding 3

Packet-level inspection allows security analysts to identify communication flows and investigate network events.

### Finding 4

Establishing a baseline of normal network activity is important for identifying future anomalies.

### Finding 5

Effective documentation improves investigation quality and supports knowledge sharing.

---

# Skills Demonstrated

## Technical Skills

* TCP/IP Networking
* Wireshark Analysis
* Network Discovery
* Linux Administration
* Packet Inspection
* Traffic Analysis
* Security Monitoring

## Professional Skills

* Technical Documentation
* Analytical Thinking
* Problem Solving
* Investigation Methodology
* Reporting and Communication

---

# Lessons Learned

This lab reinforced several important cybersecurity concepts:

* Understanding network protocols is essential for security monitoring.
* Packet captures provide valuable visibility into network communications.
* Host discovery techniques help establish situational awareness.
* Documentation is a critical component of cybersecurity investigations.
* Practical hands-on experience improves understanding of networking concepts.

---

# Conclusion

The TCP SYN Traffic Analysis Lab successfully demonstrated fundamental networking and traffic analysis concepts in a controlled environment. Through host discovery, packet capture, and protocol analysis, valuable insights were gained into TCP communication behavior and network monitoring practices.

The lab strengthened practical cybersecurity skills while providing experience with industry-standard tools such as Wireshark and Nmap. These skills are directly applicable to network security monitoring, SOC operations, and incident investigation activities.

---

# Disclaimer

This lab was conducted in a controlled and authorized environment for educational and defensive cybersecurity learning purposes only. All testing activities were performed on systems and networks where authorization was granted.

