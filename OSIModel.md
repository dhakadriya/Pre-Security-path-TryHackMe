# 🧩 OSI Model – Complete Layer Breakdown  
> TryHackMe Room Writeup  
> Author: **Riya Dhakad**

---

## 📖 Overview

This room provides a complete breakdown of the **OSI (Open Systems Interconnection) Model**, explaining how data moves through a network across seven structured layers.

It covers:

- The 7 OSI Layers  
- Encapsulation  
- Routing Concepts  
- TCP vs UDP  
- Session Management  
- Encryption & Translation  
- Application Layer Protocols  
- Practical OSI Challenge  

Understanding the OSI model is fundamental for:

- Network troubleshooting  
- Packet analysis  
- Cybersecurity investigations  
- Penetration testing  
- SOC operations  

---

# 🧠 Task 1 — What is the OSI Model?

The **OSI Model** is a 7-layer framework that standardizes communication between network devices.

When data moves down the layers, additional information is added at each stage. This process is called:

> **Encapsulation**

---

## 📊 OSI Layers (Top → Bottom)

| Layer | Name |
|-------|------|
| 7 | Application |
| 6 | Presentation |
| 5 | Session |
| 4 | Transport |
| 3 | Network |
| 2 | Data Link |
| 1 | Physical |

---

## ✅ Task 1 Answers

| Question | Answer |
|----------|--------|
| What does OSI stand for? | **Open Systems Interconnection** |
| How many layers does the OSI model have? | **7** |
| What is the key term for adding information to data? | **Encapsulation** |

---

# 🔌 Task 2 — Layer 1: Physical

The **Physical Layer** handles the actual hardware responsible for transmitting binary data (0s and 1s).

Examples:

- Ethernet cables  
- Fiber optic cables  
- Network hardware  

---

## ✅ Task 2 Answers

| Question | Answer |
|----------|--------|
| Name of this layer? | **Physical** |
| What numbering system uses 0s and 1s? | **Binary** |
| What cables connect devices? | **Ethernet Cables** |

---

# 🧩 Task 3 — Layer 2: Data Link

The **Data Link Layer** handles:

- Physical (MAC) addressing  
- Frame formatting  
- Communication within the same network  

Each device contains a:

> **Network Interface Card (NIC)**

---

## ✅ Task 3 Answers

| Question | Answer |
|----------|--------|
| Name of this layer? | **Data Link** |
| Hardware every network device has? | **Network Interface Card** |

---

# 🌐 Task 4 — Layer 3: Network

The **Network Layer** is responsible for:

- Routing  
- Determining optimal path  
- Handling IP addresses  

Common routing protocols:

- **OSPF** — Open Shortest Path First  
- **RIP** — Routing Information Protocol  

Layer 3 devices: **Routers**

---

## ✅ Task 4 Answers

| Question | Answer |
|----------|--------|
| Name of this layer? | **Network** |
| Will packets take the most optimal route? | **Y** |
| OSPF stands for? | **Open Shortest Path First** |
| RIP stands for? | **Routing Information Protocol** |
| What addresses are handled here? | **IP Addresses** |

---

# 🚚 Task 5 — Layer 4: Transport

The **Transport Layer** ensures proper data delivery.

It uses:

| Protocol | Full Form | Reliability | Speed |
|----------|------------|------------|-------|
| TCP | Transmission Control Protocol | Reliable | Slower |
| UDP | User Datagram Protocol | Unreliable | Faster |

---

## 🔐 TCP

- Guarantees delivery  
- Error checking  
- Ordered packets  
- Used for: Email, Web browsing, File downloads  

## ⚡ UDP

- Faster transmission  
- No guarantee of delivery  
- Used for: Video streaming, Gaming, VoIP  

---

## ✅ Task 5 Answers

| Question | Answer |
|----------|--------|
| Name of this layer? | **Transport** |
| TCP stands for? | **Transmission Control Protocol** |
| UDP stands for? | **User Datagram Protocol** |
| Which guarantees accuracy? | **TCP** |
| Which doesn’t guarantee delivery? | **UDP** |
| Email client uses? | **TCP** |
| File downloads use? | **TCP** |
| Video streaming uses? | **UDP** |

---

# 🔐 Task 6 — Layer 5: Session

The **Session Layer**:

- Establishes connections  
- Maintains sessions  
- Closes inactive sessions  
- Uses checkpoints  

When a connection is successfully established:

> A **Session** is created.

---

## ✅ Task 6 Answers

| Question | Answer |
|----------|--------|
| Name of this layer? | **Session** |
| Technical term for successful connection? | **Session** |

---

# 🔄 Task 7 — Layer 6: Presentation

The **Presentation Layer** acts as a:

> **Translator**

It ensures data formatting consistency between systems.

Responsibilities:

- Data translation  
- Encryption (e.g., HTTPS)  
- Compression  

Even if two users use different software, this layer ensures data is readable.

---

## ✅ Task 7 Answers

| Question | Answer |
|----------|--------|
| Name of this layer? | **Presentation** |
| Main purpose of this layer? | **Translator** |

---

# 🖥 Task 8 — Layer 7: Application

The **Application Layer** is the layer closest to the user.

It includes:

- Web browsers  
- Email clients  
- File transfer software  
- DNS  

Users interact with data through:

> **Graphical User Interface (GUI)**

---

## ✅ Task 8 Answers

| Question | Answer |
|----------|--------|
| Name of this layer? | **Application** |
| Technical term for user-interaction software? | **Graphical User Interface** |

---

# 🏰 Task 9 — Practical: OSI Dungeon

In this interactive challenge, the OSI layers had to be arranged in the correct order to escape the dungeon.

Successfully completing the challenge revealed the flag.

---

## 🏁 Flag
THM{OSI_DUNGEON_ESCAPED}


---

# 🛠️ Skills & Concepts Practiced

- OSI layer responsibilities  
- Encapsulation  
- Routing fundamentals  
- TCP vs UDP comparison  
- Session management  
- Data translation & encryption  
- Application layer protocols  

---

# 📚 Key Takeaways

- Fully understood all 7 OSI layers  
- Learned how data flows across layers  
- Distinguished between TCP & UDP  
- Understood routing decisions  
- Learned how sessions and encryption work  
- Applied knowledge in practical OSI challenge  

---
<img width="1919" height="867" alt="Screenshot 2026-02-21 173048" src="https://github.com/user-attachments/assets/b01acf46-ab63-4768-a2a7-e336dfb83360" />

