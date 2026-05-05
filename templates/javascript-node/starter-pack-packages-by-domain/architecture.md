# Arquitetura — Pacotes por domínio

- `src/<domain>/`: cada domínio tem sua própria pasta com `controllers`, `services`, `repositories`/`adapters`.
- `src/shared/` ou `src/common/`: utilitários compartilhados e tipos genéricos.
- `package.json`/`tsconfig.json`: configure paths e aliases para `src/`.

## Princípios

- Cada pacote expõe API pública mínima.
- Evite `../../..` complexos usando imports absolutos ou aliases.
- Mantenha domínio centralizado e desacoplado.

## Anti-padrões

- Dependências circulares entre pacotes.
- Pacotes que importam diretamente `infra/` ou `api/` de outros domínios.
- Lógica de infraestrutura em domínios de negócio.
