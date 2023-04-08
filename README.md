# pnpm-workspace-demo

## Summary

- [Requirements](#requirements)
- [Clone](#clone)
- [Docker Compose Build](#docker-compose-build)
- [Docker Compose Services Startup](#docker-compose-services-startup)
- [Node Modules Installation](#node-modules-installation)
- [Development](#development)
- [Build](#build)
- [Docker Compose Services Shutdown](#docker-compose-services-shutdown)
- [Endpoints](#endpoints)

## Requirements

- Docker
- Docker Compose

[Back to summary](#summary)

## Clone

```bash
git clone https://github.com/aminnairi/pnpm-workspace-demo

cd pnpm-workspace-demo
```

[Back to summary](#summary)

## Docker Compose Build

```bash
docker compose build
```

[Back to summary](#summary)

## Docker Compose Services Startup

```bash
docker compose up --detach
```

[Back to summary](#summary)

## Node Modules Installation

```bash
docker compose exec node pnpm install
```

[Back to summary](#summary)

## Development

```bash
docker compose exec node pnpm --parallel run dev
```

[Back to summary](#summary)

## Build

```bash
docker compose exec node pnpm --parallel run build
```

[Back to summary](#summary)

## Docker Compose Services Shutdown

```bash
docker compose down --remove-orphans --volumes --timeout 0
```

[Back to summary](#summary)

## Endpoints

Endpoint | Description
---|---
[`localhost:8000`](http://localhost:8000) | Frontend
[`localhost:9000`](http://localhost:9000) | Backend

[Back to summary](#summary)
