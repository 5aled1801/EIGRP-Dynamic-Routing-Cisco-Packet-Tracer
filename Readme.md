# EIGRP Dynamic Routing – Cisco Packet Tracer

## 📌 Project Overview

This project demonstrates the implementation of **EIGRP (Enhanced Interior Gateway Routing Protocol)** using Cisco Packet Tracer.

The topology consists of multiple interconnected Cisco routers configured in a multi-router network environment. The main objective is to enable dynamic routing between different networks and allow devices across remote LANs to communicate with each other.

## 🖥️ Network Topology

The network contains:

- **5 interconnected routers** forming the main routing topology.
- **2 Cisco 2960 switches** connecting end devices to the network.
- **2 PCs** representing end devices in separate LANs.
- Multiple point-to-point router connections.
- An additional router displayed separately in the workspace.

### Network Diagram

![EIGRP Network Topology](./screenShot/Screenshot%202026-11-07%20142107.png)

## 🌐 IP Addressing Scheme

The following IP addresses are labeled in the topology:

| Network Link | Router / Interface | IP Address |
|---|---|---|
| Router 1 – Router 2 | Router 1 | 11.1.1.1 |
| Router 1 – Router 2 | Router 2 | 11.1.1.2 |
| Router 1 – Router 3 | Router 1 | 10.1.1.2 |
| Router 1 – Router 3 | Router 3 | 10.1.1.1 |
| Router 2 – Router 4 | Router 2 | 12.1.1.1 |
| Router 2 – Router 4 | Router 4 | 12.1.1.2 |
| Router 4 – Router 5 | Router 4 | 13.1.1.1 |
| Router 4 – Router 5 | Router 5 | 13.1.1.2 |
| Router 5 – Router 3 | Router 5 | 14.1.1.1 |
| Router 5 – Router 3 | Router 3 | 14.1.1.2 |

### End Devices

- **PC2:** 192.168.1.1
- **PC3:** 192.168.1.2
- **Right-side LAN Gateway:** 192.168.1.1 (as labeled in the topology)

> Note: Verify the left-side LAN addressing before deployment. The router interface is labeled 220.1.1.1, while PC2 is labeled 192.168.1.1. These addresses do not belong to the same subnet.

## ⚙️ Routing Protocol

**EIGRP (Enhanced Interior Gateway Routing Protocol)**

EIGRP is a dynamic routing protocol that allows routers to automatically exchange routing information and calculate the best paths to destination networks.

Key concepts covered:

- EIGRP configuration and Autonomous System (AS) numbers.
- Neighbor adjacency formation.
- Dynamic route advertisement.
- Routing table verification.
- Connectivity between remote LANs.
- Automatic route updates when network changes occur.

## 🧪 Testing & Verification

The following Cisco IOS commands can be used to verify the EIGRP configuration and network connectivity:

**1. Verify EIGRP neighbors**
```bash
show ip eigrp neighbors
```

**2. Check EIGRP topology**
```bash
show ip eigrp topology
```

**3. Verify routing table**
```bash
show ip route
```

**4. Check EIGRP-learned routes**
```bash
show ip route eigrp
```

**5. Test end-to-end connectivity**
```bash
ping 192.168.1.2
tracert 192.168.1.2
```

## 🎯 Learning Objectives

- Understand dynamic routing concepts.
- Implement EIGRP across multiple routers.
- Understand how routers establish neighbor relationships.
- Exchange routing information dynamically.
- Troubleshoot routing and connectivity issues.
- Build and analyze multi-router network topologies.

## 🛠️ Tools & Technologies

- Cisco Packet Tracer
- Cisco IOS CLI
- EIGRP
- IPv4 Addressing
- Dynamic Routing
- LAN & WAN Networking

---

**Project Type:** Networking Lab / CCNA Practice  
**Protocol:** EIGRP  
**Simulation Tool:** Cisco Packet Tracer