# Guia de Troubleshooting

Problemas comuns com agentes Copilot e suas soluções.

## Agente Não Responde

**Sintomas**: Prompts ignorados ou respostas genéricas.

**Soluções**:
1. Verifique se `.instructions.md` existe na raiz
2. Certifique-se de que o arquivo está salvo
3. Reinicie o VS Code
4. Confirme autenticação do Copilot

## Skills Não Funcionam

**Sintomas**: Agente não executa tarefas específicas.

**Soluções**:
1. Revise instructions: Skills devem estar bem definidas
2. Forneça mais contexto no prompt
3. Teste com exemplos simples primeiro

## Erros de Contexto

**Sintomas**: Sugestões irrelevantes.

**Soluções**:
1. Abra arquivos relevantes no editor
2. Use prompts específicos com nomes de arquivos
3. Limite o escopo da tarefa

## Problemas de Performance

**Sintomas**: Respostas lentas ou truncadas.

**Soluções**:
1. Reduza tamanho do contexto
2. Divida tarefas grandes em menores
3. Verifique conexão com GitHub

## Quando Reportar

Para bugs persistentes, abra uma issue com:
- Logs do VS Code (Help > Toggle Developer Tools)
- Versão do Copilot
- Exemplo de prompt problemático

Para mais ajuda, consulte [FAQ](../guides/faq.md).