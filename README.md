# Infrastructure & Protocol Analysis: Purple Team Week 1

**Author:** Muhammad Usama Bilal  
**Date:** March 8, 2026  
**Instructor:** Muhammad Saad  

## 🎯 Project Objective
The primary goal of this project is to establish a secure, isolated **Purple Team laboratory environment**. [cite_start]Using virtualization technology, this setup facilitates safe cybersecurity simulations within an internal network, ensuring zero interference with external production systems[cite: 55, 57].

## 🛠️ Tools & Environment
* [cite_start]**Virtualization Platform:** VMware Workstation [cite: 59]
* [cite_start]**Attacker Machine:** Kali Linux (IP: `192.168.72.128`) [cite: 60, 65]
* [cite_start]**Victim Machine:** Windows 10 (IP: `192.168.72.129`) [cite: 61, 66]
* [cite_start]**Network Topology:** Host-Only architecture (VMnet1) for complete isolation [cite: 62, 63]
* [cite_start]**Analysis Tool:** Wireshark [cite: 80]

## 📝 Task Overview

### Task 1: Virtualization and Topology Setup
* [cite_start]**Configuration:** Allocated hardware resources (RAM, CPU, Disk) specifically for Kali and Windows 10[cite: 69].
* [cite_start]**Connectivity:** Implemented static IP addressing to ensure persistent communication paths[cite: 71].
* [cite_start]**Verification:** Confirmed active internal links using the `ping` utility with 0% packet loss[cite: 73, 75].

### Task 2: Packet Analysis and Protocol Deep Dive
* [cite_start]**Methodology:** Captured live traffic on the `eth0` interface during an ICMP handshake[cite: 85, 86].
* [cite_start]**Filtering:** Applied Wireshark display filters to isolate ICMP traffic from background noise[cite: 87].
* [cite_start]**Technical Findings:** * Analyzed **Type 8 (Request)** and **Type 0 (Reply)** ICMP codes[cite: 93].
    * [cite_start]Inspected hexadecimal data payloads to verify data integrity between source and destination[cite: 94].

## 🏁 Conclusion
The lab provides a robust sandbox for security simulations. [cite_start]The successful capture and analysis of traffic confirm the network visibility required for professional security operations while remaining isolated from external threats[cite: 96, 98].
