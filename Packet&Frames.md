# 📦 Packets, TCP/IP, UDP & Ports  
> TryHackMe Room Writeup  
> Author: **Riya Dhakad**

---

## 📖 Overview

This room builds deeper networking knowledge by covering:

- Packets vs Frames  
- Encapsulation  
- TCP/IP Model  
- Three-Way Handshake  
- UDP vs TCP  
- Ports & Common Services  

These concepts are fundamental for:

- Packet analysis  
- Network troubleshooting  
- SOC investigations  
- Penetration testing  
- Service enumeration  

---

# 🧠 Task 1 — Packets & Frames

Packets and frames are small units of data that combine to form larger messages.

However, they belong to different OSI layers:

| Term | OSI Layer | Description |
|------|-----------|-------------|
| Packet | Layer 3 (Network) | Contains IP header & payload |
| Frame | Layer 2 (Data Link) | Encapsulates packet + MAC addresses |

---

## 📬 Encapsulation Analogy

- **Packet** → Letter  
- **Frame** → Envelope  

Encapsulation adds addressing information as data moves down layers.

---

## 🔎 Important IP Headers

| Header | Purpose |
|--------|---------|
| Time To Live (TTL) | Prevents packets from looping forever |
| Checksum | Ensures data integrity |
| Source Address | Sender IP |
| Destination Address | Receiver IP |

---

## ✅ Task 1 Answers

| Question | Answer |
|----------|--------|
| Data with IP addressing? | **Packet** |
| Data without IP addressing? | **Frame** |

---

# 🤝 Task 2 — TCP/IP & Three-Way Handshake

The **TCP/IP Model** consists of four layers:

| Layer |
|-------|
| Application |
| Transport |
| Internet |
| Network Interface |

TCP is **connection-based**, meaning it must establish a connection before sending data.

---

## 🔄 Three-Way Handshake

| Step | Message |
|------|----------|
| 1 | SYN |
| 2 | SYN/ACK |
| 3 | ACK |

Order:SYN → SYN/ACK → ACK


After this, data transmission begins.

---

## 🔐 Important TCP Headers

| Header | Purpose |
|--------|---------|
| Source Port | Sender’s port |
| Destination Port | Receiver’s service port |
| Source IP | Sender IP |
| Destination IP | Receiver IP |
| Sequence Number | Maintains order |
| Acknowledgement Number | Confirms receipt |
| Checksum | Data integrity |
| Flags | Control handshake behavior |

---

## 🛑 TCP Connection Closing

Uses:

- **FIN** → Clean termination  
- **RST** → Abrupt termination  

---

## ✅ Task 2 Answers

| Question | Answer |
|----------|--------|
| Header ensuring integrity? | **checksum** |
| Order of handshake? | **SYN,SYN/ACK,ACK** |

---

# 💬 Task 3 — Practical Handshake

Reassembling the TCP handshake correctly revealed the flag:
THM{TCP_CHATTER}


---

# ⚡ Task 4 — UDP/IP

**UDP (User Datagram Protocol)** is:

- Stateless  
- Faster than TCP  
- No handshake  
- No guaranteed delivery  

---

## 📊 TCP vs UDP

| Feature | TCP | UDP |
|----------|-----|-----|
| Connection-based | Yes | No |
| Reliable | Yes | No |
| Speed | Slower | Faster |
| Use Case | File transfer, Email | Streaming, VoIP |

---

## ✅ Task 4 Answers

| Question | Answer |
|----------|--------|
| UDP stands for? | **User Datagram Protocol** |
| Type of connection? | **stateless** |
| Protocol for file transfer? | **TCP** |
| Protocol for video call? | **UDP** |

---

# 🚪 Task 5 — Ports 101

Ports allow services to communicate on specific numbered channels.

Range:
0 – 65535


Ports 0–1024 are known as **Common Ports**.

---

## 📌 Common Ports

| Protocol | Port | Purpose |
|----------|------|----------|
| FTP | 21 | File Transfer |
| SSH | 22 | Secure Remote Login |
| HTTP | 80 | Web Browsing |
| HTTPS | 443 | Secure Web |
| SMB | 445 | File & Printer Sharing |
| RDP | 3389 | Remote Desktop |

Applications can run on non-standard ports (e.g., 8080 instead of 80).

---

## 🏁 Practical Challenge Flag

Connecting to:
8.8.8.8:1234

THM{YOU_CONNECTED_TO_A_PORT}


---

# 🛠️ Skills & Concepts Practiced

- Packet vs Frame distinction  
- TCP Three-Way Handshake  
- TCP Header analysis  
- UDP stateless communication  
- Service ports & protocol mapping  
- Network traffic understanding  

---

# 📚 Key Takeaways

- Understood encapsulation at packet level  
- Learned TCP handshake process  
- Distinguished TCP vs UDP  
- Understood how ports control services  
- Practiced connecting to remote ports  

---
<img width="1919" height="840" alt="Screenshot 2026-02-21 173528" src="https://github.com/user-attachments/assets/0c1910c5-e194-432e-bd4f-28d7a1c0c9dc" />

