# Referência arquitetural — Pacotes por domínio

## Estrutura sugerida (`src/`)

```text
pyproject.toml
src/
  myproduct/
    __init__.py          # API pública mínima
    billing/
      __init__.py
      service.py
      models.py          # se for domínio + persistência no mesmo pacote, documente
    inventory/
      ...
    shared/              # tipos, exceções base, constantes — manter pequeno
tests/
  billing/
  inventory/
```

## Regras de dependência

- `billing` não importa detalhes internos profundos de `inventory`; só contratos (`protocols`, tipos) ou `shared`.
- `shared` não deve virar lixeira de negócio; só o realmente transversal.

## Ferramentas comuns

- Pacote instalável em modo editável: `pip install -e .`
- Namespace packages (PEP 420) apenas se o time souber o trade-off.

## Anti-padrões

- `from myproduct.billing.* import *` escondendo dependências.
- Pasta `helpers.py` ou `utils.py` sem dono de negócio crescendo sem limite.
- Testes que manipulam `sys.path` em vez de instalar o pacote corretamente.
- Dois pacotes com nomes quase idênticos (`order` vs `orders`) sem convenção.
