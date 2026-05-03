# Prompt pack — Django apps

## Nova feature em app existente

```text
Implemente <DESCRIÇÃO> no app Django `<nome_app>`. Siga models → services (se preciso) → views/viewsets → urls → testes. Não crie acoplamento desnecessário com outros apps.
```

## Revisão de fronteiras entre apps

```text
Analise imports entre apps neste projeto Django. Aponte violações de fronteira, ciclos e sugestão de extração (common/core ou API pública).
```

## Otimização de queryset

```text
Esta listagem está lenta. Revise view/queryset/serializer e sugira prefetch, select_related ou annotate sem alterar o contrato da API.
```
