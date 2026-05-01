# Referencia arquitetural (Hexagonal)

- `domain`: entidades, value objects, servicos de dominio, portas (in/out).
- `application`: implementacao de casos de uso (porta de entrada).
- `adapters/in`: REST, CLI, consumers.
- `adapters/out`: persistencia, clients externos, publishers.

## Regras

- Dominio nao depende de adaptadores.
- Aplicacao depende de dominio.
- Adaptadores implementam portas de saida.

## Anti-padroes

- dominio com `@Entity`, `@Service`, `@Component`;
- controller chamando repositorio de infra direto;
- porta generica sem linguagem de negocio.
