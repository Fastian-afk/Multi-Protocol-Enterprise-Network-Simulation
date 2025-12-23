# Enterprise Network Design & Simulation

![Project Topology](Screenshots/Full_Topology.png)

## 📌 Project Overview
This project involves the design and simulation of a complex enterprise network using **Cisco Packet Tracer 8.2.2**. The topology integrates multiple routing protocols, advanced security measures, and efficient IP addressing strategies to simulate a real-world wide area network (WAN).

**Course:** Computer Networks (CL-3001) - Fall 2025
**Role:** Network Engineer / Student

## 🚀 Key Features
- **Multi-Protocol Routing:** Successful redistribution and full connectivity between **OSPF** (Area 0, 1, 2), **EIGRP** (AS 11), and **RIPv2**.
- **VLSM Addressing:** Optimized subnetting for 14 distinct networks, handling over 70,000 hosts with zero IP conflict.
- **Network Security:** Implemented Extended **ACLs** to secure critical servers (Web, Data, TFTP) from unauthorized access.
- **NAT Implementation:** Configured NAT Overload on the edge router (R15) to translate private traffic (Network G) to the public network.
- **Dynamic Services:** Two centralized **DHCP Servers** providing dynamic IP allocation across varying subnets using IP Helper addresses.

## 🛠️ Technology Stack
- **Simulation Tool:** Cisco Packet Tracer Student Version 8.2.2
- **Routing Protocols:** OSPFv2, EIGRP, RIPv2
- **Services:** DHCP, DNS, HTTP, TFTP
- **Security & Translation:** Extended ACLs, NAT/PAT

## 📂 Repository Structure
- `Simulation/`: Contains the main `.pkt` source file.
- `Documentation/`: Includes the detailed VLSM Tree, IP Allocation Tables, and Project Requirements.
- `Screenshots/`: Visual proof of network convergence and configuration.

## ⚙️ How to Run
1. Ensure you have Cisco Packet Tracer 8.2.2 or newer installed.
2. Clone this repository or download the `.pkt` file from the `Simulation` folder.
3. Open the file. The network will converge automatically (Fast Forward time if necessary).
4. Test connectivity using the PDU (Simple PDU) tool or Ping commands between any two devices.

## 📝 Configuration Highlights
- **Redistribution Nodes:** Routers 4, 6, 7, and 17 handle the translation of routing updates between different protocol domains.
- **NAT Router:** Router 15 serves as the gateway for the private 192.168.0.0/19 block.

---
*Created by [Your Name]*
