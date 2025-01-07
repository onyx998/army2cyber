---
layout: post
title: "ports and protocols"
date: 2025-01-05
author: "onyx998"
excerpt: "This chapter covered ports and protocols"
---

# Introduction
In this section of the course, we covered the essential concepts of Ports and Protocols, which are fundamental to understanding network communication.

[CompTIA Network+ (N10-008) Course - Ports and Protocols](https://www.comptia.org/certifications/network) 

## Ports and Protocols
Ports and protocols are crucial for network communication. Different ports are assigned for various services, allowing multiple applications to run simultaneously on a single device. While ports are endpoints for communication, protocols define the rules and conventions for data exchange.

### Network Port Fundamentals
A port is a numerical identifier in the range of 0 to 65535 that helps direct network traffic to the appropriate application. Ports are categorized into three types:

#### Well-Known Ports
- **Range:** 0 to 1023
- **Description:** These ports are reserved for widely used protocols and services, such as HTTP (80) and FTP (21).

#### Registered Ports
- **Range:** 1024 to 49151
- **Description:** These ports are assigned by the Internet Assigned Numbers Authority (IANA) for specific services and applications.

#### Ephemeral Ports
- **Range:** 49152 to 65535
- **Description:** These ports are temporary and are used for client-side communication, allowing multiple connections to be established.

## Transmission Control Protocol (TCP)
Transmission Control Protocol (TCP) is a core component of the Internet Protocol Suite. It operates at the transport layer of the OSI (Open Systems Interconnection) model and is designed for reliable communication.

### Three-way Handshake
The three-way handshake process consists of:
1. **SYN:** The client sends a synchronization request to the server.
2. **SYN-ACK:** The server acknowledges the request and responds.
3. **ACK:** The client acknowledges the server's response, establishing a reliable connection.

### Error Checking
TCP employs error checking through sequence numbers, ensuring that data packets are received in the correct order and without corruption.

### Flow Control
TCP uses a technique called windowing to manage the flow of data, allowing the sender to send multiple packets before needing an acknowledgment from the receiver.

### TCP and Ports
TCP can utilize multiple ports for different applications, enabling various services to run concurrently on a single device.

## User Datagram Protocol (UDP)
User Datagram Protocol (UDP) is another transport layer protocol that shares similarities with TCP. However, it is connectionless and does not guarantee reliability, making it suitable for applications where some packet loss is acceptable, such as video streaming.

UDP is stateless, meaning it does not establish a connection before sending data, and it does not perform error checking. The UDP header is 8 bytes in size, compared to TCP's 20 to 60 bytes. Like TCP, UDP can also use multiple ports for various applications.

## Internet Control Message Protocol (ICMP)
Internet Control Message Protocol (ICMP) is primarily used for diagnosing networking issues. It prioritizes speed and simplicity in communication. ICMP messages consist of three main parts: Type, Code, and Checksum.

### ICMP Flood Attack
An ICMP flood attack is a type of Denial of Service (DoS) attack that overwhelms a target with ICMP Echo Request (ping) packets, causing network congestion and service disruption.

### Ping of Death
The Ping of Death is another DoS attack that involves sending oversized ICMP packets to a target, potentially causing system crashes or instability.

## Web Ports and Protocols
Web communication relies on specific ports and protocols. Port 80 is used for HTTP (Hypertext Transfer Protocol), while port 443 is used for HTTPS (HTTP Secure).

### Port 80: HTTP
HTTP operates over port 80 and is used for transmitting web pages. However, it lacks security features, making it vulnerable to attacks.

### Port 443: HTTPS
HTTPS operates over port 443 and provides a secure communication channel through encryption, ensuring data integrity and confidentiality.

## Email Ports and Protocols
Email communication utilizes several protocols, including:

- **Simple Mail Transfer Protocol (SMTP):** Port 25
- **Post Office Protocol (POP3):** Port 110
- **Internet Message Access Protocol (IMAP):** Port 143

### Simple Mail Transfer Protocol (SMTP)
SMTP is used for sending emails and operates over port 25. It transmits messages in plain text, but a secure alternative, SMTPS, uses port 465 for encrypted communication.

### Post Office Protocol (POP3)
POP3 is used to retrieve emails from a server and operates over port 110. It downloads emails to the client and deletes them from the server. The secure variant, POP3S, operates over port 995.

### Internet Message Access Protocol (IMAP)
IMAP allows users to manage their emails directly on the server and operates over port 143. It also has a secure variant, IMAPS, which operates over port 993.

## File Transfer Ports and Protocols
File transfer protocols are essential for transferring files over a network. The main protocols include:

- **File Transfer Protocol (FTP):** Port 21
- **Secure File Transfer Protocol (SFTP):** Port 22
- **Trivial File Transfer Protocol (TFTP):** Port 69
- **Server Message Block (SMB):** Port 445

### File Transfer Protocol (FTP)
FTP is a standard network protocol used for transferring files between a client and a server. It operates over port 21 and supports both anonymous and authenticated access. A secure variant, FTPS, uses port 990 for encrypted connections.

### Secure File Transfer Protocol (SFTP)
SFTP is a secure version of FTP that operates over port 22. It provides encryption for data in transit, ensuring confidentiality and integrity during file transfers.

### Trivial File Transfer Protocol (TFTP)
TFTP is a simplified version of FTP that operates over port 69. It is used for transferring files without the need for authentication, making it suitable for simple file transfers in local networks.

### Server Message Block (SMB)
SMB is a network file sharing protocol that operates over port 445. It allows applications to read and write to files and request services from server programs. SMB can also be secured using SMB over SSL/TLS.

## Remote Access Ports and Protocols
Remote access protocols enable users to connect to and manage devices over a network. Key protocols include:

- **Secure Shell (SSH):** Port 22
- **Telnet:** Port 23
- **Remote Desktop Protocol (RDP):** Port 3389

### Secure Shell (SSH)
SSH is a secure protocol used for remote administration and file transfers. It operates over port 22 and provides strong encryption, ensuring secure communication between the client and server.

### Telnet
Telnet is an older protocol used for remote access to devices, operating over port 23. However, it transmits data in plain text, making it insecure compared to SSH.

### Remote Desktop Protocol (RDP)
RDP is a proprietary protocol developed by Microsoft for remote desktop access. It operates over port 3389 and allows users to connect to and control a remote computer securely.

## Network Service Ports and Protocols
Network services rely on specific protocols to function effectively. Key services include:

- **Domain Name System (DNS):** Port 53
- **Dynamic Host Configuration Protocol (DHCP):** Ports 67 and 68
- **SQL Services:** Port 1433
- **Simple Network Management Protocol (SNMP):** Port 161
- **Syslog:** Port 514

### Domain Name System (DNS)
DNS translates human-readable domain names into IP addresses. It operates over port 53 and is essential for navigating the internet.

### Dynamic Host Configuration Protocol (DHCP)
DHCP automates the assignment of IP addresses to devices on a network. It uses port 67 for server communication and port 68 for client communication.

### SQL Services
SQL services, such as Microsoft SQL Server, typically operate over port 1433. This protocol is used for managing and querying databases.

### Simple Network Management Protocol (SNMP)
SNMP is used for network management and monitoring. It operates over port 161 and allows administrators to manage network devices and gather performance data.

### Syslog
Syslog is a standard for message logging in network devices. It operates over port 514 and is used for collecting and storing log messages from various devices.

## Other Network Service Ports and Protocols
In addition to the previously mentioned services, several other protocols are essential for network functionality:

- **Network Time Protocol (NTP):** Port 123
- **Session Initiation Protocol (SIP):** Port 5060
- **Lightweight Directory Access Protocol (LDAP):** Port 389

### Network Time Protocol (NTP)
NTP is used to synchronize clocks across networked devices. It operates over port 123 and ensures accurate timekeeping for various applications.

### Session Initiation Protocol (SIP)
SIP is used for initiating, maintaining, and terminating real-time communication sessions, such as voice and video calls. It typically operates over port 5060.

### Lightweight Directory Access Protocol (LDAP)
LDAP is used for accessing and maintaining distributed directory information services. It operates over port 389 and is commonly used for authentication and authorization in network environments.

# Conclusion
In the next chapter of the course, we will explore Media and Cabling, which will cover the physical aspects of networking, including different types of cables and their uses. Stay tuned for the next post!

