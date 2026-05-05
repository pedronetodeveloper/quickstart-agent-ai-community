# Starter Pack JavaScript Node — Async Workers e Filas

Pack para processar jobs assíncronos e integração com filas/worker systems como BullMQ, RabbitMQ, Redis Queue, Agenda ou similares.

## Quando usar

- Processamento em background de jobs, e-mails, notificações, integrações ou importações.
- Requer retries, idempotência e dead-letter queue.
- Worker separado da resposta HTTP principal.

## O que não é

- Não é request-response síncrono clássico.
- Não é fluxo com lógica de negócio diretamente em filas sem camada de orquestração.
