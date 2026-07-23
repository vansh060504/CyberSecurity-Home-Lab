# CyberSecurity Home Lab

![Cybersecurity](https://img.shields.io/badge/Cybersecurity-Home%20Lab-blue)
![VMware](https://img.shields.io/badge/VMware-Workstation%2017-orange)
![Kali Linux](https://img.shields.io/badge/Kali-Linux-557C94)
![Windows Server](https://img.shields.io/badge/Windows%20Server-2019-blue)
![Metasploitable](https://img.shields.io/badge/Metasploitable-2-red)
![Nmap](https://img.shields.io/badge/Nmap-Network%20Scanner-success)
![Metasploit](https://img.shields.io/badge/Metasploit-Framework-informational)
![Wireshark](https://img.shields.io/badge/Wireshark-Packet%20Analysis-blueviolet)
![License](https://img.shields.io/badge/License-MIT-yellow)

---

# Table of Contents

- [Overview](#overview)
- [Key Features](#key-features)
- [Lab Objectives](#lab-objectives)
- [Lab Architecture](#lab-architecture)
- [Virtual Machines](#virtual-machines)
- [Network Configuration](#network-configuration)
- [Cybersecurity Tools Used](#cybersecurity-tools-used)
- [Skills Demonstrated](#skills-demonstrated)
- [Documentation](#documentation)
- [Learning Outcomes](#learning-outcomes)
- [Future Improvements](#future-improvements)
- [Repository Statistics](#repository-statistics)
- [Repository Structure](#repository-structure)
- [Disclaimer](#disclaimer)

---

# Overview

This repository documents my personal CyberSecurity Home Lab built using VMware Workstation 17 Player to develop practical cybersecurity skills in a safe and isolated environment.

The lab simulates a small enterprise environment where I can perform network reconnaissance, service enumeration, vulnerability assessment, controlled exploitation, packet analysis, and Windows administration using industry-standard cybersecurity tools.

The environment consists of:

- Kali Linux (Security Testing Workstation)
- Windows Server 2019 (Windows Target)
- Metasploitable 2 (Intentionally Vulnerable Linux Machine)

This repository documents the lab architecture, technologies used, practical exercises performed, lessons learned, and the technical skills developed throughout the project.

---

# Key Features

- VMware-based virtual cybersecurity lab
- Isolated virtual network for safe testing
- Windows and Linux environments
- Network reconnaissance using Nmap
- Vulnerability validation using Metasploit Framework
- Packet analysis using Wireshark
- Windows Server administration
- Technical documentation for each lab component
- Practical cybersecurity learning environment

---

# Lab Objectives

The primary objective of this project is to develop practical cybersecurity skills through hands-on experience in a controlled laboratory environment.

This home lab was designed to:

- Build an isolated cybersecurity testing environment using VMware Workstation 17 Player
- Gain practical experience with Windows and Linux operating systems
- Practice network reconnaissance and service enumeration
- Learn vulnerability assessment methodologies
- Perform controlled exploitation in a safe environment
- Capture and analyze network traffic using Wireshark
- Strengthen networking and troubleshooting skills
- Improve technical documentation and cybersecurity reporting
- Develop a strong foundation in offensive and defensive security concepts

---

# Lab Architecture

The cybersecurity home lab consists of three virtual machines running within VMware Workstation 17 Player.

```text
                    Host Computer
                           │
              VMware Workstation 17 Player
                           │
      ┌────────────────────┼────────────────────┐
      │                    │                    │
      ▼                    ▼                    ▼

+----------------+  +------------------+  +------------------+
|   Kali Linux   |  | Windows Server   |  | Metasploitable 2 |
| Security Tools |  |      2019        |  | Vulnerable Linux |
+----------------+  +------------------+  +------------------+
```

Each virtual machine performs a specific role within the lab:

| Virtual Machine | Role |
|----------------|------|
| Kali Linux | Security testing and assessment |
| Windows Server 2019 | Windows administration and target system |
| Metasploitable 2 | Intentionally vulnerable Linux target |

The machines communicate through an isolated VMware virtual network, allowing safe experimentation with reconnaissance, enumeration, vulnerability validation, and packet analysis without interacting with production or public systems.

---

# Virtual Machines

## Kali Linux

Kali Linux serves as the primary security testing workstation within the lab.

It is used for:

- Network reconnaissance
- Port scanning
- Service enumeration
- Vulnerability assessment
- Controlled exploitation
- Packet analysis

Primary tools include:

- Nmap
- Metasploit Framework
- Wireshark

---

## Windows Server 2019

Windows Server 2019 acts as the Windows target system and administrative environment.

Practical activities included:

- Windows administration
- Local user management
- Event Viewer analysis
- Windows Firewall configuration
- Network configuration
- Security monitoring

Working with Windows Server provided practical experience with enterprise Windows administration and security concepts.

---

## Metasploitable 2

Metasploitable 2 is an intentionally vulnerable Linux virtual machine developed for cybersecurity education.

Within this lab it was used to practice:

- Host discovery
- Port scanning
- Service enumeration
- Vulnerability identification
- Controlled exploitation
- Security research

All activities were performed exclusively within the isolated laboratory environment.

---

# Network Configuration

All virtual machines are connected through VMware Workstation 17 Player using an isolated virtual network.

This configuration enables:

- Secure communication between virtual machines
- Network reconnaissance
- Service enumeration
- Packet capture and analysis
- Controlled vulnerability testing

The isolated network ensures that all testing remains confined to the home lab, preventing interaction with production environments or external systems.

---

# Cybersecurity Tools Used

The following technologies and tools were used throughout this home lab to build, manage, and assess the environment.

| Tool | Category | Purpose |
|------|----------|---------|
| VMware Workstation 17 Player | Virtualization | Hosts and manages the virtual lab environment |
| Kali Linux | Operating System | Security testing and penetration testing platform |
| Windows Server 2019 | Operating System | Windows administration and target environment |
| Metasploitable 2 | Vulnerable Machine | Intentionally vulnerable Linux system for security practice |
| Nmap | Network Reconnaissance | Host discovery, port scanning, and service enumeration |
| Metasploit Framework | Exploitation Framework | Controlled vulnerability validation and exploitation |
| Wireshark | Network Analysis | Packet capture and protocol analysis |

---

# Skills Demonstrated

This project demonstrates practical knowledge across multiple cybersecurity domains.

## Virtualization

- VMware Workstation 17 Player
- Virtual machine deployment
- Virtual hardware configuration
- Resource allocation
- Virtual networking

## Operating Systems

- Kali Linux
- Windows Server 2019
- Linux administration
- Windows administration

## Networking

- TCP/IP fundamentals
- Port scanning
- Service enumeration
- Network troubleshooting
- Packet analysis
- Virtual network configuration

## Cybersecurity

- Network reconnaissance
- Vulnerability assessment
- Controlled exploitation
- Traffic analysis
- Security documentation
- Home lab design

## Professional Skills

- Technical documentation
- Problem solving
- Research
- Continuous learning
- Hands-on laboratory practice

---

# Documentation

Comprehensive documentation for each component of the home lab is available in the **docs/** directory.

| Document | Description |
|----------|-------------|
| vmware.md | VMware installation, virtual machine configuration, and virtualization concepts |
| networking.md | Virtual networking concepts, adapters, and lab connectivity |
| kali-linux.md | Kali Linux installation, configuration, and security tools |
| windows-server.md | Windows Server installation, administration, and configuration |
| metasploitable-2.md | Purpose, setup, and role of the vulnerable Linux machine |
| nmap.md | Network discovery, port scanning, and enumeration techniques |
| metasploit.md | Metasploit Framework workflow and controlled exploitation concepts |
| wireshark.md | Packet capture, protocol analysis, and traffic inspection |

---

# Learning Outcomes

Building this cybersecurity home lab strengthened both my technical knowledge and practical skills.

Key learning outcomes include:

- Designing and managing an isolated virtual cybersecurity environment
- Deploying and configuring multiple operating systems
- Understanding virtual networking concepts
- Performing network reconnaissance and service enumeration
- Conducting vulnerability assessments in a controlled environment
- Capturing and analyzing network traffic
- Understanding exploitation workflows using Metasploit Framework
- Developing professional technical documentation
- Applying cybersecurity concepts through hands-on practice

This project reinforced the importance of practical experience in understanding how cybersecurity tools and techniques work together within a realistic laboratory environment.

---

# Future Improvements

This home lab will continue to evolve as I expand my cybersecurity knowledge and practical experience.

Planned enhancements include:

- Active Directory domain environment
- Windows 11 client deployment
- Sysmon log collection
- Splunk integration for centralized log analysis
- Wazuh SIEM deployment
- Sigma rule development
- Velociraptor endpoint monitoring
- Detection engineering use cases
- Threat hunting scenarios
- Additional vulnerable virtual machines

---

# Repository Statistics

| Metric | Value |
|---------|------:|
| Virtual Machines | 3 |
| Operating Systems | 3 |
| Cybersecurity Tools | 4 |
| Documentation Files | 8 |
| Virtualization Platform | VMware Workstation 17 Player |

---

# Repository Structure

```text
CyberSecurity-Home-Lab/
│
├── README.md
├── LICENSE
│
└── docs/
    ├── vmware.md
    ├── networking.md
    ├── kali-linux.md
    ├── windows-server.md
    ├── metasploitable-2.md
    ├── nmap.md
    ├── metasploit.md
    └── wireshark.md
```

---

# Technologies

- VMware Workstation 17 Player
- Kali Linux
- Windows Server 2019
- Metasploitable 2
- Nmap
- Metasploit Framework
- Wireshark

---

# Repository Goals

This repository was created to:

- Document the design and implementation of a personal cybersecurity home lab.
- Demonstrate practical cybersecurity skills through hands-on learning.
- Showcase technical documentation and laboratory management.
- Build a portfolio that reflects continuous learning and practical experience.
- Serve as a foundation for future cybersecurity projects and advanced lab environments.

---

# Disclaimer

This repository is intended solely for educational and portfolio purposes.

All practical exercises, vulnerability assessments, packet captures, reconnaissance, and controlled exploitation activities documented in this repository were performed exclusively within an isolated VMware-based home lab using personally managed virtual machines and intentionally vulnerable systems.

No unauthorized testing was conducted against production environments, public systems, third-party infrastructure, or organizational assets.

This repository does **not** contain:

- Production logs
- Internal IP addresses
- Organizational assets
- Client information
- Confidential data
- Proprietary configurations
- Vulnerability assessment reports from production environments

All examples, configurations, and documentation are based on a personal laboratory environment and are intended to demonstrate practical cybersecurity knowledge, responsible security practices, and continuous learning.

---

# License

This project is licensed under the **MIT License**.

See the **LICENSE** file for details.
