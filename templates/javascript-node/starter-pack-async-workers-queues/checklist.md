# Checklist — Async Workers e Filas

- [ ] Payload do job é validado e documentado.
- [ ] Job é idempotente ou tratado para duplicação.
- [ ] Retries e dead-letter queue estão configurados.
- [ ] Lógica de negócio está separada do worker/handler.
- [ ] Integrações externas estão isoladas em adaptadores.
- [ ] Testes cobrem comportamento de job e falhas comuns.
