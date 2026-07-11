# Business Requirements

## Company Overview

LankaConnect Telecommunications (Pvt) Ltd is a fictional Sri Lankan telecommunications and IT solutions provider headquartered in Colombo. The company delivers enterprise networking, cloud computing, cybersecurity, managed IT services, and VoIP solutions to businesses across Sri Lanka.

To support its growing operations, the company requires a secure, scalable, highly available, and centrally managed enterprise network that enables efficient communication between departments while maintaining strong security and reliable connectivity.

---

# Business Goals

The proposed network infrastructure must support the following business goals:

* Provide uninterrupted network connectivity for all employees.
* Ensure secure communication between departments.
* Support future business growth without requiring major network redesign.
* Protect business-critical data and services.
* Provide reliable access to cloud services hosted on Microsoft Azure.
* Enable secure internet access for employees and guests.
* Support centralized network management and monitoring.
* Ensure high availability through redundant network design.
* Improve collaboration through enterprise VoIP services.
* Deliver reliable wireless connectivity throughout the office.

---

# Office Layout

The company operates on two floors within its headquarters.

## Fourth Floor

Departments:

* Human Resources (HR)
* Finance
* Sales & Marketing
* Administration

## Fifth Floor

Departments:

* Network Operations Center (NOC)
* Network Engineering
* Cybersecurity Operations (SOC)
* Cloud Engineering
* Software Development
* Server Room

---

# Department Information

| Department                | Estimated Users |
| ------------------------- | --------------: |
| Human Resources           |              40 |
| Finance                   |              35 |
| Sales & Marketing         |              45 |
| Administration            |              30 |
| Network Operations Center |              40 |
| Network Engineering       |              30 |
| Cybersecurity Operations  |              25 |
| Cloud Engineering         |              30 |
| Software Development      |              35 |
| **Total Employees**       |         **310** |

---

# IT Infrastructure Requirements

The organization requires a modern enterprise infrastructure that includes:

* Core switching
* Distribution switching
* Access switching
* Secure internet connectivity
* Enterprise wireless networking
* Centralized wireless management
* Voice over IP (VoIP)
* Active Directory services
* DNS services
* DHCP services
* RADIUS authentication
* Internal application servers
* Firewall protection
* Microsoft Azure connectivity

---

# Hardware Requirements

The following network devices will be used:

* Cisco ASA 5525-X Firewall
* Cisco Catalyst 3850 Layer 3 Core Switches
* Cisco Catalyst 2960 Access Switches
* Cisco 2811 Voice Gateway
* Cisco Wireless LAN Controller (WLC)
* Cisco Lightweight Access Points
* Windows Server 2022
* Employee desktop computers
* IP Phones
* Network printers

---

# Network Services

The enterprise network must provide the following services:

* Active Directory Domain Services
* Dynamic Host Configuration Protocol (DHCP)
* Domain Name System (DNS)
* RADIUS Authentication
* Enterprise Wi-Fi
* Guest Wi-Fi
* Voice over IP (VoIP)
* Internet access
* Secure remote administration using SSH
* Internal ERP system
* Email services
* File sharing services

---

# Security Requirements

The network must comply with the following security requirements:

* Separate departments using VLANs.
* Isolate employee, guest wireless, and voice traffic.
* Protect the internal network using a Cisco ASA Firewall.
* Control access between network segments using Access Control Lists (ACLs).
* Secure remote device administration using SSH.
* Disable unnecessary services on network devices.
* Implement PortFast and BPDU Guard on access ports.
* Use Network Address Translation (NAT) for internet access.
* Secure management interfaces with administrator authentication.

---

# Performance Requirements

The network should:

* Support more than 300 users simultaneously.
* Deliver high-speed communication between departments.
* Minimize network downtime.
* Support real-time voice communication with low latency.
* Provide fast roaming for wireless users.
* Allow efficient access to cloud services.

---

# Scalability Requirements

The network design should support future expansion by allowing:

* Additional departments
* More employees
* Additional access switches
* More wireless access points
* Additional servers
* Expansion to future branch offices
* Integration with additional cloud services

---

# Availability Requirements

To ensure business continuity, the network must include:

* Redundant core switching
* EtherChannel (LACP) between critical switches
* Dynamic routing using OSPF
* High-speed backbone links
* Reliable internet connectivity
* Centralized network management
* Secure firewall protection

---

# Business Deliverables

At the completion of this project, the organization expects:

* A complete enterprise network topology
* Secure LAN, WLAN, and VoIP infrastructure
* Dynamic routing using OSPF
* Enterprise wireless deployment
* Firewall configuration
* Network security implementation
* Comprehensive technical documentation
* Successful connectivity and performance testing

---

# Success Criteria

The project will be considered successful if:

* All departments can communicate according to the defined security policies.
* Users receive IP addresses automatically where required.
* Internal services (ERP, Email, File Server) are accessible to authorized users.
* VoIP communication functions correctly.
* Wireless users can connect to the appropriate SSIDs.
* Internet access operates through the Cisco ASA Firewall.
* OSPF routes are exchanged successfully.
* Security controls function as designed.
* The network is fully documented and reproducible.

