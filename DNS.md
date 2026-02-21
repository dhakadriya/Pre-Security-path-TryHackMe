# 🌍 DNS (Domain Name System) Fundamentals  
> TryHackMe Room Writeup  
> Author: **Riya Dhakad**

---

## 📖 Overview

This room introduces the **Domain Name System (DNS)** — the system responsible for translating human-readable domain names into machine-readable IP addresses.

Topics Covered:

- What DNS is  
- Domain Hierarchy  
- DNS Record Types  
- DNS Request Flow  
- Practical DNS Queries  

DNS knowledge is essential for:

- Network troubleshooting  
- OSINT & Reconnaissance  
- SOC investigations  
- Red Team enumeration  
- Web infrastructure analysis  

---

# 🧠 Task 1 — What is DNS?

DNS (Domain Name System) allows users to access websites using names instead of IP addresses.

Instead of remembering:
104.26.10.229

We can simply remember:
tryhackme.com

DNS acts like the Internet’s phonebook, mapping domain names to IP addresses.

---

## ✅ Task 1 Answer

| Question | Answer |
|----------|--------|
| What does DNS stand for? | **Domain Name System** |

---

# 🌐 Task 2 — Domain Hierarchy

DNS is structured in a hierarchical format.

## 🏛 Domain Structure
subdomain.secondleveldomain.topleveldomain

Example:
admin.tryhackme.com

---

## 🔹 Top-Level Domain (TLD)

Rightmost part of domain name.

Types:

| Type | Meaning | Example |
|------|---------|----------|
| gTLD | Generic | .com, .org, .edu |
| ccTLD | Country Code | .co.uk, .ca |

---

## 🔹 Second-Level Domain (SLD)

The name registered before the TLD.

Example:
tryhackme.com

Here:

- `tryhackme` → Second-Level Domain  
- `.com` → TLD  

---

## 🔹 Subdomain

Sits before the Second-Level Domain.

Example:
admin.tryhackme.com

Rules:

- Maximum length: 63 characters  
- Allowed characters: a-z, 0-9, hyphen  
- Cannot start/end with hyphen  
- Cannot use consecutive hyphens  
- Entire domain max length: 253 characters  

---

## ✅ Task 2 Answers

| Question | Answer |
|----------|--------|
| Maximum subdomain length? | **63** |
| Character not allowed? | **_** |
| Maximum domain length? | **253** |
| Type of TLD is .co.uk? | **ccTLD** |

---

# 📦 Task 3 — DNS Record Types

DNS supports multiple record types beyond simple website lookups.

---

## 📌 Common DNS Records

| Record | Purpose |
|--------|----------|
| A | Maps to IPv4 address |
| AAAA | Maps to IPv6 address |
| CNAME | Maps to another domain |
| MX | Mail server record |
| TXT | Stores text data |

---

### 📧 MX Record

Specifies mail server responsible for handling email.

Includes:

- Server address  
- Priority value (lower number = higher priority)

---

### 🔐 TXT Record

Used for:

- SPF (email validation)  
- Domain ownership verification  
- Security validation  

---

## ✅ Task 3 Answers

| Question | Answer |
|----------|--------|
| Record used for email routing? | **MX** |
| Record used for IPv6? | **AAAA** |

---

# 🔄 Task 4 — DNS Request Process

When you request a domain:

### 1️⃣ Local Cache
Your system checks local DNS cache.

### 2️⃣ Recursive DNS Server
Usually provided by your ISP.

If not cached:

### 3️⃣ Root Server
Directs request to correct TLD server.

### 4️⃣ TLD Server
Directs to authoritative nameserver.

### 5️⃣ Authoritative Server
Provides final DNS record.

---

## 🕒 TTL (Time To Live)

TTL determines how long a DNS response should be cached (in seconds).

---

## ✅ Task 4 Answers

| Question | Answer |
|----------|--------|
| Field that controls cache duration? | **TTL** |
| DNS server usually provided by ISP? | **recursive** |
| Server that stores all domain records? | **authoritative** |

---

# 🧪 Task 5 — Practical DNS Queries

Used DNS query tool to inspect records.

---

## 🏁 Practical Answers

| Question | Answer |
|----------|--------|
| CNAME of shop.website.thm? | **shops.myshopify.com** |
| TXT record of website.thm? | **THM{7012BBA60997F35A9516C2E16D2944FF}** |
| MX priority value? | **30** |
| A record IP of www.website.thm? | **10.10.10.10** |

---

# 🛠️ Skills & Concepts Practiced

- Domain hierarchy analysis  
- DNS record identification  
- Understanding DNS request flow  
- Interpreting MX priority values  
- Reading TXT validation records  
- Mapping domains to IP addresses  

---

# 📚 Key Takeaways

- DNS translates domain names to IP addresses  
- Domains follow strict hierarchical structure  
- Multiple DNS record types serve different purposes  
- Recursive, root, TLD & authoritative servers work together  
- TTL controls caching behavior  
- DNS is crucial for both defensive monitoring & offensive reconnaissance  

---
