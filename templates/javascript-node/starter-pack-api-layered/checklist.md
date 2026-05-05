# Checklist — API em camadas

- [ ] Handler/route apenas faz parsing, validação e delegação.
- [ ] Serviço/use-case contém regra de negócio e é testável.
- [ ] Validação de entrada com Zod ou equivalente.
- [ ] Dependências externas isoladas em `repositories/` ou `adapters/`.
- [ ] Erros de domínio mapeados para respostas HTTP consistentes.
- [ ] Async/await usado corretamente e promessas tratadas.
- [ ] Cobertura mínima de testes para fluxo crítico.
