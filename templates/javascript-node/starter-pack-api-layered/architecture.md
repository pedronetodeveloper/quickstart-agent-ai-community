# Arquitetura — API em camadas

- `routes/` ou `controllers/`: apenas roteamento e delegação.
- `services/` ou `use-cases/`: regra de negócio e orquestração.
- `repositories/`, `infra/` ou `adapters/`: acesso a banco, cache, filas e APIs externas.
- `schemas/` ou `validators/`: validação de entrada/saída com Zod.

## Princípios

- Mantenha os handlers pequenos e focados.
- Evite acoplamento direto entre `controllers` e `models` de persistência.
- Use injeção de dependência leve via closures ou factories.

## Anti-padrões

- Lógica de negócio dentro de rotas.
- Modelos de banco expostos diretamente em responses.
- Funções `async` não aguardadas ou promessas não tratadas.
