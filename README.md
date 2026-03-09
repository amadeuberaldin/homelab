# Homelab Infrastructure

Welcome to my **personal homelab**, where I experiment with Linux servers, networking, VPN architectures, Docker services, and self-hosted systems.

This repository documents the infrastructure, architecture, and experiments running in my self-hosted environment.

---

# Homelab Dashboard

## Infrastructure Overview

| Component | Description |
|----------|-------------|
| Local Server | Ubuntu Server running services and experiments |
| VPS | Public server used as VPN hub |
| VPN | WireGuard tunnel connecting local network to VPS |
| Docker | Containerized services and experiments |
| Self-hosted services | Development tools, game servers, and infrastructure tests |

---

# Network Architecture

The homelab network is designed to work even when the local network is behind CGNAT.

High-level topology:

Internet
│
▼
ISP Router (CGNAT)
│
▼
Local Network
│
▼
Ubuntu Server
│
│ WireGuard VPN
▼
VPS (Public IP)
│
▼
Private VPN Network

Detailed network documentation:

→ `network/topology.md`

---

# Services and Experiments

Examples of workloads running in the lab:

- Docker services
- game server experiments
- development environments
- networking experiments
- infrastructure testing

More details:

→ `services/services.md`

---

# Documentation

Main documentation sections:

| Section | Description |
|-------|-------------|
| `docs/` | general documentation |
| `network/` | network architecture and VPN |
| `services/` | services and workloads |

---

# Technologies Used

Core technologies used in this environment:

- Linux (Ubuntu Server)
- Docker
- WireGuard VPN
- Git
- networking and system administration
- self-hosted infrastructure

---

# Related Projects

This homelab connects to other repositories documenting specific infrastructure components.

VPN Infrastructure  
https://github.com/amadeuberaldin/wireguard-vpn-infrastructure

AI Agent Infrastructure  
https://github.com/amadeuberaldin/ai-agent-infrastructure

---

# Learning Philosophy

This homelab follows a simple principle:

**learn infrastructure by building real systems and documenting them.**

Experiments evolve over time as new services, tools, and architectures are explored.

---

# Status

This repository is continuously updated as the homelab grows and new infrastructure components are added.
