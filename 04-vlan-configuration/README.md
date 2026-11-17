# Project 04: VLAN Configuration in Cisco Packet Tracer

## Overview

This project demonstrates how to configure Virtual Local Area Networks (VLANs) on a Cisco switch to logically separate devices into different network segments.

Two departments were created: IT (VLAN 10) and HR (VLAN 20).

## Objectives

- Understand the purpose of VLANs.
- Create and configure VLANs on a Cisco switch.
- Assign switch ports to specific VLANs.
- Test communication within the same VLAN.
- Verify isolation between different VLANs.
- Troubleshoot incorrect VLAN port assignments.

## Network Topology

The network consists of:
- 1 Cisco 2960 switch
- 4 PCs

### VLAN Design

| VLAN ID | VLAN Name | Assigned Devices |
|---|---|---|
| 10 | IT | PC1, PC2 |
| 20 | HR | PC3, PC4 |

## IP Addressing Plan

| Device | IP Address | Subnet Mask |
|---|---|---|
| PC1 | 192.168.10.10 | 255.255.255.0 |
| PC2 | 192.168.10.11 | 255.255.255.0 |
| PC3 | 192.168.10.12 | 255.255.255.0 |
| PC4 | 192.168.10.13 | 255.255.255.0 |

## Implementation

1. Built the network topology using a Cisco 2960 switch and four PCs.
2. Configured static IPv4 addresses on all four PCs.
3. Created VLAN 10 and named it IT.
4. Created VLAN 20 and named it HR.
5. Assigned switch ports Fa0/1 and Fa0/2 to VLAN 10.
6. Assigned switch ports Fa0/3 and Fa0/4 to VLAN 20.
7. Verified VLAN membership using `show vlan brief`.

## Connectivity Testing

The following tests were performed:

| Test | Expected Result | Actual Result |
|---|---|---|
| PC1 to PC2 (same VLAN) | Successful | Successful |
| PC1 to PC3 (different VLANs) | Failed | Failed |
| PC1 to PC4 (different VLANs) | Failed | Failed |

Communication within VLAN 10 was successful, while communication between VLAN 10 and VLAN 20 was unsuccessful because inter-VLAN routing was not configured.

## Troubleshooting

A troubleshooting scenario was performed by accidentally assigning PC2's switch port (Fa0/2) to VLAN 20 instead of VLAN 10.

This caused communication between PC1 and PC2 to fail.

The port was restored to VLAN 10, after which connectivity between PC1 and PC2 was successful again.

## Key Learnings

- Understanding VLANs and network segmentation.
- Creating and naming VLANs on a Cisco switch.
- Assigning access ports to specific VLANs.
- Understanding Layer 2 separation between VLANs.
- Testing network connectivity using ping.
- Identifying and correcting incorrect VLAN assignments.

## Tools Used

- Cisco Packet Tracer
- Cisco Catalyst 2960 switch
- Cisco IOS CLI
- IPv4 addressing
- VLAN configuration

## Screenshots

Screenshots documenting the network topology, VLAN creation, port assignments, connectivity tests, final configuration, and troubleshooting process are available in the `screenshots` folder.
:::
