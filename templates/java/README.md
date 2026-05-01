# Java Templates Index

Este diretorio centraliza templates e starter packs de arquitetura para projetos Java backend.
Os conceitos aqui sao framework-agnosticos. Spring pode ser usado como detalhe de adaptador/infraestrutura.

## Template base

- `agent-instructions.md`: template inicial para agente Java com foco em arquitetura e qualidade.

## Starter packs

### 1) MVC + SOLID + DDD

- Caminho: `starter-pack-mvc-solid-ddd/`
- Melhor quando:
  - aplicacao web em camadas classicas;
  - fluxo de negocio relativamente linear;
  - time quer onboarding rapido com boas praticas.
- Observacao: em Java, MVC costuma aparecer com Spring MVC, mas os principios continuam validos sem acoplamento no dominio.

### 2) Hexagonal (Ports and Adapters)

- Caminho: `starter-pack-hexagonal-best-practices/`
- Melhor quando:
  - dominio precisa ficar protegido de framework e infraestrutura;
  - integracoes externas mudam com frequencia;
  - testabilidade de casos de uso e prioridade.

### 3) Modular Monolith

- Caminho: `starter-pack-modular-monolith/`
- Melhor quando:
  - precisa evoluir rapido sem custo operacional de microservices;
  - varios times atuam no mesmo sistema;
  - quer fronteiras claras por modulo de negocio.

### 4) EDA + CQRS

- Caminho: `starter-pack-eda-cqrs/`
- Melhor quando:
  - eventos e assincronia sao centrais no negocio;
  - leitura e escrita tem necessidades diferentes;
  - escalabilidade e resiliencia sao requisitos chave.

## Estrutura sugerida para cada starter pack

- `README.md`: contexto e quando usar
- `instructions.md`: comportamento do agente
- `architecture.md`: regras arquiteturais e anti-padroes
