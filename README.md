# Advanced Network Configuration & Routing Project

This repository contains the complete **GNS3 project** for a complex network configuration.  
The project focuses on the implementation and redistribution of various **IP routing protocols**, including **OSPF, BGP, EIGRP, RIP, and static routing**.  
It also includes detailed configurations for a **Frame Relay WAN** and **VLANs** for network segmentation.

---

## 📌 Overview
This project showcases a **lab network built in GNS3** with multiple routers and switches.  
The files provided include the GNS3 project file and outputs from Cisco IOS devices, such as:

- Running configurations  
- IP routing tables  
- Traceroutes  
- VLAN databases  

It serves as a **practical, in-depth example** of a sophisticated network setup involving multiple routing domains, WAN technologies, and traffic engineering techniques.

---

## 🌐 Network Topology Visualization
The complete network topology is defined in the **`1.gns3`** project file.  

The layout consists of:
- A **core backbone of routers**  
- Several **access-layer switches**  
- Multiple **Frame Relay switches** acting as a WAN cloud  

---

## 🚀 Key Features
- **Advanced Dynamic & Static Routing**  
  Implementation of **OSPF (multi-area)**, **EIGRP (multi-AS)**, **RIP**, **BGP**, and **static routing**.  

- **Route Redistribution**  
  Configuration of **mutual redistribution** between routing protocols for full reachability.  

- **Layer 3 Switching**  
  Router with Switch Module (`sharifi/SW2`) performing access-layer routing.  

- **Policy-Based Routing (PBR)**  
  Route-map on **R6** influencing the path of specific traffic, overriding standard routing.  

- **Router-on-a-Stick**  
  Sub-interfaces on **R4** with `dot1Q` encapsulation for inter-VLAN routing.  

- **VLAN Segmentation**  
  VLANs for security and traffic separation: **7, 18, 26, 43, 47, 62**.  

- **Frame Relay WAN**  
  Frame Relay cloud with virtual switches (**FRSW1, FRSW2, FRSW3**) for WAN connectivity.  

- **Access Control**  
  Extensive use of **ACLs** for traffic filtering and network security.  

---

## 🖧 Network Devices
**Core/Edge Routers:**  
`R1, R2, R3, R4, R5, R6, BB1, BB2, BB3`

**Access Switches:**  
`SW1, SW2, ESW1, ESW2, ESW6, Switch1, Switch2`

**Frame Relay Switches:**  
`FRSW1, FRSW2, FRSW3`

---

## 📂 Repository Contents
- **GNS3 Project:**  
  `1.gns3`

- **Running Configurations:**  
  `R4_RC.txt, R5_RC.txt, R6_RC.txt, BB1_RC.txt, BB2_RC.txt, BB3_RC.txt, SW2-RC.txt`

- **IP Routing Tables:**  
  `R4_IR.txt, R5_IR.txt, R6_IR.txt, SW2_IR.txt, BB1_IR.txt, BB2_IR.txt, BB3_IR.txt`

- **Traceroutes:**  
  `R4_TR.txt, R5_TR.txt, BB2.txt`

- **VLAN Databases:**  
  `SW1-VLAN.txt, SW2-vlan.txt, ESW1_VLAN.txt, ESW2_VLAN.txt, ESW6_VLAN.txt`

---

## ⚡ How to Use
1. **Explore Configurations**  
   Review the text files to understand the network's architecture, routing logic, and ACL policies.  

2. **Load in GNS3**  
   Open `1.gns3` in **GNS3** to view and simulate the topology.  
   > ⚠️ You must provide your own Cisco IOS images and configure their paths in GNS3.  

3. **Learn & Experiment**  
   Use this project as a **study resource for networking certifications** or to **experiment with advanced designs**.  

---
