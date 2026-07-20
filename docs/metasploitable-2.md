# Metasploitable 2

## Introduction

Metasploitable 2 is an intentionally vulnerable Linux virtual machine developed by Rapid7 for cybersecurity education and penetration testing practice. It contains numerous known vulnerabilities and insecure services that allow security professionals to safely practice reconnaissance, enumeration, vulnerability assessment, and exploitation within a controlled laboratory environment.

In this home lab, Metasploitable 2 was deployed as the primary vulnerable target system. It was used together with Kali Linux to perform security testing inside an isolated VMware network.

---

# Purpose of Using Metasploitable 2

The primary objective of using Metasploitable 2 was to create a realistic target machine for learning offensive security techniques without affecting production systems.

It provides a safe environment for practicing:

- Network reconnaissance
- Port scanning
- Service enumeration
- Vulnerability assessment
- Controlled exploitation
- Post-exploitation learning

Because the operating system is intentionally insecure, it should only be used inside isolated laboratory environments.

---

# Installation

Metasploitable 2 was imported into VMware Workstation 17 Player as a pre-configured virtual machine.

The setup process included:

- Importing the virtual machine
- Verifying virtual hardware configuration
- Connecting the network adapter
- Booting the operating system
- Confirming network connectivity
- Identifying the assigned IP address

After deployment, the machine became accessible from Kali Linux within the virtual network.

---

# System Overview

Metasploitable 2 runs a vulnerable Linux operating system with multiple intentionally exposed services.

These vulnerable services are designed for educational purposes and allow learners to understand how attackers identify and exploit weaknesses during security assessments.

The system is intentionally outdated and should never be connected directly to the public Internet.

---

# Services Available

Several services may be available depending on the configuration.

Examples include:

- FTP
- SSH
- Telnet
- HTTP
- MySQL
- PostgreSQL
- Samba
- SMTP
- DNS

These services provide opportunities for reconnaissance, enumeration, and vulnerability analysis.

---

# Practical Activities

Within this home lab, Metasploitable 2 was used for several practical exercises.

These included:

- Identifying the host on the network
- Discovering open ports
- Enumerating running services
- Identifying service versions
- Validating vulnerabilities
- Performing controlled exploitation using Metasploit
- Analyzing network traffic with Wireshark

These activities helped simulate a real-world penetration testing workflow.

---

# Security Considerations

Metasploitable 2 is intentionally insecure and should always be isolated from production environments.

The following precautions were followed during this project:

- Used only inside VMware
- Connected only to the isolated lab network
- Never exposed to public networks
- Used solely for educational purposes

Maintaining isolation helps ensure that vulnerable services cannot be accessed by unauthorized systems.

---

# Skills Developed

Working with Metasploitable 2 improved my understanding of:

- Vulnerability assessment
- Network reconnaissance
- Service enumeration
- Linux target analysis
- Penetration testing methodology
- Security tool integration
- Practical laboratory workflows

---

# Learning Outcomes

Using Metasploitable 2 allowed me to gain practical experience with the complete penetration testing process, from discovering a target system to identifying services and validating vulnerabilities in a controlled environment.

The experience also improved my understanding of how attackers identify weaknesses and how defenders can better secure enterprise systems.

---

# Conclusion

Metasploitable 2 served as the primary vulnerable target machine within this cybersecurity home lab. It provided a safe environment for learning reconnaissance, vulnerability assessment, and controlled exploitation while reinforcing ethical hacking principles and responsible security testing practices.

---
