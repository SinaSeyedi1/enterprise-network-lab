# Enterprise Network Lab (Cisco Packet Tracer)

## Overview

Designed and implemented a segmented enterprise LAN using VLANs, inter-VLAN routing, DHCP, and DNS.

The network separates IT, HR, and Guest traffic while allowing controlled communication between VLANs.

---

## Technologies

* Cisco Packet Tracer
* VLANs (802.1Q)
* Inter-VLAN Routing (Router-on-a-Stick)
* DHCP (multi-scope + relay)
* DNS

---

## 1. Network Topology

This diagram shows the overall network design, including router, switches, server, and end devices.

![Topology](screenshots/01-network-topology.png)

---

## 2. Subnetting Plan

Defined subnet ranges for each VLAN based on department size.

![Subnet](screenshots/02-subnetting-ip-plan.png)

---

## 3. VLAN Configuration

Created VLANs for each department:

* VLAN 10 – IT
* VLAN 20 – HR
* VLAN 30 – Guest

![VLAN Creation](screenshots/03-vlan-creation.png)
![VLAN Verification](screenshots/04-vlan-verification.png)

---

## 4. Trunk Configuration

Configured trunk links between switches to allow VLAN traffic across the network.

![Trunk](screenshots/05-trunk-link.png)

---

## 5. Inter-VLAN Routing

Implemented router-on-a-stick using subinterfaces to enable communication between VLANs.

![Router](screenshots/06-router-on-a-stick.png)

---

## 6. Connectivity Test

Verified communication between devices in different VLANs.

![Ping Test](screenshots/07-inter-vlan-ping-test.png)

---

## 7. DNS Configuration

Configured a DNS server to resolve hostnames to IP addresses.

![DNS](screenshots/08-dns-resolution-test.png)

---

## 8. DHCP Configuration

Configured DHCP server with multiple scopes for each VLAN and implemented DHCP relay on the router.

![DHCP Server](screenshots/09-dhcp-server.png)
![DHCP Assignment](screenshots/10-dhcp-ip-assignment.png)
![DHCP Test](screenshots/11-dhcp-connectivity-test.png)

---

## 9. Troubleshooting

* Resolved DHCP issue caused by conflicting default server pool
* Configured `ip helper-address` for DHCP relay
* Verified VLAN trunking and correct port assignments
* Ensured DNS resolution across VLANs

---

## Conclusion

This project demonstrates the design, implementation, and troubleshooting of a small enterprise network using VLAN segmentation, routing, and network services.

---

