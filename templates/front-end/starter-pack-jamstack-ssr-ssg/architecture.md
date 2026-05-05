# Arquitetura — Jamstack/SSR/SSG

- `pages/`: páginas com pré-renderização.
- `components/`: componentes hidrativos.
- `api/`: endpoints serverless para dados.
- `content/`: CMS ou arquivos markdown.

## Princípios

- Build-time rendering para performance.
- Runtime hidratação para interatividade.
- Cache em edge para latência baixa.

## Anti-padrões

- Renderização client-side excessiva.
- Falta de cache ou otimização.
- Conteúdo dinâmico sem necessidade.