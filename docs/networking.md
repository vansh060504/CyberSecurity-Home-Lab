# Networking in a Cybersecurity Home Lab

## Introduction

Networking is one of the most fundamental concepts in cybersecurity. Every device connected to a network communicates using defined protocols, addressing schemes, and communication models. Understanding how networks operate is essential for tasks such as reconnaissance, vulnerability assessment, packet analysis, incident response, and penetration testing.

In my cybersecurity home lab, networking enabled communication between Kali Linux, Windows Server 2019, and Metasploitable 2. This allowed me to perform network discovery, service enumeration, packet capture, and other security-related activities in an isolated environment.

---

# Why Networking Matters in Cybersecurity

Most cyber attacks occur over a network. Before exploiting a target, an attacker must first identify systems, discover open ports, determine running services, and understand how devices communicate.

Networking knowledge is important for:

- Network reconnaissance
- Host discovery
- Port scanning
- Service enumeration
- Packet analysis
- Firewall configuration
- Intrusion detection
- Incident response
- Threat hunting

Without a solid understanding of networking, it is difficult to perform effective security analysis.

---

# Network Components Used in My Lab

The home lab consisted of the following systems:

| Device | Role |
|---------|------|
| Kali Linux | Security Testing Machine |
| Windows Server 2019 | Windows Target |
| Metasploitable 2 | Vulnerable Linux Target |
| VMware Workstation 17 Player | Virtualization Platform |

These systems communicated over VMware's virtual networking infrastructure, allowing realistic security testing in a controlled environment.

---

# IP Address

An IP (Internet Protocol) address is a unique identifier assigned to every device on a network. It enables systems to locate and communicate with each other.

In the home lab, each virtual machine received its own IP address, allowing communication between Kali Linux and the target machines.

Example:

```
Kali Linux        → 192.168.x.x
Windows Server    → 192.168.x.x
Metasploitable 2  → 192.168.x.x
```

Each machine could be identified and accessed using its assigned IP address.

---

# MAC Address

A MAC (Media Access Control) address is the unique hardware identifier assigned to a network interface.

Unlike IP addresses, MAC addresses operate at the Data Link Layer and are used for communication within the local network.

Each virtual machine in VMware is assigned its own virtual MAC address, allowing them to behave like separate physical computers.

---

# Common Network Protocols

Several network protocols were encountered during lab activities.

| Protocol | Purpose |
|----------|---------|
| TCP | Reliable communication |
| UDP | Fast connectionless communication |
| ICMP | Network diagnostics (Ping) |
| DNS | Domain name resolution |
| HTTP | Web communication |
| HTTPS | Secure web communication |
| SSH | Secure remote administration |
| SMB | Windows file sharing |
| RDP | Remote Desktop Protocol |

Understanding these protocols is essential when analyzing network traffic or performing reconnaissance.

---

# TCP and UDP

TCP (Transmission Control Protocol) provides reliable communication by ensuring data is delivered correctly and in order.

UDP (User Datagram Protocol) is faster but does not guarantee delivery, making it suitable for applications where speed is more important than reliability.

During network scanning and packet analysis, both TCP and UDP traffic can be identified and analyzed.

---

# OSI Model

The Open Systems Interconnection (OSI) model is a conceptual framework that explains how data travels between devices across a network. Although modern networks primarily use the TCP/IP model, understanding the OSI model helps in troubleshooting and analyzing network communication.

| Layer | Name | Function |
|------|----------------|--------------------------------|
| 7 | Application | User applications and services |
| 6 | Presentation | Data formatting and encryption |
| 5 | Session | Establishes and manages sessions |
| 4 | Transport | Reliable data transfer (TCP/UDP) |
| 3 | Network | Routing and IP addressing |
| 2 | Data Link | MAC addressing and switching |
| 1 | Physical | Transmission of electrical signals |

During packet analysis with Wireshark and network scanning using Nmap, understanding the OSI model helped identify how different protocols operate at various layers.

---

# TCP/IP Model

The TCP/IP model is the networking model used by the Internet and most modern computer networks.

| Layer | Responsibilities |
|--------|------------------|
| Application | HTTP, HTTPS, DNS, FTP, SSH |
| Transport | TCP, UDP |
| Internet | IP, ICMP |
| Network Access | Ethernet, Wi-Fi |

The TCP/IP model forms the foundation of communication between the virtual machines in this home lab.

---

# VMware Network Modes

VMware provides multiple networking modes that determine how virtual machines communicate with each other and external networks.

## NAT (Network Address Translation)

In NAT mode, virtual machines share the host computer's network connection.

Characteristics:

- Internet access available
- Private IP addresses
- Easy configuration
- Additional isolation from the physical network

NAT mode is suitable for downloading updates and installing software while keeping virtual machines isolated.

---

## Bridged Networking

Bridged mode connects a virtual machine directly to the physical network.

Characteristics:

- Receives an IP address from the physical network
- Appears as an independent device
- Can communicate with other devices on the LAN

Bridged networking is useful when testing communication with external systems.

---

## Host-Only Networking

Host-Only mode creates a completely isolated network between the host computer and virtual machines.

Characteristics:

- No Internet access
- Communication limited to host and guest machines
- Safe environment for cybersecurity experiments

Host-Only networking is ideal for penetration testing labs because testing remains isolated from external networks.

---

# Communication Between Virtual Machines

After configuring networking in VMware, the virtual machines successfully communicated with each other.

This enabled activities such as:

- Host discovery
- Ping testing
- Port scanning
- Service enumeration
- Packet capture
- Controlled vulnerability assessment

The isolated virtual network provided a realistic environment for cybersecurity practice without affecting production systems.

---

# Connectivity Testing

Connectivity between virtual machines was verified using basic network diagnostic tools.

Common checks included:

- Verifying assigned IP addresses
- Testing connectivity using ping
- Confirming network adapter configuration
- Ensuring systems could reach each other

Successful communication confirmed that the virtual network was correctly configured.

---

# Network Troubleshooting

While configuring the home lab, troubleshooting was sometimes required to resolve connectivity issues.

Common troubleshooting steps included:

- Verifying virtual network adapter settings
- Confirming IP address assignment
- Checking Windows Firewall configuration
- Restarting network services
- Ensuring all virtual machines were connected to the correct VMware network

Systematic troubleshooting helped maintain reliable communication between all virtual machines.

---

# Security Best Practices

To maintain a safe cybersecurity laboratory, the following practices were followed:

- Perform testing only within the isolated virtual environment.
- Avoid scanning public or unauthorized systems.
- Keep operating systems updated.
- Use intentionally vulnerable machines only for educational purposes.
- Verify network configurations before beginning security testing.
- Document configuration changes for future reference.

Following these practices ensures that security testing remains ethical and controlled.

---

# Learning Outcomes

Developing the networking component of this home lab improved my understanding of:

- IP addressing
- Network communication
- TCP/IP fundamentals
- Common network protocols
- Virtual networking with VMware
- Connectivity testing
- Network troubleshooting
- Cybersecurity reconnaissance
- Packet analysis

These networking concepts provide the foundation for using tools such as Nmap, Wireshark, and Metasploit in later stages of the home lab.

---

# Conclusion

Networking forms the backbone of every cybersecurity environment. Building and configuring the virtual network for this home lab provided practical experience with device communication, protocol analysis, and secure laboratory design.

The networking knowledge gained through this project supports future work in penetration testing, security monitoring, vulnerability assessment, and incident response.

