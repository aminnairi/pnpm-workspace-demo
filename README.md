# pnpm-workspace-demo

## Requirements

- Docker
- Docker Compose

## Clone

```bash
git clone https://github.com/aminnairi/pnpm-workspace-demo

cd pnpm-workspace-demo
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

## Endpoints

Endpoint | Description
---|---
[`localhost:8000`](http://localhost:8000) | Frontend
[`localhost:9000`](http://localhost:9000) | Backend
