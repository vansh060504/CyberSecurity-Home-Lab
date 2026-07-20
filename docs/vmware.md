# VMware Workstation 17 Player

## Introduction

VMware Workstation 17 Player is a desktop virtualization software developed by VMware that enables multiple operating systems to run simultaneously on a single physical computer. It creates virtual machines (VMs) that behave like independent physical computers while sharing the host machine's hardware resources.

Virtualization is one of the fundamental technologies used in modern IT infrastructure, cloud computing, software development, and cybersecurity. Instead of maintaining multiple physical computers, security professionals can build complete laboratory environments using virtual machines.

For this project, VMware Workstation 17 Player was used to create an isolated cybersecurity home lab consisting of multiple operating systems for practicing networking, system administration, vulnerability assessment, and penetration testing.

---

# Why Virtualization is Important in Cybersecurity

Cybersecurity professionals regularly interact with systems that may contain vulnerabilities or malicious software. Performing these activities directly on a personal computer introduces unnecessary risks.

Virtualization addresses this problem by providing isolated environments where security testing can be performed safely.

Some of the major advantages include:

- Safe testing of vulnerable systems
- Isolation from the host operating system
- Ability to run multiple operating systems simultaneously
- Easy deployment of laboratory environments
- Practical learning without additional hardware
- Cost-effective infrastructure
- Simplified recovery after failed experiments

Because of these advantages, virtualization has become an essential skill for penetration testers, SOC analysts, malware analysts, and security researchers.

---

# VMware Workstation 17 Player

VMware Workstation 17 Player serves as the virtualization platform for this cybersecurity home lab.

The software manages all virtual hardware required by the guest operating systems, including:

- Virtual CPU
- Virtual Memory (RAM)
- Virtual Storage
- Virtual Network Adapter
- USB Devices
- Optical Drives
- BIOS/UEFI Firmware

Each virtual machine operates independently while sharing the host computer's physical resources.

---

# Home Lab Environment

The following virtual machines were configured within VMware Workstation 17 Player.

| Virtual Machine | Purpose |
|-----------------|---------|
| Kali Linux | Security Testing Machine |
| Windows Server 2019 | Windows Administration & Security |
| Metasploitable 2 | Vulnerable Linux Target |

These systems communicate within an isolated virtual network, allowing realistic cybersecurity exercises without affecting external systems.

---

# Virtual Machine Components

Every virtual machine created in VMware consists of several configurable components.

## Virtual CPU

The virtual CPU represents the processor allocated to a guest operating system.

Assigning additional CPU cores improves performance during computationally intensive tasks, while excessive allocation may reduce the performance of the host system.

---

## Virtual Memory (RAM)

Memory allocation determines how much RAM is available to each virtual machine.

Proper RAM allocation ensures smooth execution of operating systems while leaving sufficient memory for the host computer.

---

## Virtual Hard Disk

Each virtual machine stores its operating system and user data inside a virtual disk file.

The virtual disk behaves like a traditional hard drive and can be resized or expanded when additional storage is required.

---

## Virtual Network Adapter

The virtual network adapter enables communication between virtual machines and external networks.

Different networking modes such as NAT, Bridged, and Host-Only provide flexibility depending on laboratory requirements.

---

## Virtual Optical Drive

ISO installation files are attached through the virtual optical drive during operating system installation.

After installation, the ISO image can be detached from the virtual machine.

---

# Operating Systems Installed

Three operating systems were configured within this home lab.

## Kali Linux

Kali Linux functions as the primary attack machine used for reconnaissance, scanning, vulnerability assessment, and network analysis.

The operating system contains hundreds of security tools commonly used by penetration testers and cybersecurity professionals.

---

## Windows Server 2019

Windows Server 2019 provides a Windows enterprise environment for learning administration, event logging, networking, and security configuration.

The Desktop Experience edition was installed to simplify system management through a graphical user interface.

---

## Metasploitable 2

Metasploitable 2 is an intentionally vulnerable Linux operating system designed specifically for cybersecurity education.

It contains numerous insecure services that can be safely analyzed within an isolated laboratory environment.

No testing performed in this repository targets public systems or production infrastructure.

---

# Benefits of My Home Lab

Building this laboratory provided practical experience in several important cybersecurity concepts.

These include:

- Virtual machine deployment
- Operating system installation
- Resource management
- Network configuration
- Security testing
- Vulnerability research
- Windows administration
- Linux administration
- Laboratory troubleshooting
- Documentation

