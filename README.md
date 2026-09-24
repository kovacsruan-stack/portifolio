# Ruan Kovacs — Portfólio de Desenvolvimento de Software

<p align="center">
  <strong>AI • Full Stack • Data • Automação • APIs • QA • Arquitetura</strong>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Java-21-informational?logo=openjdk&logoColor=white" alt="Java 21">
  <img src="https://img.shields.io/badge/Spring%20Boot-4-informational?logo=springboot&logoColor=white" alt="Spring Boot">
  <img src="https://img.shields.io/badge/TypeScript-informational?logo=typescript&logoColor=white" alt="TypeScript">
  <img src="https://img.shields.io/badge/React-informational?logo=react&logoColor=white" alt="React">
  <img src="https://img.shields.io/badge/PostgreSQL-informational?logo=postgresql&logoColor=white" alt="PostgreSQL">
  <img src="https://img.shields.io/badge/Docker-informational?logo=docker&logoColor=white" alt="Docker">
</p>

<p align="center">
  <a href="https://github.com/kovacsruan-stack">GitHub</a> •
  <a href="https://github.com/kovacsruan-stack/kovi-ai">KOVI AI</a> •
  <a href="https://github.com/kovacsruan-stack/kovian-fitness">KOVIAN Fitness</a> •
  <a href="https://github.com/kovacsruan-stack/kovian-finance">KOVIAN Finance</a>
</p>

---

## 📄 CV e perfis profissionais

