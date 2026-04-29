# Skills dos Agentes Copilot

As Skills representam as capacidades técnicas que os agentes dominam. Este guia explica como desenvolver e utilizar skills efetivamente.

## O que são Skills?

Skills são conhecimentos específicos que permitem ao agente executar tarefas complexas, como:
- Gerar testes automatizados
- Refatorar código para melhores práticas
- Validar dados com bibliotecas específicas

## Desenvolvendo Skills

1. **Identifique Necessidades**: Analise seu projeto e tecnologias usadas
2. **Defina Exemplos**: Forneça prompts com exemplos de entrada/saída
3. **Incorpore em Instructions**: Adicione skills relevantes ao arquivo `.instructions.md`

## Skills por Tecnologia

| Tecnologia | Skills Comuns | Exemplo |
|------------|---------------|---------|
| Java Spring | Mappers entidade-DTO, JUnit 5 | Gerar testes para controllers |
| Node.js | Async/await, Zod validation | Validar schemas de API |
| FastAPI | Type hints, Pydantic | Criar endpoints com validação |
| Angular | Signals, RXJS | Refatorar para componentes standalone |

## Melhores Práticas

- Seja específico: Descreva o que o agente deve fazer, não como
- Teste iterativamente: Refine skills com base em resultados
- Compartilhe: Contribua skills para a comunidade

Para exemplos práticos, veja [Exemplos](../guides/examples.md).