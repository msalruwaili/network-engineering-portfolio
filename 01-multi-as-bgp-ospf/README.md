# Multi-AS BGP & OSPF Enterprise Network

**Tool:** GNS3
**Category:** Routing (BGP, OSPF, Routing Policy)

## 🎯 Objective

Design and build a simulated enterprise network with an internal OSPF domain, interconnected with multiple external Autonomous Systems (AS) via BGP, while ensuring the internal network does not act as an unintended transit path between external providers.

## 🖧 Topology Overview

- Internal network running **OSPF** as the IGP (Interior Gateway Protocol)
- **eBGP** peering established with **4 external Autonomous Systems (AS)**, interconnecting a total of **5 AS domains** (including the internal network)
- **Route redistribution** configured between BGP and OSPF for full end-to-end reachability between internal and external networks

## ⚙️ Key Configuration Highlights

- OSPF adjacency and route propagation across internal routers
- eBGP peering and AS-path handling across 4 external AS domains
- Two-way route redistribution (BGP ↔ OSPF)
- **Route-map and prefix-list filtering** to prevent external AS domains from using the internal network as a transit path — a core BGP routing-policy and security best practice

## 🧠 What This Project Demonstrates

- Practical understanding of multi-AS BGP peering and route exchange
- Ability to integrate BGP with an internal IGP (OSPF) through redistribution
- Awareness of BGP transit-policy risks and how to mitigate them using route filtering

## 📌 Notes

This is a self-directed lab project built to apply CCNP Enterprise (Core & ENARSI) concepts in a realistic multi-AS topology. It was not part of a production environment.

---
*Screenshots and configuration files to be added.*
