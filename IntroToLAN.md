# 🖧 LAN, Subnetting & Core Networking Protocols  
> TryHackMe Room Writeup  
> Author: **Riya Dhakad**

---

## 📖 Overview

This room expands foundational networking knowledge by covering:

- LAN Topologies  
- Switches & Routers  
- Subnetting  
- ARP (Address Resolution Protocol)  
- DHCP (Dynamic Host Configuration Protocol)  

These concepts are critical for understanding network architecture, troubleshooting, and security analysis in both **Red Team** and **Blue Team** environments.

---

# 🧠 Task 1 — LAN Topologies

A **LAN (Local Area Network)** connects devices within a limited geographic area such as a home, school, or office.

Network topology refers to the **design or layout** of a network.

---

## ⭐ Star Topology

Devices connect to a **central device** (usually a switch).

### ✔ Advantages
- Highly scalable  
- Easier to add devices  
- More reliable than bus topology  

### ✖ Disadvantages
- Expensive to set up  
- Dependent on central device  
- More maintenance required  

---

## 🚌 Bus Topology

All devices connect to a single **backbone cable**.

### ✔ Advantages
- Cost-efficient  
- Simple setup  

### ✖ Disadvantages
- Single point of failure  
- Bottlenecks under heavy traffic  
- Difficult troubleshooting  

---

## 🔁 Ring Topology

Devices connect in a circular loop.

### ✔ Advantages
- Less prone to congestion  
- Easier fault detection  

### ✖ Disadvantages
- One failure can break entire network  
- Inefficient data travel path  

---

## 🔌 What is a Switch?

A **Switch**:

- Connects multiple devices in a LAN  
- Sends packets only to the intended device  
- Reduces unnecessary network traffic  

---

## 🌐 What is a Router?

A **Router**:

- Connects different networks  
- Sends data between networks  
- Performs **Routing**

---

## ✅ Task 1 Answers

| Question | Answer |
|----------|--------|
| What does LAN stand for? | **Local Area Network** |
| What is the verb given to the job that routers perform? | **Routing** |
| What device centrally connects multiple devices? | **Switch** |
| What topology is cost-efficient? | **Bus Topology** |
| What topology is expensive to set up and maintain? | **Star Topology** |
| What is the lab flag? | **THM{TOPOLOGY_FLAWS}** |

---

# 🧠 Task 2 — A Primer on Subnetting

Subnetting is the process of dividing a network into **smaller subnetworks**.

It improves:

- Efficiency  
- Security  
- Network control  

---

## 🧮 Subnet Mask

- Consists of **32 bits**
- Divided into **4 octets**
- Each octet ranges from **0–255**

---

## 🏷 IP Address Roles in Subnetting

| Type | Purpose | Example |
|------|----------|----------|
| Network Address | Identifies start of network | 192.168.1.0 |
| Host Address | Identifies a device | 192.168.1.100 |
| Default Gateway | Sends data outside network | 192.168.1.254 |

---

## ✅ Task 2 Answers

| Question | Answer |
|----------|--------|
| What is dividing a network into smaller pieces called? | **Subnetting** |
| How many bits are in a subnet mask? | **32** |
| What is the range of an octet? | **0-255** |
| What identifies the start of a network? | **Network Address** |
| What identifies devices within a network? | **Host Address** |
| What device sends data to another network? | **Default Gateway** |

---

# 🧠 Task 3 — ARP (Address Resolution Protocol)

Devices have two identifiers:

- IP Address (Logical)
- MAC Address (Physical)

**ARP** links these two together.

---

## 🔄 How ARP Works

1. Device sends **ARP Request** (broadcast)
2. Device owning the IP responds with **ARP Reply**
3. Mapping is stored in ARP Cache

---

## ✅ Task 3 Answers

| Question | Answer |
|----------|--------|
| What does ARP stand for? | **Address Resolution Protocol** |
| What ARP packet asks for IP ownership? | **Request** |
| What is the physical identifier? | **MAC Address** |
| What is the logical identifier? | **IP Address** |

---

# 🧠 Task 4 — DHCP

**DHCP (Dynamic Host Configuration Protocol)** automatically assigns IP addresses.

---

## 📦 DHCP Process (DORA)

| Step | Packet |
|------|--------|
| Discover | DHCP Discover |
| Offer | DHCP Offer |
| Request | DHCP Request |
| Acknowledge | DHCP ACK |

---

## ✅ Task 4 Answers

| Question | Answer |
|----------|--------|
| Packet used to retrieve IP address? | **DHCP Discover** |
| Packet sent after IP offer? | **DHCP Request** |
| Final packet from DHCP server? | **DHCP ACK** |

---

# 🛠️ Tools & Concepts Practiced

- LAN Topology Simulation  
- Subnet Addressing  
- ARP Mechanism  
- DHCP Address Allocation  
- Network Architecture Analysis  

---

# 📚 Key Takeaways

- Understood major LAN topologies and their trade-offs  
- Learned how switches and routers function  
- Gained clarity on subnetting fundamentals  
- Understood ARP mapping process  
- Learned DHCP DORA process  
- Strengthened core networking knowledge for cybersecurity  

---

# 👩‍💻 Author

**Riya Dhakad**  
Cybersecurity Learner | TryHackMe Path Progress
