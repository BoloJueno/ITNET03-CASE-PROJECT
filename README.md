---

# **AITC Network Expansion – ITNET03 Case Project**

This project designs and implements an expanded enterprise network for the Alonzo IT Training Center (AITC), following the ITNET03 Case Project specifications (SY 2021–2022). The goal of the network upgrade is to scale the previous ITNET02 network to support increased users, improved performance, redundancy for fault tolerance, wireless access, and centralized management capabilities.

---

## **📍 Project Objectives**

This project demonstrates the ability to:

* Analyze technical requirements and translate them into a complete network design
* Apply subnetting, VLAN segmentation, DHCP, routing, wireless, and security mechanisms
* Discuss and justify design decisions and implementation choices
* Produce a working network simulation and documentation

---

## **🏢 Scenario Overview**

The organization is expanding and adding:

* More faculty, operations staff, and students
* A new Guest user group
* An additional building floor to accommodate new training rooms and a library

The network must scale accordingly using the existing address space **192.168.0.0/20**.

---

# **PHASE 1 – Network Scaling, Performance, and Redundancy**

The Phase 1 deliverables extend the ITNET02 design to support more users and ensure performance and availability.

---

## **📌 Phase 1 Requirements**

### **1. Logical Addressing**

* Continue using **192.168.0.0/20**
* Reallocate subnets based on the expanded user groups
* Assume each user brings **1 personal device** on WLAN
* IP addressing must remain systematic and aligned with VLAN assignments
* DHCP required for dynamic host address assignment

---

### **2. Network Performance**

Implement performance-enhancing configurations such as:

* High-speed link selection
* Link aggregation where appropriate
* Protocol optimizations to ensure efficient traffic flow

---

### **3. Network Fault Tolerance**

Ensure network availability through:

* Redundant physical paths and equipment
* Failover-ready routing/switching mechanisms
* Fast convergence protocol tuning

---

### **4. Network Security**

Apply baseline infrastructure protection:

* Strengthen passwords across device access
* Secure remote access (SSH)
* Apply Layer-2 switch security controls
* Perform housekeeping cleanup on devices
* Disable ACLs from ITNET02 (remove from interfaces, retain configs)

---

### **5. Network Manageability**

Maintain the ITNET02 manageability features:

* VLAN grouping + inter-VLAN routing via VTP
* Consistent IP addressing scheme
* DHCP-enabled address distribution

---

## **📁 Phase 1 Deliverables**

### Documentation

Required sections include:

* **IP Addressing Scheme**

  * VLAN/subnet tables
  * Host address assignment tables

* **Physical Topology**

  * Updated floor plan
  * Device interface connections

* **Logical Topology**

  * All routers/switches + servers/printers
  * Representative PC per user group

* **Device Passwords Summary**

* **Design Discussion**

  * How performance + redundancy were implemented
  * What technologies were selected
  * Why they were configured that way

### Packet Tracer Simulation

* Fully configured routers, switches, and servers
* 1 wired endpoint per major user group

---

# **PHASE 2 – Wireless Networking + Advanced Management + Policy Update**

The Phase 2 requirements continue building on Phase 1 by adding organizational wireless networks and improved management/security mechanisms.

---

## **📌 Phase 2 Requirements**

### **1. Wireless Connectivity**

* WLAN access for supported groups
* Wireless hosts must map to VLAN of owner group
* Wired/wireless must follow identical security policies
* Wireless networks must have proper authentication

---

### **2. Centralized Management**

* Devices log events to the Orion server
* Logs must have correct timestamps
* Enable SNMP and enforce access restrictions

  * Admin PC – read/write access
  * IT staff – read-only access

---

### **3. Updated Access Policies**

* Guest users may only communicate with the IT group
* Regular employees may access each other and Services networks
* Access to Management network reserved for network admin PCs only
* Policy must apply uniformly to wired and wireless devices

---

## **📁 Phase 2 Deliverables**

### Documentation

Must update based on Phase 1 feedback and include:

* Updated addressing if needed
* Updated physical + logical topologies showing WAPs
* Updated password summaries
* Extended Design Discussion including wireless + SNMP implementations

### Packet Tracer Simulation

* Fully configured routers, switches, servers, and WAPs
* Working Phase 1 + Phase 2 configuration
* At least:

  * 1 wired + 1 wireless endpoint per user group (except students, wired only)

---

## **🛠 Technologies + Tools**

* Cisco Packet Tracer
* VLANs + VTP
* DHCP
* OSPF / Static Routes (depending on design approach)
* SSH + SNMP
* WLAN + secured access
* ACL-based policy enforcement
* Redundancy + convergence protocols

---
