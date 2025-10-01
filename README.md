# abszerolabs: My Homelab

Welcome to my homelab! This is my sandbox for **computers**, **networking**, and **cybersecurity**. I use it to learn, experiment, and build projects related to my Master’s program, as well as to run fun self-hosted apps and services.

> I use this lab as part of my Master’s in Cybersecurity and Privacy program and for hands-on projects in malware analysis, network defense, and infrastructure automation.

---

## Table of Contents
- [Architecture](#architecture)
- [Core Technologies](#core-technologies)
- [Services](#services)
- [Projects](#projects)
- [Real World Applications](#real-world-applications)
- [Lessons and Skills Learned](#lessons-and-skills-learned)
- [Hardware](#hardware)

---

## Architecture
![Lab Diagram](architecture-diagrams/homelab-overview.png)

### Servers
| Name | Hardware | OS |  Application |
|------|----------|----|--------------|
| [Apotheosis](docs/Apotheosis.md) | Beelink Mini PC | Proxmox | Main server for projects and learning |
| [BoreasStation](docs/BoreasStation.md) | Raspberry Pi 5 | Raspberry Pi OS | For fun and experimenting and SDR applications |
| [CelestialScriptarium](docs/CelestialScriptarium.md) | Dell Optiplex 3080 | TrueNAS Scale |  |
| [DemiurgeCore](docs/DemiurgeCore.md) | Dell Precision Tower 7420 | Proxmox |  |

### Networking Hardware
- Ubiquiti Ultra Cloud Gateway
- Ubiquiti 8-port PoE Switch
- (Planned) Ubiquiti WiFi Router


## Core Technologies
<details>
<summary>Virtualization</summary>
Proxmox on 2 machines
</details>
<details>
<summary>Storage</summary>
TrueNAS Scale (dedicated), 2TB Pi drive for quick storage</details>
<details>
<summary>Containers & Apps</summary>
Docker + CasaOS on the Pi + LXC Containers through Proxmox</details>
<details>
<summary>Remote Access</summary>
Twingate (LXC connector) + Backup Twingate connector on Pi, Ubiquiti VPN</details>
<details>
<summary>Networking</summary>
All managed through the Ubiquiti Ultra Cloud Gateway (firewall, VPN, VLANs, monitoring)</details>
<details>
<summary>Security</summary>
SIEM, vulnerability scanners, Suricata</details>
<details>
<summary>Operating Systems</summary>
Ubuntu Server for VMs unless required otherwise</details>
<details>
<summary>Databases</summary>
Self-hosted DB in Beelink Proxmox LXC</details>
<details>
<summary>Special Hardware</summary>
SDR dongle for radio experiments</details>

## Services
| Category       | Services                  |
|----------------|------------------------|
| Infrastructure & Management | CasaOS, Portainer, Dashy, Ubiquiti apps, Twingate, ProtonVPN, Gluetun        |
| Media     | Jellyfin, Radarr, Sonarr, qBittorrent |
| Automation & AI       | n8n, Ollama, Open WebUI for Ollama |
| Security | Pi-hole, Wazuh, Suricata, OpenVAS |
| Web & Monitoring | Nginx, Grafana, Prometheus |
| Other Experiments | (various apps for testing/learning) |


## Projects
- Malware Analysis: Static & dynamic analysis on Windows VM for my Master’s program
- Detection & Pen Testing Lab: SIEM, IDS/IPS, scanners, red/blue team experiments
- Logging & Monitoring: Centralized dashboards & alerts

  
## Real World Applications
- AI Server – n8n + Ollama workflows
- Media Streaming – Jellyfin setup for future family use
- Cloud Storage – Personal data + backups
- Dashboards – Network/service visibility
- Sandbox – General skill-building and experiments

  
## Lessons and Skills Learned
- Networking & Security – firewall, VPN, VLANs, SIEM, IDS/IPS, vulnerability scanning
- Systems Administration – virtualization, container orchestration, storage management
- Automation & Scripting – workflow automation (n8n), infrastructure management (Ansible, LXC/Docker)
- Monitoring & Troubleshooting – log collection, dashboards, alerting
- Trade-offs between VMs, LXC containers, and Docker in resource usage
