# Starter Pack Python — Workers assíncronos e filas

Pack para o padrão **muito frequente** em Python: trabalho fora do request HTTP usando **Celery**, **Dramatiq**, **RQ** ou filas similares, com retries, idempotência e tratamento de falhas.

## Quando usar

- Envio de e-mail, geração de relatórios, webhooks downstream, indexação.
- Picos de carga que não podem bloquear a API.
- Integração com Redis, RabbitMQ, SQS, Kafka consumers em processo worker.

## O que não é

- Não prescreve um broker único; os princípios valem para qualquer fila que o projeto use.
