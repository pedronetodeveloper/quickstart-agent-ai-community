# Checklist de Qualidade (EDA + CQRS)

- Command side e query side estao separados?
- Evento possui contrato versionado e metadados?
- Publicacao de evento e confiavel?
- Consumidores sao idempotentes?
- Retry, timeout e DLQ definidos?
- Read model atende consultas sem depender do write model?
- Correlation id permite rastreio ponta a ponta?
- Testes de contrato e fluxo assincrono criados?
