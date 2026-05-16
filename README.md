# Multi-Branch Enterprise Network (DHCP, DNS, RIP, VLAN, WLAN)

A comprehensive enterprise network simulation built in Cisco Packet Tracer,
connecting two geographically separate branches through a central server
infrastructure using RIP routing protocol.

## Overview

This project simulates a two-branch company network with five departments
per branch, centralized DHCP/HTTP and DNS servers, and mixed IP assignment
methods including static, dynamic, and wireless.

## Technologies Used

- **Routing:** RIP Protocol
- **Switching:** VLAN, Inter-VLAN Routing
- **Wireless:** WLAN (Access Points)
- **Services:** DHCP, HTTP, DNS
- **Addressing:** Static IP, Dynamic IP (DHCP), Subnetting (/27)

## Network Topology

| Color | Department Type | IP Method |
|-------|----------------|-----------|
| Yellow | Finance, HR, Security, IT, SD | DHCP Server |
| Sky Blue | Marketing | DHCP via WLAN |
| Purple/Pink | IT (VLAN groups) | Static IP via VLAN |

## Sites

| Site | Subnet Range |
|------|-------------|
| Branch 1 (B1) | 192.168.2.0/27 subnets |
| Branch 2 (B2) | 192.168.3.0/24 |
| Server Network | 192.168.1.0/24 |
| WAN B1-Server | 10.0.0.0/8 |
| WAN B2-Server | 20.0.0.0/8 |

## Server Infrastructure

| Server | IP | Services |
|--------|-----|---------|
| DHCP + HTTP Server | 192.168.1.2 | DHCP pools, HTTP |
| DNS Server | 192.168.1.x | DNS resolution |

## Files

| File | Description |
|------|-------------|
| `DHCP - Final.pkt` | Main Packet Tracer simulation file |

## How to Open

1. Download and install [Cisco Packet Tracer](https://www.netacad.com/courses/packet-tracer)
2. Open the `.pkt` file
3. Test DHCP by setting any yellow PC to DHCP mode
4. Test DNS via Web Browser on any PC

## Status

>  Project is functional but under review.
> DNS and inter-branch ping issues are being investigated.
