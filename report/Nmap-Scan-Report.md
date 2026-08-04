# Network Scanning Report using Nmap

## Project Overview

This project demonstrates the use of Nmap for network reconnaissance and enumeration against a Metasploitable 2 virtual machine in a controlled lab environment. Multiple scan techniques were used to identify live hosts, open ports, running services, operating system information, firewall behavior, and known vulnerabilities.

> **Disclaimer**
>
> All scans were performed in a controlled lab environment using Metasploitable 2, an intentionally vulnerable virtual machine. This project is intended for educational purposes only.

---

# Target Information

| Item | Value |
|------|-------|
| Scanner | Nmap 7.99 |
| Target IP | 192.168.56.101 |
| Target Machine | Metasploitable 2 |
| Environment | Oracle VirtualBox |
| Operating System | Linux (Estimated by Nmap) |

---

# Scan Summary

| Scan | Status |
|------|--------|
| Host Discovery | ✅ Completed |
| Port Scanning | ✅ Completed |
| Service & Version Detection | ✅ Completed |
| Operating System Detection | ✅ Completed |
| NSE Vulnerability Scan | ✅ Completed |
| Firewall Detection | ✅ Completed |

---

# 1. Host Discovery

## Objective

Verify whether the target host is reachable before performing detailed scans.

### Command

```bash
nmap -sn 192.168.56.101
```

### Result

The target host responded successfully and was confirmed to be online.

### Evidence

- 📄 **Raw Output:** [01-host-discovery.txt](/Scans/01-host-discovery.txt)
- 🖼️ **Screenshot:** [host-discovery.png](/Screenshots/host-discovery.png)

---

# 2. Port Scanning

## Command

```bash
nmap 192.168.56.101
```

## Result

The scan identified **23 open TCP ports**.

Several additional ports were filtered and closed.

### Important Open Services

- FTP
- SSH
- Telnet
- SMTP
- DNS
- HTTP
- SMB
- MySQL
- PostgreSQL
- VNC
- IRC
- Apache Tomcat

### Analysis

The target exposes numerous network services, increasing the attack surface. Service enumeration is required to determine software versions and identify potential vulnerabilities.

### Evidence

- 📄 **Raw Output:** [02-port-scan.txt](/Scans/02-port-scan.txt)
- 🖼️ **Screenshot:** [port-scan.png](/Screenshots/port-scan.png)

---

# 3. Service & Version Detection

## Command

```bash
nmap -sV 192.168.56.101
```

## Result

Nmap successfully identified the versions of several running services, including:

- vsFTPd 2.3.4
- OpenSSH 4.7p1
- Apache HTTP Server 2.2.8
- Samba 3.x
- MySQL 5.0.51a
- PostgreSQL 8.3.x
- UnrealIRCd

### Analysis

Service version detection helps identify outdated software and supports vulnerability assessment.

### Evidence

- 📄 **Raw Output:** [04-service-version.txt](/Scans/04-service-version.txt)
- 🖼️ **Screenshot:** [service-version.png](/Screenshots/service-version.png)

---

# 4. Operating System Detection

## Command

```bash
nmap -O 192.168.56.101
```

## Result

Nmap could not determine the exact operating system but suggested Oracle VirtualBox and Linux-based environments with high confidence.

### Analysis

OS fingerprinting relies on TCP/IP characteristics. Virtualization and network conditions may reduce fingerprint accuracy.

### Evidence

- 📄 **Raw Output:** [03-os-detection.txt](/Scans/03-os-detection.txt)
- 🖼️ **Screenshot:** [os-detection.png](/Screenshots/os-detection.png)

---

# 5. NSE Vulnerability Scan

## Command

```bash
sudo nmap --script vuln 192.168.56.101
```

## Major Findings

The vulnerability scan identified several known vulnerabilities, including:

- vsFTPd 2.3.4 Backdoor (CVE-2011-2523)
- SSL POODLE (CVE-2014-3566)
- Logjam (CVE-2015-4000)
- Weak Diffie-Hellman Parameters
- HTTP TRACE Enabled
- Possible CSRF Endpoints
- RMI Registry Remote Code Execution
- UnrealIRCd Backdoor
- SSL CCS Injection (CVE-2014-0224)

### Analysis

The detected vulnerabilities are expected because the target system is Metasploitable 2, which is intentionally designed for penetration testing practice.

### Evidence

- 📄 **Raw Output:** [05-nse-script.txt](S/scans/05-nse-script.txt)
- 🖼️ **Screenshot:** [nse-script.png](/Screenshots/nse-script.png)
---

# 6. Firewall Detection

## Command

```bash
sudo nmap -sA 192.168.56.101
```

## Result

The ACK scan reported all scanned TCP ports as **unfiltered**.

### Analysis

The target responded with TCP RST packets, indicating that ACK packets reached the target successfully. No packet filtering was detected during this scan.

### Evidence

- 📄 **Raw Output:** [06-firewall-detection.txt](/Scans/06-firewall-detection.txt)
- 🖼️ **Screenshot:** [firewall-detection.png](/Screenshots/firewall-detection.png)

---

# Skills Demonstrated

- Network Reconnaissance
- Host Discovery
- TCP Port Scanning
- Service Enumeration
- Version Detection
- Operating System Fingerprinting
- Firewall Detection
- Vulnerability Assessment
- Nmap Scripting Engine (NSE)
- Security Reporting

---

# Tools Used

- Nmap 7.99
- Kali Linux
- Metasploitable 2
- Oracle VirtualBox

---

# Conclusion

This project demonstrates practical experience with Nmap by performing host discovery, port scanning, service and version detection, operating system fingerprinting, firewall analysis, and vulnerability assessment in a safe lab environment.

The project also highlights the importance of proper documentation by including commands, raw scan outputs, screenshots, and technical analysis for each scan type.
