# qBittorrent-sorter

## Overview

The qBittorrent-sorter is a simple script that sorts your torrents by type, such as movies, TV series, and general data. This sorting feature is particularly useful for users of media server applications like `Jellyfin`. 

## Usage 

docker-compose:

```yml
version: '3.8'
services:
  qBittorrent-sorter:
    image: ghcr.io/chubru/qbittorrent-sorter:latest
    environment:
      QBITTORRENT_HOST: "http://localhost:8088"
      QBITTORRENT_USERNAME: "admin"
      QBITTORRENT_PASSWORD: "admin"
      REFRESH_INTERVAL: "60"
      RETRY_INTERVAL: "60"
      LOG_LEVEL: "INFO"
```

Supported Architectures:

    AMD64 ✅
    ARM64 ✅
    ARMv7 ✅