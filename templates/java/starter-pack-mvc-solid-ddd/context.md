# Guia de Contexto para o Agente (MVC + SOLID + DDD)

## Sempre enviar

- objetivo da tarefa;
- classes de API (entrada/saida);
- caso de uso e classes de dominio relacionadas;
- persistencia e testes envolvidos.

## Por tarefa

### Nova feature
- endpoint atual/semelhante;
- caso de uso alvo;
- entidades/VOs impactados;
- contratos de repositorio.

### Bug
- stacktrace;
- fluxo completo (controller -> aplicacao -> dominio -> infra);
- teste que falha (ou cenario reproduzivel).

### Refatoracao
- pacote completo da feature;
- convencoes atuais do projeto;
- restricoes de compatibilidade.
