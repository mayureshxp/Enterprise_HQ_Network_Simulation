Operation Enterprise HQ Network

Enterprise LAN | Network Administration | Network Security

A simulated enterprise headquarters network designed and configured using Cisco Packet Tracer, implementing VLAN segmentation, inter-VLAN routing, automated IP addressing, internal network services, secure remote management, and Layer 2 switch security.

1. Project Overview

Operation Enterprise HQ Network demonstrates the design and configuration of a segmented enterprise headquarters network.

The network separates HR, IT, Administration, and Server departments into dedicated VLANs to improve network organization, traffic management, and security.

- Tool: Cisco Packet Tracer
- Project Type: Enterprise LAN Simulation
- Domain: Computer Networking
- Environment: Simulated Network Infrastructure

2. Network Architecture

The simulated infrastructure consists of:

- 1 Cisco Router (R1_HQ)
- 1 Managed Layer 2 Switch
- 2 HR Workstations
- 1 IT Workstation
- 1 Administration Workstation
- 1 Server

3. VLAN and IP Addressing Design

VLAN| Department| Network| Gateway
10| HR| 192.168.10.0/24| 192.168.10.1
20| IT| 192.168.20.0/24| 192.168.20.1
30| ADMIN| 192.168.30.0/24| 192.168.30.1
40| SERVER| 192.168.40.0/24| 192.168.40.1

4. Technologies Implemented

VLAN Segmentation

Created four departmental VLANs to logically separate network devices and departmental traffic.

Router-on-a-Stick

Configured 802.1Q trunking and router subinterfaces to enable communication between different VLANs.

DHCP

Configured DHCP pools for HR, IT, and ADMIN clients to automatically assign IP addresses, subnet masks, gateways, and DNS information.

DNS

Configured an internal DNS service to provide hostname resolution for the internal server.

Internal HTTP Web Server

Configured an internal web server with a static IP address and enabled HTTP service.

Created a custom webpage titled:

Operation Enterprise HQ Network

SSH Remote Management

Configured secure remote router administration using:

- SSH Version 2
- RSA 2048-bit keys
- Local user authentication
- Privilege level 15
- SSH-only VTY access

Example verification command:

"ssh -l admin 192.168.10.1"

Layer 2 Port Security

Implemented switch port security on five access ports using:

- Maximum one secure MAC address
- Sticky MAC address learning
- Shutdown violation mode

5. Testing and Verification

The following functions were tested in the simulation:

- VLAN assignment and segmentation
- Inter-VLAN connectivity
- DHCP address allocation
- Client-to-gateway communication
- Client-to-server connectivity
- DNS hostname resolution
- Internal HTTP webpage access
- SSH remote router login
- Port security and MAC address learning

6. Important Verification Commands

show vlan brief
show interfaces trunk
show ip interface brief
show port-security
show running-config
ping 192.168.40.10

7. Repository Contents

- "README.md" — Project overview and technical documentation
- Project report — Detailed project documentation
- "packet-tracer/" — Cisco Packet Tracer simulation file

8. Technical Skills Demonstrated

- Cisco Packet Tracer
- VLAN Configuration
- 802.1Q Trunking
- Router-on-a-Stick
- Inter-VLAN Routing
- DHCP
- DNS
- HTTP Server Configuration
- SSH Remote Management
- Switch Port Security
- Sticky MAC Learning
- Network Troubleshooting
- Connectivity Testing

9. Project Scope

This project was designed, configured, and tested entirely in Cisco Packet Tracer.

It represents a simulated enterprise network environment and was not deployed on physical enterprise networking hardware.

---

Project Name: Operation Enterprise HQ Network
Domain: Computer Networking
Focus: Enterprise Network Administration and Security
