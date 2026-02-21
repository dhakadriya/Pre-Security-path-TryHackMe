# 🔐 Port Forwarding, Firewalls & VPNs  
> TryHackMe Room Writeup  
> Author: **Riya Dhakad**

---

## 📖 Overview

This room covers critical networking security concepts including:

- Port Forwarding  
- Firewalls (Stateful vs Stateless)  
- VPN Fundamentals  
- Routers & Switches  
- VLAN Segmentation  
- Network Simulation (TCP Packet Flow)  

These concepts are essential for:

- SOC Analysts  
- Network Engineers  
- Penetration Testers  
- Blue Team Operations  

---

# 🚪 Task 1 — Port Forwarding

Port forwarding allows services inside a private network to be accessible from the Internet.

Without port forwarding:

- Services (e.g., web servers) are only accessible internally (Intranet)

With port forwarding:

- Public traffic is forwarded to a specific internal IP and port

---

## 📌 Key Concept

Port forwarding is configured on the:

> **Router**

It opens specific ports and forwards traffic to a designated internal device.

⚠ Important distinction:
- Port forwarding opens ports
- Firewalls decide whether traffic is allowed

---

## ✅ Task 1 Answer

| Question | Answer |
|----------|--------|
| Device used to configure port forwarding? | **router** |

---

# 🔥 Task 2 — Firewalls

A **Firewall** controls incoming and outgoing network traffic.

It determines traffic based on:

- Source address  
- Destination address  
- Port number  
- Protocol (TCP/UDP)  

Firewalls operate at:

> OSI Layer 3 & Layer 4

---

## 🛡 Firewall Types

| Category | Description |
|------------|-------------|
| Stateful | Inspects entire connection |
| Stateless | Inspects individual packets |

---

### 🔍 Stateful Firewall
- Monitors full connection
- Dynamic decision-making
- Higher resource usage
- Blocks entire device if malicious

### ⚡ Stateless Firewall
- Uses fixed rules
- Inspects packets individually
- Faster, fewer resources
- Ideal for high traffic (e.g., DDoS)

---

## ✅ Task 2 Answers

| Question | Answer |
|----------|--------|
| OSI Layers firewalls operate at? | **3 & 4** |
| Firewall that inspects entire connection? | **stateful** |
| Firewall that inspects individual packets? | **stateless** |

---

# 🧪 Task 3 — Practical Firewall Challenge

Configured the firewall to block malicious traffic on port 80.

### 🏁 Flag
THM{FIREWALLS_RULE}


---

# 🌐 Task 4 — VPN Basics

A **Virtual Private Network (VPN)** creates a secure encrypted tunnel over the Internet.

It allows:

- Secure communication between remote networks
- Encrypted traffic over public WiFi
- Privacy & anonymity

TryHackMe uses a VPN to:

- Securely connect users to lab machines
- Prevent public exposure of vulnerable systems

---

## 🔒 VPN Technologies

| Technology | Description |
|------------|-------------|
| PPP | Authentication & encryption only |
| PPTP | Allows PPP data to travel |
| IPSec | Encrypts using IP framework |

---

## ✅ Task 4 Answers

| Question | Answer |
|----------|--------|
| VPN technology that encrypts & authenticates data? | **PPP** |
| VPN technology using IP framework? | **IPSec** |

---

# 🌍 Task 5 — LAN Networking Devices

---

## 📡 Router

A router:

- Connects networks
- Performs routing
- Operates at OSI Layer 3
- Decides optimal path based on:
  - Shortest path
  - Reliability
  - Speed (copper vs fibre)

---

## 🔌 Switch

A switch connects devices within the same network.

Switch Types:

| Type | Function |
|-------|----------|
| Layer 2 | Forwards frames using MAC |
| Layer 3 | Routes packets using IP |

---

## 🏢 VLAN (Virtual LAN)

VLAN allows devices to be logically separated within the same physical network.

Benefits:

- Improved security
- Network segmentation
- Controlled communication between departments

Example:
- Sales & Accounting can access Internet
- But cannot communicate directly

---

## ✅ Task 5 Answers

| Question | Answer |
|----------|--------|
| Verb for router action? | **routing** |
| Two switch layers? | **Layer 2,Layer 3** |

---

# 🖥 Task 6 — Network Simulator Practical

Simulated sending a TCP packet from Computer1 to Computer3.

The simulator displayed:

- Full TCP handshake
- Packet encapsulation steps
- Routing process

---

## 🏁 Flag
THM{YOU'VE_GOT_DATA}


---

## 📊 Additional Question

| Question | Answer |
|----------|--------|
| Number of HANDSHAKE entries? | **5** |

---

# 🛠️ Skills & Concepts Practiced

- Port forwarding configuration  
- Firewall rule logic  
- Stateful vs Stateless inspection  
- VPN architecture  
- Router vs Switch functionality  
- VLAN segmentation  
- TCP packet traversal  

---

# 📚 Key Takeaways

- Understood public access via port forwarding  
- Learned firewall traffic control mechanisms  
- Distinguished stateful & stateless firewalls  
- Understood VPN encryption & tunneling  
- Differentiated router & switch roles  
- Explored VLAN-based segmentation  
- Visualized TCP handshake in simulation  

---

