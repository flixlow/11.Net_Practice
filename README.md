*This project has been created as part of the 42 curriculum by flauweri.*

# NetPractice

## Overview

NetPractice is a hands-on learning project from the 42 curriculum that helps students build practical intuition about how computer networks work.

The main goal is to understand how network devices (hosts, routers, switches) communicate: how IPv4 addresses are structured, how subnet masks partition networks, the role of a default gateway, and how a router forwards packets between networks using its routing table.

More generally, the project trains students to diagnose network misconfigurations: given a failing communication, identify the root cause and correct the configuration.

## Getting started

1. Download and extract the project archive to a folder of your choice.
2. From the project root, run the launch script:

```bash
./run.sh
```

This script starts a local web server and opens the NetPractice interface in your browser.

## Using the interface

- Enter your intranet login in the **Training** tab to generate a personalized configuration.
- Use the **Evaluation** tab to generate a random configuration for testing or assessment.
- Each level shows a non-functioning network diagram and one or more objectives to achieve.
- Edit the editable fields (IP addresses, subnet masks, gateways, static routes) until the **Check again** button reports the configuration as correct.
- The log area at the bottom helps diagnose issues (missing route, wrong gateway, invalid address, etc.).

## Exporting a configuration

After you complete a level, click **Get my config** to download the configuration file for that level. Do this before advancing to the next level using **Next level**.

Important: you must enter your intranet login in the interface before exporting configurations; otherwise the exported files will not be linked to your student account.

## Submission

The Git repository submitted for evaluation must contain 10 exported configuration files (one per level) placed at the repository root.

## Resources

- Peer-to-peer learning
- IP Calculator: https://jodies.de/ipcalc
- TCP: https://en.wikipedia.org/wiki/Transmission_Control_Protocol
- OSI model (French): https://fr.wikipedia.org/wiki/Mod%C3%A8le_OSI

## Network concepts covered

- **IPv4 Addressing:** Structure of an IPv4 address (32 bits, dotted decimal) and the distinction between network and host portions.
- **Subnet Masks:** Calculating masks to determine network size, available hosts, network and broadcast addresses, and CIDR notation (for example, /24).
- **Default Gateway:** The gateway's role as an exit point from a local network and the need to configure it correctly on hosts for inter-network communication.
- **Routers and Switches:** Functional difference between a switch (Layer 2 switching within the same LAN) and a router (Layer 3 device forwarding packets between networks, with distinct IPs per interface).
- **Routing Tables and Static Routes:** How routes instruct a device which interface or gateway to use for a destination (including the default route 0.0.0.0/0).
- **OSI Layers:** Placing IP addressing and routing at Layer 3 and switches/physical addresses at Layer 2 to help locate the source of problems.
- **Packet Forwarding:** Understanding the path a packet takes from source to destination through intermediate devices; useful when reading the interface logs.

## Notes about AI usage

- AI assistance was used to translate and reformat this README. It was also use to explain or reformulate concepts.

---
