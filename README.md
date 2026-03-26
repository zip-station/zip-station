# Zip Station

A simple, modern, open-source helpdesk system. Receive support emails, manage tickets, and respond to customers — all from one dashboard.

**[Live Demo](https://demo.zipstation.dev)** · **[Documentation](https://zipstation.dev)** · **[GitHub](https://github.com/zip-station)**

> Demo login: `demo@zipstation.dev` / `TestAccount` (read-only)

## Quick Start

```bash
git clone https://github.com/zip-station/zip-station.git
cd zip-station
cp .env.example .env
# Edit .env with your values
docker compose up -d
```

Open `http://localhost:3000` and create your account. Full setup guide at [zipstation.dev/docs/setup-guide/quick-start](https://zipstation.dev/docs/setup-guide/quick-start).

## What's Inside

| Container | Image | Purpose |
|---|---|---|
| **API** | `ghcr.io/zip-station/zip-station-service` | REST API |
| **Worker** | `ghcr.io/zip-station/zip-station-service-worker` | Background jobs (email polling, alerts) |
| **SPA** | `ghcr.io/zip-station/zip-station-spa` | Web dashboard |
| **MongoDB** | `mongo:7` | Database |

## Requirements

- Docker & Docker Compose
- Firebase project (free tier) for authentication
- Email account with IMAP/SMTP access
- 1 GB RAM minimum

## License

GPLv3 — see [LICENSE](LICENSE).
