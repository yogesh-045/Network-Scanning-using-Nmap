# 📜 NSE Script Scanning

## 📌 Objective

The purpose of this scan is to identify potential security vulnerabilities on the target host using the Nmap Scripting Engine (NSE). The `vuln` script category executes a collection of vulnerability detection scripts against the target's exposed services.

---

## 🛠️ Command

```bash
nmap --script=vuln 192.168.56.101
```

---

## 📖 Command Breakdown

| Option | Description |
|---------|-------------|
| `nmap` | Launches the Nmap scanner. |
| `--script=vuln` | Executes vulnerability detection scripts from the NSE library. |
| `192.168.56.101` | Specifies the target host IP address. |

---

## ⚙️ How It Works

- Performs port scanning on the target.
- Identifies running network services.
- Executes vulnerability detection scripts against discovered services.
- Reports any potential security issues identified by the scripts.

---

## 🎯 Purpose

- Detect known vulnerabilities.
- Identify security misconfigurations.
- Assess exposed services for common weaknesses.
- Support vulnerability assessment and security auditing.

---

## 📂 Raw Output

The complete scan output is available in:

- 📄 **Raw Scan Output:** [05-nse-script.txt](/Scans/05-nse-script.txt)

---

## 📸 Screenshot

- 🖼️ **Screenshot:** [NSE-Script.png](/Screenshots/nse-script.png)

---

## 📚 Key Learning

- Learned how to use the Nmap Scripting Engine (NSE).
- Executed vulnerability detection scripts against a target.
- Understood how NSE automates security checks.
- Learned the importance of validating detected vulnerabilities before remediation.
