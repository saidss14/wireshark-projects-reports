# Nmap Network Scanning Project

## Project Overview
This project demonstrates the use of Nmap for performing basic network scanning and host discovery. The purpose of this project is to gain hands-on experience with network reconnaissance techniques and understand how Nmap identifies hosts, ports, and running services.

---

## Project Objective
The main objective of this project is to:

- Learn the basics of network scanning
- Identify local system IP address
- Discover active hosts
- Identify open ports
- Understand service detection
- Gain practical experience with Nmap

---

## Tools Used
- Nmap
- Windows Command Prompt (CMD)
- VS Code
- GitHub

---

# Step 1: Identifying Local IP Address

## Command Used

```bash
ipconfig
```

## Screenshot

![IP Configuration](<Imges/ip config.png>)
## Purpose
The `ipconfig` command is used to view network configuration details of the system and identify the local IPv4 address before performing network scans.

## Findings
- IPv4 address identified
- Default gateway identified
- Network adapter information observed

## What I Learned
- How to identify my local IP address
- Understanding basic network configuration
- Importance of identifying the target system before scanning

---

# Scan 1: Ping Scan (Host Discovery)

## Command Used

```bash
nmap -sn 192.168.1.0/24
```

## Screenshot

![Ping Scan Result](screenshots/pingscan.png)

## Purpose
This scan is used to identify active devices available on the network without scanning ports.

## Findings
- Active hosts were discovered
- Network devices responded successfully

## What I Learned
- Host discovery basics
- Difference between active and inactive hosts
- Basic understanding of network reconnaissance

---

# Scan 2: Fast Port Scan

## Command Used

```bash
nmap -F 192.168.1.3
```

## Screenshot

![Fast Scan Result](screenshots/fastscan.png)

## Purpose
This scan checks commonly used ports quickly instead of scanning all ports.

## Findings
- Open ports were identified
- Host responded successfully

## What I Learned
- Fast scanning techniques
- Importance of port scanning
- Understanding open ports

---

# Scan 3: Service Version Detection

## Command Used

```bash
nmap -sV 192.168.1.3
```

## Screenshot

![Service Detection Result](screenshots/servicescan.png)

## Purpose
This scan identifies services running on open ports and their versions.

## Findings
- Running services were detected
- Service versions were identified

## What I Learned
- Service detection concepts
- Importance of version identification
- Enumeration basics

---

## Challenges Faced
Initially, understanding Nmap commands and interpreting scan outputs was challenging. With practice, it became easier to understand scan results and identify different scan purposes.

---

## Key Takeaways
- Learned how to identify local IP address
- Understood host discovery using Nmap
- Learned fast port scanning
- Practiced service version detection
- Improved practical cybersecurity skills

---

## Conclusion
This project helped me understand the basics of network scanning using Nmap and improved my practical knowledge of reconnaissance techniques in cybersecurity.