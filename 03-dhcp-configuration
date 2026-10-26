# Project 03: DHCP Configuration in Cisco Packet Tracer

## Overview

This project demonstrates how to configure a Dynamic Host Configuration Protocol (DHCP) server to automatically assign IP configuration settings to client computers on a local area network (LAN).

## Objectives

- Configure a router as the default gateway.
- Assign a static IP address to the DHCP server.
- Configure a DHCP address pool.
- Enable automatic IP configuration on client PCs.
- Verify network connectivity between devices.

## Network Topology

The network consists of:
- 1 Cisco 2911 router (R1)
- 1 Cisco 2960 switch (SW1)
- 1 Server-PT device
- 3 client PCs

All devices are connected to the same LAN through the switch.

## IP Addressing Plan

| Device | IP Address | Configuration |
|---|---|---|
| Router R1 | 192.168.10.1 | Static |
| DHCP Server | 192.168.10.2 | Static |
| PC1 | DHCP-assigned | Automatic |
| PC2 | DHCP-assigned | Automatic |
| PC3 | DHCP-assigned | Automatic |

**Subnet mask:** 255.255.255.0

## DHCP Pool Configuration

| Setting | Value |
|---|---|
| Pool Name | LAN_POOL |
| Default Gateway | 192.168.10.1 |
| DNS Server | 192.168.10.2 |
| Starting IP Address | 192.168.10.100 |
| Subnet Mask | 255.255.255.0 |
| Maximum Users | 50 |

## Implementation

1. Connected the router, switch, server, and three PCs.
2. Configured the router's GigabitEthernet interface with IP address `192.168.10.1/24`.
3. Assigned the DHCP server a static IP address of `192.168.10.2/24`.
4. Enabled the DHCP service on the server.
5. Created and configured the `LAN_POOL` address pool.
6. Set all three client PCs to obtain their IP configuration automatically.

## Verification and Testing

- Confirmed that all three PCs received IP addresses automatically.
- Used `ipconfig /all` to inspect client network configuration.
- Used `ping` to test connectivity between client PCs, the router gateway, and the DHCP server.

## Key Learnings

- Understood how DHCP automates IP address assignment.
- Practised configuring a DHCP pool and default gateway.
- Learned the difference between static and dynamically assigned IP addresses.
- Verified basic LAN connectivity using command-line tools.

## Tools Used

- Cisco Packet Tracer
- Cisco IOS CLI
- DHCP
- IPv4 addressing
- Command Prompt

## Screenshots

Screenshots documenting the topology, router configuration, server settings, DHCP pool, client IP configuration, and connectivity tests are available in the `screenshots` folder.
