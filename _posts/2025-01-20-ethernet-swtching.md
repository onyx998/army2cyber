---
layout: post
title: "wireless networks"
date: 2025-01-20
author: "onyx998"
excerpt: "Diving into concetps surrounding Ethernet Switching"
---

# Introduction
In this section of the course, we covered the fundamentals of networking, focusing on Ethernet switching and the various network devices that facilitate communication within a network. We explored how these components work together to create efficient and secure networks. For more details, you can check out the course here: [CompTIA Network+ (N10-009) Full Course & Practice Exam - Ethernet Switching](https://www.udemy.com/course/comptia-network-009).

## Ethernet Switching
Ethernet is a protocol used for local area networks (LANs) and is generally implemented with twisted pair cables. It defines how data packets are transmitted over the network, ensuring reliable communication between devices.

### How will Ethernet work?
When Ethernet was being developed, engineers had to choose between two primary methods of data transmission: deterministic and contention-based.

#### Deterministic
Deterministic methods ensure that data packets are sent in a predictable manner, with a defined order and timing. This approach can lead to more efficient use of the network but may introduce delays.

#### Contention-Based
Contention-based methods allow multiple devices to compete for access to the network medium. This approach was chosen for Ethernet due to its lower overhead and greater flexibility, enabling devices to transmit data as needed without waiting for a predetermined time slot.

### CSMA/CD (Carrier Sense Multiple Access with Collision Detection)
CSMA/CD is a network protocol that helps prevent and manage collisions in a network. When two devices attempt to send data simultaneously, a collision occurs. In this case, both devices will wait for a random amount of time before attempting to resend their data. The likelihood of collisions increases as more devices are connected to a single segment. However, switches can separate collision domains for each client, reducing the chances of collisions.

#### CS (Carrier Sensing)
Carrier Sensing refers to the process where a device listens to the network before transmitting data to ensure that the medium is free.

#### MA (Multiple Access)
Multiple Access allows multiple devices to share the same communication medium, enabling them to send and receive data.

#### CD (Collision Detection)
Collision Detection is the mechanism that identifies when a collision occurs and initiates the process of waiting before retransmission.

## Network Devices
A network device is any hardware that facilitates communication between computers and other devices on a network.

### Hub: Layer 1
A hub is a basic networking device known as a "Multi Port Repeater." Clients connected to a hub share the same collision domain, which can lead to network inefficiencies. 

#### Passive Hub
A passive hub simply connects devices without any processing or amplification of the signal.

#### Active Hub
An active hub can amplify signals and extend the maximum distance of Ethernet cables beyond 100 meters by breaking it up with hubs every 60 meters.

#### Smart Hub
A smart hub includes additional features such as management capabilities and monitoring of network traffic.

### Bridge: Layer 2
A bridge is a device that connects two or more network segments and analyzes source MAC (Media Access Control) addresses to make intelligent decisions based on destination MAC frames. It breaks up collision domains, and when combined with a hub, it forms a switch.

### Switch: Layer 2
A switch is often referred to as a multi-port bridge. It uses MAC tables and Address Resolution Protocol (ARP) to direct traffic and separate collision domains, improving network efficiency.

### Router: Layer 3
A router is a device that connects different networks and uses IP (Internet Protocol) addressing to route data. It separates broadcast domains, ensuring that data packets reach their intended destinations.

### Layer 3 Switch
A Layer 3 switch combines the functionalities of a router and a switch, making routing decisions and interconnecting entire networks rather than just network segments. However, it is not as efficient as a dedicated router.

## Virtual Local Area Network (VLAN)
A VLAN is a logical subdivision of a given network that segments it into separate broadcast domains. Before VLANs, multiple switches were required to achieve similar segmentation. VLANs tag each data packet with a VLAN ID as it passes through the switch.

### Benefits of VLAN
- **Enhanced Security**: VLANs can isolate sensitive data and devices, reducing the risk of unauthorized access.
- **Improved Performance**: By segmenting traffic, VLANs can reduce congestion and improve overall network performance.
- **Increased Management**: VLANs simplify network management by allowing administrators to group devices logically rather than physically.
- **Improved Cost Efficiency**: VLANs reduce the need for additional hardware, leading to cost savings.

### Switch Virtual Interface
A Switch Virtual Interface (SVI) allows a switch to route traffic between different VLANs without requiring a separate router, streamlining communication.

## VLAN Configuration
VLAN configuration involves setting up VLANs on a switch to manage network traffic effectively. 

### Trunking
Trunking refers to using the same switch to support multiple VLANs, allowing for efficient data transmission across different segments.

### 802.1Q (VLAN) Tagging
802.1Q is a networking standard that defines a method for tagging Ethernet frames with VLAN information. This tagging allows switches to identify which VLAN a particular frame belongs to as it traverses the network.

### Native VLAN Default
The Native VLAN is the default VLAN assigned to a port on a switch. If a frame arrives on a trunk port without a VLAN tag, it is assumed to belong to the Native VLAN. This configuration helps maintain compatibility with devices that do not support VLAN tagging.

### Voice VLAN
A Voice VLAN is a dedicated VLAN for voice traffic, such as Voice over IP (VoIP) calls. By segregating voice traffic from data traffic, it ensures better quality of service (QoS) and reduces latency for voice communications.

### Link Aggregation
Link Aggregation is a technique that combines multiple network connections into a single logical link to increase bandwidth and provide redundancy. This configuration helps improve network performance and reliability.

### Speed and Duplex Configurations
Speed and Duplex Configurations refer to the settings that determine the speed of the network connection (e.g., 10/100/1000 Mbps) and the mode of communication (half-duplex or full-duplex). Proper configuration of these settings is essential for optimal network performance.

## Spanning Tree Protocol
The Spanning Tree Protocol (STP) is a network protocol that prevents redundant links between switches and avoids looping of traffic. By creating a loop-free topology, STP ensures efficient data transmission across the network.

### Broadcast Domain (No Spanning Tree)
In a network without Spanning Tree Protocol, multiple copies of frames can be forwarded back and forth, leading to broadcast storms and network congestion.

### How Spanning Tree Protocol Works
STP operates by designating specific ports on switches to either forward or block traffic, creating a loop-free network topology. The following components are essential to its operation:

- **Root Bridge**: The central switch in the STP topology, which all other switches use as a reference point.
- **Non-root Bridge**: Any switch that is not the root bridge but participates in the STP process.
- **Root Ports**: The port on a non-root bridge that has the lowest cost path to the root bridge.
- **Designated Ports**: The port on a network segment that has the lowest cost to reach the root bridge, allowing traffic to flow.
- **Blocked Ports**: Ports that are disabled to prevent loops in the network.

STP uses these ports to create an efficient network topology, ensuring that data flows smoothly without looping.

## Network Access Control
Network Access Control (NAC) is a security solution that enforces policies for devices attempting to access a network. It ensures that only authorized devices can connect and operate within the network.

### Port Security
Port Security is a feature that restricts the number of devices that can connect to a specific port on a switch. It helps prevent unauthorized access and MAC address spoofing.

### MAC Filtering
MAC Filtering allows network administrators to specify which devices can connect to the network based on their MAC addresses. This method provides an additional layer of security.

### 802.1x Authentication
802.1x is a network access control protocol that provides an authentication mechanism for devices attempting to connect to a network. It ensures that only authenticated users can access network resources.

### Persistent and Non-persistent Agents
Persistent agents remain on a device after it connects to the network, maintaining its authentication status. Non-persistent agents, on the other hand, require re-authentication each time the device connects.

### Types of Other Access Controls
- **Time-Based**: Access control that restricts network access based on specific time frames.
- **Location-Based**: Access control that allows or denies access based on the physical location of the device.
- **Role-Based**: Access control that grants permissions based on the user's role within the organization.
- **Rule-Based**: Access control that uses predefined rules to determine access permissions.

## Maximum Transmission Unit (MTU)
The Maximum Transmission Unit (MTU) refers to the largest data packet or frame that can be sent over a given network. The standard MTU size is 1500 bytes. Adjusting the MTU size can significantly impact network performance; decreasing it can lead to increased overhead, while increasing it can enhance throughput but may cause fragmentation.

Wireless networks typically use a smaller MTU due to the nature of wireless communication. A Jumbo Frame is any frame that exceeds the default MTU size of 1500 bytes, with a standard Jumbo Frame size of 9000 bytes. Jumbo Frames can improve performance by allowing larger packets to be transmitted, reducing the number of packets sent over the network.

# Next Steps
In the next chapter of the course, we will delve into IP Addressing. This topic is crucial for understanding how devices communicate over networks and will provide a foundation for more advanced networking concepts. Stay tuned for the next post, where we will explore the intricacies of IP Addressing and its significance


