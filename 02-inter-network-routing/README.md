# Project 02: Inter-Network Routing

## Overview
Built two separate IPv4 networks in Cisco Packet Tracer and connected them using a Cisco router. Configured router interfaces, assigned IP addresses and default gateways, and tested communication between devices on different networks.

## Objectives
- Understand communication between different IP networks.
- Configure Cisco router interfaces.
- Configure default gateways on client PCs.
- Verify interface status using Cisco IOS commands.
- Test connectivity and troubleshoot gateway configuration.

## Network Topology
- 1 Cisco 2911 router
- 2 Cisco 2960 switches
- 4 PCs
- Copper straight-through Ethernet cables

## IP Addressing Plan

| Device | IPv4 Address | Subnet Mask | Default Gateway |
|---|---|---|---|
| Router G0/0 | 192.168.10.1 | 255.255.255.0 | N/A |
| PC1 | 192.168.10.10 | 255.255.255.0 | 192.168.10.1 |
| PC2 | 192.168.10.11 | 255.255.255.0 | 192.168.10.1 |
| Router G0/1 | 192.168.20.1 | 255.255.255.0 | N/A |
| PC3 | 192.168.20.10 | 255.255.255.0 | 192.168.20.1 |
| PC4 | 192.168.20.11 | 255.255.255.0 | 192.168.20.1 |

## Implementation
1. Created two LANs using separate switches.
2. Configured IPv4 addresses on both router interfaces.
3. Enabled the router interfaces using `no shutdown`.
4. Configured each PC's IP address, subnet mask and default gateway.
5. Verified router interface status using `show ip interface brief`.
6. Tested connectivity using `ping`.

## Testing and Troubleshooting
- Successfully pinged the local gateway from PC1.
- Successfully pinged PC3 from PC1 across the router.
- Tested the effect of configuring an incorrect default gateway on PC3.
- Restored PC3's correct gateway address, `192.168.20.1`.

## Key Learnings
- Routers forward traffic between different IP networks.
- A default gateway allows a device to send traffic to destinations outside its local subnet.
- Router interfaces must be correctly configured and operational.
- Incorrect IP addresses, subnet masks or gateways can cause connectivity problems.
- `show ip interface brief` helps verify router interface status.

## Tools and Technologies
- Cisco Packet Tracer
- Cisco IOS CLI
- IPv4 addressing
- Ethernet switching and routing
- ICMP and ping testing
- Network troubleshooting

## Screenshots
See the `screenshots/` folder for visual evidence of the topology, router configuration and connectivity testing.
