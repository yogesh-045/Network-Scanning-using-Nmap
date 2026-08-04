# 🌐 Port Scanning

## 📌 Objective

The purpose of this scan is to identify open TCP ports on the target host. Open ports indicate which network services are available and help determine the potential attack surface for further assessment.

---

## 🛠️ Command

```bash
nmap 192.168.56.101
```

---

## 📖 Command Breakdown

| Option | Description |
|---------|-------------|
| `nmap` | Launches the Nmap scanner. |
| `192.168.56.101` | Specifies the target host IP address. |

---

## ⚙️ How It Works

- Sends TCP SYN probes to the most common ports.
- Determines whether each port is open, closed, or filtered.
- Lists the services associated with the detected ports.

---

## 🎯 Purpose

- Discover open TCP ports.
- Identify accessible network services.
- Prepare for service enumeration and vulnerability assessment.

---

## 📂 Raw Output

The complete scan output is available in:

```text
scans/02-port-scan.txt
```

---

## 📸 Screenshot

```text
screenshots/port-scan.png
```

---

## 📚 Key Learning

- Learned how to perform a basic TCP port scan.
- Identified open ports on the target host.
- Understood the importance of port enumeration during reconnaissance.
- Recognized how exposed services increase the attack surface.