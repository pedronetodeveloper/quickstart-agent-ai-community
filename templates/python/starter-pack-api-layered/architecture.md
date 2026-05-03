# Referência arquitetural — API em camadas

## Estrutura sugerida (exemplo com `src/`)

```text
src/
  myapp/
    api/                 # routers, deps FastAPI ou blueprints Flask
      routes/
      schemas/           # Pydantic ou equivalente
    services/            # ou use_cases/
    domain/              # entidades puras opcionais
    infra/
      db/
      repositories/
    main.py              # ou app factory
tests/
  api/
  services/
```

## Responsabilidades

| Camada | Papel |
|--------|--------|
| `api` | HTTP, validação de borda, autenticação declarada |
| `services` / `use_cases` | Regra, transação lógica, chamadas a repositórios |
| `infra` | ORM, drivers, clients externos |

## Anti-padrões

- Lógica de negócio de dezenas de linhas dentro da rota.
- Import circular entre `api` e `infra` sem camada intermediária.
- Retornar modelo ORM direto sem DTO quando o contrato público importa.
- `global` ou estado mutável compartilhado entre requests sem necessidade.

## Notas FastAPI

- `Depends()` para serviços e sessões; evitar singletons mutáveis.
- Lifespan para startup/shutdown de pools.

## Notas Flask

- Blueprints por domínio; `before_request` com moderação.
- Mesma ideia: view fina, serviço grosso no sentido de responsabilidade, não de tamanho.
