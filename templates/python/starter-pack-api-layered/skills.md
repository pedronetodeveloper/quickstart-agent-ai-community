# Skills prioritárias — API em camadas

1. Modelar schemas Pydantic (ou equivalente) separados de entidades internas.
2. Extrair serviços coesos com uma responsabilidade clara por módulo.
3. Configurar injeção de dependência (FastAPI `Depends`, factory Flask).
4. Organizar testes: unitários em `services/`, testes de API com `TestClient` ou httpx.
5. Tratar exceções de domínio e mapear para status HTTP consistentes.
6. Usar `Annotated` e aliases de tipo para legibilidade (Python 3.9+).
7. Documentar contratos OpenAPI quando usar FastAPI.
8. Evitar N+1 queries: uso consciente de eager loading ou queries explícitas.
