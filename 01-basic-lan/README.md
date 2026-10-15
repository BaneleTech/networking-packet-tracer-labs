# Project 01: Basic LAN Configuration

## Overview
Built a basic Local Area Network (LAN) in Cisco Packet Tracer using four PCs connected through a Cisco 2960 switch. Configured static IPv4 addresses and tested connectivity between devices.

## Objectives
- Understand basic LAN connectivity.
- Configure IPv4 addresses and subnet masks.
- Observe how a switch learns MAC addresses.
- Test connectivity using ping.
- Practise basic network troubleshooting.

## Network Topology
- 1 Cisco 2960 switch
- 4 PCs
- Copper straight-through Ethernet cables

## IP Addressing Plan

| Device | IPv4 Address | Subnet Mask |
|---|---|---|
| PC1 | 192.168.10.10 | 255.255.255.0 |
| PC2 | 192.168.10.11 | 255.255.255.0 |
| PC3 | 192.168.10.12 | 255.255.255.0 |
| PC4 | 192.168.10.13 | 255.255.255.0 |

Network: `192.168.10.0/24`

No default gateway was required for communication within this LAN.

## Implementation
1. Added four PCs and a Cisco 2960 switch.
2. Connected the devices using Ethernet cables.
3. Manually configured IPv4 addresses and subnet masks.
4. Tested connectivity between PCs using `ping`.
5. Inspected the switch MAC address table using `show mac address-table`.

## Testing and Troubleshooting
- Verified connectivity between PCs on the same subnet.
- Changed PC3's address to `192.168.20.12/24` to simulate an addressing problem.
- Observed a ping timeout when PC1 attempted to reach PC3 at the new address without a router.
- Investigated the relationship between IP addressing, subnet masks and routing.

## Key Learnings
- Switches learn MAC addresses and use their MAC address tables to forward Ethernet frames.
- A `/24` subnet uses the mask `255.255.255.0`.
- Devices on different IP networks generally require a router or another Layer 3 device to communicate.
- A ping timeout means a reply was not received; additional troubleshooting is needed to identify the cause.

## Tools and Technologies
- Cisco Packet Tracer
- IPv4 addressing
- Ethernet switching
- ICMP
- Network troubleshooting

## Project Files
- `screenshots/` — Evidence of the lab configuration and testing.
