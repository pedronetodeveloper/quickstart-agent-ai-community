# Repositório Copilot Agents Quickstart

Bem-vindo ao Repositório Copilot Agents Quickstart! Este projeto foi desenvolvido para ajudar novos usuários a começarem com agentes de IA e fornecer recursos para desenvolver skills e contribuir para a comunidade.

## Índice

- [Introdução](#introdução)
- [Entendendo Instructions, Skills e Context](#entendendo-instructions-skills-e-context)
- [Primeiros Passos](#primeiros-passos)
- [Skills](#skills)
- [Instruções](#instruções)
- [Contribuição](#contribuição)
- [Guias](#guias)
- [Templates](#templates)
- [Licença](#licença)

## Introdução

Este repositório serve como um recurso abrangente para indivíduos interessados em trabalhar com agentes de IA. Ele inclui documentação, guias e templates para facilitar o aprendizado e desenvolvimento, com foco em agentes personalizados para o GitHub Copilot.

## Entendendo Instructions, Skills e Context

Para otimizar o uso do GitHub Copilot e agentes de IA, é fundamental compreender três conceitos-chave que definem como o assistente se comporta e opera:

### Instructions (Instruções)
As **Instructions** definem o "comportamento" e "estilo de escrita" do agente. Elas estabelecem a persona do assistente, suas regras de conduta, workflow de trabalho e guia de estilo. Por exemplo, uma instrução pode especificar que o agente deve sempre priorizar código assíncrono em Node.js ou usar Records em Java para melhor performance. Isso garante respostas consistentes e alinhadas com melhores práticas, promovendo alta eficiência no desenvolvimento brasileiro e comunitário.

### Skills (Habilidades)
As **Skills** representam as capacidades técnicas e ferramentas que o agente domina. Elas incluem conhecimentos específicos como gerar mappers de entidade para DTO em Spring Boot, validar dados com Zod em JavaScript ou refatorar componentes para Signals em Angular. As skills permitem que o agente execute tarefas complexas, como criar testes automatizados ou otimizar queries, focando em soluções de alta performance e compartilhamento de conhecimento na comunidade.

### Context (Contexto)
O **Context** refere-se a como fornecer os arquivos certos para o agente não se perder. Inclui a leitura de arquivos locais relevantes, como configurações de projeto (tsconfig.json, package.json) ou código existente, para dar respostas mais precisas e contextualizadas. Fornecer o contexto adequado evita sugestões genéricas, permitindo que o agente entenda a arquitetura do projeto e sugira melhorias alinhadas com o ecossistema brasileiro de desenvolvimento.

Esses três elementos trabalham juntos para transformar o Copilot em um parceiro técnico especializado, capaz de acelerar o desenvolvimento com foco em qualidade e performance.

## Primeiros Passos

Para começar com os agentes do Copilot, consulte o guia [Primeiros Passos](docs/getting-started.md), que fornece instruções de configuração e passos iniciais.

## Skills

Explore várias skills que podem ser desenvolvidas ou utilizadas com os agentes do Copilot na documentação [Skills](docs/skills.md). Esta seção inclui descrições e exemplos para ajudar a entender as capacidades dos agentes.

## Instruções

Para instruções detalhadas sobre como usar os agentes do Copilot, incluindo comandos, configurações e melhores práticas, consulte o arquivo [Instruções](docs/instructions.md).

## Contribuição

Aceitamos contribuições da comunidade! Se você estiver interessado em contribuir, leia as diretrizes [Contribuição](docs/contributing.md) para informações sobre como enviar issues, pull requests e aderir aos padrões de codificação.

## Guias

Para informações mais aprofundadas, consulte os seguintes guias:
- [Guia do Agente Copilot](guides/ai-agent.md): Visão geral abrangente dos recursos e capacidades dos agentes.
- [Guia de Workflow](guides/workflow.md): Passos detalhados e processos para usar os agentes.
- [FAQ](guides/faq.md): Respostas para perguntas frequentes sobre os agentes.

## Templates

Explore os templates de instruções para agentes especializados em diferentes tecnologias. Estes templates servem como base para criar agentes personalizados no GitHub Copilot, focando em melhores práticas de arquitetura e Clean Code:

- [Java](templates/java/agent-instructions.md): Focado em arquitetura Java com SOLID e DDD, mantendo framework como detalhe técnico.
- [JavaScript Node — índice e starter packs](templates/javascript-node/README.md): APIs em camadas, pacotes por domínio, serverless e workers.
- [Python — índice e starter packs](templates/python/README.md): API em camadas, Django por apps, pacotes por domínio e workers com filas.
- [Front-end — índice e starter packs](templates/frontend/README.md): Microfrontends, SPA component-driven, design systems e Jamstack.
- [Angular](templates/angular/agent-instructions.md): Especializado em Angular 17+ com Signals, Standalone Components e RXJS.

### Formatos Alternativos

Para maior flexibilidade, oferecemos templates em formatos alternativos:
- [Skills em JSON](templates/alternatives/skills.json): Estrutura clara para parsing e reutilização.
- [Skills em YAML](templates/alternatives/skills.yaml): Legível e conciso para manutenção manual.
- [Instructions em XML](templates/alternatives/instructions.xml): Validação rigorosa com schemas para instructions complexas.