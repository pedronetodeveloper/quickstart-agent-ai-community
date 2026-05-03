# Prompt pack — Pacotes por domínio

## Novo pacote de domínio

```text
Crie o pacote `<nome>` sob `src/<produto>/` com API pública mínima em `__init__.py`, serviço principal e testes em `tests/<nome>/`. Respeite o pyproject.toml existente.
```

## Resolver import circular

```text
Temos import circular entre <pacote_a> e <pacote_b>. Analise o traceback, proponha extração mínima (shared ou Protocol) e mostre o diff conceitual de imports.
```

## Revisão de fronteiras

```text
Revise a árvore de pacotes deste repositório. Liste acoplamentos indevidos entre domínios e sugestões de fronteira clara sem microservices.
```
