# KOVIAN Fitness — Fitness Management Platform

**Principal project:** https://github.com/kovacsruan-stack/kovian-fitness

KOVIAN Fitness is a full-stack fitness management platform focused on domain modeling, authentication, workouts, assessments, nutrition, memberships, notifications and governed AI integration.

## Technical highlights

- Java 21
- Spring Boot 4
- PostgreSQL + Flyway
- Redis
- Spring Security
- JWT
- REST/OpenAPI
- React + Vite
- Modular domain structure
- SSE real-time notifications
- Asynchronous application events
- Scheduled jobs
- Cache
- Metrics and health endpoints
- Governed KOVI AI integration

## Architecture

```text
React SPA
   ↓ HTTP
Spring Boot API
   ↓
Security / JWT / Method Authorization
   ↓
Controllers
   ↓
Domain Services
   ↓
Repositories
   ↓
PostgreSQL

Cross-cutting:
Redis · Events · SSE · Mail · Metrics
```

## Domain ownership

Fitness owns its facts and deterministic business rules.

KOVI AI consumes explicitly authorized context through integration contracts instead of accessing Fitness persistence directly.

## Engineering practices

- DTO boundaries instead of exposing entities
- Service/repository separation
- Server-side authorization
- Database migrations
- Consistent error responses
- Validation
- Caching
- Event-driven side effects
- Browser smoke QA

## Stack

Java 21 · Spring Boot 4 · PostgreSQL · Flyway · Redis · Spring Security · React · Vite · Docker

## Evidence

- [Original README](https://github.com/kovacsruan-stack/kovian-fitness/blob/main/README.md)
- [Architecture](https://github.com/kovacsruan-stack/kovian-fitness/blob/main/docs/ARCHITECTURE.md)
- [Security policy](https://github.com/kovacsruan-stack/kovian-fitness/blob/main/SECURITY.md)
