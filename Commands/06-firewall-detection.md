# 🛡️ Firewall Detection

## 📌 Objective

The purpose of this scan is to determine whether a firewall is filtering packets between the scanner and the target host. ACK scanning helps identify firewall filtering rules rather than discovering open ports.

---

## 🛠️ Command

```bash
sudo nmap -sA 192.168.56.101
```

---

## 📖 Command Breakdown

| Option | Description |
|---------|-------------|
| `sudo` | Runs the command with administrative privileges. |
| `nmap` | Launches the Nmap scanner. |
| `-sA` | Performs a TCP ACK scan to detect firewall filtering. |
| `192.168.56.101` | Specifies the target host IP address. |

---

## ⚙️ How It Works

- Sends TCP ACK packets to the target.
- Determines whether packets are filtered by a firewall.
- Does not identify open or closed ports.
- Classifies ports as **filtered** or **unfiltered**.

---

## 🎯 Purpose

- Detect firewall filtering.
- Verify packet filtering rules.
- Assist in network reconnaissance.
- Understand the target's security controls.

---

## 📂 Raw Output

The complete scan output is available in:

- 📄 **Raw Scan Output:** [06-firewall-detection.txt](/Scans/06-firewall-detection.txt)

---

## 📸 Screenshot

- 🖼️ **Screenshot:** [firewall-detection.png](/Screenshots/firewall-detection.png)
---

## 📚 Key Learning

- Learned how to perform firewall detection using an ACK scan.
- Understood the difference between ACK scans and SYN scans.
- Learned how Nmap classifies ports as filtered or unfiltered.
- Gained insight into how firewall rules affect network reconnaissance.
