# Wireshark

## Introduction

Wireshark is a widely used open-source network protocol analyzer that captures and analyzes network traffic in real time. It allows security professionals to inspect packets, troubleshoot network issues, investigate suspicious activity, and understand communication between systems.

Within this cybersecurity home lab, Wireshark was used to capture and analyze network traffic generated between Kali Linux, Windows Server 2019, and Metasploitable 2 inside an isolated VMware environment.

---

# Why Wireshark?

Understanding network traffic is an essential cybersecurity skill.

Wireshark helps security professionals:

- Monitor network communication
- Analyze protocols
- Detect suspicious traffic
- Investigate security incidents
- Troubleshoot connectivity issues
- Learn how applications communicate

Packet analysis is commonly performed by SOC analysts, incident responders, penetration testers, and network administrators.

---

# Lab Environment

The following virtual machines were used during packet analysis.

| Machine | Purpose |
|---------|---------|
| Kali Linux | Packet Capture & Analysis |
| Windows Server 2019 | Windows Traffic |
| Metasploitable 2 | Vulnerable Linux Target |
| VMware Workstation 17 Player | Virtualization Platform |

All traffic was captured within an isolated virtual network.

---

# Starting Wireshark

## Objective

Capture packets from the virtual network interface.

## Steps

1. Open Wireshark.
2. Select the VMware network adapter.
3. Start packet capture.
4. Generate traffic between virtual machines.
5. Stop the capture for analysis.

## Learning Outcome

Successfully captured network traffic generated inside the virtual laboratory.

---

# Packet Capture

## Objective

Record network communication for analysis.

Captured traffic included:

- ICMP
- TCP
- UDP
- DNS
- HTTP
- ARP

Capturing packets allows investigators to understand how systems communicate and identify abnormal behavior.

---

# ICMP Analysis

## Display Filter

```text
icmp
```

## Purpose

ICMP packets are commonly generated during ping requests.

## Observation

Used to verify communication between virtual machines.

## Security Significance

ICMP can be used for:

- Connectivity testing
- Network mapping
- Host discovery

---

# TCP Analysis

## Display Filter

```text
tcp
```

## Purpose

Displays all TCP traffic.

## Observation

Observed TCP three-way handshakes and communication between systems.

## Security Significance

Understanding TCP sessions helps identify:

- Normal connections
- Unexpected communications
- Service activity

---

# UDP Analysis

## Display Filter

```text
udp
```

## Purpose

Displays UDP packets.

## Observation

Captured UDP-based protocol traffic generated within the lab.

## Security Significance

Many infrastructure services rely on UDP, making it important during investigations.

---

# DNS Analysis

## Display Filter

```text
dns
```

## Purpose

Analyze DNS requests and responses.

## Observation

Observed hostname resolution performed by systems inside the laboratory.

## Security Significance

DNS analysis helps identify:

- Malicious domains
- Suspicious DNS requests
- Data exfiltration attempts
- Malware communication

---

# HTTP Analysis

## Display Filter

```text
http
```

## Purpose

View HTTP communication.

## Observation

Captured HTTP requests between systems.

## Security Significance

HTTP analysis helps investigators identify:

- Web browsing activity
- File downloads
- Unencrypted credentials
- Application communication

---

# ARP Analysis

## Display Filter

```text
arp
```

## Purpose

Analyze address resolution traffic.

## Observation

Observed MAC address resolution between virtual machines.

## Security Significance

ARP traffic can help detect:

- ARP spoofing
- Duplicate IP addresses
- Network mapping

---

# Useful Display Filters

| Filter | Description |
|---------|-------------|
| icmp | Show ICMP packets |
| tcp | Show TCP packets |
| udp | Show UDP packets |
| dns | Show DNS traffic |
| http | Show HTTP traffic |
| arp | Show ARP packets |
| ip.addr == 192.168.x.x | Filter by IP address |
| tcp.port == 80 | Filter by TCP port |
| tcp.port == 22 | SSH traffic |
| tcp.port == 445 | SMB traffic |

These filters simplify packet analysis during investigations.

---

# Practical Activities

During this project, Wireshark was used to:

- Capture network packets
- Analyze communication between virtual machines
- Verify connectivity
- Observe common network protocols
- Practice packet filtering
- Understand packet structure
- Inspect protocol headers

These exercises improved my ability to analyze network traffic within a controlled environment.

---

# Challenges Faced

While learning Wireshark, I encountered several challenges:

- Selecting the correct VMware network adapter
- Capturing traffic from the intended virtual machine
- Understanding protocol structures
- Interpreting packet details
- Applying appropriate display filters

Troubleshooting these issues improved my understanding of network communication and packet analysis.

---

# Skills Developed

Working with Wireshark helped strengthen my knowledge of:

- Packet analysis
- Network protocols
- Protocol filtering
- Traffic inspection
- Network troubleshooting
- Security investigation
- Communication analysis

---

# Learning Outcomes

Using Wireshark in this cybersecurity home lab improved my understanding of how devices communicate across a network and how packet analysis supports security monitoring, troubleshooting, and incident response.

The practical experience gained from analyzing real network traffic provides a strong foundation for future work in SOC operations and network security.

---

# Conclusion

Wireshark was an essential tool throughout this cybersecurity home lab, enabling detailed inspection of network traffic between virtual machines. By capturing and analyzing packets, I developed practical skills in protocol analysis, troubleshooting, and security investigation while reinforcing core networking concepts.

All packet captures and analyses documented in this repository were performed exclusively within an isolated VMware-based laboratory for educational purposes.
