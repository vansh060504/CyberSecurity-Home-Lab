# Metasploit Framework

## Introduction

The Metasploit Framework is one of the most widely used penetration testing frameworks in cybersecurity. Developed by Rapid7, it provides a collection of exploits, payloads, auxiliary modules, encoders, and post-exploitation tools that help security professionals identify, validate, and understand vulnerabilities in a controlled environment.

Within this cybersecurity home lab, Metasploit Framework was used from Kali Linux to perform controlled exploitation exercises against Metasploitable 2 in an isolated VMware environment.

---

# Why Metasploit?

After identifying open ports and services using Nmap, the next step during a penetration test is determining whether discovered services are vulnerable.

Metasploit helps security professionals:

- Validate vulnerabilities
- Test exploitability
- Understand attack paths
- Practice penetration testing
- Learn post-exploitation techniques
- Improve defensive knowledge

It is one of the most commonly used frameworks during authorized security assessments.

---

# Lab Environment

The following systems were used throughout the practical exercises.

| Machine | Role |
|---------|------|
| Kali Linux | Attacker Machine |
| Metasploitable 2 | Vulnerable Target |
| VMware Workstation 17 Player | Virtualization Platform |

All activities were performed exclusively inside an isolated virtual laboratory.

---

# Starting Metasploit

## Objective

Launch the Metasploit Framework.

## Command

```bash
msfconsole
```

## Explanation

The `msfconsole` command starts the Metasploit interactive console, which provides access to all framework modules.

After loading, the framework can be used to search for exploits, configure payloads, execute modules, and manage sessions.

---

# Searching for Exploits

## Objective

Find available exploit modules.

## Command

```bash
search <service-name>
```

Example:

```bash
search vsftpd
```

## Explanation

The search command locates exploit modules related to a service, application, or vulnerability.

## Learning Outcome

Learned how Metasploit organizes exploit modules for different services and vulnerabilities.

---

# Selecting an Exploit

## Objective

Load a specific exploit module.

## Command

```bash
use <module-name>
```

Example:

```bash
use exploit/unix/ftp/vsftpd_234_backdoor
```

## Explanation

The selected exploit becomes the active module for configuration and execution.

---

# Viewing Module Options

## Objective

Display required configuration parameters.

## Command

```bash
show options
```

## Explanation

This command lists all configurable parameters required before running the exploit.

Typical options include:

- Target IP
- Target Port
- Payload
- Local Host
- Local Port

---

# Configuring the Target

## Objective

Specify the target machine.

## Command

```bash
set RHOSTS <target-ip>
```

Example

```bash
set RHOSTS 192.168.x.x
```

## Explanation

RHOSTS defines the remote target that will receive the exploit.

---

# Selecting a Payload

## Objective

Choose a payload for the exploit.

## Command

```bash
show payloads
```

Then

```bash
set PAYLOAD <payload-name>
```

## Explanation

Payloads define what happens after successful exploitation.

Examples include:

- Reverse Shell
- Bind Shell
- Meterpreter

---

# Running the Exploit

## Objective

Execute the configured exploit.

## Command

```bash
run
```

or

```bash
exploit
```

## Explanation

Metasploit attempts to exploit the configured vulnerability.

If successful, a session is created.

---

# Managing Sessions

## Objective

View active sessions.

## Command

```bash
sessions
```

To interact with a session:

```bash
sessions -i <session-id>
```

## Explanation

Sessions provide access to compromised systems within the isolated laboratory.

---

# Meterpreter

Meterpreter is an advanced payload that provides an interactive shell after successful exploitation.

Common capabilities include:

- File navigation
- Process enumeration
- System information
- Screenshot capture
- Network configuration
- Privilege information

Meterpreter was studied as part of understanding post-exploitation workflows.

---

# Practical Workflow

The practical workflow followed during this home lab consisted of:

1. Discover target system
2. Perform Nmap scan
3. Identify running services
4. Search for available exploits
5. Configure exploit parameters
6. Execute exploit
7. Verify results
8. Analyze findings

This structured methodology reflects the typical workflow followed during authorized penetration testing engagements.

---

# Security Considerations

Metasploit is a powerful security framework and should only be used against systems where explicit authorization has been granted.

During this project:

- Testing was performed only inside VMware.
- Only personally managed virtual machines were used.
- No production or public systems were targeted.
- Activities were conducted solely for educational purposes.

---

# Skills Developed

Working with Metasploit helped strengthen my understanding of:

- Penetration testing methodology
- Vulnerability validation
- Exploit configuration
- Payload selection
- Session management
- Post-exploitation concepts
- Ethical security testing

---

# Learning Outcomes

Using Metasploit within this cybersecurity home lab provided practical experience with the exploitation phase of a security assessment.

It reinforced the importance of:

- Accurate reconnaissance
- Careful vulnerability validation
- Responsible testing practices
- Controlled laboratory environments

---

# Conclusion

Metasploit Framework complemented the reconnaissance performed with Nmap by enabling controlled vulnerability validation inside an isolated virtual environment.

Working with the framework improved my understanding of exploitation workflows while emphasizing the importance of ethical hacking principles and responsible cybersecurity practices.
