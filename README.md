# 🏠 Home Assistant Configuration

This repository contains my personal Home Assistant configuration, including automations, integrations, and customizations used in my home lab environment.

---

## 📌 Overview

This setup is designed to support a self-hosted smart home environment with a focus on:

- Reliability and uptime
- Network segmentation (VLAN-aware devices)
- Security-first design
- Scalable automation

---

## 🧱 Environment

- **Platform:** Home Assistant (Core / Container / VM)
- **Host:** Proxmox (LXC / VM)
- **Networking:** VLAN-based segmentation (IoT, Home, Guest)
- **DNS:** AdGuard Home + Unbound
- **Remote Access:** Cloudflare / Tailscale
- **Monitoring:** Uptime Kuma, Wazuh (IDS)

---

## 📁 Repository Structure

```bash
.
├── configuration.yaml
├── automations.yaml
├── scripts.yaml
├── scenes.yaml
├── templates/
├── integrations/
├── packages/
```

---

## ⚙️ Features

- Automated routines (lighting, presence, scheduling)
- IoT device integration (cameras, sensors, switches)
- Secure remote access via Zero Trust (Cloudflare / Tailscale)
- Monitoring and alerting
- Custom templates and advanced automations

---

## 🚀 Deployment

1. Clone the repository:
```bash
git clone https://github.com/mdziegiel/home-assistant-config.git
```

2. Copy files into your Home Assistant config directory:
```bash
/config
```

3. Restart Home Assistant:
- Settings → System → Restart

---

## ⚠️ Important Notes

- Secrets are **NOT stored** in this repository  
- Use `secrets.yaml` for sensitive values  
- Update entity IDs and IPs to match your environment  
- Review automations before enabling  

---

## 🔐 Security Considerations

- IoT devices isolated on VLANs  
- No direct exposure where possible (Zero Trust access)  
- DNS filtering via AdGuard Home  
- Monitoring via Wazuh  

---

## 📌 Disclaimer

This configuration is provided as-is for reference and learning purposes.

- No guarantees on stability or compatibility  
- Use at your own risk  
- Always review before deploying  

---

## 📫 Contact

Open an issue if needed.
