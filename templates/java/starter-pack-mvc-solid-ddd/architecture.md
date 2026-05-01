# Referencia arquitetural (MVC + SOLID + DDD)

- `interfaces`/`api`: controllers e contratos HTTP.
- `application`: casos de uso e coordenacao de fluxo.
- `domain`: entidades, value objects, regras e invariantes.
- `infrastructure`: banco, mensageria, clients externos.

## Anti-padroes

- regra de negocio em controller;
- service gigante sem fronteira de caso de uso;
- entidades de persistencia vazando para API.
