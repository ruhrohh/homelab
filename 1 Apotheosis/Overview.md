# Apotheosis — Proxmox Node

## Purpose
Primary hypervisor running all core VMs.

## Hardware
- CPU:
- RAM:
- Storage:
- External: 2TB SSD (backups/snapshots)

## Network
- Hostname: apotheosis
- IP Address:
- Connected Switch Port:
- Twingate: No (LXC connector handles it)

## Core Services
- Proxmox 8.x
- LXC: Twingate Connector

## Virtual Machines
- Polarion (Kali)
- Noctus Bastion (SIEM)
- Nullborne (Malware Lab)
- Aetherion (Ubuntu)

## Backup Strategy
- VM snapshots → 2TB attached drive
- Frequency: Manual / Weekly?
