# Starter Pack Python — Pacotes por domínio (`src/` / feature-first)

Pack para o layout **muito comum** em bibliotecas e serviços Python modernos: pacotes por contexto de negócio ou feature, frequentemente sob **`src/`**, com imports explícitos e dependências controladas.

## Quando usar

- Monólito sem framework único, ou CLI + lib + API no mesmo repo.
- Time quer evitar “pasta única de scripts” e imports implícitos.
- Necessidade de testar pacotes isoladamente e publicar um pacote com `pyproject.toml`.

## O que não é

- Não exige DDD formal; é organização física e de dependências alinhada ao ecossistema Python.
