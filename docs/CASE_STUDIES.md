# Engineering Case Studies

Este documento transforma os projetos do portfólio em evidências objetivas de engenharia.

## 1. KOVI AI — IA com fronteiras de segurança

### Problema
Uma aplicação com LLM precisa integrar providers, memória, ferramentas e dados de domínio sem transformar o modelo em autoridade sobre o sistema.

### Decisões
- Separar autenticação/autorização da camada generativa.
- Encapsular providers atrás de um router com fallback.
- Expor tools por contratos tipados e escopos.
- Tratar contexto retornado por domínios como dado não confiável.
- Registrar operações relevantes para auditoria.
- Aplicar idempotência e rate limiting antes de operações sensíveis.

### Resultado técnico
A arquitetura permite trocar providers e evoluir ferramentas sem conceder ao modelo acesso direto ao banco ou às regras de negócio.

### O que demonstra
**TypeScript, APIs, LLM orchestration, RAG, tool calling, segurança, observabilidade e arquitetura.**

---

## 2. KOVIAN Fitness — domínio separado da inteligência

### Problema
Uma plataforma fitness precisa manter dados e regras de negócio consistentes enquanto oferece recursos de IA.

### Decisões
- Fitness permanece como dono dos fatos do domínio.
- KOVI AI acessa somente contratos autorizados.
- PostgreSQL mantém persistência transacional.
- Redis apoia cache e infraestrutura de execução.
- Eventos e SSE desacoplam atualizações de algumas experiências do frontend.
- Segurança fica no servidor.

### Resultado técnico
A IA pode explicar, consultar e apoiar decisões sem substituir a fonte de verdade do domínio.

### O que demonstra
**Java, Spring Boot, PostgreSQL, Redis, React, REST, JWT, RBAC, eventos, SSE e testes.**

---

## 3. KOVIAN Finance — integridade antes de inteligência

### Problema
Sistemas financeiros exigem precisão, rastreabilidade e operações previsíveis.

### Decisões
- Valores monetários com precisão decimal.
- Idempotência para entradas externas.
- Auditoria de operações relevantes.
- Estados reversíveis quando apropriado.
- Outbox para publicação confiável de eventos.
- IA limitada a insights e apoio, sem mutações financeiras silenciosas.

### Resultado técnico
A arquitetura prioriza consistência e rastreabilidade antes de adicionar automação generativa.

### O que demonstra
**Java, Spring Boot, JPA, PostgreSQL, Flyway, Redis, modelagem de domínio, idempotência, outbox e auditoria.**

---

## Como avaliar estes projetos

Ao revisar o portfólio, vale observar quatro camadas:

1. **Problema** — qual necessidade o sistema resolve?
2. **Decisão** — por que a arquitetura foi escolhida?
3. **Implementação** — quais tecnologias e contratos foram usados?
4. **Validação** — como testes, QA, observabilidade e segurança reduzem risco?

O objetivo deste documento é mostrar raciocínio de engenharia, não apenas uma lista de tecnologias.
