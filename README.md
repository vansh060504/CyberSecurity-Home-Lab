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

# Overview

This repository documents my personal Cybersecurity Home Lab built using VMware Workstation 17 Player. The lab was created to gain practical experience in virtualization, networking, penetration testing, vulnerability assessment, packet analysis, and Windows security within a safe and isolated environment.

Rather than learning security concepts only through theory, I designed this lab to simulate real-world systems where I could perform reconnaissance, network enumeration, vulnerability assessment, controlled exploitation, and traffic analysis using industry-standard cybersecurity tools.

The environment includes Kali Linux as the primary security testing machine, Windows Server 2019 as the Windows target system, and Metasploitable 2 as an intentionally vulnerable Linux machine for hands-on practice.

This repository documents the technologies used, the lab setup, practical exercises performed, lessons learned, and the skills developed while working in the environment.

---

# Features

- VMware-based virtual cybersecurity lab
- Multiple virtual machines running simultaneously
- Windows and Linux environments
- Network reconnaissance using Nmap
- Vulnerability validation using Metasploit Framework
- Network packet analysis using Wireshark
- Windows Server administration
- Practical cybersecurity documentation
- Safe isolated testing environment

---

# Lab Objectives

The primary goal of this project is to build practical cybersecurity skills through hands-on experience.

The objectives of this home lab include:

- Understand virtualization using VMware Workstation.
- Build an isolated cybersecurity testing environment.
- Practice Windows and Linux administration.
- Learn network reconnaissance techniques.
- Perform service enumeration.
- Analyze network traffic using Wireshark.
- Understand vulnerability assessment concepts.
- Practice controlled exploitation within an isolated lab.
- Improve troubleshooting and networking skills.
- Develop technical documentation skills.

---

# Lab Architecture

The home lab consists of three virtual machines running inside VMware Workstation 17 Player.

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

The virtual machines communicate within an isolated network, allowing security testing without impacting external systems. This controlled setup enables safe experimentation with network scanning, service enumeration, packet analysis, and other cybersecurity activities.

---

# Virtual Machines

## Kali Linux

Kali Linux serves as the primary security testing workstation within the lab. It contains numerous open-source security tools used for reconnaissance, enumeration, penetration testing, and network analysis.

Examples of tools used include:

- Nmap
- Metasploit Framework
- Wireshark

---

## Windows Server 2019

Windows Server 2019 provides a Windows-based environment for learning system administration and security monitoring. It is used to generate Windows events, understand server configuration, and practice security-related tasks within a controlled environment.

---

## Metasploitable 2

Metasploitable 2 is an intentionally vulnerable Linux virtual machine designed for cybersecurity education. It contains multiple vulnerable services that can be safely analyzed and tested inside the isolated lab.

It is used only within this personal laboratory environment for educational purposes.

---
# Network Configuration

The virtual machines are connected through VMware Workstation 17 Player, creating an isolated virtual network for security testing and experimentation. This configuration allows communication between the virtual machines while preventing unintended interaction with external production systems.

The lab network supports:

- Communication between Kali Linux and target systems
- Network reconnaissance
- Service enumeration
- Packet capture and analysis
- Controlled security testing

The isolated nature of the environment provides a safe platform for learning offensive and defensive cybersecurity concepts.

---

# Cybersecurity Tools Used

The following tools were used throughout this home lab.

| Tool | Purpose |
|------|---------|
| VMware Workstation 17 Player | Virtualization Platform |
| Kali Linux | Security Testing Operating System |
| Windows Server 2019 | Windows Target Environment |
| Metasploitable 2 | Vulnerable Linux Machine |
| Nmap | Network Discovery & Port Scanning |
| Metasploit Framework | Exploitation Framework |
| Wireshark | Network Packet Analysis |

---

# VMware Workstation

VMware Workstation 17 Player is used as the virtualization platform for hosting multiple operating systems simultaneously. It provides an isolated environment where cybersecurity experiments can be performed safely without affecting the host operating system.

Key benefits include:

- Virtual machine isolation
- Snapshot support (where available)
- Custom networking
- Resource allocation
- Safe testing environment

---

# Kali Linux

Kali Linux serves as the attack machine within the laboratory environment.

It contains numerous open-source cybersecurity tools used for:

- Network reconnaissance
- Enumeration
- Vulnerability assessment
- Security testing
- Packet analysis

Using Kali Linux allowed me to gain practical experience with widely used penetration testing and network analysis tools.

---

# Windows Server 2019

Windows Server 2019 was configured as the Windows target environment.

