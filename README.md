# abszeroLabs Homelab

> *A modular, self-hosted environment for cybersecurity research, automation, and experimentation.*

---

## Overview

This homelab serves as a hybrid environment for **cybersecurity research**, **malware analysis**, **AI automation**, and **media management**.  
It’s designed to evolve. Starting small and scaling over time with improved documentation, services, and automation.

---

## Current Infrastructure

### Beelink Mini PC — `Apotheosis`
**OS:** Proxmox VE  
**Specs:** 32GB RAM | 512 GB NVMe SSD  

#### Virtual Machines & Containers
| Type | Hostname | Name | Purpose |
|------|----------|------|----------|
| LXC |  | Twingate Connector | Secure remote access |
| VM | | Kali Linux | Penetration testing lab |
| VM | | SIEM Server | Centralized logging and security monitoring |
| VM | | Windows 11 (Malware Lab) | Malware analysis & testing sandbox |
| VM | | Ubuntu Server | General-purpose server for misc. projects |

---

### Raspberry Pi 5 — `BoreasStation`
**OS:** Raspberry Pi OS + CasaOS  
**Access:** Raspberry Pi Connect / Twingate Connector  

#### Uses
- Lightweight Docker containers  
- SDR (Software-Defined Radio) applications  
- CasaOS app management  
- Experimental IoT and edge workloads  

---

### Dell OptiPlex — `Cryovast`
**OS:** Proxmox VE  

#### Virtual Machines
| Type | Hostname | Name | Purpose |
|------|----------|------|----------|
| VM | | Media Server | Jellyfin media library |
| VM | | AI Automation | n8n workflows & Ollama LLM service |

---

## Network Stack

| Device | Name | Purpose |
|---------|------|----------|
| Ubiquiti Cloud Gateway Ultra | `Umbrathis` | Core routing, firewall, and VPN |
| Ubiquiti 8-Port PoE Switch | `Nexora` | Power & network distribution |

---

## Access & Security

- **Remote Access:** Twingate connector deployed on Beelink & Pi  
- **Internal Network:** Segmented VLANs (to be implemented)  
- **Authentication:** Local accounts + Twingate + MFA enforcement planned  

---
