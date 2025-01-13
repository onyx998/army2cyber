---
layout: post
title: "wireless networks"
date: 2025-01-013
author: "onyx998"
excerpt: "Covering the basics to wireless networks"
---

# Introduction
In this section of the course, we covered the fundamentals of wireless networks, focusing on the 802.11 standard. Understanding these concepts is crucial for anyone looking to work in networking and cybersecurity, as wireless technology is an integral part of modern communication systems.

[CompTIA Network+ (N10-009) Full Course & Practice Exam - Wireless Networks](https://www.udemy.com/course/comptia-network-009)

## Wireless Network Types
There are multiple wireless network types, each serving different purposes and use cases. The main types include Ad Hoc, Infrastructure, Point-to-Point, and Mesh.

### Ad Hoc
Ad Hoc networks are decentralized and allow devices to connect directly to each other without a central access point. This type of network is often used for temporary connections, such as in a meeting where participants share files directly between their devices.

### Infrastructure
Infrastructure networks rely on a central access point to connect devices. This setup is common in home and office environments. Key terms in this context include:
- **Basic Service Set Identifier (BSSID)**: The unique identifier for a specific access point in a wireless network.
- **Service Set Identifier (SSID)**: The name of the wireless network that devices use to connect.
- **Extended Service Set Identifier (ESSID)**: A name that identifies a set of access points that are part of the same network.

### Point-to-Point
Point-to-Point networks connect two devices directly, often used for connecting remote locations. An example is a wireless link between two buildings, allowing data transfer without physical cabling.

### Mesh
Mesh networks consist of multiple interconnected devices that communicate with each other. This type of network provides redundancy and improved coverage, making it ideal for large areas like campuses or smart cities.

## Wireless Antenna
Antennas are crucial components of wireless networks, as they transmit and receive radio signals. Different types of antennas serve various purposes, including:

- **Omnidirectional**: These antennas radiate signals in all directions, making them suitable for general coverage in a wide area.
- **Unidirectional**: These focus the signal in one direction, providing stronger coverage over longer distances, ideal for point-to-point connections.
- **Yagi**: A type of unidirectional antenna that is highly directional and often used for long-range communication.
- **Parabolic**: These antennas use a parabolic reflector to focus signals, providing high gain and long-range capabilities, commonly used in satellite communications.

## Wireless Frequencies
Wireless networks operate using radio waves, which are electromagnetic waves that carry data. The primary frequency bands used in wireless networking are 2.4GHz, 5GHz, and 6GHz, each with overlapping channels.

### 2.4GHz Frequency Band
The 2.4GHz frequency band is widely used for various wireless devices, including Wi-Fi and Bluetooth. It offers long-range capabilities, typically up to 300 feet indoors, and good penetration through walls. This band has 11 channels, but only channels 1, 6, and 11 are non-overlapping, making them the best choices for minimizing interference. The frequency range for this band is from 2.400 to 2.495 GHz.

### 5GHz Frequency Band
The 5GHz frequency band provides a higher performance option with less interference. It has a range of 5.180 to 5.825 GHz and offers 24 non-overlapping channels, each 20MHz wide. While it has a shorter range of about 150 feet indoors, it supports higher data rates, making it ideal for high-bandwidth applications.

### 6GHz Frequency Band
The 6GHz frequency band is relatively new and offers more channels and greater bandwidth. This band reduces congestion and provides improved performance for modern devices. It is designed to support the increasing demand for wireless connectivity.

### Other Mentions
- **Dynamic Frequency Selection (DFS)**: A feature that allows devices to automatically switch to less congested channels to improve performance.
- **Transmit Power Control (TPC)**: A mechanism that adjusts the power output of a device to minimize interference and optimize coverage.
- **Band Steering**: A technique that encourages dual-band devices to connect to the less congested 5GHz band instead of the 2.4GHz band.
- **Channel Bonding**: A method that combines two or more channels to increase bandwidth and improve data transfer rates.

## 802.11 Wireless Standards
There are multiple 802.11 standards used for different applications in wireless networking. Below is a summary of these standards:

| Name       | Frequency Band | Max Speed | Max Range |
|------------|----------------|-----------|-----------|
| 802.11     | 2.4GHz         | 2 Mbps    | 30m       |
| 802.11b    | 2.4GHz         | 11 Mbps   | 30m       |
| 802.11g    | 2.4GHz         | 54 Mbps   | 30m       |
| 802.11n    | 2.4GHz & 5GHz  | 600 Mbps  | 70m       |
| 802.11ac   | 5GHz           | 1.3 Gbps  | 100m      |
| 802.11ax   | 2.4GHz & 5GHz  | 9.6 Gbps  | 100m      |

## Wireless Security
Wireless security is essential to protect data transmitted over wireless networks. It involves various measures to safeguard against unauthorized access and attacks. 

### Wireless Authentication
Wireless security primarily relies on two main authentication methods: Pre-Shared Key (PSK) and Enterprise Authentication.

- **Pre-Shared Key (PSK)**: This method uses a shared password or passphrase to authenticate users. It is commonly used in home networks and small businesses, where a single key is shared among all users.
  
- **Enterprise Authentication**: This method employs a more robust security framework, often using protocols like 802.1X. It requires users to authenticate individually, typically through a username and password, making it suitable for larger organizations with more stringent security needs.

# Up Next
In the next chapter of the course, we will delve into Ethernet Switching. This topic will cover the fundamentals of how data is transmitted over wired networks, including the role of switches and the importance of network segmentation. Stay tuned for the next post, where we will explore this critical aspect of networking!


