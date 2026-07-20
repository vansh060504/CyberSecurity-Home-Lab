# Nmap

## Introduction

Nmap (Network Mapper) is one of the most widely used open-source network reconnaissance tools in cybersecurity. It is designed to discover hosts, identify open ports, detect running services, determine operating systems, and gather valuable information about target systems.

Nmap is commonly used by penetration testers, security analysts, network administrators, and incident responders to understand network infrastructure and identify potential attack surfaces.

Within this cybersecurity home lab, Nmap was used from Kali Linux to perform reconnaissance against Windows Server 2019 and Metasploitable 2 inside an isolated VMware environment.

---

# Why Nmap?

Reconnaissance is the first phase of almost every penetration test.

Before interacting with a target system, security professionals need to identify:

- Whether the host is online
- Open ports
- Running services
- Service versions
- Operating system
- Possible vulnerabilities

Nmap provides this information quickly and accurately, making it one of the most important tools in cybersecurity.

---

# Lab Environment

The scans documented in this file were performed only inside my isolated VMware home lab.

Environment:

| Machine | Purpose |
|---------|---------|
| Kali Linux | Scanning Machine |
| Windows Server 2019 | Windows Target |
| Metasploitable 2 | Vulnerable Linux Target |

No public or unauthorized systems were scanned.

---

# Basic Host Discovery

## Objective

Determine whether a target system is reachable.

## Command

```bash
ping <target-ip>
```

or

```bash
nmap -sn <target-ip>
```

## Explanation

Host discovery identifies active devices on the network before performing detailed scans.

## Learning Outcome

Verified communication between virtual machines inside the isolated laboratory.

---

# TCP Port Scan

## Objective

Identify open TCP ports on the target system.

## Command

```bash
nmap <target-ip>
```

## Explanation

This is the default Nmap scan. It checks the most common TCP ports and reports whether they are open, closed, or filtered.

## Information Collected

- Open ports
- Closed ports
- Host availability

## Security Significance

Open ports represent services that may be accessible to attackers.

---

# Service Version Detection

## Objective

Identify services running on open ports.

## Command

```bash
nmap -sV <target-ip>
```

## Explanation

The `-sV` option performs service version detection by communicating with open ports and identifying the applications running on them.

## Information Collected

- Service name
- Version number
- Product information

## Security Significance

Knowing the exact software version helps determine whether known vulnerabilities exist.

---

# Operating System Detection

## Objective

Identify the target operating system.

## Command

```bash
sudo nmap -O <target-ip>
```

## Explanation

Operating system detection uses TCP/IP fingerprinting techniques to estimate the target operating system.

## Information Collected

- Operating system family
- Device type
- Network distance

## Security Significance

Operating system identification helps security professionals understand the target environment before further assessment.

---

# Aggressive Scan

## Objective

Collect as much information as possible in a single scan.

## Command

```bash
sudo nmap -A <target-ip>
```

## Explanation

The `-A` option enables:

- OS Detection
- Version Detection
- Script Scanning
- Traceroute

## Security Significance

Aggressive scans provide detailed reconnaissance data that can assist in vulnerability assessment.

---

# Scan All TCP Ports

## Objective

Scan every TCP port on the target system.

## Command

```bash
sudo nmap -p- <target-ip>
```

## Explanation

Instead of scanning only the default ports, this scan checks all 65,535 TCP ports.

## Security Significance

Services running on uncommon ports can sometimes be overlooked during standard scans.

---

# UDP Scan

## Objective

Identify UDP services.

## Command

```bash
sudo nmap -sU <target-ip>
```

## Explanation

Many important services use UDP instead of TCP.

Examples include:

- DNS
- DHCP
- SNMP
- NTP

## Security Significance

UDP services are frequently forgotten during security assessments.

---

# Saving Scan Results

## Command

```bash
nmap -oN scan.txt <target-ip>
```

## Explanation

Stores scan results in normal text format for later analysis.

Other output formats include:

```bash
-oX
```

(XML)

```bash
-oG
```

(Grepable)

```bash
-oA
```

(All formats)

---

# Practical Learning

During this home lab I performed:

- Host discovery
- Port scanning
- Service enumeration
- Operating system detection
- Version detection
- Result analysis

The information collected from Nmap scans was later used during vulnerability assessment and controlled exploitation exercises.

---

# Learning Outcomes

Using Nmap in this home lab helped me develop practical experience with:

- Network reconnaissance
- Host discovery
- Port scanning
- Service identification
- Operating system fingerprinting
- Attack surface analysis
- Reconnaissance methodology

Nmap served as the foundation for subsequent security testing activities and significantly improved my understanding of how attackers and defenders analyze networked systems.

---

# Conclusion

Nmap was one of the primary tools used throughout this cybersecurity home lab. It enabled accurate reconnaissance, service discovery, and target identification while reinforcing the importance of careful information gathering before performing any security assessment.

All scans documented in this repository were conducted exclusively within my isolated VMware-based laboratory environment for educational purposes.
