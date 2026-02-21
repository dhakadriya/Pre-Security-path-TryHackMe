<img width="1913" height="860" alt="image" src="https://github.com/user-attachments/assets/2cf157d7-b067-4526-9e63-8cdc9cfa3049" />

# 🌐 Networking Fundamentals  
> TryHackMe Room Writeup  
> Author: **Riya Dhakad**

---

## 📖 Overview

This room introduces the fundamental concepts of networking that form the backbone of cybersecurity. It explains how devices communicate, how the Internet works, and how systems are uniquely identified using IP and MAC addresses.

The room also provides hands-on practical exercises involving:

- IP Addressing  
- MAC Address Spoofing  
- ICMP & Ping  

Understanding networking is essential for both **Red Team (Offensive Security)** and **Blue Team (Defensive Security)** roles.

---

# 🧠 Task 1 — What is Networking?

Networking refers to devices connected together to communicate and share data.

A network can consist of:

- Two connected devices  
- A local office network  
- Billions of interconnected devices globally (Internet)

Networking powers critical infrastructure such as:

- Transportation systems  
- Power grids  
- Communication services  
- Internet services  

### ✅ Answer

| Question | Answer |
|----------|--------|
| What is the key term for devices that are connected together? | **Network** |

---

# 🌍 Task 2 — What is the Internet?

The Internet is a global system of interconnected networks.

It originated from:

- **ARPANET (1960s)**  
- The invention of the **World Wide Web (1989)**  

The World Wide Web was invented by **Tim Berners-Lee**, transforming the Internet into a global information-sharing platform.

### Network Types

| Type | Description |
|------|------------|
| Private Network | Internal communication between devices |
| Public Network | Internet-facing communication |

### ✅ Answer

| Question | Answer |
|----------|--------|
| Who invented the World Wide Web? | **Tim Berners-Lee** |

---

# 🖥️ Task 3 — Identifying Devices on a Network

Devices are identified in two primary ways:

| Identification Type | Description | Changeable? |
|---------------------|------------|------------|
| IP Address | Logical network address | Yes |
| MAC Address | Physical hardware address | Can be spoofed |

---

## 🌐 IP Address

- IPv4 consists of **4 sections**
- Each section is called an **Octet**
- Public IP → Identifies device on the Internet
- Private IP → Identifies device within a local network

---

## 🔌 MAC Address

- Stands for **Media Access Control**
- 12-character hexadecimal value
- Assigned to the network interface card (NIC)
- Can be spoofed to bypass weak network controls

### 🔍 MAC Spoofing Lab Result

By spoofing Bob’s MAC address to match Alice’s, access to restricted Wi-Fi was successfully gained.

### ✅ Answers

| Question | Answer |
|----------|--------|
| What does IP stand for? | **Internet Protocol** |
| What is each section of an IP address called? | **Octet** |
| How many sections does IPv4 have? | **4** |
| What does MAC stand for? | **Media Access Control** |
| What is the flag from the MAC spoofing lab? | **THM{YOU_GOT_ON_TRYHACKME}** |

---

# 📡 Task 4 — Ping (ICMP)

Ping is a diagnostic tool used to test connectivity between devices.

It uses:

> **ICMP — Internet Control Message Protocol**

Ping sends:

- Echo Request  
- Echo Reply  

to verify if a host is reachable and measure response time (latency).

---

## 🖥️ Ping Syntax
ping 10.10.10.10

🏁 Ping Lab Result

Pinging 8.8.8.8 revealed the following flag:

THM{I_PINGED_THE_SERVER}

✅ Answers
| Question | Answer |
|----------|--------|
| What protocol does ping use? |	**ICMP** |
| What is the syntax to ping 10.10.10.10? |	**ping 10.10.10.10** |
| What flag do you get when pinging 8.8.8.8? |	**THM{I_PINGED_THE_SERVER}**|

