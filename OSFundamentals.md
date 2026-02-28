# 💻 Operating System Fundamentals
> TryHackMe Room Writeup  
> Author: **Riya Dhakad**

---

## 📖 Overview

Every time you turn on your computer or smartphone, an **Operating System (OS)** works behind the scenes to manage hardware, applications, and users.

This room explains:

- What an Operating System is
- Responsibilities of an OS
- OS privilege levels
- Types of Operating Systems
- GUI vs CLI interaction
- Real-world OS examples

---

## 🎯 Learning Objectives

After completing this room:

- Understand what an Operating System is
- Learn OS responsibilities
- Understand Kernel vs User space
- Identify OS types
- Practice gathering system information

---

# 🧠 Task 1 — Introduction

An **Operating System (OS)** is the core software that connects:

- User
- Applications
- Hardware

Without an OS:

- Applications would control hardware directly
- Systems would crash frequently
- No structured resource management

---

# 🧩 Task 2 — The Invisible Manager

The OS acts as the **central coordinator** of a computer system.

### Computer Architecture Layers
User
↓
Applications
↓
Operating System
↓
Hardware


---

## ✈️ OS Airport Analogy

| Component | Analogy |
|----------|---------|
| Hardware | Runways and planes |
| Applications | Airlines |
| Operating System | Air Traffic Control |

The OS ensures:

- Resource scheduling
- Conflict prevention
- Safe operations

---

# 🔐 System Privilege Layers

Operating systems separate access levels for safety.

---

## Kernel Space

- Full hardware access
- Core OS functions
- Highest privilege

Examples:

- CPU control
- Memory management
- Device control

---

## User Space

- Runs applications
- Restricted access
- Uses system calls

Examples:

- Browsers
- Music players
- Games

---

## ✅ Task 2 Answers

| Question | Answer |
|---------|--------|
| OS space with hardware access | **Kernel Space** |
| Responsibility managing users | **User Management** |
| Ubuntu Mate version | **1.26.2** |
| Memory allocated | **1.9 GiB** |

---

# ⚙️ Operating System Responsibilities

Operating systems perform several core duties.

---

## 🧠 OS Core Duties

| Responsibility | Description | Example |
|--------------|-------------|---------|
| Process Management | Controls running programs | Running multiple apps |
| Memory Management | Allocates RAM | Opening many programs |
| File System Management | Organizes files | Creating folders |
| User Management | Controls access | Login system |
| Device Management | Controls hardware | Plugging USB |

---

# 🔒 OS Security Functions

Operating systems provide built-in security.

### Security Features

- Authentication
- Permissions
- Isolation
- System Protection

---

# 🖥 Task 3 — OS Interaction

Users interact with operating systems in two ways.

---

## 🖱 Graphical User Interface (GUI)

Features:

- Icons
- Windows
- Menus
- Mouse interaction

Example:

- File Explorer

---

## ⌨ Command Line Interface (CLI)

Features:

- Text commands
- Precise control
- Faster operations

Example:
ls

## 🧭 GUI vs CLI

| Feature | GUI | CLI |
|--------|-----|-----|
| Ease of Use | Easy | Medium |
| Speed | Slower | Faster |
| Control | Limited | High |

---

## 🌍 Operating System Types

Different devices require different operating systems.

---

### 🖥 Desktop OS

**Use Cases**

- Personal computers
- Gaming
- Workstations

**Examples**

- Windows 10 / 11
- macOS
- Ubuntu Linux

---

### 🗄 Server OS

**Use Cases**

- Web servers
- Databases
- Cloud systems

**Examples**

- Ubuntu Server
- Windows Server
- Red Hat Linux

---

### 📱 Mobile OS

**Use Cases**

- Smartphones
- Tablets

**Examples**

- Android
- iOS

---

### ⚙ Embedded OS

**Use Cases**

- Smart devices
- Routers
- Appliances

**Examples**

- Embedded Linux
- FreeRTOS
- QNX

---

### ☁ Virtual / Cloud OS

**Use Cases**

- Virtual machines
- Containers

**Examples**

- Ubuntu LTS
- Amazon Linux
- Alpine Linux

---

## 🌐 Popular Operating Systems

| OS Family | Examples |
|----------|----------|
| Windows | Windows 10, Windows 11 |
| Linux | Ubuntu, Debian |
| macOS | Sonoma, Sequoia |
| Mobile | Android, iOS |

---

## 🔎 Task 3 Investigation

System analysis was performed using:

- System Monitor
- File Explorer

---

## ✅ Task 3 Answers

| Question | Answer |
|---------|--------|
| File system type | **ext4** |
| Number of user directories | **3** |
| Flag in note.txt | **THM{new_pc_for_free!}** |

---

## 🛠 Skills & Concepts Practiced

- Understanding OS architecture
- Kernel vs User space
- OS responsibilities
- System monitoring
- File system investigation
- GUI navigation
- OS types

---

## 📚 Key Takeaways

- Operating Systems connect hardware and applications
- Kernel space has full system access
- Applications run in user space
- OS manages CPU, RAM and storage
- OS provides built-in security
- GUI and CLI both interact with the OS
- Different OS exist for different purposes
