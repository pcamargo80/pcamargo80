# Pablo Camargo

**Platform Engineer | DevOps | Cloud Infrastructure | AI Automation | Flutter**

I design and build self-hosted platforms that combine infrastructure, observability, automation, backend services, and mobile applications.

My current focus is **KINVIA**, a personal platform used to validate production-like architecture patterns with Docker, Cloudflare Tunnel, Traefik, Authelia, observability tooling, backend services, and Flutter apps.

---

## Current Focus

- Building the **KINVIA Platform** as a self-hosted homelab and SaaS foundation.
- Improving infrastructure security and service exposure with Cloudflare, Traefik, and Authelia.
- Implementing observability with Grafana, Prometheus, Loki, Node Exporter, cAdvisor, Promtail, and Uptime Kuma.
- Developing Flutter apps with offline-first architecture.
- Designing automation workflows with n8n, Python, and AI-assisted processes.

---

## Featured Project

### KINVIA Platform

KINVIA Platform is a self-hosted platform built on Fedora Server using Docker and Docker Compose.

The public edge architecture follows this flow:

```text
Internet
  ↓
Cloudflare DNS / Proxy
  ↓
Cloudflare Tunnel
  ↓
Traefik Reverse Proxy
  ↓
Authelia Forward Auth
  ↓
Docker Services
```

Core services include:

- Public landing page: `kinvia.dev`
- Authentication layer: Authelia
- Reverse proxy: Traefik
- Observability: Grafana, Prometheus, Loki, Promtail
- Host and container metrics: Node Exporter, cAdvisor
- Availability monitoring: Uptime Kuma
- Automation foundation: n8n
- SaaS foundation: PostgreSQL and Redis on the internal Docker network

Repository:

- [kinvia-platform-showcase](https://github.com/pcamargo80/kinvia-platform-showcase)

---

## Technical Stack

### Infrastructure & DevOps

- Fedora Server
- Linux
- Docker
- Docker Compose
- Traefik
- Cloudflare Tunnel
- Cloudflare DNS / Proxy
- Authelia
- Nginx

### Observability

- Grafana
- Prometheus
- Loki
- Promtail
- Node Exporter
- cAdvisor
- Uptime Kuma

### Backend

- Node.js
- TypeScript
- Fastify
- Prisma
- PostgreSQL
- Redis

### Mobile

- Flutter
- Dart
- Riverpod
- Hive
- Material 3
- Offline-first architecture

### Automation

- n8n
- Python
- AI workflows
- Monitoring scripts
- Operational reports

---

## Project Areas

### Platform Engineering

- [KINVIA Platform Showcase](https://github.com/pcamargo80/kinvia-platform-showcase)
- KINVIA Homelab
- KINVIA API
- KINVIA Site

### Mobile Applications

- KINVIA Student
- KINVIA Home
- KINVIA Finance
- KINVIA Control

### Automation & Operations

- Monitor Helps
- QR generation tools
- Requirements control tools
- Operational reporting tools

---

## Engineering Principles

- Keep public services minimal and intentional.
- Protect internal observability and admin services.
- Prefer internal Docker networking for databases and infrastructure dependencies.
- Document architecture decisions clearly.
- Build small, functional MVPs before adding complexity.
- Avoid exposing secrets, internal IPs, credentials, or sensitive runtime configuration.

---

## Currently Building

- KINVIA SaaS backend foundation
- API service exposure through `api.kinvia.dev`
- Future app surface through `app.kinvia.dev`
- Reduced attack surface for observability services
- CI/CD roadmap with GitHub Actions
- Additional automation workflows with n8n and AI
