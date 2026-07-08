# Module 02 — Introduction to Networking

## Overview
This module covers how devices actually communicate with each other — the 
foundation for understanding how attacks (and defenses) work at the network level.

## Key Concepts

### The OSI Model
A 7-layer conceptual model for how data moves across a network:
1. **Physical** — raw bits, cables, signals
2. **Data Link** — MAC addresses, switches, local frame delivery
3. **Network** — IP addresses, routing between networks
4. **Transport** — TCP/UDP, ports, reliable vs unreliable delivery
5. **Session** — managing connections between applications
6. **Presentation** — data formatting, encryption, compression
7. **Application** — what the user actually interacts with (HTTP, DNS, etc.)

### TCP/IP Model
The more practical 4-layer model actually used on real networks (Application, 
Transport, Internet, Network Access) — maps roughly onto the OSI model but is 
what's actually implemented in real systems.

### IP Addressing & Ports
- IP addresses identify a device on a network
- Ports identify a specific service/application running on that device
- Together, an IP + port is how traffic gets routed to the right destination

### Common Protocols
- **TCP** — reliable, connection-based (handshake, guaranteed delivery)
- **UDP** — faster, connectionless, no delivery guarantee
- **DNS** — translates domain names into IP addresses
- **HTTP/HTTPS** — how web traffic is transmitted

## What Clicked For Me
You can't understand how systems get attacked until you understand how data 
actually moves between them. Concepts like port scanning, sniffing, or spoofing 
only make sense once you see how a packet actually travels from one device to 
another through these layers.

## Questions I'm Still Working Through
- How do these layers map to real tools I'll use later (Wireshark, Nmap)?
- What does abnormal/malicious traffic actually look like at each layer?
