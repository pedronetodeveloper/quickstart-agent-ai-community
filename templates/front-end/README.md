# Front-end Templates Index

Este diretório centraliza o template base e **starter packs** alinhados às arquiteturas mais comuns de front-end: microfrontends, SPA component-driven, design systems e Jamstack/SSR/SSG.

## Template base

- [`agent-instructions.md`](agent-instructions.md): persona e regras gerais para agente Front-end (component-driven, performance, UX, acessibilidade, modularidade).

## Starter packs (arquiteturas frequentes em front-end)

### 1) Microfrontends
- Caminho: [`starter-pack-microfrontends/README.md`](starter-pack-microfrontends/README.md)
- Melhor quando: múltiplos times entregam front-end independentemente, integração gradual, orquestração de shell e federated modules.

### 2) SPA Component-Driven
- Caminho: [`starter-pack-component-driven-spa/README.md`](starter-pack-component-driven-spa/README.md)
- Melhor quando: aplicação SPA moderna com componentes reutilizáveis, feature modules, roteamento e estado local/global.

### 3) Design System
- Caminho: [`starter-pack-design-system/README.md`](starter-pack-design-system/README.md)
- Melhor quando: consistência visual e UI compartilhada entre múltiplas aplicações, biblioteca de componentes e tokens.

### 4) Jamstack/SSR/SSG
- Caminho: [`starter-pack-jamstack-ssr-ssg/README.md`](starter-pack-jamstack-ssr-ssg/README.md)
- Melhor quando: sites de marketing, e-commerces, docs; alto desempenho, SEO, cache e pré-renderização.

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

- [`agent-instructions.md`](agent-instructions.md): atalho rápido para agentes front-end que precisam do comportamento base sem starter pack específico.

## Guia rápido de escolha

| Situação | Pack |
|----------|------|
| Múltiplos times front-end | Microfrontends |
| SPA moderna com componentes | Component-Driven SPA |
| Consistência UI compartilhada | Design System |
| Performance e SEO | Jamstack/SSR/SSG |