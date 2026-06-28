# CivicOS

**The open civic operating system — built for citizens, representatives, and communities.**

We're building the infrastructure layer for democratic participation: a platform that closes the gap between elections by giving citizens a direct line to their government and giving governments a real-time pulse on what their communities care about.

---

## What We're Building

CivicOS is a civic engagement platform for Africa and beyond. Citizens report local issues, sign petitions, and engage with elected representatives. Representatives respond, track community sentiment, and demonstrate accountability — all in one place.

**Core modules (MVP):**
- Issue reporting with status tracking (OPEN → IN_PROGRESS → RESOLVED)
- Community petitions with signature goals and deadlines
- Representative dashboards linked to constituencies
- Role-based access: citizen, representative, government admin, NGO, moderator

---

## Repositories

| Repo | Description |
|------|-------------|
| [`civicos`](https://github.com/civicos-hq/civicos) | Main monorepo — Go backend services + React frontend |

---

## Stack

| Layer | Technology |
|-------|-----------|
| Backend | Go 1.22 · Gin · GORM |
| Frontend | React 18 · Vite · TypeScript · Tailwind CSS |
| Database | PostgreSQL 16 |
| Cache | Redis 7 |
| Messaging | NATS |
| Auth | JWT (golang-jwt/jwt/v5) · bcrypt |
| Infra | Docker · GitHub Actions |

---

## Services

```
api-gateway        :3000  — reverse proxy, JWT validation
identity-service   :3001  — auth, users, roles
community-service  :3002  — communities, issues, petitions
web (frontend)     :5173  — React + Vite
```

---

## Status

🚧 **Active development — MVP in progress.**

- [x] Monorepo scaffold
- [x] Identity Service (auth, JWT, bcrypt)
- [x] Community Service (communities, issues)
- [x] API Gateway (reverse proxy)
- [ ] Frontend auth flow
- [ ] Issue reporting UI
- [ ] Representative pages
- [ ] Petitions
- [ ] Notifications

---

## Contributing

The project is in early development. If you're interested in contributing or following along, watch the main repo — contribution guidelines are coming with the first public release.

---

## Philosophy

Government doesn't have to be opaque. CivicOS is built on the belief that the infrastructure for civic life should be open, accountable, and community-owned — the same way roads and water pipes are public infrastructure.

---

*Built with Go and React · Open source · Made for Africa*
