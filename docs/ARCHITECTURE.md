# Portfolio Architecture

The portfolio is a presentation layer over the original software projects.

## Source of truth

The original repositories remain authoritative:

- https://github.com/kovacsruan-stack/kovi-ai
- https://github.com/kovacsruan-stack/kovian-fitness
- https://github.com/kovacsruan-stack/kovian-finance

This repository should not become a second copy of their complete source code.

## Structure

```text
portifolio
├── README.md
├── projects/
│   ├── kovi-ai/
│   ├── kovian-fitness/
│   └── kovian-finance/
└── docs/
    ├── ARCHITECTURE.md
    ├── SKILLS.md
    ├── SECURITY.md
    └── PROJECT_STATUS.md
```

## Why this architecture?

A recruiter should understand the portfolio quickly without navigating three large codebases first.

The project pages provide:

- problem/context
- responsibilities
- architecture
- technology
- engineering practices
- direct source links

The original repositories provide the complete implementation and commit history.

## Maintenance rule

When a major technical capability changes in an original project, update the corresponding portfolio page rather than duplicating source files.
