# Referencia arquitetural (Modular Monolith)

- `modules/<modulo>/api`: contratos internos.
- `modules/<modulo>/application`: casos de uso.
- `modules/<modulo>/domain`: regras de negocio.
- `modules/<modulo>/infrastructure`: detalhes tecnicos.

## Regras

- Sem acesso direto a internals de outro modulo.
- Integracao por API de modulo ou eventos internos.
- Sem ciclos de dependencia entre modulos.
