# 🖥 Virtualization Fundamentals
> TryHackMe Room Writeup  
> Author: **Riya Dhakad**

---

## 📖 Overview

This room introduces the concept of **virtualization**, a key technology that powers modern cloud computing and large-scale infrastructure.

Virtualization allows multiple applications and operating systems to run on the same physical hardware efficiently and securely.

Topics Covered:

- Problems with physical servers
- Virtualization basics
- Hypervisors
- Virtual Machines (VMs)
- Containers
- Virtual Machine Management

Virtualization knowledge is essential for:

- Cybersecurity labs
- Cloud computing
- DevOps
- SOC environments
- Penetration testing labs

---

# 🧠 Task 1 — Introduction

In previous rooms, we learned about:

- Computer components
- Computer types
- Client-server architecture

This room explains how companies **optimize hardware usage** using virtualization.

---

## ❓ Why Virtualization?

Before virtualization:

> One Server = One Application

Problems:

- Expensive hardware
- Low hardware utilization
- Slow deployment
- Hard scaling

Example:

- Website → Server 1
- Database → Server 2
- Email → Server 3
- Internal App → Server 4

Most servers used only **5–20% capacity**, wasting resources.

---

# 🏢 Virtualization Concept

Virtualization allows:

> Multiple applications to share a single physical server safely.

---

## 🏢 Building Analogy

| Real World | Virtualization |
|----------|----------------|
| Building | Physical Server |
| Apartments | Virtual Machines |
| Tenants | Applications |
| Building Manager | Hypervisor |

---

## ✅ Task 2 Answers

| Question | Answer |
|---------|--------|
| What does virtualization allow applications to share? | **physical server** |
| Software managing virtual machines? | **hypervisor** |

---

# ⚙ Task 3 — Virtualization Components

## 🧩 Hypervisor

A hypervisor is software that manages virtual machines.

Responsibilities:

- Divides physical hardware
- Allocates resources
- Isolates VMs
- Controls VM lifecycle

---

## 🧠 Hypervisor Types

| Type | Description | Use Case |
|------|-------------|----------|
| Type 1 | Runs directly on hardware | Production servers |
| Type 2 | Runs on an OS | Labs & testing |

---

### 📌 Examples

Type 1:

- Data Centers
- Production Servers

Type 2:

- VirtualBox
- VMware Workstation
- Kali Linux Lab

---

## 🖥 Virtual Machines

Virtual Machines behave like real computers.

Each VM has:

- Virtual CPU
- Virtual RAM
- Virtual Disk
- Virtual Network

Features:

- Independent OS
- Isolation
- Fault tolerance

---

### 📌 VM Use Cases

- Running Kali Linux
- Malware testing
- Software testing
- Learning cybersecurity

---

## 📦 Containers

Containers are lightweight environments.

They:

- Run single applications
- Share OS kernel
- Start quickly
- Use fewer resources

---

## 🆚 VM vs Containers

| Feature | Virtual Machine | Container |
|---------|----------------|-----------|
| OS Included | Yes | No |
| Resource Usage | High | Low |
| Speed | Slower | Fast |
| Isolation | Strong | Moderate |

---

## 🐳 Docker

Docker is used to deploy containers.

Features:

- Fast deployment
- Application packaging
- Scalability

---

## ✅ Task 3 Answers

| Question | Answer |
|---------|--------|
| Hypervisor type for study lab? | **type 2** |
| Host multiple apps inside VM? | **containers** |

---

# 🖥 Task 4 — Managing Virtual Machines

You were assigned to manage the virtualization environment for **AutoGalo Company**.

Tasks included:

- Troubleshooting virtual machines
- Creating virtual machines
- Monitoring hosts
- Analyzing resource usage

---

## 🔧 Troubleshooting VM

Problem:

- Email service stopped working

Investigation:

- VM **Mail-SERVER** was in error state

Solution:

- Restart VM

Result:

✔ Email service restored

---

## 🏗 Creating Virtual Machine

New VM created:

| Setting | Value |
|---------|------|
| Name | Marketing-VM |
| CPU | 4 Cores |
| Memory | 8 GB |
| Disk | 100 GB |

---

## 🖥 Host Analysis

Hosts Status:

| Host | Status |
|------|--------|
| HV-PROD-01 | Available capacity |
| HV-PROD-02 | Nearly full |
| HV-BACKUP-01 | Disconnected |

---

## ✅ Task 4 Answers

| Question | Answer |
|---------|--------|
| VM running longest time | **Monitoring-SYS** |
| VM using most memory | **DB-Cluster-01** |
| Running VMs count | **8** |
| Host with most VMs | **HV-PROD-02** |

---

# 🛠 Skills & Concepts Practiced

- Understanding virtualization
- Understanding hypervisors
- Managing virtual machines
- Resource allocation
- Infrastructure monitoring
- Troubleshooting VMs

---

# 📚 Key Takeaways

- Virtualization improves hardware utilization
- Hypervisors manage virtual machines
- VMs behave like real computers
- Containers are lightweight alternatives
- Virtualization powers cloud computing
- Type 2 hypervisors are best for labs

---

# 👩‍💻 Author

**Riya Dhakad**  
Cybersecurity Learner | TryHackMe Fundamentals Path
