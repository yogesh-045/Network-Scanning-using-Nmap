# 🔍 Service & Version Detection

## 📌 Objective

The purpose of this scan is to identify the services running on open ports and determine their version information. This helps in understanding the target environment and identifying outdated or vulnerable software.

---

## 🛠️ Command

```bash
nmap -sV 192.168.56.101
```

---

## 📖 Command Breakdown

| Option | Description |
|---------|-------------|
| `nmap` | Launches the Nmap scanner. |
| `-sV` | Detects the version of services running on open ports. |
| `192.168.56.101` | Specifies the target host IP address. |

---

## ⚙️ How It Works

- Scans open ports on the target.
- Communicates with running services.
- Matches responses against the Nmap service fingerprint database.
- Displays the detected service names and versions.

---

## 🎯 Purpose

- Identify running network services.
- Detect software versions.
- Discover outdated or vulnerable services.
- Support vulnerability assessment.

---

## 📂 Raw Output

The complete scan output is available in:

- 📄 **Raw Scan Output:** [04-service-version.txt](/Scans/04-service-version.txt)

---

## 📸 Screenshot

- 🖼️ **Screenshot:** [service-version.png](/Screenshots/service-version.png)

---

## 📚 Key Learning

- Learned how to detect running services.
- Identified software versions on open ports.
- Understood the importance of version detection in vulnerability assessment.
- Learned how service enumeration supports penetration testing and security analysis.
