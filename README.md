# Network Traffic Analysis using Wireshark

## 📌 Objective
The objective of this project is to analyze website network traffic using Wireshark and understand how data packets are transmitted between a client and a web server. This project focuses on observing network protocols such as DNS, TCP, HTTP/HTTPS, and TLS, along with studying packet flow, connection establishment, and encrypted communication during website access.

---

## 🛠 Tools Used
- Wireshark – Used for capturing and analyzing network packets  
- Google Chrome – Used to generate network traffic by accessing websites  
- Windows 10 – Operating system used for performing the analysis  

---

## 📊 Protocols Observed
- DNS (Domain Name System)
- TCP (Transmission Control Protocol)
- TLS (Transport Layer Security)
- HTTP/HTTPS
- ARP (Address Resolution Protocol)
- QUIC (modern secure transport protocol)
- ICMP (network diagnostics)

---

## 🔄 Steps Followed
- Installed and opened Wireshark  
- Selected active network interface (Wi-Fi/Ethernet)  
- Started packet capture  
- Accessed websites using Google Chrome  
- Generated network traffic by browsing  
- Stopped capture after collecting data  
- Applied filters: `dns`, `tcp`, `tls`, `http`  
- Analyzed packets (DNS, TCP handshake, TLS encryption)  
- Used **Protocol Hierarchy Statistics**  
- Used **I/O Graph** for traffic analysis  
- Captured screenshots and documented findings  

---

## 🔍 Key Analysis

### 1. DNS Analysis
- DNS resolves domain names into IP addresses  
- Client sends DNS queries and receives responses from DNS server  
- Communication occurs over UDP port 53  

---

### 2. TCP Analysis
- TCP 3-way handshake observed: SYN → SYN-ACK → ACK  
- Reliable connection established between client and server  
- HTTPS traffic uses TCP port 443  
- Some retransmissions and packet errors observed during capture  
- Connection termination observed using FIN/ACK  

---

### 3. TLS Analysis
- TLS handshake used for secure communication  
- Client Hello and Server Hello observed  
- Data encrypted using HTTPS (TLS 1.2/1.3)  
- QUIC protocol observed in some modern connections  
- Secure communication established with multiple web services  

---

### 4. HTTP Analysis
- No significant HTTP traffic observed  
- Most websites use HTTPS with TLS encryption  

---

## 📈 Protocol Hierarchy Summary
- Total packets captured: ~31,000+  
- TCP dominates network traffic (~63%)  
- TLS contributes significant encrypted traffic (~24%)  
- UDP and QUIC used for fast communication  
- DNS used for domain resolution  
- ARP and ICMP observed for network operations  

---

## 📊 I/O Graph Analysis
- Initial traffic was low and stable  
- Major spike observed during webpage loading (~30–35 sec)  
- Smaller bursts during background activity  
- Traffic returned to normal after activity reduced  

---

## 🔎 Findings
- DNS resolves domain names before connection starts  
- TCP ensures reliable communication via handshake  
- TLS encrypts data for secure browsing  
- Modern web traffic is mostly HTTPS (not HTTP)  
- Traffic varies based on user activity and background processes  

---

## ✅ Conclusion
This project successfully analyzed real-time network traffic using Wireshark. It helped understand packet-level communication between client and server, including DNS resolution, TCP connection establishment, and TLS encryption. The analysis also provided insights into real-world web traffic behavior and protocol distribution.

---

## 👨‍💻 Author
Sai



