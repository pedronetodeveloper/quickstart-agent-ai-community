# Arquitetura — Async Workers e Filas

- `workers/` ou `jobs/`: definições e processadores de job.
- `queues/`: criação e configuração das filas.
- `adapters/` ou `infra/`: integração com Redis, RabbitMQ, etc.
- `services/` ou `domain/`: lógica de negócio reutilizável.

## Princípios

- Separe recepção de evento, validação e execução.
- Cada job deve ter payload explícito e schema.
- Use mecanismo de retries e DLQ para falhas.

## Anti-padrões

- Jobs que fazem várias tarefas sem isolamento.
- Falta de idempotência em jobs repetíveis.
- Lógica de negócio embutida diretamente no worker setup.
