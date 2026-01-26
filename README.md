## 👋 Welcome to joplin 🚀

Open-source note-taking and to-do application

## 📋 Description

Open-source note-taking and to-do application

## 🚀 Services

- **joplin**: joplin/joplin:latest

### Infrastructure Components

- **joplin-db**: Postgres database


## 📦 Installation

### Option 1: Quick Install
```bash
curl -q -LSsf "https://raw.githubusercontent.com/composemgr/joplin/main/docker-compose.yaml" -o compose.yml
```

### Option 2: Git Clone
```bash
git clone "https://github.com/composemgr/joplin" ~/.local/srv/docker/joplin
cd ~/.local/srv/docker/joplin
docker compose up -d
```

### Option 3: Using composemgr
```bash
composemgr install joplin
```

## 🔧 Configuration

### Environment Variables

```shell
TZ=America/New_York
```

See `docker-compose.yaml` for complete list of configurable options.

## 🌐 Access

- **Web Interface**: http://172.17.0.1:22300

## 📂 Volumes

- `./rootfs/data/joplin` - Data storage
- `./rootfs/config/joplin` - Data storage
- `./rootfs/data/db/postgres/joplin` - Data storage

## 🔐 Security

- Change all default passwords before deploying to production
- Use strong secrets for all authentication tokens
- Configure HTTPS using a reverse proxy (nginx, traefik, caddy)
- Regularly update Docker images for security patches
- Backup your data regularly

## 🔍 Logging

```shell
docker compose logs -f joplin
```

## 🛠️ Management

```bash
# Start services
docker compose up -d

# Stop services
docker compose down

# Update to latest images
docker compose pull && docker compose up -d

# View logs
docker compose logs -f

# Restart services
docker compose restart
```

## 📋 Requirements

- Docker Engine 20.10+
- Docker Compose V2+

## 🤝 Author

🤖 casjay: [Github](https://github.com/casjay) 🤖  
🦄 composemgr: [Github](https://github.com/composemgr) 🦄
