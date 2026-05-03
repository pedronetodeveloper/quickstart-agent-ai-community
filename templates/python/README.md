# Python Templates Index

Este diretório centraliza o template base e **starter packs** alinhados aos padrões mais comuns de projetos Python backend: APIs em camadas, Django por apps, layout por domínio e workers com filas.

## Template base

- [`agent-instructions.md`](agent-instructions.md): persona e regras gerais para agente Python (type hints, testes, PEP 8).

## Starter packs (arquiteturas frequentes em Python)

### 1) API em camadas (FastAPI / Flask)

- Caminho: [`starter-pack-api-layered/`](starter-pack-api-layered/README.md)
- Melhor quando: APIs REST novas, rotas finas, validação na borda (Pydantic), regra em serviços ou casos de uso.

### 2) Django monólito modular (apps)

- Caminho: [`starter-pack-django-apps/`](starter-pack-django-apps/README.md)
- Melhor quando: projeto Django, fronteiras por `app`, ORM e admin no ecossistema Django.

### 3) Pacotes por domínio (feature-first / `src/`)

- Caminho: [`starter-pack-packages-by-domain/`](starter-pack-packages-by-domain/README.md)
- Melhor quando: layout `src/`, módulos por contexto de negócio, imports explícitos e evitar acoplamento entre pacotes.

### 4) Workers assíncronos e filas

- Caminho: [`starter-pack-async-workers-queues/`](starter-pack-async-workers-queues/README.md)
- Melhor quando: Celery, Dramatiq, RQ ou similar; retries, idempotência, DLQ e efeitos fora do request HTTP.

## Estrutura de cada starter pack

Cada pasta contém:

- `README.md` — contexto e quando usar
- `instructions.md` — comportamento do agente
- `architecture.md` — pastas, camadas e anti-padrões
- `skills.md` — habilidades prioritárias
- `context.md` — o que anexar ao agente por tipo de tarefa
- `prompts.md` — prompts reutilizáveis
- `checklist.md` — critérios de qualidade

## Template legado por stack

- [`../python-fastapi/agent-instructions.md`](../python-fastapi/agent-instructions.md): foco rápido só em FastAPI + Pydantic (útil como atalho).

## Guia rápido de escolha

| Situação | Pack |
|----------|------|
| API nova FastAPI/Flask | API em camadas |
| Projeto Django | Django apps |
| Monólito sem framework único definido | Pacotes por domínio |
| Tarefas em background / filas | Workers e filas |
