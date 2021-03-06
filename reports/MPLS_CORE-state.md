
# Validate State Report

**Table of Contents:**

- [Validate State Report](validate-state-report)
  - [Test Results Summary](#test-results-summary)
  - [Failed Test Results Summary](#failed-test-results-summary)
  - [All Test Results](#all-test-results)

## Test Results Summary

### Summary Totals

| Total Tests | Total Tests Passed | Total Tests Failed |
| ----------- | ------------------ | ------------------ |
| 107 | 98 | 9 |

### Summary Totals Devices Under Tests

| DUT | Total Tests | Tests Passed | Tests Failed | Categories Failed |
| --- | ----------- | ------------ | ------------ | ----------------- |
| P1 |  14 | 13 | 1 | NTP |
| P2 |  11 | 10 | 1 | NTP |
| P3 |  14 | 13 | 1 | NTP |
| P4 |  11 | 10 | 1 | NTP |
| PE-1A |  12 | 11 | 1 | NTP |
| PE-1B |  12 | 11 | 1 | NTP |
| PE-2A |  12 | 11 | 1 | NTP |
| PE-2B |  12 | 11 | 1 | NTP |
| RR |  9 | 8 | 1 | NTP |

### Summary Totals Per Category

| Test Category | Total Tests | Tests Passed | Tests Failed |
| ------------- | ----------- | ------------ | ------------ |
| NTP |  9 | 0 | 9 |
| Interface State |  53 | 53 | 0 |
| LLDP Topology |  20 | 20 | 0 |
| IP Reachability |  20 | 20 | 0 |
| BGP |  5 | 5 | 0 |

## Failed Test Results Summary

| Test ID | Node | Test Category | Test Description | Test | Test Result | Failure Reason |
| ------- | ---- | ------------- | ---------------- | ---- | ----------- | -------------- |
| 1 | P1 | NTP | Synchronised with NTP server | NTP | FAIL | Not synchronised to NTP server |
| 2 | P2 | NTP | Synchronised with NTP server | NTP | FAIL | Not synchronised to NTP server |
| 3 | P3 | NTP | Synchronised with NTP server | NTP | FAIL | Not synchronised to NTP server |
| 4 | P4 | NTP | Synchronised with NTP server | NTP | FAIL | Not synchronised to NTP server |
| 5 | PE-1A | NTP | Synchronised with NTP server | NTP | FAIL | Not synchronised to NTP server |
| 6 | PE-1B | NTP | Synchronised with NTP server | NTP | FAIL | Not synchronised to NTP server |
| 7 | PE-2A | NTP | Synchronised with NTP server | NTP | FAIL | Not synchronised to NTP server |
| 8 | PE-2B | NTP | Synchronised with NTP server | NTP | FAIL | Not synchronised to NTP server |
| 9 | RR | NTP | Synchronised with NTP server | NTP | FAIL | Not synchronised to NTP server |

## All Test Results

| Test ID | Node | Test Category | Test Description | Test | Test Result | Failure Reason |
| ------- | ---- | ------------- | ---------------- | ---- | ----------- | -------------- |
| 1 | P1 | NTP | Synchronised with NTP server | NTP | FAIL | Not synchronised to NTP server |
| 2 | P2 | NTP | Synchronised with NTP server | NTP | FAIL | Not synchronised to NTP server |
| 3 | P3 | NTP | Synchronised with NTP server | NTP | FAIL | Not synchronised to NTP server |
| 4 | P4 | NTP | Synchronised with NTP server | NTP | FAIL | Not synchronised to NTP server |
| 5 | PE-1A | NTP | Synchronised with NTP server | NTP | FAIL | Not synchronised to NTP server |
| 6 | PE-1B | NTP | Synchronised with NTP server | NTP | FAIL | Not synchronised to NTP server |
| 7 | PE-2A | NTP | Synchronised with NTP server | NTP | FAIL | Not synchronised to NTP server |
| 8 | PE-2B | NTP | Synchronised with NTP server | NTP | FAIL | Not synchronised to NTP server |
| 9 | RR | NTP | Synchronised with NTP server | NTP | FAIL | Not synchronised to NTP server |
| 10 | P1 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet1 - P2P_LINK_TO_P2_Ethernet1 | PASS | - |
| 11 | P1 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet2 - P2P_LINK_TO_PE-1A_Ethernet2 | PASS | - |
| 12 | P1 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet3 - P2P_LINK_TO_P3_Ethernet3 | PASS | - |
| 13 | P1 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet4 - P2P_LINK_TO_RR_Ethernet4 | PASS | - |
| 14 | P2 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet1 - P2P_LINK_TO_P1_Ethernet1 | PASS | - |
| 15 | P2 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet2 - P2P_LINK_TO_PE-1B_Ethernet2 | PASS | - |
| 16 | P2 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet3 - P2P_LINK_TO_P4_Ethernet3 | PASS | - |
| 17 | P3 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet1 - P2P_LINK_TO_P4_Ethernet1 | PASS | - |
| 18 | P3 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet2 - P2P_LINK_TO_PE-2A_Ethernet2 | PASS | - |
| 19 | P3 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet3 - P2P_LINK_TO_P1_Ethernet3 | PASS | - |
| 20 | P3 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet5 - P2P_LINK_TO_RR_Ethernet5 | PASS | - |
| 21 | P4 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet1 - P2P_LINK_TO_P3_Ethernet1 | PASS | - |
| 22 | P4 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet2 - P2P_LINK_TO_PE-2B_Ethernet2 | PASS | - |
| 23 | P4 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet3 - P2P_LINK_TO_P2_Ethernet3 | PASS | - |
| 24 | PE-1A | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet2 - P2P_LINK_TO_P1_Ethernet2 | PASS | - |
| 25 | PE-1A | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet3 - A_CPE1_SITE1_PO2_Ethernet3 | PASS | - |
| 26 | PE-1A | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet4 - ROUTED_PORTS_CPE1 | PASS | - |
| 27 | PE-1A | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet1 -  | PASS | - |
| 28 | PE-1B | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet2 - P2P_LINK_TO_P2_Ethernet2 | PASS | - |
| 29 | PE-1B | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet3 - A_CPE1_SITE1_PO2_Ethernet4 | PASS | - |
| 30 | PE-1B | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet4 - ROUTED_PORTS_CPE1 | PASS | - |
| 31 | PE-1B | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet1 -  | PASS | - |
| 32 | PE-2A | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet2 - P2P_LINK_TO_P3_Ethernet2 | PASS | - |
| 33 | PE-2A | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet3 - A_CPE2_SITE2_PO2_Ethernet3 | PASS | - |
| 34 | PE-2A | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet4 - ROUTED_PORTS_CPE2 | PASS | - |
| 35 | PE-2A | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet1 -  | PASS | - |
| 36 | PE-2B | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet2 - P2P_LINK_TO_P4_Ethernet2 | PASS | - |
| 37 | PE-2B | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet3 - A_CPE2_SITE2_PO2_Ethernet4 | PASS | - |
| 38 | PE-2B | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet4 - ROUTED_PORTS_CPE2 | PASS | - |
| 39 | PE-2B | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet1 -  | PASS | - |
| 40 | RR | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet4 - P2P_LINK_TO_P1_Ethernet4 | PASS | - |
| 41 | RR | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet5 - P2P_LINK_TO_P3_Ethernet5 | PASS | - |
| 42 | PE-1A | Interface State | Port-Channel Interface & Line Protocol == "up" | Port-Channel3 - A_CPE1_SITE1_PO2_EVPN-A-A-PortChannel | PASS | - |
| 43 | PE-1A | Interface State | Port-Channel Interface & Line Protocol == "up" | Port-Channel1 -  | PASS | - |
| 44 | PE-1B | Interface State | Port-Channel Interface & Line Protocol == "up" | Port-Channel3 - A_CPE1_SITE1_PO2_EVPN-A-A-PortChannel | PASS | - |
| 45 | PE-1B | Interface State | Port-Channel Interface & Line Protocol == "up" | Port-Channel1 -  | PASS | - |
| 46 | PE-2A | Interface State | Port-Channel Interface & Line Protocol == "up" | Port-Channel3 - A_CPE2_SITE2_PO2_EVPN-A-A-PortChannel | PASS | - |
| 47 | PE-2A | Interface State | Port-Channel Interface & Line Protocol == "up" | Port-Channel1 -  | PASS | - |
| 48 | PE-2B | Interface State | Port-Channel Interface & Line Protocol == "up" | Port-Channel3 - A_CPE2_SITE2_PO2_EVPN-A-A-PortChannel | PASS | - |
| 49 | PE-2B | Interface State | Port-Channel Interface & Line Protocol == "up" | Port-Channel1 -  | PASS | - |
| 50 | PE-1A | Interface State | Vlan Interface & Line Protocol == "up" | Vlan1001 - TENANT_A_SITE1_IRB | PASS | - |
| 51 | PE-1B | Interface State | Vlan Interface & Line Protocol == "up" | Vlan1001 - TENANT_A_SITE1_IRB | PASS | - |
| 52 | PE-2A | Interface State | Vlan Interface & Line Protocol == "up" | Vlan1002 - TENANT_A_SITE2_IRB | PASS | - |
| 53 | PE-2B | Interface State | Vlan Interface & Line Protocol == "up" | Vlan1002 - TENANT_A_SITE2_IRB | PASS | - |
| 54 | P1 | Interface State | Loopback Interface Status & Line Protocol == "up" | Loopback0 - LSR_Router_ID | PASS | - |
| 55 | P2 | Interface State | Loopback Interface Status & Line Protocol == "up" | Loopback0 - LSR_Router_ID | PASS | - |
| 56 | P3 | Interface State | Loopback Interface Status & Line Protocol == "up" | Loopback0 - LSR_Router_ID | PASS | - |
| 57 | P4 | Interface State | Loopback Interface Status & Line Protocol == "up" | Loopback0 - LSR_Router_ID | PASS | - |
| 58 | PE-1A | Interface State | Loopback Interface Status & Line Protocol == "up" | Loopback0 - MPLS_Overlay_peering | PASS | - |
| 59 | PE-1B | Interface State | Loopback Interface Status & Line Protocol == "up" | Loopback0 - MPLS_Overlay_peering | PASS | - |
| 60 | PE-2A | Interface State | Loopback Interface Status & Line Protocol == "up" | Loopback0 - MPLS_Overlay_peering | PASS | - |
| 61 | PE-2B | Interface State | Loopback Interface Status & Line Protocol == "up" | Loopback0 - MPLS_Overlay_peering | PASS | - |
| 62 | RR | Interface State | Loopback Interface Status & Line Protocol == "up" | Loopback0 - MPLS_Overlay_peering | PASS | - |
| 63 | P1 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet1 - remote: P2_Ethernet1 | PASS | - |
| 64 | P1 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet2 - remote: PE-1A_Ethernet2 | PASS | - |
| 65 | P1 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet3 - remote: P3_Ethernet3 | PASS | - |
| 66 | P1 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet4 - remote: RR_Ethernet4 | PASS | - |
| 67 | P2 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet1 - remote: P1_Ethernet1 | PASS | - |
| 68 | P2 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet2 - remote: PE-1B_Ethernet2 | PASS | - |
| 69 | P2 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet3 - remote: P4_Ethernet3 | PASS | - |
| 70 | P3 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet1 - remote: P4_Ethernet1 | PASS | - |
| 71 | P3 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet2 - remote: PE-2A_Ethernet2 | PASS | - |
| 72 | P3 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet3 - remote: P1_Ethernet3 | PASS | - |
| 73 | P3 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet5 - remote: RR_Ethernet5 | PASS | - |
| 74 | P4 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet1 - remote: P3_Ethernet1 | PASS | - |
| 75 | P4 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet2 - remote: PE-2B_Ethernet2 | PASS | - |
| 76 | P4 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet3 - remote: P2_Ethernet3 | PASS | - |
| 77 | PE-1A | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet2 - remote: P1_Ethernet2 | PASS | - |
| 78 | PE-1B | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet2 - remote: P2_Ethernet2 | PASS | - |
| 79 | PE-2A | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet2 - remote: P3_Ethernet2 | PASS | - |
| 80 | PE-2B | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet2 - remote: P4_Ethernet2 | PASS | - |
| 81 | RR | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet4 - remote: P1_Ethernet4 | PASS | - |
| 82 | RR | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet5 - remote: P3_Ethernet5 | PASS | - |
| 83 | P1 | IP Reachability | ip reachability test p2p links | Source: P1_Ethernet1 - Destination: P2_Ethernet1 | PASS | - |
| 84 | P1 | IP Reachability | ip reachability test p2p links | Source: P1_Ethernet2 - Destination: PE-1A_Ethernet2 | PASS | - |
| 85 | P1 | IP Reachability | ip reachability test p2p links | Source: P1_Ethernet3 - Destination: P3_Ethernet3 | PASS | - |
| 86 | P1 | IP Reachability | ip reachability test p2p links | Source: P1_Ethernet4 - Destination: RR_Ethernet4 | PASS | - |
| 87 | P2 | IP Reachability | ip reachability test p2p links | Source: P2_Ethernet1 - Destination: P1_Ethernet1 | PASS | - |
| 88 | P2 | IP Reachability | ip reachability test p2p links | Source: P2_Ethernet2 - Destination: PE-1B_Ethernet2 | PASS | - |
| 89 | P2 | IP Reachability | ip reachability test p2p links | Source: P2_Ethernet3 - Destination: P4_Ethernet3 | PASS | - |
| 90 | P3 | IP Reachability | ip reachability test p2p links | Source: P3_Ethernet1 - Destination: P4_Ethernet1 | PASS | - |
| 91 | P3 | IP Reachability | ip reachability test p2p links | Source: P3_Ethernet2 - Destination: PE-2A_Ethernet2 | PASS | - |
| 92 | P3 | IP Reachability | ip reachability test p2p links | Source: P3_Ethernet3 - Destination: P1_Ethernet3 | PASS | - |
| 93 | P3 | IP Reachability | ip reachability test p2p links | Source: P3_Ethernet5 - Destination: RR_Ethernet5 | PASS | - |
| 94 | P4 | IP Reachability | ip reachability test p2p links | Source: P4_Ethernet1 - Destination: P3_Ethernet1 | PASS | - |
| 95 | P4 | IP Reachability | ip reachability test p2p links | Source: P4_Ethernet2 - Destination: PE-2B_Ethernet2 | PASS | - |
| 96 | P4 | IP Reachability | ip reachability test p2p links | Source: P4_Ethernet3 - Destination: P2_Ethernet3 | PASS | - |
| 97 | PE-1A | IP Reachability | ip reachability test p2p links | Source: PE-1A_Ethernet2 - Destination: P1_Ethernet2 | PASS | - |
| 98 | PE-1B | IP Reachability | ip reachability test p2p links | Source: PE-1B_Ethernet2 - Destination: P2_Ethernet2 | PASS | - |
| 99 | PE-2A | IP Reachability | ip reachability test p2p links | Source: PE-2A_Ethernet2 - Destination: P3_Ethernet2 | PASS | - |
| 100 | PE-2B | IP Reachability | ip reachability test p2p links | Source: PE-2B_Ethernet2 - Destination: P4_Ethernet2 | PASS | - |
| 101 | RR | IP Reachability | ip reachability test p2p links | Source: RR_Ethernet4 - Destination: P1_Ethernet4 | PASS | - |
| 102 | RR | IP Reachability | ip reachability test p2p links | Source: RR_Ethernet5 - Destination: P3_Ethernet5 | PASS | - |
| 103 | PE-1A | BGP | ArBGP is configured and operating | ArBGP | PASS | - |
| 104 | PE-1B | BGP | ArBGP is configured and operating | ArBGP | PASS | - |
| 105 | PE-2A | BGP | ArBGP is configured and operating | ArBGP | PASS | - |
| 106 | PE-2B | BGP | ArBGP is configured and operating | ArBGP | PASS | - |
| 107 | RR | BGP | ArBGP is configured and operating | ArBGP | PASS | - |
