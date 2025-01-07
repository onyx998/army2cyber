---
layout: post
title: "media and cabling"
date: 2025-01-07
author: "onyx998"
excerpt: "Learning about media, cabling, and different connectors"
---


# Introduction
In this part of the course, we covered the fundamentals of media and cabling, focusing on the various types of copper and fiber optic cables used in networking. Understanding these components is essential for building and maintaining efficient network infrastructures.

[CompTIA Network+ (N10-009) Full Course & Practice Exam - Media and Cabling](https://www.udemy.com/course/comptia-network-009) 

## Copper Media
Copper cabling is the most common type of cabling used in networking today. The types of copper cables that will be mentioned include twisted pair, coaxial, and twinaxial.

### Twisted Pair
Twisted pair cables consist of pairs of wires twisted together to reduce electromagnetic interference. There are two types of twisted pair cables: shielded twisted pair (STP) and unshielded twisted pair (UTP). The twisting helps to minimize interference from external sources. The different categories of twisted pair cables include:

- **CAT5**: 100 Mbps, 100 meters, 100 MHz (100BASE-T 'Fast Ethernet')
- **CAT5e**: 1 Gbps, 100 meters, 100 MHz (1000BASE-T 'Gigabit Ethernet')
- **CAT6**: 1 Gbps, 100 meters, 250 MHz (1000BASE-T 'Gigabit Ethernet')
- **CAT6a**: 10 Gbps, 100 meters, 500 MHz (10GBASE-T '10 Gigabit Ethernet')
- **CAT7**: 10 Gbps, 100 meters, 600 MHz (10GBASE-T '10 Gigabit Ethernet')
- **CAT8**: 25-40 Gbps, 30 meters, 2000 MHz (25GBASE-T/40GBASE-T)

### Coaxial (Coax) Cable
Coaxial cables are used for transmitting data, video, and audio signals. They generally support speeds up to 10 Gbps and are typically used in cable television and internet connections. Additionally, Direct Attach Copper (DAC) cables are a type of coaxial cable used for short-distance connections in data centers.

### Twinaxial Cable 
Twinaxial cables are similar to coaxial cables but consist of two inner conductors. They are used for high-speed data transmission, typically supporting speeds up to 10 Gbps over short distances. Twinaxial cables are often preferred for data center interconnects due to their lower cost and flexibility compared to traditional coaxial cables.

### Plenum Cables
Plenum cables are designed for use in spaces with high airflow, such as air ducts. These cables are important for fire safety regulations, as they are made with materials that emit low smoke and are less likely to ignite. Plenum-rated cables are essential in environments with high levels of oxygen, where fire hazards are a concern.

### IEEE 802.3 Standard
The IEEE 802.3 standard defines the physical and data link layers of wired Ethernet networks. It is used with copper cabling and operates at the OSI model's physical and data link layers. This standard utilizes Media Access Control (MAC) addresses and ports to facilitate communication between devices on a network.

## Copper Network Connectors
Copper network connectors are essential for establishing connections between devices. 

### RJ-x - Registered Jack Type 
Registered Jack connectors are primarily used for twisted pair cables. 

#### RJ-11
RJ-11 connectors are typically used for telephone lines and have a smaller form factor with 4 or 6 positions.

#### RJ-45
RJ-45 connectors are the most common type of connector used for Ethernet cables. They have 8 positions and are what most people think of when they think of Ethernet connections.

### RG-x - Radio Guide Type
Radio Guide connectors are used with coaxial cables.

#### RG-6
RG-6 connectors are commonly used for cable television and internet connections, providing better shielding and higher frequencies.

#### RG-59
RG-59 connectors are being replaced by RG-6 due to their lower performance and higher attenuation over longer distances.

#### Other
- **Bayonet**: A type of connector that locks in place with a twist, commonly used in video applications.
- **F Type**: A connector used for coaxial cables, often found in cable television and satellite installations.

## Building Copper Cable
Building copper cables involves adhering to specific wiring standards, such as T-568A and T-568B. The primary difference is that T-568B is typically used for internal wiring and is applied on both ends of a straight-through cable. 

Data Terminal Equipment (DTE) refers to devices that communicate over a network, such as computers and printers, while Data Communications Equipment (DCE) includes devices that facilitate communication, such as modems and switches.

### Straight-through Cable
A straight-through cable has both ends wired to T-568B standards. This type of connection is used for connecting DTE to DCE devices. For example, a straight-through cable can connect a laptop to a switch or a computer to a router.

### Cross Over Cable
A crossover cable has one end wired to T-568A and the other end wired to T-568B. This type of connection is used for connecting DTE to DTE devices or DCE to DCE devices. Examples include connecting two computers directly or linking two switches together.

## Fibre Media
Fiber optic cables are immune to electromagnetic interference (EMI), offer very high speeds, and have a vastly increased range compared to copper cables. However, they are generally more expensive. The two main types of fiber optic cables are Single-Mode Fiber and Multi-Mode Fiber.

### Single-Mode Fiber
Single-Mode Fiber is designed for long-distance communication and is typically housed in a yellow color sheath. It allows for a single light path, which minimizes signal loss and enables higher bandwidth over longer distances.

### Multi-Mode Fiber
Multi-Mode Fiber is tailored for short-range communication and is usually found in aqua blue or orange sheaths. It supports multiple light paths, making it suitable for shorter distances, such as within a building or campus.

## Fibre Network Connections
Fiber network connections utilize various types of connectors, including SC, LC, ST, MTRJ, and MPO. 

- **SC (Subscriber Connector)**: A push-pull connector that is easy to use and commonly found in data centers.
- **LC (Lucent Connector)**: A smaller form factor connector that allows for higher density connections.
- **ST (Straight Tip)**: A bayonet-style connector often used in legacy systems.
- **MTRJ (Mechanical Transfer-Registered Jack)**: A compact connector that combines both the transmitter and receiver in one unit.
- **MPO (Multi-Fiber Push-On)**: A high-density connector used for multi-fiber applications.

Different polishes, such as UPC (Ultra Physical Contact), APC (Angled Physical Contact), and PC (Physical Contact), affect the performance of fiber connections. These polishes determine how the fiber ends are finished, impacting the amount of light reflected back and the overall signal quality.

## Transceivers
Transceivers are devices that combine a transmitter and a receiver in a single unit, allowing for bidirectional data transmission over a single medium. Each transceiver is designed to work with different protocols and can support various types of connections, including fiber and copper. Key points to consider include compatibility with network standards, distance capabilities, and the type of media used.

# Conclusion
In the next chapter of the course, we will explore Distribution Systems, which will cover the organization and management of network cabling and connections. Stay tuned for insights and information on this critical aspect of networking!

