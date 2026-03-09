# Network Topology

This homelab uses a local server behind CGNAT, connected to a VPS through WireGuard.

## High-Level Topology

Internet  
↓  
ISP Router (CGNAT)  
↓  
Local Network  
↓  
Ubuntu Server  
↓  
WireGuard Tunnel  
↓  
VPS with public IP

## Purpose

This design allows secure remote access to internal services even when the local network is behind CGNAT.

## Main Components

- ISP router
- local Ubuntu server
- VPS with public IP
- WireGuard VPN
- private access to services
