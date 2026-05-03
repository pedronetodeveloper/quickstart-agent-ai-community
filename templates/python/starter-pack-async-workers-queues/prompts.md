# Prompt pack — Workers e filas

## Nova task assíncrona

```text
Implemente uma task <NOME> para <Ferramenta> que <OBJETIVO>. Payload mínimo, idempotência documentada, retry com backoff e tratamento para falha permanente (DLQ ou equivalente). Reuse serviço em `services/` se existir.
```

## Revisão de resiliência

```text
Revise esta implementação de worker/fila. Avalie idempotência, retries, timeouts, vazamento de payload grande, observabilidade e risco de duplicação at-least-once.
```

## Debugging de mensagem duplicada

```text
Mensagens estão sendo processadas duas vezes. Com broker <X> e ack/retry atuais, explique causas prováveis e mitigação (idempotency key, outbox, dedup store).
```
