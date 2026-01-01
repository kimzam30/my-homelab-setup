# 🏠 My HomeLab Setup
- A centralized, Docker-based infrastructure for managing my NAS, services, and monitoring.

## 🛠 The Stack
```
| Service | Purpose | Port |
| :--- | :--- | :--- |
| **Homepage** | Main Dashboard | `3000` |
| **FileBrowser** | Web-based NAS Manager | `8080` |
| **Uptime Kuma** | Service Monitoring | `3001` |
| **Nginx** | Reverse Proxy | `80` |
```

## 🚀 Getting Started

### 1. **Clone the Repo**
```bash
   git clone [https://github.com/kimzam30/my-homelab-setup.git](https://github.com/kimzam30/my-homelab-setup.git)
   cd my-homelab-setup


- Configure Environment Duplicate the example file and fill in your secrets:

    cp .env.example .env
    Edit .env with your PUID, PGID, and NAS_ROOT path.
    Deploy

    docker-compose up -d
```

## 📂 Configuration

    Homepage: configs located in config/homepage/

    Nginx: rules located in config/nginx/nginx.conf

    FileBrowser: settings in config/filebrowser/

## 🔒 Security

- This repository uses "dummy" config files. Sensitive data (databases, .env files) are gitignored.
