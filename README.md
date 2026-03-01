# overm-contracts

OpenAPI specs and Kafka message schemas for OVERMenu microservices.

## Contracts

- `user-auth-api.yaml` — Auth API (mobile/internal)
- `user-auth-web.yaml` — Auth Web (browser)
- `recipe-catalog.yaml` — Recipe management
- `kafka-contracts.yaml` — Async event schemas

## Quick Start

**View contracts:**
```bash
docker-compose up -d
# Open http://localhost:8090
```

**Validate:**
```bash
npm install -g @stoplight/spectral-cli
spectral lint contracts/*.yaml
```

Validation runs automatically on PRs via GitHub Actions.