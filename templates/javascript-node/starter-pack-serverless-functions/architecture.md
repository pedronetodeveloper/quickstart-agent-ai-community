# Arquitetura — Serverless Functions

- `functions/`, `api/` ou `routes/` contém entrypoints leves.
- Lógica de negócio em `lib/`, `services/` ou `domain/` compartilháveis.
- Configurações de deploy e adaptadores de runtime isolados.

## Princípios

- Minimizar dependências carregadas por função.
- Evitar estado local entre execuções.
- Usar caching externo (Redis, CDN) quando necessário.

## Anti-padrões

- Funções com longas inicializações síncronas.
- Uso de variáveis globais mutáveis para estado.
- Lógica de negócio densa dentro de handlers.
