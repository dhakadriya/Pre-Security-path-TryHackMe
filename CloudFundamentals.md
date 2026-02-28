# ☁️ Cloud Computing Fundamentals
> TryHackMe Room Writeup  
> Author: **Riya Dhakad**

---

## 📖 Overview

This room introduces the fundamentals of **Cloud Computing**, a technology that allows applications and services to run on shared infrastructure accessible over the Internet.

Cloud computing solves problems such as:

- Application lag for global users
- Limited hardware resources
- System downtime
- Poor scalability

The cloud is built on technologies such as:

- Virtualization
- Containers

---

## 🎯 Learning Objectives

After completing this room:

- Understand Cloud Computing
- Learn Cloud Service Models (IaaS, PaaS, SaaS)
- Understand Cloud Types
- Learn Cloud Benefits
- Understand Real-World Cloud Usage

---

# 🧠 Task 1 — Introduction

Running an application on a personal computer has limitations:

- Limited performance
- Single location access
- Downtime if computer is off
- Cannot handle many users

Cloud computing solves these problems by allowing applications to run on distributed infrastructure.

---

# ☁️ Task 2 — Cloud Computing Overview

Cloud computing allows applications to run on **remote servers over the Internet**.

Instead of using one physical machine:

✔ Applications run on shared infrastructure  
✔ Users can access services globally  
✔ Systems scale automatically  

---

## 📈 Evolution of Servers

Infrastructure evolved through several stages:

1. Physical Servers
2. Virtual Machines
3. Containers
4. Cloud Computing

Each stage improved:

- Cost efficiency
- Resource utilization
- Scalability

---

# 🚀 Cloud Benefits

| Feature | Description |
|---------|-------------|
| Scalability | Increase or decrease resources easily |
| On-Demand Service | Create servers instantly |
| Pay-As-You-Go | Pay only for usage |
| Security | Provider-managed infrastructure security |
| High Availability | Minimal downtime |
| Global Access | Worldwide availability |

---

## ✅ Task 2 Answers

| Question | Answer |
|---------|--------|
| Feature that handles traffic spikes | **Scalability** |
| Most common cloud deployment | **Public Cloud** |
| Best service model for app development | **PaaS** |

---

# ☁️ Cloud Types

Cloud environments come in three deployment models.

---

## 🌐 Public Cloud

Features:

- Affordable
- Scalable
- Provider-managed

Used by:

- Startups
- Websites
- Applications

Examples:

- AWS
- Azure
- Google Cloud

---

## 🔒 Private Cloud

Features:

- High control
- High security
- Custom environments

Used by:

- Banks
- Healthcare
- Government

---

## 🔀 Hybrid Cloud

Features:

- Combination of public + private cloud
- Sensitive data kept private
- Scalable infrastructure

Used by:

- E-commerce companies
- Enterprise systems

---

# 🧩 Cloud Service Models

Cloud providers offer different levels of responsibility.

---

## 🖥 Infrastructure as a Service (IaaS)

User manages:

- Operating System
- Applications

Provider manages:

- Hardware
- Networking

Example:

- AWS EC2

---

## ⚙ Platform as a Service (PaaS)

User manages:

- Application

Provider manages:

- OS
- Hardware
- Infrastructure

Examples:

- Heroku
- Google App Engine

---

## 🌐 Software as a Service (SaaS)

Provider manages everything.

User only uses software.

Examples:

- Gmail
- Zoom
- Dropbox

---

# 🏢 Major Cloud Providers

| Provider | Specialization |
|---------|---------------|
| AWS | Industry leader |
| Microsoft Azure | Enterprise cloud |
| Google Cloud | AI & Analytics |
| Alibaba Cloud | Asia market |
| IBM Cloud | Hybrid cloud |
| Oracle Cloud | Enterprise databases |

---

# 🌍 Real World Cloud Usage

| Company | Usage |
|---------|-------|
| Netflix | Video streaming infrastructure |
| Spotify | Music storage & streaming |
| Instagram | Photo & video storage |
| E-Commerce | Traffic scaling |

---

# 🧪 Task 3 — Deploying Cloud Instances

You deployed cloud virtual machines similar to AWS EC2.

---

## 📌 EC2 Instances Created

| Instance Name | Type | Status |
|--------------|------|--------|
| application-interface | t3.micro | Running |
| study-machine-1 | m5.large | Running |
| study-machine-2 | m5.large | Running |

---

## 🌍 Region Selection

Region represents:

- Geographic location of servers

Example:

- Europe
- North America

Choosing a closer region reduces latency.

---

# 💰 Billing Analysis

Stopping unused instances reduces costs.

---

## ✅ Task 3 Answers

| Question | Answer |
|---------|--------|
| Total cost after stopping study machines | **30** |
| Cost of m5.large instance | **70** |
| Cost if new instances running | **150** |
| Cost with extra t3a.small instance | **188** |

---

# 🛠 Skills & Concepts Practiced

- Understanding cloud architecture
- Cloud service models
- Cloud deployment models
- Deploying virtual machines
- Cost optimization
- Cloud infrastructure basics

---

# 📚 Key Takeaways

- Cloud computing enables global applications
- Virtualization powers cloud infrastructure
- Public cloud is most common
- PaaS simplifies application deployment
- Cloud resources scale automatically
- Costs depend on usage
- Cloud is essential for modern applications
