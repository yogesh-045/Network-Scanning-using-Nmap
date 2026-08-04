# 1. Host Discovery

## Objective

Identify active hosts on the target network before performing detailed enumeration.

---

## Command

```bash
nmap -sn 192.168.56.0/24
```

---

## Command Breakdown

| Option | Description |
|---------|-------------|
| `nmap` | Launches the Nmap scanner. |
| `-sn` | Performs host discovery without scanning ports. |
| `192.168.56.0/24` | Target subnet. |

---

## Purpose

- Discover active hosts.
- Identify reachable systems.
- Prepare for further scanning.

---

## Raw Output

See:

- 📄 **Raw Scan Output:** [01-host-discovery.txt](/Scans/01-host-discovery.txt)

---

## Screenshot

- 🖼️ **Screenshot:** [host-discovery.png](/Screenshots/host-discovery.png)
