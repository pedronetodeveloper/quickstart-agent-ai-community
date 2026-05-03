# Skills prioritárias — Workers e filas

1. Modelar tasks idempotentes com chaves de deduplicação quando necessário.
2. Configurar retries, jitter exponencial e DLQ alinhados ao tipo de falha.
3. Serializar payloads seguros (JSON) e tamanho controlado.
4. Integrar observabilidade: structlog, OpenTelemetry ou correlation id propagado.
5. Testar tasks isoladamente com broker mock ou modo eager.
6. Dimensionar prefetch e concorrência para não saturar DB ou API externa.
7. Implementar outbox quando a operação precisar ser atômica com commit em DB.
8. Documentar semântica de entrega (at-least-once) para o time.
