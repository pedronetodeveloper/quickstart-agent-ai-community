# Guia de contexto — Pacotes por domínio

## Sempre enviar

- `pyproject.toml` (ou `setup.cfg` legado).
- Árvore do pacote sob `src/` ou raiz com `__init__.py`.
- Arquivo que está na raiz do conflito de import.
- Teste que quebra com `ImportError` ou ciclo.

## Por tipo de tarefa

### Novo domínio

- Lista de módulos que vão consumir o novo pacote.
- Nome desejado na API pública (`myproduct.billing`).

### Refatoração de imports

- Traceback de import circular completo.
- Grafo informal (quem importa quem) se souber.

### Lib publicável

- Versão atual e política de semver do time.
- O que é API pública garantida vs interno (`_` prefix).

## Evite

- Pedir “reorganizar o repo” sem um domínio ou feature concreta.
- Misturar código de aplicação e exemplos sem pasta `examples/`.
