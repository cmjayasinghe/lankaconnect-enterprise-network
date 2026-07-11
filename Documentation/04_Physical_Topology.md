# Physical Topology

## Purpose

This document describes the physical layout of the enterprise campus network for LankaConnect Telecommunications (Pvt) Ltd. It identifies the network devices, their physical locations, and how they are interconnected to provide a secure, scalable, and highly available network infrastructure.

---

# Headquarters Location

**Company:** LankaConnect Telecommunications (Pvt) Ltd

**Head Office:** Colombo 03, Sri Lanka

The headquarters occupies the fourth and fifth floors of a commercial office building.

---

# Physical Layout

## Fourth Floor

Departments:

* Human Resources (HR)
* Finance
* Sales & Marketing
* Administration

Network equipment:

* Access Switch 1
* Access Switch 2
* Two Lightweight Access Points

---

## Fifth Floor

Departments:

* Network Operations Center (NOC)
* Network Engineering
* Cybersecurity Operations (SOC)
* Cloud Engineering
* Software Development

Network equipment:

* Access Switch 3
* Access Switch 4
* Two Lightweight Access Points

---

## Server Room

The server room is located on the fifth floor and contains the organization's core networking and server infrastructure.

Equipment installed:

* Cisco ASA 5525-X Firewall
* ISP Router
* Core Switch 1
* Core Switch 2
* Distribution Switch 1
* Distribution Switch 2
* Server Access Switch
* Cisco 2811 Voice Gateway
* Cisco Wireless LAN Controller (WLC)
* Windows Server 2022
* ERP Server
* Email Server
* File Server
* Two Lightweight Access Points for server room coverage

---

# Network Device Inventory

| Device                                  | Quantity |
| --------------------------------------- | -------: |
| ISP Router                              |        1 |
| Cisco ASA 5525-X Firewall               |        1 |
| Cisco Catalyst 3850 Layer 3 Core Switch |        2 |
| Cisco Catalyst 2960 Distribution Switch |        2 |
| Cisco Catalyst 2960 Access Switch       |        5 |
| Cisco Wireless LAN Controller           |        1 |
| Cisco Lightweight Access Point          |        6 |
| Cisco 2811 Voice Gateway                |        1 |
| Windows Server 2022                     |        1 |
| ERP Server                              |        1 |
| Email Server                            |        1 |
| File Server                             |        1 |
| Desktop PCs                             |      310 |
| IP Phones                               |      310 |
| Network Printers                        |        8 |

---

# Device Naming Convention

| Device Type               | Naming Format    |
| ------------------------- | ---------------- |
| ISP Router                | ISP-RTR          |
| Firewall                  | ASA-FW           |
| Core Switches             | CORE-01, CORE-02 |
| Distribution Switches     | DIST-01, DIST-02 |
| Access Switches           | ACC-01 to ACC-05 |
| Voice Gateway             | VOICE-RTR        |
| Wireless LAN Controller   | WLC-01           |
| Lightweight Access Points | AP-01 to AP-06   |
| Windows Server            | SERVER-AD        |
| ERP Server                | SERVER-ERP       |
| Email Server              | SERVER-MAIL      |
| File Server               | SERVER-FILE      |

---

# Physical Connections

The network will be connected using the following hierarchy:

Internet

↓

ISP Router

↓

Cisco ASA Firewall

↓

Core Switch 1

↓

Core Switch 2

↓

Distribution Switches

↓

Access Switches

↓

End Devices

---

# Cabling Standards

The following cable types will be used:

| Connection                     | Cable Type                        |
| ------------------------------ | --------------------------------- |
| PC ↔ Switch                    | Copper Straight-Through           |
| Printer ↔ Switch               | Copper Straight-Through           |
| Server ↔ Switch                | Copper Straight-Through           |
| IP Phone ↔ Switch              | Copper Straight-Through           |
| Access Point ↔ Switch          | Copper Straight-Through           |
| Router ↔ Firewall              | Copper Straight-Through           |
| Firewall ↔ Core Switch         | Copper Straight-Through           |
| Switch ↔ Switch (EtherChannel) | Copper Cross-Over (Packet Tracer) |
| Console PC ↔ Network Device    | Console Cable                     |

---

# Redundant Links

To improve availability, redundant connections will be implemented between:

* Core Switch 1 and Core Switch 2
* Core Switches and Distribution Switches
* Distribution Switches and Access Switches (where applicable)

EtherChannel using LACP will be configured on critical switch-to-switch links.

---

# Wireless Coverage

The wireless infrastructure will provide coverage for all office areas.

Wireless deployment includes:

* Employee Wi-Fi
* Guest Wi-Fi
* Centralized management using the Wireless LAN Controller
* Lightweight Access Points distributed across both floors

---

# Server Farm

The server farm hosts the following services:

* Active Directory
* DNS
* DHCP
* RADIUS
* ERP System
* Email Server
* File Server

All servers are connected to the dedicated server access switch using Gigabit Ethernet.

---

# Internet Edge

The enterprise internet connection consists of:

* SLT Enterprise Fiber ISP
* ISP Router
* Cisco ASA Firewall
* Core Switching Layer

The Cisco ASA Firewall acts as the security boundary between the internal network and the public internet.

---

# Physical Design Objectives

The physical topology has been designed to:

* Minimize single points of failure
* Support future expansion
* Improve network availability
* Simplify troubleshooting
* Centralize infrastructure management
* Provide reliable wired and wireless connectivity

---

# Summary

The proposed physical topology follows Cisco's hierarchical campus network design model and provides a secure, scalable, and redundant infrastructure. The design supports the organization's operational requirements while allowing future growth with minimal changes to the physical architecture.
