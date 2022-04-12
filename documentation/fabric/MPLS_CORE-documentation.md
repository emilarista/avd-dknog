# MPLS_CORE

# Table of Contents

- [Fabric Switches and Management IP](#fabric-switches-and-management-ip)
  - [Fabric Switches with inband Management IP](#fabric-switches-with-inband-management-ip)
- [Fabric Topology](#fabric-topology)
- [Fabric IP Allocation](#fabric-ip-allocation)
  - [Fabric Point-To-Point Links](#fabric-point-to-point-links)
  - [Point-To-Point Links Node Allocation](#point-to-point-links-node-allocation)
  - [Loopback Interfaces (BGP EVPN Peering)](#loopback-interfaces-bgp-evpn-peering)
  - [Loopback0 Interfaces Node Allocation](#loopback0-interfaces-node-allocation)
  - [ISIS CLNS interfaces](#isis-clns-interfaces)
  - [VTEP Loopback VXLAN Tunnel Source Interfaces (VTEPs Only)](#vtep-loopback-vxlan-tunnel-source-interfaces-vteps-only)
  - [VTEP Loopback Node allocation](#vtep-loopback-node-allocation)

# Fabric Switches and Management IP

| POD | Type | Node | Management IP | Platform | Provisioned in CloudVision |
| --- | ---- | ---- | ------------- | -------- | -------------------------- |
| MPLS_CORE | p | P1 | 10.30.30.103/24 | vEOS-LAB | Provisioned |
| MPLS_CORE | p | P2 | 10.30.30.104/24 | vEOS-LAB | Provisioned |
| MPLS_CORE | p | P3 | 10.30.30.106/24 | vEOS-LAB | Provisioned |
| MPLS_CORE | p | P4 | 10.30.30.107/24 | vEOS-LAB | Provisioned |
| MPLS_CORE | pe | PE-1A | 10.30.30.101/24 | vEOS-LAB | Provisioned |
| MPLS_CORE | pe | PE-1B | 10.30.30.102/24 | vEOS-LAB | Provisioned |
| MPLS_CORE | pe | PE-2A | 10.30.30.108/24 | vEOS-LAB | Provisioned |
| MPLS_CORE | pe | PE-2B | 10.30.30.109/24 | vEOS-LAB | Provisioned |
| MPLS_CORE | rr | RR | 10.30.30.105/24 | vEOS-LAB | Provisioned |

> Provision status is based on Ansible inventory declaration and do not represent real status from CloudVision.

## Fabric Switches with inband Management IP
| POD | Type | Node | Management IP | Inband Interface |
| --- | ---- | ---- | ------------- | ---------------- |

# Fabric Topology

| Type | Node | Node Interface | Peer Type | Peer Node | Peer Interface |
| ---- | ---- | -------------- | --------- | ----------| -------------- |
| p | P1 | Ethernet1 | p | P2 | Ethernet1 |
| p | P1 | Ethernet2 | pe | PE-1A | Ethernet2 |
| p | P1 | Ethernet3 | p | P3 | Ethernet3 |
| p | P1 | Ethernet4 | rr | RR | Ethernet4 |
| p | P2 | Ethernet2 | pe | PE-1B | Ethernet2 |
| p | P2 | Ethernet3 | p | P4 | Ethernet3 |
| p | P3 | Ethernet1 | p | P4 | Ethernet1 |
| p | P3 | Ethernet2 | pe | PE-2A | Ethernet2 |
| p | P3 | Ethernet5 | rr | RR | Ethernet5 |
| p | P4 | Ethernet2 | pe | PE-2B | Ethernet2 |

# Fabric IP Allocation

## Fabric Point-To-Point Links

| Uplink IPv4 Pool | Available Addresses | Assigned addresses | Assigned Address % |
| ---------------- | ------------------- | ------------------ | ------------------ |

## Point-To-Point Links Node Allocation

| Node | Node Interface | Node IP Address | Peer Node | Peer Interface | Peer IP Address |
| ---- | -------------- | --------------- | --------- | -------------- | --------------- |
| P1 | Ethernet1 | 100.64.48.0/31 | P2 | Ethernet1 | 100.64.48.1/31 |
| P1 | Ethernet2 | 100.64.48.2/31 | PE-1A | Ethernet2 | 100.64.48.3/31 |
| P1 | Ethernet3 | 100.64.48.4/31 | P3 | Ethernet3 | 100.64.48.5/31 |
| P1 | Ethernet4 | 100.64.48.16/31 | RR | Ethernet4 | 100.64.48.17/31 |
| P2 | Ethernet2 | 100.64.48.7/31 | PE-1B | Ethernet2 | 100.64.48.6/31 |
| P2 | Ethernet3 | 100.64.48.8/31 | P4 | Ethernet3 | 100.64.48.9/31 |
| P3 | Ethernet1 | 100.64.48.10/31 | P4 | Ethernet1 | 100.64.48.11/31 |
| P3 | Ethernet2 | 100.64.48.12/31 | PE-2A | Ethernet2 | 100.64.48.13/31 |
| P3 | Ethernet5 | 100.64.48.18/31 | RR | Ethernet5 | 100.64.48.19/31 |
| P4 | Ethernet2 | 100.64.48.14/31 | PE-2B | Ethernet2 | 100.64.48.15/31 |

## Loopback Interfaces (BGP EVPN Peering)

| Loopback Pool | Available Addresses | Assigned addresses | Assigned Address % |
| ------------- | ------------------- | ------------------ | ------------------ |
| 100.70.0.0/24 | 256 | 9 | 3.52 % |

## Loopback0 Interfaces Node Allocation

| POD | Node | Loopback0 |
| --- | ---- | --------- |
| MPLS_CORE | P1 | 100.70.0.31/32 |
| MPLS_CORE | P2 | 100.70.0.32/32 |
| MPLS_CORE | P3 | 100.70.0.33/32 |
| MPLS_CORE | P4 | 100.70.0.34/32 |
| MPLS_CORE | PE-1A | 100.70.0.11/32 |
| MPLS_CORE | PE-1B | 100.70.0.12/32 |
| MPLS_CORE | PE-2A | 100.70.0.13/32 |
| MPLS_CORE | PE-2B | 100.70.0.14/32 |
| MPLS_CORE | RR | 100.70.0.21/32 |

## ISIS CLNS interfaces

| POD | Node | CLNS Address |
| --- | ---- | ------------ |
| MPLS_CORE | P1 | 49.0001.0000.0003.0001.00 |
| MPLS_CORE | P2 | 49.0001.0000.0003.0002.00 |
| MPLS_CORE | P3 | 49.0001.0000.0003.0003.00 |
| MPLS_CORE | P4 | 49.0001.0000.0003.0004.00 |
| MPLS_CORE | PE-1A | 49.0001.0000.0001.0001.00 |
| MPLS_CORE | PE-1B | 49.0001.0000.0001.0002.00 |
| MPLS_CORE | PE-2A | 49.0001.0000.0001.0003.00 |
| MPLS_CORE | PE-2B | 49.0001.0000.0001.0004.00 |
| MPLS_CORE | RR | 49.0001.0000.0002.0001.00 |

## VTEP Loopback VXLAN Tunnel Source Interfaces (VTEPs Only)

| VTEP Loopback Pool | Available Addresses | Assigned addresses | Assigned Address % |
| --------------------- | ------------------- | ------------------ | ------------------ |

## VTEP Loopback Node allocation

| POD | Node | Loopback1 |
| --- | ---- | --------- |
