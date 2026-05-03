# Referência arquitetural — Django por apps

## Estrutura sugerida

```text
project_name/
  settings.py
  urls.py
apps/
  catalog/
    models.py
    views.py
    urls.py
    services.py      # opcional: regra que não cabe no model
    api/
      serializers.py
  orders/
    models.py
    ...
tests/
  catalog/
  orders/
```

## Regras entre apps

- Dependência preferencial: **app A** pode importar **API pública** de **app B** (ex.: `services` expostos), não internals frágeis de `models` de B em todo lugar.
- Foreign keys entre apps são normais; mantenha relacionamentos documentados.
- Evite import circular: às vezes extrair contrato comum para `apps/common/` ou pacote `core/`.

## Camadas dentro do app

| Área | Papel |
|------|--------|
| `models` | Persistência, `clean()`, constraints |
| `views` / `viewsets` | HTTP, permissões, delegação |
| `serializers` | Validação e representação API |
| `services` | Regra que envolve vários models ou integrações |

## Anti-padrões

- Lógica de negócio massiva em `signals` sem testes.
- Querysets gigantes em templates ou serializers sem otimização.
- `null=True` e `blank=True` em tudo “para facilitar” sem modelo mental de dados.
- Lógica duplicada em `save()` override e serializer sem uma fonte da verdade.
