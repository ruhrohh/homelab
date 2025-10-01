# My Homelab

Welcome to my homelab! This is my sandbox for **computers**, **networking**, and **cybersecurity**. I use it to learn, experiment, and build projects related to my Master’s program, as well as to run fun self-hosted apps and services.

I use this lab as part of my Master’s in Cybersecurity and Privacy program and for hands-on projects in malware analysis, network defense, and infrastructure automation.

---

## Table of Contents
- [Architecture](#architecture)
- [Core Technologies](#core-technologies)
- [Services](#services)
- [Projects](#projects)
- [Real World Applications](#real-world-applications)
- [Lessons and Skills Learned](#lessons-and-skills-learned)

---

## Architecture
![Lab Diagram](architecture-diagrams/homelab-overview.png)
| Category       | Hardware                  | OS          |
|----------------|------------------------|-------------|
| Server | Beelink Mini PC | Proxmox |
| | Dell Optiplex 3080 | TrueNAS Scale |
| | Raspberry Pi 5 | Raspberry Pi OS |
| | Dell Precision Tower 7420 | Proxmox |
| Networking     | Ubiquiti Ultra Cloud Gateway (firewall, VPN, VLANs, monitoring) |          |
| | Ubiquiti 8-port PoE Switch | |
| | (Planned) Ubiquiti WiFi Router | |


## Core Technologies
<details>
<summary>Click to expand</summary>

| Category       | Services                  |
|----------------|------------------------|
| Virtualization | Proxmox on 2 machines |
| Storage     | TrueNAS Scale (dedicated), 2TB Pi drive for quick storage |
| Containers & Apps       | Docker + CasaOS on the Pi + LXC Containers through Proxmox|
| Remote Access | Twingate (LXC connector) + Backup Twingate connector on Pi, Ubiquiti VPN |
| Networking | All managed through the Ubiquiti Ultra Cloud Gateway (firewall, VPN, VLANs, monitoring) |
| Security | SIEM, vulnerability scanners, Suricata |
| Operating Systems | Ubuntu Server for VMs unless required otherwise |
| Databases | Self-hosted DB in Beelink Proxmox LXC |
| Special Hardware | SDR dongle for radio experiments |
</details>



## Services
<details>
<summary>Services</summary>

| Category       | Services                  |
|----------------|------------------------|
| Infrastructure & Management | CasaOS, Portainer, Dashy, Ubiquiti apps, Twingate, ProtonVPN, Gluetun        |
| Media     | Jellyfin, Radarr, Sonarr, qBittorrent |
| Automation & AI       | n8n, Ollama, Open WebUI for Ollama |
| Security | Pi-hole, Wazuh, Suricata, OpenVAS |
| Web & Monitoring | Nginx, Grafana, Prometheus |
| Other Experiments | (various apps for testing/learning) |
</details>


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
