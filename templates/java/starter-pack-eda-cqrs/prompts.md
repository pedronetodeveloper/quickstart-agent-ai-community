# Prompt Pack (EDA + CQRS)

## Nova feature

```text
Implemente "<NOME_FEATURE>" com EDA + CQRS.
1) crie comando e command handler;
2) aplique regra no write side;
3) publique evento versionado com confiabilidade;
4) atualize read side por consumidor idempotente;
5) exponha query otimizada;
6) adicione testes de contrato e fluxo assincrono.
```

## Review arquitetural

```text
Revise este fluxo com foco em EDA + CQRS:
- separacao write/read;
- publicacao confiavel de eventos;
- idempotencia de consumidores;
- versionamento de contrato;
- retry/DLQ.
```

## Refatoracao

```text
Refatore fluxo sincrono para EDA + CQRS mantendo compatibilidade externa e adicionando plano de migracao gradual.
```
