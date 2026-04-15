# TryHackMe - Pre-Security Path

**Labs completed:** 31  
**Time to complete:** 19 hours 10 minutes  
**Profile:** [JCER](https://tryhackme.com/p/JCER)

---

## Overview
Foundational cybersecurity path covering networking, operating systems, web technologies, 
and introductory offensive and defensive security concepts. Completed alongside CompTIA 
A+ and Network+ certifications, with focus on cybersecurity-specific applications and 
hands-on CLI work.

---

## Network Fundamentals
Reinforced core networking concepts including TCP/IP, UDP, DHCP, packet forwarding, 
firewalls, and VPN basics — building on existing CompTIA Network+ knowledge with a 
security-focused lens.

---

## How the Web Works
DNS hierarchy and record types, HTTP methods and status codes, headers, cookies, and 
web application architecture. Covered security-relevant topics including sensitive data 
exposure, HTML injection, Web Application Firewalls, and the difference between static 
and dynamic content.

---

## Computer Fundamentals
Virtualization architecture, hypervisor basics, and containers. Notable hands-on tools:

- **Virtualization Manager** — TryHackMe simulated hypervisor management platform. 
Managed VMs across multiple hosts, monitored CPU/memory/storage usage. Real-world 
equivalents: VMware vSphere, Proxmox VE.
- **TryHackMe Cloud Console (EC2 Simulation)** — Provisioned and managed virtual 
machine instances across compute tiers (t3.micro, t3.small, m5.large). Practiced 
instance state management, resource allocation, and cost monitoring — directly 
applicable to real AWS EC2 environments.

---

## Operating Systems Basics
Dual focus on Linux and Windows CLI — the core of day-to-day SOC analyst work.

**Linux CLI commands practiced:**
`pwd`, `ls`, `ls -l`, `ls -al`, `cd`, `find`, `cat`, `whoami`, `uname -a`, `df -h`, 
`ssh`, `su`, `history`

Key tasks: navigating the filesystem, searching for files, reading configuration files, 
accessing system information, escalating to root using valid credentials, and completing 
guided investigation missions inside a Linux environment.

**Windows CLI commands practiced:**
`ping`, `dir`, `dir /a`, `cd`, `type`, `whoami`, `hostname`, `systeminfo`, `ipconfig`

---

## Software Basics
Number systems (binary, octal, decimal, hex), data encoding standards (ASCII, Unicode, 
UTF-8/16/32), and introductory scripting concepts in Python and JavaScript — variables, 
conditionals, and loops. SQL fundamentals including writing queries using `SELECT`, 
`FROM`, `WHERE`, `ORDER BY`, and `DESC`.

---

## Attacks and Defenses
The most cybersecurity-focused module of the path — covering both offensive and 
defensive fundamentals.

**Blue Team / Defensive:**
- CIA Triad — completed scenario-based exercises classifying real cybersecurity incidents 
into Confidentiality, Integrity, and Availability categories
- Cryptography — plaintext vs. ciphertext, symmetric vs. asymmetric encryption, public/
private key infrastructure, and how encryption protects web browsing
- Blue team methodology — prevention, detection, mitigation, analysis, response, and 
continuous improvement
- Infrastructure protection — employee devices, web servers, mail servers, firewalls, 
and internet traffic
- Key concepts: threat anticipation, attack awareness, risk prioritization

**Red Team / Offensive:**
- Offensive security terminology — red teaming, pen testing, vulnerability, exploit, scope
- Used **Gobuster** to enumerate hidden pages on a simulated target website by 
directory brute-forcing
- Chained discovered login page vulnerability to gain admin account access
- Used **Hydra** to perform a dictionary attack via CLI against the target
- All techniques practiced in a safe, permission-based environment

---

*Completed as part of an active transition from physical security into cybersecurity, 
building toward a blue team / incident response career path.*