The server was used to understand:

- Windows administration
- Event Viewer
- User management
- Windows Firewall
- Network configuration
- Windows security concepts

Working with Windows Server provided valuable experience with enterprise operating system administration and security.

---

# Metasploitable 2

Metasploitable 2 is an intentionally vulnerable Linux virtual machine developed for cybersecurity education.

It provides numerous vulnerable services that enable students and security professionals to safely practice:

- Enumeration
- Vulnerability identification
- Controlled exploitation
- Service analysis
- Security research

All testing was performed exclusively within the isolated laboratory environment.

---

# Nmap

Nmap was used as the primary reconnaissance tool throughout the lab.

Activities performed included:

- Host discovery
- Port scanning
- Service version detection
- Operating system detection
- Network enumeration

These activities improved my understanding of network visibility and attack surface identification.

---

# Metasploit Framework

Metasploit Framework was used for controlled exploitation within the isolated lab environment.

Practical exercises included:

- Module discovery
- Exploit selection
- Payload configuration
- Session management
- Post-exploitation exploration

Using Metasploit improved my understanding of exploit workflows and vulnerability validation.

---

# Wireshark

Wireshark was used to capture and analyze network traffic generated during laboratory exercises.

Protocols analyzed included:

- TCP
- UDP
- DNS
- HTTP
- ICMP
- ARP

Packet analysis helped me better understand network communication and protocol behavior.

---

# Skills Demonstrated

This project demonstrates practical experience with:

## Virtualization

- VMware Workstation 17 Player
- Virtual machine deployment
- Virtual networking
- Resource allocation

## Operating Systems

- Kali Linux
- Windows Server 2019
- Linux administration
- Windows administration

## Networking

- TCP/IP
- Network troubleshooting
- Port scanning
- Service enumeration
- Network communication

## Cybersecurity

- Network reconnaissance
- Vulnerability assessment
- Controlled exploitation
- Packet analysis
- Security documentation

## Professional Skills

- Technical documentation
- Cybersecurity lab design
- Problem solving
- Research
- Continuous learning

---

# Documentation

Detailed documentation for each component of the home lab is available in the `docs/` directory.

# Repository Documentation

| Documentation | Description |
|--------------|-------------|
| vmware.md | VMware installation, configuration and virtualization concepts |
| networking.md | Virtual networking concepts and lab connectivity |
| kali-linux.md | Kali Linux setup and security tools |
| windows-server.md | Windows Server configuration and administration |
| metasploitable-2.md | Vulnerable machine overview and purpose |
| nmap.md | Network discovery and scanning techniques |
| metasploit.md | Metasploit Framework usage and workflow |
| wireshark.md | Packet capture and traffic analysis |

---

# Learning Outcomes

Through building this cybersecurity home lab, I gained practical experience in:

- Virtual machine deployment
- Windows Server administration
- Linux administration
- Network reconnaissance
- Port and service enumeration
- Packet capture and protocol analysis
- Controlled exploitation concepts
- Technical documentation
- Cybersecurity lab management

More importantly, this project strengthened my understanding of how different cybersecurity tools work together within a realistic laboratory environment.

---

# Future Improvements

This home lab will continue to evolve with additional technologies and security tools.

Planned improvements include:

- Active Directory domain environment
- Wazuh SIEM integration
- Sysmon log collection
- Splunk integration for centralized logging
- Sigma rule development
- Velociraptor endpoint monitoring
- Windows 11 client deployment
- Additional vulnerable virtual machines
- Detection engineering use cases
- Threat hunting scenarios

---

# Repository Structure

```text
CyberSecurity-Home-Lab/
│
├── README.md
├── LICENSE
│
└── docs
    ├── vmware.md
    ├── kali-linux.md
    ├── windows-server.md
    ├── metasploitable-2.md
    ├── networking.md
    ├── nmap.md
    ├── metasploit.md
    └── wireshark.md
```

---

# Disclaimer

This repository is intended solely for educational purposes.

All practical exercises, vulnerability assessments, packet captures, and controlled exploitation activities documented in this repository were performed exclusively within an isolated VMware-based home lab using personally managed virtual machines and intentionally vulnerable systems.

No unauthorized testing was conducted against production environments, public systems, third-party infrastructure, or organizational assets.

This repository does **not** contain confidential organizational information, internal IP addresses, production logs, proprietary configurations, or sensitive data. All documentation is based on a personal laboratory environment and is intended to demonstrate practical cybersecurity skills and responsible security practices.
