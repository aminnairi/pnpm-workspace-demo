# pnpm-workspace-demo

## Requirements

- Docker
- Docker Compose

## Clone

```bash
git clone https://github.com/aminnairi/pnpm-workspace-demo

cd pnpm-workspace-demo
```

## Docker Compose Build

```bash
docker compose build
```

## Docker Compose Services Startup

```bash
docker compose up --detach
```

## Node Modules Installation

```bash
docker compose exec node pnpm install
```

## Development

```bash
docker compose exec node pnpm --parallel run dev
```

## Build

```bash
docker compose exec node pnpm --parallel run build
```

## Docker Compose Services Shutdown

```bash
docker compose down --remove-orphans --volumes --timeout 0
```

## Endpoints

Endpoint | Description
---|---
[`localhost:8000`](http://localhost:8000) | Frontend
[`localhost:9000`](http://localhost:9000) | Backend
