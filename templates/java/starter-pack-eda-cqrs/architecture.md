# Referencia arquitetural (EDA + CQRS)

- `command`: comandos, regras de escrita e persistencia do estado.
- `eventing`: publicacao/consumo de eventos.
- `query`: projecoes e consultas otimizadas.

## Regras

- comando altera estado e publica evento confiavel;
- consumidor atualiza read model com idempotencia;
- query nunca depende diretamente do modelo de escrita.

## Anti-padroes

- publicar evento antes de persistir comando;
- usar o mesmo modelo para tudo sem necessidade;
- ignorar versionamento e observabilidade de eventos.
