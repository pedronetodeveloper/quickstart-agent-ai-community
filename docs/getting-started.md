# Primeiros Passos com Agentes Copilot

Este guia fornece instruções passo a passo para começar a usar agentes de IA no GitHub Copilot, desde a configuração inicial até o primeiro uso prático.

## Pré-requisitos

- Conta GitHub ativa
- VS Code instalado
- Extensão GitHub Copilot instalada

## Passos para Configuração

1. **Instale a Extensão Copilot**:
   - Abra o VS Code
   - Vá para Extensions (Ctrl+Shift+X)
   - Procure por "GitHub Copilot" e instale

2. **Autentique sua Conta**:
   - Após instalação, clique em "Sign in" na notificação
   - Autorize o acesso ao GitHub

3. **Configure um Agente Básico**:
   - Crie um arquivo `.instructions.md` na raiz do projeto
   - Defina persona e regras básicas

## Primeiro Uso

Use um template existente para testar:
- Copie um template de `templates/` (ex.: `python/README.md` para escolher um starter pack, ou `python-fastapi/agent-instructions.md` para FastAPI direto)
- Adapte para seu projeto
- Teste com um prompt simples no chat do Copilot

## Troubleshooting Básico

- Se o agente não responder: Verifique se o arquivo `.instructions.md` está na raiz
- Problemas de autenticação: Reautentique no VS Code

Para mais detalhes, consulte [Guia do Agente Copilot](../guides/ai-agent.md).