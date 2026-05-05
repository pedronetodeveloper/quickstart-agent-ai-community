# JavaScript Node Templates Index

Este diretório centraliza o template base e **starter packs** alinhados às arquiteturas mais comuns de backend Node.js: APIs em camadas, pacotes por domínio, serverless e workers/queues.

## Template base

- [`agent-instructions.md`](agent-instructions.md): persona e regras gerais para agente Node.js (ESM, async/await, Zod).

## Starter packs (arquiteturas frequentes em Node.js)

### 1) API em camadas
- Caminho: [`starter-pack-api-layered/README.md`](starter-pack-api-layered/README.md)
- Melhor quando: APIs REST ou HTTP, rotas finas, separação entre handlers, serviços e persistência.

### 2) Pacotes por domínio
- Caminho: [`starter-pack-packages-by-domain/README.md`](starter-pack-packages-by-domain/README.md)
- Melhor quando: projeto maior ou monolito bem modularizado, com `src/` e pacotes orientados a contexto.

### 3) Serverless functions
- Caminho: [`starter-pack-serverless-functions/README.md`](starter-pack-serverless-functions/README.md)
- Melhor quando: APIs ou backends em nuvem que usam Vercel/Lambda/Netlify/FaaS.

### 4) Async workers e filas
- Caminho: [`starter-pack-async-workers-queues/README.md`](starter-pack-async-workers-queues/README.md)
- Melhor quando: processamento assíncrono, jobs, tarefas em background e integração com filas.

## Estrutura de cada starter pack

Cada pasta contém:

- `README.md` — contexto e quando usar
- `instructions.md` — comportamento do agente
- `architecture.md` — pastas, camadas e anti-padrões
- `skills.md` — habilidades prioritárias
- `context.md` — o que anexar ao agente por tipo de tarefa
- `prompts.md` — prompts reutilizáveis
- `checklist.md` — critérios de qualidade

## Template rápido

- [`agent-instructions.md`](agent-instructions.md): atalho rápido para agentes Node.js que precisam do comportamento base sem starter pack específico.

## Guia rápido de escolha

| Situação | Pack |
|----------|------|
| API REST nova ou em evolução | API em camadas |
| Projeto maior com domínio dividido | Pacotes por domínio |
| Deploy serverless / funções na nuvem | Serverless functions |
| Jobs, workers, processamento assíncrono | Async workers e filas |