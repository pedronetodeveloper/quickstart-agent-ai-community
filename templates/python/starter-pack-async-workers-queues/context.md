# Guia de contexto — Workers e filas

## Sempre enviar

- Ferramenta (Celery / Dramatiq / RQ / outro) e versão.
- Definição da task e fila/rota usada.
- Payload de exemplo (sem segredos).
- Configuração relevante de broker e retry do ambiente.

## Por tipo de tarefa

### Nova task

- Código que enfileira e código do worker.
- Serviço de domínio compartilhado, se existir.
- Modelo de dados afetado e transações.

### Bug em produção

- Log do worker com timestamp e correlation id.
- Mensagem reprocessada ou duplicada? Quantas vezes?
- Política atual de ack e retry.

### Performance

- Tamanho médio de fila, tempo de processamento por mensagem.
- Gargalo (DB, API externa, CPU).

## Evite

- Descrever bug sem dizer se a mensagem foi redelivered.
- Omitir broker e versão da lib de fila.
