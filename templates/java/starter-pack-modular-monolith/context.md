# Guia de Contexto para o Agente (Modular Monolith)

## Sempre enviar

- modulo alvo;
- objetivo da tarefa;
- API do modulo;
- classes de dominio/aplicacao/infra impactadas;
- testes existentes.

## Por tarefa

### Nova feature
- contrato da API interna do modulo;
- pontos de integracao com outros modulos;
- endpoints externos afetados.

### Bug
- stacktrace;
- caminho entre modulos;
- teste que falha.

### Refatoracao
- dependencias atuais entre modulos;
- regra de ownership por modulo;
- restricoes de backward compatibility.
