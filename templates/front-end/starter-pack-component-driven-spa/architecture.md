# Arquitetura — SPA Component-Driven

- `components/`: componentes reutilizáveis.
- `features/`: módulos por domínio/feature.
- `pages/`: páginas com roteamento.
- `store/`: estado global e local.

## Princípios

- Componentes independentes e reutilizáveis.
- Feature modules isolados com suas dependências.
- Lazy loading para otimização de bundles.

## Anti-padrões

- Componentes gigantes sem reutilização.
- Estado espalhado sem controle.
- Roteamento sem code splitting.