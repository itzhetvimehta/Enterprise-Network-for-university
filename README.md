# Enterprise-Network-for-university

## Overview
This project is a **Final Year Diploma Project** aimed at designing and implementing a **secure and efficient enterprise network** for a university using **Cisco Packet Tracer**.

## Project at a Glance
- Provides connectivity between **three sections/labs** (Accounts, Faculty, Student) located at different locations.
- Implements **OSPF Routing** for internet connectivity.
- **Access Control Lists (ACLs)** restrict students from accessing faculty and account servers.
- **VLANs** are configured to break broadcast traffic between departments.
- **Port Security** is enforced to prevent unauthorized devices from connecting to the network.
- Flexible network setup, allowing easy modification of ACLs and VLANs as needed.

## Purpose
- Ensures **efficient management and maintenance** of the university’s network.
- Students can only access the **CMS server**.
- Faculty members can access both the **CMS server and faculty server**.
- The **Accounts section** can access all three servers (CMS, Faculty, and Accounts server).
- The **Accounts server** is restricted to the **Accounts section** only.

## Scope
This network is designed to manage connectivity among three sections:
1. **Accounts**
   - Can access any website via the Internet.
   - Can access all three servers (Accounts, CMS, and Faculty server).
2. **Faculty**
   - Can access any website via the Internet.
   - Can access CMS and Faculty servers.
3. **Students**
   - Can only access **educational websites** through the Internet.
   - Can access the **CMS server**.

## Technical Description
### **Packet Tracer**
- Developed by **Cisco**, Packet Tracer is a **network simulation tool**.
- Allows users to **design, configure, and simulate** complex network topologies.
- Supports various Cisco **routing and switching** protocols.
- Enables **multi-user collaboration and competition** in real-time.
- Simulates **command-line configurations** for routers and switches.

## System Analysis
### **Introduction to the Network**
- Enterprise network design for a **university campus**.
- Three sections: **Student Lab, Faculty Block, and Accounts Section**.
- Three servers:
  - **Account Server**: `account.edu.in`
  - **Faculty Server**: `faculty.edu.in`
  - **CMS Server**: `cms.edu.in`
- IP addressing scheme:
  - **Student Lab**: `192.168.10.2 - 192.168.10.9` (connected via **Switch-2**)
  - **Accounts Section**: `192.168.40.2 - 192.168.40.8` (included in **VLAN-3**)
  - **Faculty Block**: `192.168.20.2 - 192.168.20.7` (included in **VLAN-2**)
- **Router-1** and **Router-2** connect all sections via **Switch-3**.
- External access provided through an **ISP Router**.

### **Hardware and Software Requirements**
#### **Software:**
- **Cisco Packet Tracer**

#### **Hardware:**
- **Computers**: 21
- **Switches**: 3
- **Routers**: 6
- **Servers**: 6

### **Protocols and Technologies Used**
- **OSPF Routing**
- **Access Control Lists (ACLs)**
- **VLAN & Inter-VLAN Routing**
- **Network Address Translation (NAT)**
- **Port Security**
- **Domain Name System (DNS)**
- **Secure Shell (SSH)**

## Limitations
- Requires a **qualified Network Administrator** to manage and maintain the network.
- **No backup system** available in Cisco Packet Tracer’s virtual environment.
- **Cannot configure alternate DNS** in Packet Tracer.
- If a link fails, the network **disconnects due to the lack of backup links**.

## Future Enhancements
- **Network Expansion** to accommodate more departments and sections.
- **Implementation of DHCP** for automatic IP address allocation.


