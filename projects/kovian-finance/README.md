# KOVIAN Finance — Personal Finance Platform

**Principal project:** https://github.com/kovacsruan-stack/kovian-finance

KOVIAN Finance is the financial domain of the KOVIAN ecosystem, covering personal finance management, planning, forecasting, reconciliation and controlled AI integration.

## Technical highlights

- Java 21
- Spring Boot 4
- Spring Data JPA
- PostgreSQL + Flyway
- Redis
- Spring Security
- OpenAPI
- Accounts
- Transactions
- Categories
- Budgets
- Goals
- Recurring transactions
- Cards
- Debts
- Assets/liabilities
- Forecasting
- CSV import/reconciliation
- Audit
- Idempotency
- Transactional outbox
- Domain integration

## Financial invariants

1. Monetary values use decimal precision.
2. External events are idempotent.
3. Sensitive mutations are auditable.
4. Authorization is enforced server-side.
5. Financial records prefer reversible lifecycle states.
6. AI insights are advisory and cannot silently mutate financial data.

## Architecture

```text
Client
  ↓
Spring Boot API
  ↓
Security / Authorization
  ↓
Finance Domain Services
  ↓
Repositories
  ↓
PostgreSQL

Supporting infrastructure:
Redis · Flyway · Outbox · Audit
```

## AI boundary

KOVI AI receives governed application-level context. It does not receive unrestricted database access and does not become the source of truth for financial records.

## Stack

Java 21 · Spring Boot 4 · Spring Data JPA · PostgreSQL · Flyway · Redis · Spring Security · OpenAPI

## Evidence

- [Original README](https://github.com/kovacsruan-stack/kovian-finance/blob/main/README.md)
- [Architecture](https://github.com/kovacsruan-stack/kovian-finance/blob/main/docs/ARCHITECTURE.md)
- [Security policy](https://github.com/kovacsruan-stack/kovian-finance/blob/main/SECURITY.md)
