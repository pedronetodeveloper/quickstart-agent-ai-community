# Starter Pack JavaScript Node — API em camadas

Pack para o padrão mais comum em Node.js: **handlers finos → serviços/casos de uso → persistência e infra**. Ideal para Express, Fastify, Koa e outros frameworks HTTP.

## Quando usar

- API REST ou HTTP nova ou em evolução.
- Time quer separação clara entre rota, regra de negócio e acesso a dados.
- Validação de entrada na borda com Zod ou validação equivalente.

## O que não é

- Não exige microservices distribuídos nem DDD completo; é um modelo pragmático para APIs mantíveis.
- Não é projeto sem camadas, onde todo o negócio vive nas rotas.
