# Guia de Contexto para o Agente (EDA + CQRS)

## Sempre enviar

- comando ou query alvo;
- contrato dos eventos envolvidos;
- componentes produtores/consumidores;
- read model/projecoes;
- testes do fluxo assincrono.

## Por tarefa

### Nova feature
- command handler;
- schema/version de evento;
- consumidores impactados;
- API de consulta impactada.

### Bug
- payload de evento (anonimizado);
- logs com correlation id;
- estado de retries/DLQ;
- cenario de reproducao temporal.

### Evolucao de contrato
- versao atual e nova;
- mapa de produtores/consumidores;
- estrategia de compatibilidade.
