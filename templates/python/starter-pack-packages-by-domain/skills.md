# Skills prioritárias — Pacotes por domínio

1. Refatorar árvore de pacotes sem quebrar imports públicos documentados.
2. Introduzir `Protocol` ou ABC para contratos entre domínios sem acoplamento concreto.
3. Configurar `pyproject.toml` com pacotes, extras e entry points (`[project.scripts]`).
4. Espelhar testes em `tests/` alinhados aos pacotes de `src/`.
5. Detectar e quebrar ciclos de import com extração para `shared/` ou inversão de dependência.
6. Publicar wheel/sdist com metadados corretos e versão semântica.
7. Usar `python -m` ou console scripts para CLIs em vez de scripts soltos na raiz.
