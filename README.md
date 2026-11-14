# Secure Multi-VLAN Office Network (Cisco Packet Tracer)

## Overview
Office network with three departments (HR, IT, Sales) separated using VLANs, with inter-VLAN routing, DHCP and an ACL.

## What I built
- 3 VLANs on a Cisco 2960 switch
- Router-on-a-stick inter-VLAN routing (Cisco 2911)
- DHCP pools for each VLAN
- ACL blocking Sales from accessing IT

## IP Plan
| Department | VLAN | Subnet | Gateway | Ports |
|---|---|---|---|---|
| HR | 10 | 192.168.10.0/24 | 192.168.10.1 | Fa0/1-2 |
| IT | 20 | 192.168.20.0/24 | 192.168.20.1 | Fa0/3-4 |
| Sales | 30 | 192.168.30.0/24 | 192.168.30.1 | Fa0/5-6 |

## Testing
- Sales to IT: blocked by ACL
- Sales to HR: allowed
- HR to IT: allowed

## Tools
Cisco Packet Tracer 9.0.1
