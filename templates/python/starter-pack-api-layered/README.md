# Starter Pack Python — API em camadas (FastAPI / Flask)

Pack para o padrão mais comum em APIs Python: **rotas finas → serviços ou casos de uso → persistência**. Funciona bem com **FastAPI** (Pydantic na borda) ou **Flask** (schemas equivalentes).

## Quando usar

- API REST ou JSON nova ou em evolução.
- Time quer separação clara entre HTTP, regra de negócio e acesso a dados.
- Validação de entrada na camada de interface, não espalhada no domínio.

## O que não é

- Não obriga DDD completo nem hexagonal; é o “pão com manteiga” de APIs Python maduras.
