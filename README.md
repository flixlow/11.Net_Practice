*This project has been created as part of the 42 curriculum by flauweri.*

# NetPractice

## Description

NetPractice is a hands-on learning project from the 42 curriculum that helps students build practical understanding of how computer networks work.

The main objective is to learn how network devices (hosts, routers, switches) communicate: how IPv4 addresses are structured, how subnet masks partition networks, the role of a default gateway, and how a router forwards packets between networks using its routing table.

The project also trains students to diagnose network misconfigurations: when a communication fails, identify the root cause and correct the configuration.

## Instructions

1. Download and extract the project archive to a folder of your choice.
2. From the project root, run the launcher script:

```bash
./run.sh
```

This script starts a local web server and opens the NetPractice interface in your browser.

## How to run the training interface

- In the **Training** tab, enter your intranet login to generate a personalized configuration.
- In the **Evaluation** tab, generate a random configuration for practice or assessment.
- Each level displays a non-working network diagram and one or more objectives to complete.
- Edit the editable fields (IP addresses, subnet masks, gateways, static routes) until the **Check again** button reports the configuration as correct.
- The log area at the bottom helps diagnose problems (missing route, wrong gateway, invalid address, etc.).

## Exporting a configuration

After completing a level, click **Get my config** to download the configuration file for that level. Do this before moving to the next level using **Next level**.

Important: enter your intranet login in the interface before exporting configurations; otherwise the exported files will not be linked to your student account.

## Submission

For evaluation, the Git repository must contain 10 exported configuration files (one per level) placed at the repository root.

## Resources

- Peer learning
- IP calculator: https://jodies.de/ipcalc
- TCP: https://en.wikipedia.org/wiki/Transmission_Control_Protocol
- OSI model (FR): https://fr.wikipedia.org/wiki/Mod%C3%A8le_OSI

## Network concepts covered

- **IPv4 addressing:** structure of an IPv4 address (32 bits, dotted-decimal) and the distinction between network and host portions.
- **Subnet masks:** how to calculate masks to determine network size, available hosts, network and broadcast addresses, and CIDR notation (e.g. /24).
- **Default gateway:** the gateway's role as an exit point from a local network and why hosts must be configured with the correct gateway to communicate across networks.
- **Routers and switches:** the functional difference between a switch (Layer 2 forwarding within the same LAN) and a router (Layer 3 device that forwards packets between networks and uses distinct IPs per interface).
- **Routing tables and static routes:** how routing entries tell a device which interface or gateway to use for a destination (including the default route 0.0.0.0/0).
- **OSI layers:** mapping IP addressing and routing to Layer 3 and switching/physical addresses to Layer 2 to help locate problems.
- **Packet forwarding:** understanding the path a packet takes from source to destination through intermediate devices; useful when reading the interface logs.

### Key terms and notes

- Host: a device connected to the network (computer, phone, server, etc.).
- IP address: the identifier of a device on a network.
- Router: a device that forwards packets toward their destination.
- Packet: a unit of data sent over the network.
- Protocol: a set of communication rules (e.g. TCP, IP, HTTP, HTTPS).
- DNS: a service that translates human-readable domain names into IP addresses.
- Switch: connects devices within the same local network.
- ISP: Internet Service Provider (e.g. Your PC → Router → ISP → Internet).
- MAC address: hardware identifier of a network interface.
- ARP: mechanism that maps a local IP address to a MAC address for local delivery.
- Gateway: the exit point of a network toward other networks.
- Subnet mask: defines which part of an IP address is the network and which part is the host.
- CIDR: notation that indicates the network prefix length (e.g. /24).
- Common ports: 80 → HTTP, 443 → HTTPS, 22 → SSH.

### Transport protocols

- TCP (Transmission Control Protocol):
	- establishes a connection before data exchange
	- guarantees delivery
	- reorders segments
	- retransmits lost packets

- UDP (User Datagram Protocol):
	- connectionless
	- no delivery guarantee
	- no reordering
	- low overhead

## Notes about AI usage

AI assistance was used to explain concepts and translate and reformat this README.

---
