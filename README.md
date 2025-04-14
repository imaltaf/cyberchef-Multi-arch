# CyberChef (codesec/cyberchef)

[![Docker Pulls](https://img.shields.io/docker/pulls/codesec/cyberchef?style=for-the-badge)](https://hub.docker.com/r/codesec/cyberchef)
[![Docker Image Size](https://img.shields.io/docker/image-size/codesec/cyberchef/latest?style=for-the-badge)](https://hub.docker.com/r/codesec/cyberchef)
[![Docker Platforms](https://img.shields.io/badge/platform-linux%2Famd64%20%7C%20linux%2Farm64-blue?style=for-the-badge)](https://hub.docker.com/r/codesec/cyberchef)

🚀 Multi-arch Docker image for [CyberChef](https://github.com/imaltaf/cyberchef-Multi-arch.git) — built and maintained by **codesec**.

---

## 📦 Install & Run

You can quickly run CyberChef using **Docker** or **Docker Compose**.

---

---

## 🐳 Run with Docker

```bash
docker pull codesec/cyberchef:latest

```
```bash
docker run -d --name cyberchef -p 8000:80 codesec/cyberchef:latest
```

✅ Open your browser and visit: http://localhost:8000



# 📑 Run with Docker Compose

## 📥 Download docker-compose.yml
You can download the pre-configured multi-arch Docker Compose file from this repository:

```sh
curl -O https://raw.githubusercontent.com/imaltaf/cyberchef-Multi-arch/main/docker-compose.yml
```

### Then run it with:

```sh
docker compose up -d
```

### 📦 This will automatically pull and run the CyberChef multi-arch images as defined in the compose file.

```bash
version: '3.8'

services:
  cyberchef:
    image: codesec/cyberchef:latest
    container_name: cyberchef
    ports:
      - "8000:80"
    restart: unless-stopped

```
Then run:

```sh
docker compose up -d

```
✅ Open your browser and visit: http://localhost:8000

## 📥 Pulling Single-Architecture Images

You can pull pre-built CyberChef images for a specific architecture:

---

### ✅ Pull `arm64` image

```bash
docker pull codesec/cyberchef:arm64

docker pull codesec/cyberchef:amd64
```
## ✅ You can then run them like this:

```sh
docker run -d --name cyberchef-arm64 -p 8000:80 codesec/cyberchef:arm64
```
### or

```sh
docker run -d --name cyberchef-amd64 -p 8000:80 codesec/cyberchef:amd64

```



## 📌 Image Details
📦 Image: codesec/cyberchef:latest

🏗️ Platforms: linux/amd64, linux/arm64

🖥️ Exposes port: 80 (mapped to your host on 8000)

## 🛠️ Environment Variables
N/A — CyberChef static build requires no additional environment configuration.

## 📖 License

CyberChef is © GCHQ, licensed under Apache License 2.0.
