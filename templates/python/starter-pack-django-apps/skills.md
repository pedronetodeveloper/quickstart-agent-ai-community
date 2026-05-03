# Skills prioritárias — Django apps

1. Particionar features novas no app correto ou criar app novo com nome de domínio.
2. Modelar models com índices e constraints alinhados a consultas reais.
3. Usar DRF serializers, permissions e throttling de forma consistente.
4. Extrair serviços quando views ou serializers passam de ~30–40 linhas de regra.
5. Escrever testes de integração com banco (pytest-django ou TestCase).
6. Gerenciar migrations com planejamento de dados existentes.
7. Configurar `AppConfig.ready` apenas quando necessário e testável.
8. Isolar queries N+1 em listagens com `annotate` / `prefetch_related`.
