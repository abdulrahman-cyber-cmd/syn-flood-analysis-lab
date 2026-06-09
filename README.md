# TCP SYN Traffic Analysis Lab

## Overview

This project documents a controlled cybersecurity lab focused on analyzing TCP SYN traffic patterns, packet captures, and network behavior in a virtualized environment.

The purpose of this lab was to strengthen my understanding of:

- TCP/IP Networking
- TCP Three-Way Handshake
- Network Traffic Analysis
- Packet Inspection
- Security Monitoring
- Documentation and Reporting

> All activities were performed in a controlled and authorized lab environment for educational and defensive security learning purposes.

---

## Objectives

- Understand how TCP connections are established.
- Analyze TCP SYN packet behavior.
- Capture and inspect network traffic using Wireshark.
- Perform network discovery and service identification.
- Document observations and findings.
- Develop practical network analysis skills.

---

## Lab Environment

| Component | Description |
|------------|------------|
| Operating System | Kali Linux |
| Virtualization | VirtualBox |
| Network Analysis | Wireshark |
| Network Discovery | Nmap |
| Test Network | Isolated Lab Environment |

---

## Network Topology

![Network Topology](screenshots/topology.png)

---

## Host Discovery

Host discovery was performed to identify active systems within the lab network.

### Command Used

```bash
nmap -sn 10.20.30.0/24
```

### Results

![Host Discovery](screenshots/host-discovery.png)

### Key Observations

- Multiple hosts were identified within the subnet.
- ICMP and ARP responses were used to determine active systems.
- Baseline network visibility was established before further analysis.

---

## Service Enumeration

Service discovery was conducted to identify accessible services and open ports.

### Example Command

```bash
nmap -sV <target-ip>
```

### Objectives

- Identify running services
- Determine service versions
- Understand network exposure

---

## Traffic Analysis

Network traffic was captured and analyzed using Wireshark.

### Wireshark Capture

![Wireshark Analysis](screenshots/wireshark-analysis.png)

### Analysis Focus

- TCP SYN packets
- TCP ACK packets
- Connection establishment process
- Network communication patterns

### Observations

- TCP traffic patterns were clearly visible.
- Three-way handshake behavior could be observed.
- Packet-level visibility provided insight into network communications.

---

## Findings Summary

![Findings Summary](screenshots/findings-summary.png)

### Key Findings

- TCP SYN packets were successfully identified in packet captures.
- Network traffic analysis provided visibility into connection behavior.
- Host discovery techniques identified active systems within the subnet.
- Packet inspection helped understand communication patterns.
- Documentation and analysis are essential components of cybersecurity investigations.

---

## Skills Demonstrated

### Technical Skills

- Network Analysis
- Wireshark
- Nmap
- Linux Administration
- TCP/IP Networking
- Packet Inspection
- Security Monitoring

### Professional Skills

- Technical Documentation
- Cybersecurity Reporting
- Investigation Methodology
- Analytical Thinking
- Problem Solving

---

## Lessons Learned

This lab reinforced several important cybersecurity concepts:

- Understanding network protocols is fundamental for defenders.
- Traffic analysis provides valuable visibility into system communications.
- Packet captures can reveal abnormal network behavior.
- Proper documentation improves investigation quality and reproducibility.

---

## Future Improvements

- Explore automated traffic detection techniques.
- Create custom detection rules.
- Analyze additional protocol behavior.
- Expand the lab with multiple network segments.
- Implement monitoring and alerting solutions.

---

## Project Structure

```text
tcp-syn-traffic-analysis-lab
│
├── README.md
│
├── screenshots
│   ├── topology.png
│   ├── host-discovery.png
│   ├── wireshark-analysis.png
│   └── findings-summary.png
│
└── findings.md
```

---

## Disclaimer

This project was conducted in a controlled and authorized lab environment for educational and defensive security learning purposes only.

No unauthorized systems or networks were targeted.

---

## Author

**Abdul Rahman Siddiqui**

Cybersecurity Student | Network Security Enthusiast | SOC Analyst Aspirant

GitHub: https://github.com/YOUR_USERNAME
LinkedIn: https://linkedin.com/in/YOUR_PROFILE
