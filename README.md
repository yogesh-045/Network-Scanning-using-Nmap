# 🌐 Network Scanning using Nmap

A hands-on cybersecurity project demonstrating network reconnaissance using **Nmap**. This project covers host discovery, port scanning, service enumeration, operating system detection, firewall detection, and vulnerability assessment against a **Metasploitable 2** virtual machine in a controlled lab environment.

> **Disclaimer**
>
> This project was performed in a controlled lab environment using **Metasploitable 2**, an intentionally vulnerable virtual machine created for cybersecurity training. No unauthorized systems were scanned.

---

# 📖 Project Overview

Network scanning is one of the first steps in penetration testing and security assessments. In this project, I used **Nmap** to identify live hosts, discover open ports, detect running services, identify the operating system, analyze firewall behavior, and perform vulnerability scanning using the Nmap Scripting Engine (NSE).

---

# 🎯 Objectives

- Discover live hosts on the network.
- Identify open TCP ports.
- Detect running services and versions.
- Perform operating system fingerprinting.
- Analyze firewall filtering behavior.
- Detect known vulnerabilities using NSE scripts.
- Document findings in a professional security report.

---

# 🛠️ Tools Used

- **Nmap 7.99**
- **Kali Linux**
- **Metasploitable 2**
- **Oracle VirtualBox**
- **Git & GitHub**

---

# 📂 Project Structure

```text
Network-Scanning-using-Nmap/
│
├── README.md
├── LICENSE
│
├── commands/
│   ├── 01-host-discovery.md
│   ├── 02-port-scanning.md
│   ├── 03-service-version-detection.md
│   ├── 04-os-detection.md
│   ├── 05-nse-script-scanning.md
│   └── 06-firewall-detection.md
│
├── scans/
│   ├── 01-host-discovery.txt
│   ├── 02-port-scan.txt
│   ├── 03-service-version.txt
│   ├── 04-os-detection.txt
│   ├── 05-nse-script.txt
│   └── 06-firewall-detection.txt
│
├── report/
│   └── Nmap-Scan-Report.md
│
└── screenshots/
    ├── host-discovery.png
    ├── port-scan.png
    ├── service-version.png
    ├── os-detection.png
    ├── nse-script.png
    └── firewall-detection.png
```

---

# 🔍 Scan Techniques Covered

| Scan | Description |
|------|-------------|
| Host Discovery | Identifies whether the target host is online. |
| Port Scanning | Discovers open TCP ports on the target. |
| Service & Version Detection | Identifies running services and software versions. |
| OS Detection | Estimates the operating system using TCP/IP fingerprinting. |
| NSE Script Scanning | Detects known vulnerabilities using Nmap scripts. |
| Firewall Detection | Determines whether firewall filtering is present. |

---

# 📊 Key Findings

- Successfully identified the target host.
- Discovered multiple open TCP ports.
- Enumerated running services and software versions.
- Performed operating system fingerprinting.
- Detected several known vulnerabilities using NSE scripts.
- Verified firewall behavior using an ACK scan.
- Produced a structured technical report with evidence.

---

# 📁 Documentation

- **Commands:** `commands/`
- **Raw Scan Outputs:** `Scans/`
- **Technical Report:** `report/Nmap-Scan-Report.md`
- **Screenshots:** `Screenshots/`

---

# 📚 Skills Demonstrated

- Network Reconnaissance
- Nmap Scanning
- Port Enumeration
- Service Enumeration
- Operating System Fingerprinting
- Firewall Detection
- Vulnerability Assessment
- Security Documentation
- Technical Reporting

---

# 🚀 Learning Outcomes

Through this project, I learned how to:

- Perform different types of Nmap scans.
- Identify exposed services on a target system.
- Detect software versions.
- Analyze firewall behavior.
- Use the Nmap Scripting Engine (NSE) for vulnerability detection.
- Document technical findings professionally.

---

# 📄 License

This project is licensed under the **MIT License**.
