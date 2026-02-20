**Networking Fundamentals**
<img width="1913" height="860" alt="image" src="https://github.com/user-attachments/assets/2cf157d7-b067-4526-9e63-8cdc9cfa3049" />

📌 Room Overview
This TryHackMe room introduces the fundamental concepts of computer networking, including how devices communicate within networks and across the Internet.

The room covers:

Network basics

Internet fundamentals

IP & MAC addressing

IPv4 vs IPv6

MAC spoofing

ICMP & Ping utility

These networking concepts form the foundation for understanding cybersecurity and penetration testing practices.

🎯 Objectives
Understand what networking is

Learn about private & public networks

Identify devices using IP & MAC addresses

Understand IPv4 & IPv6 addressing

Learn MAC spoofing concept

Use Ping tool for network testing

📍 Task 1: What is Networking?
A network refers to devices that are connected together in order to share information and communicate with one another.

In computing, networks can consist of:

Laptops

Smartphones

Servers

Security Cameras

IoT Devices

Networking is an essential concept in cybersecurity as it enables data communication across systems.

✅ Answer:
Network

📍 Task 2: What is the Internet?
The Internet is a global network of interconnected smaller networks.

It originated from the ARPANET project and later evolved with the invention of the World Wide Web (WWW) in 1989 by Tim Berners-Lee.

Networks can be classified as:

Private Networks

Public Networks

✅ Answer:
Tim Berners-Lee

📍 Task 3: Identifying Devices on a Network
Devices on a network are identified using:

IP Address → Logical Address

MAC Address → Physical Address

🌍 IP Address
An IP Address is used to uniquely identify a device on a network.

Consists of 4 sections in IPv4

Each section is known as an Octet

Public IP → Identifies device on Internet

Private IP → Identifies device within a local network

🖥️ MAC Address
MAC (Media Access Control) Address is:

A unique physical address

Assigned to network interface cards

Represented as hexadecimal values

Can be spoofed to bypass network restrictions

MAC Spoofing allows a device to impersonate another device by modifying its MAC address.

✅ Answers:
IP Stands For:
Internet Protocol

Section of an IP Address:
Octet

IPv4 Sections:
4

MAC Stands For:
Media Access Control

MAC Spoofing Lab Flag:
THM{YOU_GOT_ON_TRYHACKME}

📍 Task 4: Ping (ICMP)
Ping is a network utility used to test connectivity between devices using:

ICMP (Internet Control Message Protocol)

Ping sends:

Echo Request

Echo Reply

to measure network performance and availability.

🖥️ Ping Syntax:
ping 10.10.10.10

✅ Answers:
Protocol Used by Ping:
ICMP

Ping Syntax:
ping 10.10.10.10

Flag from 8.8.8.8:
THM{I_PINGED_THE_SERVER}

🛠️ Tools Used
TryHackMe Interactive Labs

Ping Utility

MAC Spoofing Simulation

📚 Key Takeaways
Understood networking fundamentals

Learned device identification methods

Explored IP & MAC addressing

Understood MAC Spoofing

Learned ICMP protocol usage

Tested connectivity using Ping

🚀 Author
Riya Dhakad
Cybersecurity Enthusiast | TryHackMe Learner
