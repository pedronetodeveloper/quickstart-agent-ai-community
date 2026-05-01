# Guia de Contexto para o Agente (Hexagonal)

## Sempre enviar

- objetivo da tarefa;
- porta de entrada do caso de uso;
- portas de saida envolvidas;
- adaptadores impactados;
- testes existentes.

## Por tarefa

### Nova feature
- interfaces de portas;
- implementacao do caso de uso;
- entidades/VOs afetados;
- adaptadores a criar/alterar.

### Bug
- cenario esperado x atual;
- logs/stacktrace;
- ponto de falha (porta, caso de uso ou adaptador);
- teste que reproduz.

### Refatoracao
- fronteiras atuais;
- dependencias entre camadas;
- restricoes de compatibilidade.
