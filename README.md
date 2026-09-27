# University Enterprise Network Topology & VPN Simulation

## Computer Networks – Banana Problem

A Cisco Packet Tracer project that models a structured **University Enterprise Network Topology** with multiple academic blocks connected through a common campus network and VPN connectivity.

---

## Project Overview

This project represents a university network organized using a structured hierarchical model.

The network consists of four major university blocks:

1. Engineering Block
2. Mechanical Block
3. Pharmacy Block
4. Medical Block

These blocks are connected to a **common main campus switch**.

The network design focuses on:

- Efficient network segmentation
- Network security
- Ease of network management
- Centralized campus connectivity
- VPN connectivity for web browser access

---

## Network Topology

The conceptual structure of the university network is:

```text
                    UNIVERSITY NETWORK
                           |
                  Main Campus Switch
              _________|_____|_________
             |         |     |         |
             |         |     |         |
       Engineering  Mechanical Pharmacy Medical
          Block        Block     Block   Block
The complete topology is implemented in the Cisco Packet Tracer project.
```
🔐 ## VPN Connectivity

The project includes a VPN connection to provide secure connectivity between the university network and external network resources.

The exact router interfaces, IP addresses, peer addresses, authentication parameters, ACLs, and cryptographic configuration should be inspected directly from the .pkt file.

## VPN Verification Commands

If Cisco IOS IPsec VPN is configured:
```text
show crypto isakmp sa
show crypto ipsec sa
show crypto map
show running-config | section crypto
```
## VPN Testing

Generate traffic between the required networks:
```text
ping <destination-ip>
```
Then verify the VPN:
```text
show crypto isakmp sa
show crypto ipsec sa

Check the IPsec packet counters to confirm that VPN traffic is being processed.
```
## 🛠️ Technologies & Tools
Cisco Packet Tracer
Cisco IOS
Computer Networking
VPN / IPsec
## Hierarchical Network Topology
📂 Project Structure
University-Enterprise-Network-Topology-VPN-Simulation/
│
├── README.md
├── University_Enterprise_Network_VPN.pkt
├── Computer-Networks-Banana-Problem.docx

## ▶️ How to Run
1. Install Cisco Packet Tracer

Install Cisco Packet Tracer on your computer.

2. Open the Project

Open:

University_Enterprise_Network_VPN.pkt

using Cisco Packet Tracer.

3. Inspect the Topology

Check the:

Routers
Switches
End devices
Network connections
IP addressing
VPN configuration
4. Open Router CLI

Select a router → CLI and use Cisco IOS commands to inspect the configuration.

💻 Useful Cisco IOS Commands
Interface Status
show ip interface brief
Running Configuration
show running-config
Routing Table
show ip route
Connectivity Test
ping <destination-ip>

Example:

ping 192.168.2.1
Trace Network Path
traceroute <destination-ip>
🧪 VPN Testing Procedure
Check interface status:
show ip interface brief
Check routing:
show ip route
Test the VPN peer:
ping <peer-ip>
Generate traffic between the networks:
ping <destination-ip>
Check IKE/ISAKMP:
show crypto isakmp sa
Check IPsec:
show crypto ipsec sa
Check the crypto map:
show crypto map
Inspect the complete crypto configuration:
show running-config | section crypto
🔍 Troubleshooting

If VPN connectivity is not working, verify:

show ip interface brief
show ip route
show crypto isakmp sa
show crypto ipsec sa
show crypto map
show running-config | section crypto

Also verify that the VPN peer is reachable and that the required interfaces are operational.

🎯 Project Objectives
Design a structured university enterprise network.
Connect multiple academic blocks through centralized campus infrastructure.
Provide network segmentation and organized connectivity.
Incorporate network security considerations.
Demonstrate VPN-based connectivity.
Simulate and verify the network using Cisco Packet Tracer.
📚 Documentation

The repository also contains the academic documentation:

PES2UG23CS652_THANVI G ACHAR_J UNIVERSITY_BANANA PRBLM.docx

The Cisco Packet Tracer .pkt file contains the actual implemented topology and device configuration.


👩‍💻 Author

Thanvi G Achar

GitHub:
https://github.com/thanvigachar

🔗 Repository

https://github.com/thanvigachar/University-Enterprise-Network-Topology-VPN-Simulation
