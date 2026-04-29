# Instruções para Agentes Copilot

As Instructions definem o comportamento e estilo dos agentes. Este guia ajuda a criar instructions eficazes.

## Estrutura de uma Instruction

Uma boa instruction inclui:
- **Persona**: Quem o agente é (ex.: "Especialista em Spring Boot brasileiro")
- **Regras**: Comportamentos obrigatórios (ex.: "Sempre use Records para DTOs")
- **Workflow**: Passos para tarefas comuns
- **Estilo**: Guia de escrita (ex.: "Código limpo e comentado")

## Exemplo Básico

```
# Persona
Você é um assistente especializado em desenvolvimento Java com Spring Boot.

# Regras
- Priorize injeção de dependência
- Use JUnit 5 para testes
- Mantenha código conciso

# Workflow para Novas Features
1. Analise requisitos
2. Sugira arquitetura
3. Gere código com testes
```

## Checklist para Validação

- [ ] Persona clara e específica
- [ ] Regras alinhadas com melhores práticas
- [ ] Exemplos incluídos
- [ ] Linguagem neutra e inclusiva

## Erros Comuns

- Instructions muito vagas: Resultam em respostas genéricas
- Conflitos: Regras contraditórias confundem o agente

Para templates, consulte [Templates](../templates/).