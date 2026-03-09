# Network Topology

This document describes the network architecture used in the homelab.

The environment connects a local server behind CGNAT to a VPS with a public IP using WireGuard.

---

## Network Diagram

```mermaid
flowchart TD

Internet[Internet]

Router[ISP Router\nCGNAT]

LAN[Local Network\n192.168.100.0/24]

Server[Ubuntu Server\n192.168.100.50]

VPN[WireGuard Tunnel\n10.10.10.0/24]

VPS[VPS\nWireGuard Hub\n10.10.10.1]

Services[Self Hosted Services\nDocker\nMinecraft\nAI Agents]

Internet --> Router
Router --> LAN
LAN --> Server
Server --> VPN
VPN --> VPS
Server --> Services
