# self-hosting

This repository documents the self-hosted services I run in my homelab, primarily managed via [Proxmox VE](https://www.proxmox.com/en/) on HP EliteDesk.

---

## 📦 Infrastructure

### 🖥️ Proxmox VE
- **Role**: Hypervisor for virtual machines and LXC containers
- **Backups**: Integrated with Proxmox Backup Server (PBS)
- **Features**: Snapshots

### 📁 Synology DSM
- **Role**: Central NAS for storage, media, and backups
- **Model**: Synology DS918+
- **Features**: Shared folders for media, backups, docker volumes

---

## 🔧 Services

### [🎧 Audiobookshelf](https://github.com/advplyr/audiobookshelf)
- **Description**: Audiobook and podcast server

### [🌐 Caddy](https://github.com/caddyserver/caddy) (Reverse Proxy)
- **Description**: Automatic HTTPS reverse proxy server
- **Configuration**:
  - Handles TLS certificates automatically via Let's Encrypt
  - Routes incoming requests to backend services (e.g., Audiobookshelf)

### [📄 Paperless-ngx](https://github.com/paperless-ngx/paperless-ngx)
- **Description**: Document management system with tags, correspondents, full-text search, and more