The ability to repeatedly create, modify, and rebuild the environment significantly improved my understanding of virtualization and system administration.

---

# Installing VMware Workstation 17 Player

The first step in building the cybersecurity home lab was installing VMware Workstation 17 Player on the host system.

The installation process included:

1. Downloading VMware Workstation 17 Player.
2. Running the installer with administrator privileges.
3. Accepting the license agreement.
4. Completing the installation using default settings.
5. Restarting the host system after installation.

After installation, VMware Workstation 17 Player became the central platform used to manage all virtual machines within the lab.

---

# Creating a New Virtual Machine

Each operating system was deployed as an individual virtual machine.

The general workflow for creating a virtual machine included:

- Creating a new virtual machine
- Selecting the installation media (ISO file)
- Choosing the guest operating system
- Naming the virtual machine
- Allocating processor and memory resources
- Creating a virtual hard disk
- Reviewing the hardware configuration
- Powering on the virtual machine

Each virtual machine operates independently while sharing the host computer's physical resources.

---

# Installing Kali Linux

Kali Linux was installed as the primary security testing operating system.

The installation involved:

- Booting from the Kali Linux ISO image
- Selecting the graphical installer
- Configuring language and keyboard settings
- Creating a user account
- Partitioning the virtual disk
- Installing the operating system
- Rebooting into the newly installed environment

After installation, Kali Linux was updated to ensure the latest packages and security tools were available.

---

# Installing Windows Server 2019

Windows Server 2019 (Desktop Experience) was installed to provide a Windows-based server environment for learning administration and security.

The installation process included:

- Booting from the Windows Server ISO
- Selecting the Desktop Experience edition
- Creating a virtual hard disk
- Completing the Windows installation wizard
- Configuring the administrator account
- Applying system updates
- Verifying network connectivity

The graphical Desktop Experience edition simplifies management and provides access to administrative tools through a familiar interface.

---

# Importing Metasploitable 2

Metasploitable 2 was added to the laboratory as an intentionally vulnerable Linux system.

Unlike a standard operating system installation, Metasploitable 2 is commonly distributed as a preconfigured virtual machine.

After importing the virtual machine into VMware Workstation, the system was configured with appropriate networking settings and integrated into the isolated lab environment.

The machine serves as a safe target for practicing reconnaissance, enumeration, and vulnerability assessment.

---

# Hardware Resource Allocation

Proper allocation of hardware resources is essential for maintaining good performance across all virtual machines.

The following resources were configured for each virtual machine:

- Virtual CPUs
- Memory (RAM)
- Virtual Hard Disk
- Network Adapter
- Display Adapter

Resource allocation was balanced to ensure both the host operating system and guest virtual machines remained responsive during laboratory activities.

---

# Virtual Hard Disk Configuration

Each virtual machine stores its operating system and data within a virtual hard disk.

Advantages of virtual disks include:

- Easy backup
- Portable storage
- Efficient disk management
- Simplified migration
- Flexible storage allocation

Virtual disks provide the same functionality as physical storage devices while remaining completely software-based.

---

# Virtual Networking

Networking is one of the most important components of any cybersecurity laboratory.

VMware Workstation supports several networking modes.

## NAT

Network Address Translation (NAT) allows virtual machines to access external networks through the host computer while remaining hidden from other devices.

Advantages include:

- Internet connectivity
- Simple configuration
- Additional isolation
- Suitable for software updates

---

## Bridged Networking

Bridged mode connects a virtual machine directly to the physical network.

The virtual machine receives its own IP address and behaves as if it were another physical computer connected to the same network.

This mode is useful for realistic enterprise network simulations.

---

## Host-Only Networking

Host-Only networking creates a completely isolated environment where communication occurs only between the host computer and virtual machines.

This mode is particularly useful when performing cybersecurity experiments that should remain disconnected from external networks.

---

# Communication Between Virtual Machines

After configuring networking, the virtual machines were able to communicate with one another within the laboratory.

This enabled practical exercises such as:

- Connectivity testing
- Network discovery
- Port scanning
- Service enumeration
- Packet capture
- Vulnerability assessment

The isolated environment allowed these activities to be performed safely without affecting external systems.

---

# VMware Tools

VMware Tools is a collection of utilities that improves the interaction between the host system and guest operating systems.

Benefits include:

- Improved graphics performance
- Better mouse integration
- Clipboard sharing
- Time synchronization
- Enhanced display resolution
- Improved virtual hardware support

Installing VMware Tools improves both usability and overall virtual machine performance.

---
