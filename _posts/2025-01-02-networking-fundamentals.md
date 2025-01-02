---
layout: post
title: "Network Fundamentals"
date: 2025-01-02
author: "onyx998"
excerpt: "Learning networking fundamental knowledge covered in [CompTIA Network+ (N10-008) Course](https://www.udemy.com/course/comptia-network-009/)"
---

## Introduction

Networks encompass a diverse range of connectors that extend to both wireless and wired networks. Understanding these fundamentals is crucial,
as high availability and uptime are essential for any network's success. The "five nines" standard, which refers to 99.999% uptime, 
highlights the importance of reliability in network design and operation. Achieving this level of availability ensures that services remain accessible and functional, 
minimizing downtime and enhancing user experience.

[CompTIA Network+ (N10-008) Course](https://www.udemy.com/course/comptia-network-009/)
Networking Fundamentals Chapter

## Network Components

Understanding the various components that make up a network is vital for anyone pursuing a career in IT and networking. Below is a list of key network components along with their definitions:

- **Clients**: Devices that request services or resources from servers, such as computers, smartphones, or tablets.
- **Servers**: Powerful computers that provide resources, data, or services to clients over the network.
- **Hub**: A basic networking device that connects multiple Ethernet devices, making them act as a single network segment.
- **Wireless Access Point (WAP)**: A device that allows wireless devices to connect to a wired network using Wi-Fi.
- **Router**: A device that forwards data packets between computer networks, directing traffic and connecting different networks.
- **Firewall**: A security device that monitors and controls incoming and outgoing network traffic based on predetermined security rules.
- **Load Balancer**: A device that distributes network or application traffic across multiple servers to ensure no single server becomes overwhelmed.
- **Proxy**: An intermediary server that separates end users from the websites they browse, providing anonymity and security.
- **Intrusion Detection System (IDS)**: A device or software application that monitors network traffic for suspicious activity and alerts administrators.
- **Intrusion Prevention System (IPS)**: Similar to an IDS, but it also takes action to block or prevent detected threats.
- **Controllers**: Devices that manage and control network resources, often used in wireless networks to manage access points.
- **Network Attached Storage (NAS)**: A dedicated file storage device that provides data access to clients over a network (often referred to as NAT).
- **Storage Area Network (SAN)**: A specialized network designed to provide access to consolidated, block-level data storage.
- **Media**: The physical medium through which data is transmitted, such as cables (fiber optic, coaxial, etc.) or wireless signals.
- **Wide Area Network (WAN)**: A telecommunications network that extends over a large geographical area, connecting multiple local area networks (LANs).

## Network Resources

In networking, there are two main models for resource sharing: the client/server model and the peer-to-peer model.

- **Client/Server Model**: In this model, clients (devices requesting services) communicate with a centralized server that provides resources or services. This model is beneficial because it allows for centralized management, security, and resource allocation. However, it can create a single point of failure; if the server goes down, clients cannot access the resources.

- **Peer-to-Peer Model**: In a peer-to-peer (P2P) model, each device (or peer) on the network can act as both a client and a server, sharing resources directly with one another. This model is advantageous for its simplicity and reduced costs, as it does not require a dedicated server. However, it can lead to security challenges and difficulties in managing resources effectively.

## Network Geography

Network geography refers to the physical and logical layout of networks based on geographical distance. Various types of networks are categorized by their geographical scope:

- **Personal Area Network (PAN)**: A small network, typically within a range of a few meters, used for connecting personal devices like smartphones, tablets, and laptops.

- **Local Area Network (LAN)**: A network that connects devices within a limited area, such as a home, office, or building. LANs are commonly used for sharing resources like printers and files.

- **Campus Area Network (CAN)**: A network that connects multiple LANs within a specific campus, such as a university or corporate campus, allowing for resource sharing across buildings.

- **Metropolitan Area Network (MAN)**: A network that spans a city or a large campus, connecting multiple LANs and providing high-speed connectivity over a larger geographical area.

- **Wide Area Network (WAN)**: A network that covers a broad geographical area, connecting multiple LANs and MANs. For example, the internet is the largest WAN, and it typically consists of numerous LANs interconnected.

These networks are generally found within each other; for instance, a collection of LANs can be part of a larger WAN.

## Wired Network Topology

Wired network topology refers to the arrangement of different elements that make up a network. There are two main ways to view topology: physical topology and logical topology.

- **Physical Topology**: This refers to the actual physical layout of the network, including the devices and cables used to connect them.

- **Logical Topology**: This describes how data flows within the network, regardless of its physical layout.

Different types of wired network topologies include:

- **Point-to-Point**: A direct connection between two devices, providing a dedicated link.

- **Ring**: Each device is connected to two other devices, forming a circular pathway for data. Data travels in one direction, which can lead to delays if one device fails.

- **Bus**: All devices share a single communication line (the bus). While it is easy to set up, a failure in the bus can bring down the entire network.

- **Star**: All devices are connected to a central hub or switch. This topology is easy to manage and troubleshoot, but if the central hub fails, the entire network goes down.

- **Hub and Spoke**: A variation of the star topology where multiple remote sites (spokes) connect to a central site (hub). This is commonly used in WANs.

- **Mesh**: In a mesh topology, each device is interconnected, providing multiple pathways for data. There are two types: 
  - **Full Mesh**: Every device is connected to every other device, offering high redundancy.
  - **Partial Mesh**: Some devices are connected to all others, while some are only connected to those with which they exchange the most data.

## Wireless Network Topology

Wireless network topology refers to the arrangement of devices in a wireless network. The three main types include:

- **Infrastructure Mode**: This is the most common wireless topology, where devices connect to a central access point (AP). Examples include home Wi-Fi networks and corporate wireless networks.

- **Ad Hoc Mode**: In this mode, devices connect directly to each other without a central access point. This is useful for temporary networks, such as when sharing files between devices in close proximity.

- **Wireless Mesh Topology**: In this topology, multiple access points communicate with each other to extend coverage. This is often used in large areas where a single access point cannot provide sufficient coverage.


## Data Center Topology

Data centers utilize specific topologies to manage large amounts of data and resources efficiently. Common topologies include:

- **Three-Tier Hierarchy**: This architecture consists of three layers:
  - **Core Layer**: The backbone of the network, providing high-speed connectivity between different parts of the data center.
  - **Distribution/Aggregation Layer**: This layer connects the core layer to the access layer, managing traffic and policy enforcement.
  - **Access/Edge Layer**: The layer where end devices connect, providing access to the network resources.

- **Collapsed Core**: In this topology, the core and distribution layers are combined into a single layer, simplifying the architecture and reducing costs. This is often used in smaller data centers where high availability is still required.

- **Spine and Leaf Architecture**: This design consists of two layers: the spine layer, which connects all leaf switches, and the leaf layer, which connects to servers and storage. This architecture allows for high bandwidth and low latency, making it suitable for modern data centers.

Traffic flows in data centers are generally regarded as **North-South** and **East-West**:

- **North-South Traffic**: Refers to data flowing between the data center and external networks (e.g., users accessing applications hosted in the data center). This traffic typically involves higher latency and is subject to more security checks.

- **East-West Traffic**: Refers to data flowing between devices within the data center (e.g., communication between servers). This traffic is usually more frequent and requires high bandwidth, as it supports the internal operations of applications and services.

Understanding these topologies and traffic flows is essential for designing efficient and scalable data center networks.


  
## Upcoming

In the next blog post, I will cover the OSI Model, exploring its seven layers and their functions in network communication. Stay tuned for insights into how this foundational concept shapes networking practices!

  

---


