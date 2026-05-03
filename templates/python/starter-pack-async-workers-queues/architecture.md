# Referência arquitetural — Workers e filas

## Estrutura sugerida

```text
src/
  myapp/
    api/                 # produz mensagens / enfileira jobs
    workers/
      tasks.py           # Celery/RQ entrypoints finos
      consumers.py       # ou handlers Dramatiq
    services/            # regra compartilhada com API
    infra/
      queue.py           # factory de conexão, settings
```

## Fluxo típico

1. Request valida e enfileira job com payload mínimo.
2. Worker recebe mensagem, deduplica se necessário.
3. Worker chama serviço de domínio; persiste e publica efeitos colaterais.
4. Falha transitória → retry; falha permanente → DLQ ou alerta.

## Padrões úteis

- **Outbox** (tabela + publicador) quando precisar consistência entre DB e fila.
- **Chunking** para jobs longos; heartbeat ou subdivisão.
- **Rate limit** no consumer quando API externa for gargalo.

## Anti-padrões

- Passar instância de modelo Django/SQLAlchemy session pela fila.
- Retry infinito em erro de validação de negócio.
- Task de 3000 linhas sem extração para serviço.
- Log sem correlation id em sistema com múltiplos workers.

## Notas por ferramenta

- **Celery**: `acks_late`, `task_reject_on_worker_lost` — entender trade-offs.
- **Dramatiq**: middleware para retries e métricas.
- **RQ**: simplicidade; combinar com Redis Sentinel/HA se for produção séria.
