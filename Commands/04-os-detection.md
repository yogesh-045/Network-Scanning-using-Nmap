# 🖥️ Operating System Detection

## 📌 Objective

The purpose of this scan is to identify the operating system running on the target host. Operating system detection helps security professionals understand the target environment and plan further security assessments.

---

## 🛠️ Command

```bash
sudo nmap -O 192.168.56.101
```

---

## 📖 Command Breakdown

| Option | Description |
|---------|-------------|
| `sudo` | Runs the command with administrative privileges. |
| `nmap` | Launches the Nmap scanner. |
| `-O` | Enables operating system detection. |
| `192.168.56.101` | Specifies the target host IP address. |

---

## ⚙️ How It Works

- Sends a series of TCP/IP probes to the target.
- Analyzes TCP/IP stack characteristics.
- Compares the responses with the Nmap OS fingerprint database.
- Displays the most likely operating system.

---

## 🎯 Purpose

- Identify the target operating system.
- Improve system profiling.
- Support vulnerability assessment.
- Assist in selecting appropriate security testing techniques.

---

## 📂 Raw Output

The complete scan output is available in:

```text
scans/04-os-detection.txt
```

---

## 📸 Screenshot

```text
screenshots/os-detection.png
```

---

## 📚 Key Learning

- Learned how Nmap performs operating system fingerprinting.
- Understood why administrative privileges are required for OS detection.
- Learned how OS identification supports penetration testing and security assessments.
- Recognized the importance of accurate OS detection during reconnaissance.