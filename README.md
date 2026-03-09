# Homelab

This repository documents my personal **homelab infrastructure**, where I experiment with networking, Linux administration, VPN architecture, Docker services, and self-hosted systems.

The purpose of this lab is to learn by building real systems and documenting how they are designed and operated.

---

# Goals

The homelab is used to:

- practice Linux server administration
- experiment with networking and VPN architectures
- run self-hosted services
- build and test infrastructure setups
- document practical learning and experiments

---

# Infrastructure

The current lab environment includes both **local infrastructure** and **remote infrastructure**.

## Local Server

Main self-hosted machine running multiple services.

System:

- Ubuntu Server
- Docker
- development environment
- game server experiments
- infrastructure testing

---

## Remote Infrastructure

A VPS with a public IP address used to enable remote connectivity.

Main roles:

- WireGuard VPN hub
- secure remote access
- bridge between external network and local services

---

# Network Architecture

The homelab network is designed to work even with the local network behind CGNAT.

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


This architecture allows secure remote access to the internal network.

---

# Technologies Used

Core technologies used in the homelab:

- Linux (Ubuntu Server)
- Docker
- WireGuard VPN
- Git
- self-hosted services
- networking and system administration

---

# Related Projects

This homelab connects with other repositories that document specific parts of the infrastructure:

- VPN infrastructure  
  https://github.com/amadeuberaldin/wireguard-vpn-infrastructure

- AI agent infrastructure  
  https://github.com/amadeuberaldin/ai-agent-infrastructure

---

# Status

This homelab is continuously evolving as new services, experiments, and infrastructure improvements are added.
