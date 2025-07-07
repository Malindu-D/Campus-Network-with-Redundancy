# Campus-Network-with-Redundancy

![Screenshot 2025-06-23 022559](https://github.com/user-attachments/assets/a0af8b10-b2c2-442d-9133-c0e935e45a0c)

This project demonstrates the design and implementation of a three-tier campus network featuring VLAN segmentation, dynamic routing with OSPF, and RIP as a backup protocol to ensure robust and efficient connectivity.

Overview
Architecture: Three-tier campus network (Core, Distribution, Access)

Segmentation: VLANs for each building and function (including CCTV and VoIP)

Dynamic Routing: OSPF as the primary protocol, RIP as a backup for redundancy

Traffic Management: VLANs improve traffic isolation and management

Network Topology
Core Layer ↔ Distribution Layer:

VLAN: 6

IP Range: 192.168.6.0/24

Internal Distribution Layer Connectivity:

VLAN: 16

IP Range: 172.16.6.0/24

Access Layer (Buildings):

Each building assigned a unique VLAN for its function

All buildings include dedicated VLANs for CCTV and VoIP

Dynamic Routing
Dynamic routing automates the process of updating routing tables, enabling the network to adapt to topology changes and failures without manual intervention.

OSPF (Open Shortest Path First):

Primary dynamic routing protocol

Fast convergence and scalability

Ensures optimal path selection between VLANs and buildings

RIP (Routing Information Protocol):

Configured as a backup protocol

Provides redundancy in case OSPF fails

Ensures continuous network connectivity

Core Switch Routing Table

![Screenshot 2025-06-23 015944](https://github.com/user-attachments/assets/e9efdf12-455b-4c3d-bf4c-4969f2606d28)
