# cisco-network-project
This project demonstrates a small enterprise network designed in Cisco Packet Tracer. Multiple departments are connected through a central router, enabling communication across separate subnets and a centralized server. The setup simulates a real-world business network with efficient inter-network connectivity and resource sharing.

# Small Enterprise Network Simulation — Cisco Packet Tracer

## Overview
A simulated enterprise network built in Cisco Packet Tracer featuring
inter-department routing, a DNS-configured HTTPS web server, and
segmented subnets per department.


## IP Addressing Table
| Device    | Interface | IP Address      | Subnet         | Role         |
|-----------|-----------|-----------------|----------------|--------------|
| Router1   | Fa0/0     | 192.168.1.1     | 192.168.1.0/24 | VLAN1 Gateway|
| Router1   | Fa0/1     | 192.168.2.1     | 192.168.2.0/24 | VLAN2 Gateway|
| Router1   | Fa0/2     | 192.168.3.1     | 192.168.3.0/24 | VLAN3 Gateway|
| Router1   | Fa0/3     | 192.168.4.1     | 192.168.4.0/24 | VLAN4 Gateway|
| Server-PT | NIC       | 192.168.1.100   | 192.168.1.0/24 | Web + DNS    |
| PC (Dept2)| NIC       | 192.168.2.2/.3  | 192.168.2.0/24 | End Hosts    |
| PC (Dept3)| NIC       | 192.168.3.2/.3  | 192.168.3.0/24 | End Hosts    |
| PC (Dept4)| NIC       | 192.168.4.2/.3  | 192.168.4.0/24 | End Hosts    |

## Features Implemented
- Multi-department network with centralized routing via Router1
- Static IP addressing across 4 subnets
- DNS server configured on Server-PT (192.168.1.100)
- HTTPS web server hosted on Server-PT, accessible from all departments
- Inter-VLAN communication via Router1
- Verified connectivity using ICMP (ping) simulation

## Tools Used
- Cisco Packet Tracer 8.x
- Devices: 2811 Router, 2960-24TT Switches, PC-PT, Server-PT

## How to Open
1. Install [Cisco Packet Tracer](https://www.netacad.com/cisco-packet-tracer)
2. Clone this repo
3. Open `network-project.pkt`

## Skills Demonstrated
`Network Design` `Subnetting` `DNS Configuration` `HTTPS Server Setup`
`Static Routing` `Inter-department Connectivity` `Cisco IOS`

## Testing

Successful ICMP communication was verified between all departments and the server.

## Author

Bharath Raj
