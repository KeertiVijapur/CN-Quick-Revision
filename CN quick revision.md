# 💻 Computer Networking – Quick Revision Notes

*A system that connects numerous independent computers in order to share information & resources. Useful for interviews, MCQs, and placement preparation.*

---

## ➤ Types of Networks

| Type | Full Form                | Scope                        |
|------|--------------------------|------------------------------|
| LAN  | Local Area Network       | Small area (office, home)    |
| PAN  | Personal Area Network    | Individual (Bluetooth, etc.) |
| MAN  | Metropolitan Area Network| City or campus               |
| WAN  | Wide Area Network        | Large area (Internet)        |

---

## ➤ IP Address

**IP → Internet Protocol (Rules)**

| IP Type     | Description                                |
|-------------|--------------------------------------------|
| Public IP   | ➝ Helps to connect with the Internet        |
| Private IP  | ➝ Used in an internal network               |
| IPv4        | ➝ 2³² = 4.3 billion addresses               |
| IPv6        | ➝ 2¹²⁸ = THAT is a huge number              |
| Static IP   | ➝ That never changes                        |
| Dynamic IP  | ➝ Periodically changes                      |

---

## ➤ Subnetting

- Divides an IP network into smaller sub-networks (subnets)
- Improves routing efficiency and security

**CIDR Notation Examples:**

- `192.168.1.0/24` → 256 IPs  
- `/30` → 4 IPs (2 usable)

**Formula:**  
- Hosts per subnet = 2ⁿ - 2 (n = number of host bits)

---

## ➤ MAC Address

**MAC → Media Access Control**

- Physical address provided by the manufacturer  
- Cannot be changed (normally)  
- 48 bits  
- Router uses MAC to identify devices  

> 💡 *MAC Spoofing* allows changing MAC address via software tools

---

## 🧱 OSI Model vs TCP/IP Model

OSI describes how a network system functions.  
TCP/IP is the practical implementation used on the Internet.

### ➤ OSI Model

| Layer | Name         | Examples                                           |
|-------|--------------|----------------------------------------------------|
| 7     | Application  | HTTP, FTP, SMTP, NFS, Telnet, others               |
| 6     | Presentation | JPG, PNG, GIF, ASCII, CSS, HTML…                  |
| 5     | Session      | RPS, TLS, SCP                                      |
| 4     | Transport    | TCP (connection-oriented), UDP (connection-less)   |
| 3     | Network      | IPv4, IPv6, ICMP, ARP                              |
| 2     | Data Link    | MAC, ATM, HDLC, Frame Relay                        |
| 1     | Physical     | Ethernet, USB, DSL, ISDN                           |

### ➤ OSI Mnemonics

- 🔼 7→1: **All People Seem To Need Data Processing**  
- 🔽 1→7: **Please Do Not Throw Sausage Pizza Away**

---

### ➤ TCP/IP Model

| Layer No. | Layer             | Examples                            |
|-----------|-------------------|-------------------------------------|
| 4         | Application        | HTTP, Telnet, FTP, SMTP, DNS, SNMP  |
| 3         | Transport          | UDP, TCP                            |
| 2         | Network/Internet   | IP, ICMP, ARP                       |
| 1         | Network Interface  | Ethernet, Frame Relay               |

---

## ➤ TCP vs UDP

| Feature       | TCP                            | UDP                         |
|---------------|--------------------------------|-----------------------------|
| Connection    | Connection-oriented            | Connection-less             |
| Reliability   | Reliable (acknowledgement)     | Unreliable                  |
| Speed         | Slower                         | Faster                      |
| Use Cases     | HTTP, FTP, Email               | Video streaming, DNS, VoIP |

---

## ➤ TCP 3-Way Handshake

1. **SYN** – Client sends connection request  
2. **SYN-ACK** – Server acknowledges  
3. **ACK** – Client confirms  

➡ Connection established

---

## ➤ HTTP vs HTTPS

| Protocol | Security | Use |
|----------|----------|-----|
| HTTP     | ❌ Not encrypted | Basic web browsing |
| HTTPS    | ✅ Encrypted via SSL/TLS | Secure transactions |

---

## ➤ Common Port Numbers

| Protocol | Port |
|----------|------|
| HTTP     | 80   |
| HTTPS    | 443  |
| FTP      | 21   |
| SSH      | 22   |
| DNS      | 53   |
| DHCP     | 67/68|
| SMTP     | 25   |
| POP3     | 110  |

---

## 🛠 Network Functions & Protocols

- **DNS** – Converts domain names to IP addresses (*Domain Name System*)
- **DHCP** – Assigns dynamic IPs to devices (*Dynamic Host Control Protocol*)
- **ARP** – Maps IP to MAC (*Address Resolution Protocol*)
- **NAT** – Allows internal (private) IPs to communicate with external networks (*Network Address Translation*)

---

## ➤ What Happens When You Type a URL?

1. Browser checks **cache/DNS**  
2. DNS translates domain to **IP address**  
3. **TCP connection** established (3-way handshake)  
4. **HTTP/HTTPS request** sent  
5. Server responds with **HTML**  
6. Browser renders page

---

## 🔐 Security & Devices

- **VPN** – Encrypts connection, hides IP  
- **Firewall** – Controls incoming/outgoing traffic  
- **Router** – Connects different networks  
- **Switch** – Connects multiple devices, sends data to specific host  
- **Hub** – Broadcasts to all connected devices
