# Guia de contexto — Django apps

## Sempre enviar

- `INSTALLED_APPS` ou lista de apps tocados.
- Models, migrations, views/viewsets e serializers envolvidos.
- `urls.py` que monta a rota.
- Trecho de settings se envolver middleware, cache ou DB router.

## Por tipo de tarefa

### Nova feature

- App dono e modelo relacionado.
- Wireframe de URL e método HTTP.
- Permissões esperadas (grupo, staff, objeto).

### Bug

- Traceback Django completo.
- Query problemática (SQL debug se possível).
- Teste que falha ou passos no admin/shell.

### Refatoração entre apps

- Mapa de quem importa quem hoje.
- Contrato desejado após a mudança.

## Evite

- Colar só `models.py` sem a view ou serializer que dispara o bug.
- Pedir mudança em `User` sem dizer se usa `AbstractUser` ou modelo custom.
