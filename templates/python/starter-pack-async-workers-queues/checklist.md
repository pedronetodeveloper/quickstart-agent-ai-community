# Checklist — Workers e filas

- [ ] Task idempotente ou com deduplicação explícita?
- [ ] Payload serializável e sem dados sensíveis em claro?
- [ ] Timeout e retry definidos para falhas transitórias?
- [ ] Falha de negócio não entra em retry infinito?
- [ ] DLQ ou alerta para falhas permanentes?
- [ ] Logs com correlation id ou task id rastreável?
- [ ] Testes da task (unitário + integração com broker de teste se possível)?
- [ ] Semântica de entrega documentada (ex.: at-least-once)?
