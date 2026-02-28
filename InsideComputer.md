# 💻 Computer Fundamentals – Introduction
> TryHackMe Room Writeup  
> Author: **Riya Dhakad**

---

## 📖 Overview

Before learning cybersecurity, it is essential to understand **what we are securing**.  
This room introduces the fundamental components of a computer system and explains how they work together.

Topics Covered:

- Computer system components  
- Hardware basics  
- Boot process  
- Firmware and bootloaders  

Understanding computer fundamentals is important for:

- Cybersecurity beginners  
- SOC analysts  
- Ethical hackers  
- System administrators  

---

# 🧠 Task 1 — Introduction

Before defending a system, we must first understand how it works.

### 🏰 Analogy

Defending a computer without understanding it is like:

> Defending a castle you have never seen.

We must understand:

- Components  
- Structure  
- Access methods  
- Data flow  

---

## 🎯 Learning Objectives

After completing this room:

- Understand computer components
- Understand component functions
- Understand how components interact

---

## ✅ Task 1 Result

No answer required.

---

# 🖥 Task 2 — Inside a Computer System

Most computer systems contain similar components.

Each component has a specific function, and together they allow the system to operate.

---

## 🔧 Core Computer Components

Typical components include:

- CPU (Processor)
- RAM (Memory)
- Storage Devices
- Motherboard
- Power Supply Unit (PSU)
- Input Devices
- Output Devices

These components work together to process data and provide services to users.

---

## 🧪 Practical Exercise Flag
THM{4llpccomp0n3nts1d3nt1f13d}


---

# ⚡ Task 3 — Boot Process

The boot process begins when the power button is pressed.

This process prepares the computer to run the operating system.

---

## 🧩 Boot Sequence Steps

### 1️⃣ Power Button Pressed

- Power signal sent to PSU
- Electricity flows through components

---

### 2️⃣ Firmware Starts

Firmware initializes hardware.

Main firmware:

- **UEFI**
- **BIOS (legacy)**

Firmware prepares system components.

---

### 3️⃣ Power-On Self Test (POST)

POST checks:

- Hardware presence
- Hardware configuration
- Hardware functionality

If something fails → Error detected.

---

### 4️⃣ Boot Device Selection

UEFI checks boot priority list.

Examples:

- Hard Disk
- SSD
- USB
- Network Boot

---

### 5️⃣ Bootloader Execution

Bootloader:

- Loads Operating System
- Transfers OS to RAM
- Hands control to OS

After this:

✔ Operating System starts  
✔ User interface appears

---

## 🧪 Practical Exercise Flag
THM{pc5ucce55fully5t4rt3d}


---

# 🛠 Skills & Concepts Practiced

- Understanding computer architecture
- Identifying hardware components
- Understanding firmware
- Understanding boot process
- Understanding operating system loading

---

# 📚 Key Takeaways

- Cybersecurity requires understanding computer systems
- Computers consist of multiple components
- Each component has a specific function
- Firmware initializes hardware
- Bootloaders start operating systems
- OS manages system resources

---
