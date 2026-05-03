# Checklist — API em camadas

- [ ] Handler/rota com poucas linhas e sem regra de negócio pesada?
- [ ] Serviço ou caso de uso testável sem HTTP?
- [ ] Validação de entrada na borda (Pydantic / schema equivalente)?
- [ ] Resposta não expõe acidentalmente modelo interno sensível?
- [ ] Erros mapeados para status e corpo previsíveis?
- [ ] Testes pytest para o serviço e, se crítico, para o fluxo HTTP?
- [ ] Type hints nas funções públicas da camada de aplicação?
