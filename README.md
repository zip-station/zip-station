# Zip Station

A simple, modern, open-source helpdesk system. Receive support emails, manage tickets, and respond to customers — all from one dashboard.

## Quick Start

```bash
git clone https://github.com/zipstation/zip-station.git
cd zip-station
cp .env.example .env
# Edit .env with your values
docker compose up -d
```

Open `http://localhost:3000` and create your account.

## Documentation

Full docs at [zipstation.github.io/zip-station-docs](https://zipstation.github.io/zip-station-docs) (or see the [zip-station-docs](https://github.com/zipstation/zip-station-docs) repo).

## What's Inside

| Container | Image | Purpose |
|---|---|---|
| **API** | `ghcr.io/zipstation/zip-station-service` | REST API |
| **Worker** | `ghcr.io/zipstation/zip-station-service-worker` | Background jobs (email polling, alerts, reports) |
| **SPA** | `ghcr.io/zipstation/zip-station-spa` | Web dashboard |
| **MongoDB** | `mongo:7` | Database (included, or bring your own) |

## Requirements

- Docker & Docker Compose
- Firebase project (free tier) for authentication
- Email account (any IMAP/SMTP provider)
- 1 GB RAM minimum

## License

MIT
