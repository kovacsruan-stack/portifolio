# Public Portfolio Security

This repository is intentionally public and is designed to showcase engineering work.

## Never publish

- passwords
- API keys
- access tokens
- JWT private keys
- private certificates
- production .env files
- database credentials
- infrastructure credentials
- production database dumps
- real customer, student or financial data
- logs containing sensitive information

## Safe to publish

- source code
- architecture diagrams
- tests
- documentation
- sanitized examples
- .env.example files containing placeholders
- public API contracts
- technical decisions
- local development instructions

## Rule of thumb

If an artifact explains **how the system works**, it can usually be part of the portfolio.

If an artifact provides **access to a system or exposes private data**, it should remain private.

The original projects maintain their own security policies. This document defines the publication standard for this portfolio.
