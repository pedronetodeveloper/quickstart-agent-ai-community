# Project-aware Agent

Este template cria um agente voltado para entender o projeto ao qual ele é anexado e gerar skills específicas para otimizar o uso de IA nesse contexto.

## Objetivo

O agente deve:
- ler o projeto inteiro disponível no contexto;
- identificar arquitetura, linguagem, dependências e padrões existentes;
- descobrir necessidades reais do projeto;
- criar vários arquivos de skills separados e focados em otimização, refatoração, testes, documentação e qualidade.

## Conteúdo deste template

- `agent-instructions.md`: instruções para o agente agir como um analista de projeto e construtor de skills.
- `skills/`: pasta com arquivos de exemplo que mostram o formato e as categorias de skills esperadas.
  - `skills/analysis.json`: exemplo de skills para análise de arquitetura, dependências e contexto.
  - `skills/refactor.json`: exemplo de skills para refatoração e melhoria de código.
  - `skills/testing.json`: exemplo de skills para geração e melhoria de testes.
  - `skills/documentation.json`: exemplo de skills para documentação e explicação de decisões.
  - `skills/quality.json`: exemplo de skills para qualidade, CI/CD e manutenção.
