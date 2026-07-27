[README.md](https://github.com/user-attachments/files/30428756/README.md)
## Small Office Network – Static & Dynamic Topology (Packet Tracer)

## Project Overview

This lab implements a small office network divided into two segments:

- Static Network (192.168.10.0/24)

- Dynamic Network with DHCP (192.168.20.0/24)

## Topology Summary

The topology consists of two independent networks connected through routers.

## Static Network

- Cisco 1941 Router (R1)

- Cisco 2960 Switch

- 4 PCs (PC07PC3)

- 1 Server

- All devices configured with static IP addresses

- Dual-stack IPv4 & IPv6

## Dynamic Network

- Cisco 1941 Router (R2)

- Cisco 2960 Switch

- 2 PCs (PC47PC5)

- Access Point

- Laptop connected via WiFi

- DHCP enabled on the router

## Interconnection

- A direct link between R1 and R2 allows communication between both subnets.


## IP Addressing

## Static Network

Subnet: 192.168.10.0/24

- Default Gateway: 192.168.10.1

- Manual IP configuration on all hosts

## Dynamic Network

Subnet: 192.168.20.0/24

- DHCP Gateway: 192.168.20.1

- Router assigns IPs to PCs and laptop

## IP Addressing Table

| Device | IP Address |   | Subnet Mask Default Gateway |
| --- | --- | --- | --- |
|   | R1 G0/0 192.168.10.1 2001:db8:10::1/64 | 255.255.255.0 N/A |   |
|   | R1 G0/1 10.10.10.1 | 255.255.255.252 N/A |   |
|   | R2 G0/0 192.168.20.1 | 255.255.255.0 N/A |   |
|   | R2 G0/1 10.10.10.2 | 255.255.255.252 N/A |   |
| PC0 | 192.168.10.10 2001:DB8:10::10/64 | 255.255.255.0 | 192.168.10.1 |
| PC1 | 192.168.10.11 2001:DB8:10::11/64 | 255.255.255.0 | 192.168.10.1 |
| PC2 | 192.168.10.12 2001:DB8:10::12/64 | 255.255.255.0 | 192.168.10.1 |
| PC3 | 192.168.10.13 2001:DB8:10::13/64 | 255.255.255.0 | 192.168.10.1 |
| PC4 | DHCP | 255.255.255.0 | 192.168.20.1 |
| PC5 | DHCP | 255.255.255.0 | 192.168.20.1 |
| Laptop DHCP |   | 255.255.255.0 | 192.168.20.1 |


| Server | 192.168.10.100 2001:DB8:10::100/64 | 255.255.255.0 | 192.168.10.1 |
| --- | --- | --- | --- |

## Configuration Details

## Router R1 (Static Network)

- Gig0/0 and Gig0/1 configured

- Default gateway for hosts

- Static route to reach 192.168.20.0/24

- SSH enabled

- Local admin user configured

- RSA keys generated

## Router R2 (Dynamic Network)

- Gig0/0 and Gig0/1 configured

- Default gateway for hosts

- DHCP pool for 192.168.20.0/24

- Static route to reach 192.168.10.0/24

- SSH enabled

- Local admin user configured

- RSA keys generated

## Switches

- Default VLAN

- Connections to routers and end devices

## Access Point

- SSID configured

- WPA2 security

- Laptop successfully connected

## Server

- DNS configured

- HTTP configured

## Cabling

- Straight-through cables to connect hosts to the switch

- Crossover cable to connect both routers

## Testing & Verification

- Ping tests within each subnet

- Ping tests across subnets (inter-network routing)

- Tracert verification test

- DHCP assignment verification

- Wireless connectivity test

- Server access from both networks

## Included Files

- SmallOfficeNetwork.pkt  Packet Tracer project file

- README.md  Documentation

- PDF  Documentation

## Screenshots