- [CV oficial — Português (PDF)](./docs/CV_OFICIAL.md)
- [Perfil profissional / base do CV](./docs/RESUME_PROFILE.md)
- [LinkedIn](https://www.linkedin.com/in/kovacs-ruan)
- [GitHub](https://github.com/kovacsruan-stack)

## 📌 Evidências profissionais

| Recurso | Objetivo |
|---|---|
| [Estudos de caso](./docs/CASE_STUDIES.md) | Problema → decisão → implementação → validação |
| [Guia para recrutadores](./docs/RECRUITER_GUIDE.md) | Leitura rápida do perfil e projetos |
| [Perfil profissional](./docs/RESUME_PROFILE.md) | Base para currículo e LinkedIn |
| [Demos](./docs/DEMO_LINKS.md) | Ambientes e links públicos |
| [Roadmap](./docs/ROADMAP.md) | Próximas evoluções |

## 🧑‍💻 Perfil profissional

- [GitHub Profile README](./docs/GITHUB_PROFILE_README.md)
- [Estratégia de organização do GitHub](./docs/GITHUB_ORGANIZATION.md)

## 🧭 Navegação rápida

- [Projetos principais](#-projetos-principais)
- [Como os projetos se conectam](#-como-os-projetos-se-conectam)
- [Estudos de caso](./docs/CASE_STUDIES.md)
- [Competências](./docs/SKILLS.md)
- [Arquitetura do portfólio](./docs/ARCHITECTURE.md)
- [Segurança](./docs/SECURITY.md)
- [Status dos projetos](./docs/PROJECT_STATUS.md)
- [Roadmap](./docs/ROADMAP.md)

## 👋 Sobre mim

Sou **Ruan Kovacs**, estudante de **Análise e Desenvolvimento de Sistemas (ADS)** e desenvolvedor em formação com foco em construir software real, com arquitetura, segurança, testes, observabilidade e integração entre sistemas.

Meu objetivo profissional é atuar em ambientes onde eu possa combinar **desenvolvimento de software, inteligência artificial, dados e automação de processos** para transformar problemas reais em produtos digitais funcionais.

Este repositório é o meu **índice profissional**: reúne os projetos que melhor representam minha evolução técnica, as decisões de arquitetura e os principais conhecimentos que estou desenvolvendo.

> **Não é apenas uma coleção de códigos. É um registro de problemas, decisões, implementação, validação e evolução de produtos.**

---

## 🎯 Foco profissional

| Área | Tecnologias / competências |
|---|---|
| Backend | Java, Spring Boot, Node.js, TypeScript, REST APIs |
| Frontend | React, TypeScript, Vite, SPA, PWA |
| IA | Orquestração de modelos, RAG, memória, tool calling, agentes e integração governada |
| Dados | PostgreSQL, SQL, modelagem, persistência e análise |
| Cache / eventos | Redis, eventos, idempotência, outbox |
| Segurança | JWT, RBAC, isolamento por workspace, validação, auditoria, least privilege |
| DevOps | Docker, GitHub Actions, Railway, Vercel |
| QA | testes automatizados, lint, build, Playwright/Chromium, smoke tests e quality gates |
| Arquitetura | Clean Architecture, separação de domínios, contratos de integração e SOLID |
| Processos | documentação técnica, automação, observabilidade e melhoria contínua |

---

# 🚀 Projetos principais

## 1. KOVI AI — Intelligence & Orchestration Layer

**KOVI AI** é a camada de inteligência do ecossistema KOVIAN.

🔗 **Repositório:** https://github.com/kovacsruan-stack/kovi-ai

### O que o projeto demonstra

- Abstração multi-provider de modelos de IA
- Roteamento com fallback
- Integração com provedores compatíveis com OpenAI
- Tool calling tipado
- RBAC e limites de autorização
- Memória semântica
- RAG e versionamento de embeddings
- Idempotência
- Rate limiting
- Telemetria de providers
- Estimativa de uso e custo
- Audit logging
- API autenticada
- API keys com escopos, expiração e rotação
- Contrato OpenAPI
- Integração governada com domínios do ecossistema
- Federação segura de ferramentas
- Contexto de domínio tratado como dado não confiável
- QA local com Chromium/Playwright

### Stack

**TypeScript · Node.js · PostgreSQL/Supabase · pgvector · Vitest · Playwright · Docker**

### Principal aprendizado

O projeto explora uma arquitetura em que o modelo de IA **não recebe autoridade direta sobre dados ou ações**.

Fluxo:

**Cliente → API → Autenticação → Orquestração → Provider Router → Tools → Memória/RAG → Auditoria → Resposta**

---

## 2. KOVIAN Fitness — Fitness Management Platform

**KOVIAN Fitness** é o domínio de gestão fitness do ecossistema.

🔗 **Repositório:** https://github.com/kovacsruan-stack/kovian-fitness

### O que o projeto demonstra

- Backend Java/Spring Boot
- Arquitetura modular
- Autenticação JWT
- Autorização baseada em papéis
- PostgreSQL + Flyway
- Redis
- REST/OpenAPI
- React SPA
- Gestão de usuários
- Treinos
- Exercícios
- Planos
- Presença
- Avaliações
- Nutrição
- Progresso
- Notificações em tempo real
- SSE
- Eventos assíncronos
- Jobs agendados
- Cache
- Métricas
- Integração governada com KOVI AI

### Stack

**Java 21 · Spring Boot 4 · PostgreSQL · Flyway · Redis · Spring Security · React · Vite · Docker**

### Principal aprendizado

O projeto trabalha com uma regra arquitetural importante:

> **O domínio Fitness é o dono dos fatos. O KOVI AI é a camada de raciocínio generativo.**

Isso evita que a IA se torne uma fonte paralela de verdade ou tenha acesso irrestrito ao banco de dados.

---

## 3. KOVIAN Finance — Personal Finance Platform

**KOVIAN Finance** é a plataforma financeira do ecossistema KOVIAN.

🔗 **Repositório:** https://github.com/kovacsruan-stack/kovian-finance

### O que o projeto demonstra

- Contas
- Transações
- Categorias
- Orçamentos
- Metas
- Transações recorrentes
- Cartões
- Dívidas
- Ativos e passivos
- Forecasting
- Importação e reconciliação
- Auditoria
- Idempotência
- Regras financeiras
- Outbox transacional
- Integração com Fitness
- Integração controlada com IA

### Stack

**Java 21 · Spring Boot 4 · Spring Data JPA · PostgreSQL · Flyway · Redis · Spring Security · OpenAPI**

### Princípios financeiros

- Valores monetários usam precisão decimal
- Eventos externos são idempotentes
- Operações sensíveis são auditáveis
- Autorização acontece no servidor
- Registros financeiros privilegiam estados reversíveis
- Insights de IA são consultivos
- IA não pode executar mutações financeiras silenciosamente

---

# 🧠 Como os projetos se conectam

```
                    ┌─────────────────────┐
                    │       KOVI AI       │
                    │ Intelligence Layer  │
                    └──────────┬──────────┘
                               │
                Governed contracts / tools
                               │
              ┌────────────────┴────────────────┐
              │                                 │
      ┌───────▼────────┐               ┌────────▼────────┐
      │ KOVIAN Fitness │               │ KOVIAN Finance  │
      │ Domain Owner   │               │ Domain Owner    │
      └───────┬────────┘               └────────┬────────┘
              │                                 │
        PostgreSQL + Redis                PostgreSQL + Redis
```

### Regra central

**Domínios possuem os dados e regras de negócio. KOVI AI possui a orquestração generativa.**

Essa separação permite evoluir cada produto de forma independente e reduz acoplamento entre inteligência artificial e persistência de domínio.

---

# 🏗️ O que este portfólio demonstra tecnicamente

### Engenharia de software

- modelagem de domínio
- APIs
- autenticação
- autorização
- persistência
- migrations
- cache
- eventos
- contratos
- tratamento de erros
- observabilidade
- testes
- documentação

### Desenvolvimento Full Stack

A experiência percorre:

**React → API REST → Services → Repositories → PostgreSQL/Redis**

com autenticação e regras de negócio no backend.

### Inteligência Artificial aplicada

O KOVI AI explora:

- seleção de providers
- fallback
- custo
- rate limiting
- memória
- RAG
- ferramentas
- autorização
- auditoria
- integração entre domínios

### Segurança

- JWT
- RBAC
- workspace isolation
- scopes
- API keys
- secrets server-side
- validação
- confirmação para operações sensíveis
- audit logs
- least privilege
- fail-closed boundaries

### Qualidade

- testes unitários
- testes de integração
- lint
- build
- smoke tests
- Playwright/Chromium
- validação responsiva
- health checks
- observabilidade
- quality gates

---

# 📚 Estrutura deste portfólio

```
portifolio/
├── README.md
├── projects/
│   ├── kovi-ai/
│   │   └── README.md
│   ├── kovian-fitness/
│   │   └── README.md
│   └── kovian-finance/
│       └── README.md
├── docs/
│   ├── ARCHITECTURE.md
│   ├── SKILLS.md
│   ├── SECURITY.md
│   └── PROJECT_STATUS.md
└── .gitignore
```

Os repositórios originais continuam sendo a **fonte do código**. Este repositório funciona como uma camada profissional de apresentação, documentação e navegação.

---

# 📈 Evolução técnica

**Fundamentos → Programação → APIs e Backend → Banco de Dados → Frontend → Integrações → Testes e QA → Segurança → Arquitetura → IA aplicada → Observabilidade → Produtos completos**

O objetivo não é apenas aprender uma tecnologia isoladamente, mas aprender a **entregar sistemas completos**.

---

# 💼 Para recrutadores

Se você chegou aqui procurando entender rapidamente meu perfil:

### Estou desenvolvendo experiência prática em

**Backend:** Java, Spring Boot, Node.js, TypeScript, REST APIs

**Frontend:** React, TypeScript, Vite, PWA

**Dados:** PostgreSQL, SQL, pgvector, JPA, Flyway, Redis

**IA:** LLM orchestration, RAG, embeddings, tool calling, provider routing e AI security boundaries

**Qualidade:** JUnit/Vitest, Playwright, lint, CI, smoke testing e quality gates

**Infraestrutura:** Docker, Git, GitHub Actions, Railway e Vercel

---

# 🧪 Status dos projetos

> O status abaixo descreve o estágio de engenharia do portfólio, não significa que todos os ambientes de produção estejam permanentemente disponíveis.

| Projeto | Papel | Backend | Frontend | IA | QA | Infra |
|---|---|---:|---:|---:|---:|---:|
| KOVI AI | Intelligence / orchestration | ✅ | ✅ | ✅ | ✅ | 🟡 |
| KOVIAN Fitness | Fitness domain | ✅ | ✅ | 🔗 | ✅ | 🟡 |
| KOVIAN Finance | Finance domain | ✅ | 🚧 | 🔗 | 🟡 | 🟡 |

Legenda: **✅ implementado / 🟡 em evolução / 🚧 em desenvolvimento / 🔗 integração**

---

# 🛡️ Segurança

Este repositório não deve conter:

- senhas
- API keys
- tokens
- arquivos .env reais
- chaves privadas
- certificados privados
- dumps de bancos
- dados reais de usuários
- credenciais de infraestrutura
- logs com dados sensíveis

Arquivos de configuração pública devem utilizar placeholders e exemplos seguros.

---

# 🗺️ Próximos passos

1. Consolidar os três projetos principais
2. Melhorar documentação e demonstrações
3. Fortalecer testes automatizados
4. Expandir QA de navegador
5. Melhorar observabilidade
6. Finalizar integrações entre os domínios
7. Criar projetos menores focados em dados e automação
8. Publicar estudos técnicos e decisões arquiteturais
9. Organizar projetos acadêmicos de ADS
10. Transformar os projetos em evidências profissionais para processos seletivos

---

# 📌 Outros projetos que entrarão aqui

Além dos três produtos principais:

- projetos acadêmicos de ADS
- análise de dados
- SQL
- Python
- automações
- APIs pequenas
- experimentos de IA
- scripts de produtividade
- projetos de QA
- estudos de arquitetura
- pequenos projetos de frontend

Projetos experimentais podem continuar em repositórios separados para preservar a clareza deste portfólio.

---

# 🤝 Contato

**GitHub:** https://github.com/kovacsruan-stack

**LinkedIn:** https://www.linkedin.com/in/kovacs-ruan

**CV oficial:** [PDF](./docs/CV_OFICIAL.md)

**Portfólio:** https://github.com/kovacsruan-stack/portifolio

**Perfil profissional:** [docs/RESUME_PROFILE.md](./docs/RESUME_PROFILE.md)

Aberto a oportunidades de **estágio e posições júnior**, especialmente em:

- Desenvolvimento Backend
- Full Stack
- IA aplicada
- Data / Analytics
- Automação
- QA / Engenharia de Software

---

<p align="center">
  <strong>Construindo software real enquanto evoluo como desenvolvedor.</strong>
</p>
