# Guia de contexto — API em camadas

## Sempre enviar

- Framework (FastAPI ou Flask) e versão aproximada.
- Arquivo de rota e schema de request/response afetados.
- Serviço ou caso de uso chamado.
- Repositório ou acesso a dados envolvido.
- `pyproject.toml` ou `requirements.txt` se mudar dependências.

## Por tipo de tarefa

### Nova feature de endpoint

- Router/blueprint existente similar.
- Serviço de referência com bom padrão.
- Modelos de banco ou migrations relacionadas.

### Bug

- Request que falha (corpo e headers relevantes, sem segredos).
- Stack trace e linha da rota ou do serviço.
- Teste que reproduz.

### Refatoração

- Grafo de imports entre `api`, `services`, `infra`.
- Contratos públicos da API que não podem mudar.

## Evite

- Mandar só `main.py` sem o serviço que implementa a regra.
- Pedir “refatorar tudo” sem um endpoint ou fluxo concreto.
