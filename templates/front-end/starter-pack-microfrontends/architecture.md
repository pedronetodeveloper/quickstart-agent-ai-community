# Arquitetura — Microfrontends

- `shell/`: aplicação principal que orquestra microfrontends.
- `microfrontends/<domain>/`: cada domínio em pasta isolada.
- `shared/`: código compartilhado via federated modules.

## Princípios

- Cada microfrontend é independente e deployável separadamente.
- Comunicação via eventos customizados ou APIs.
- Versionamento semântico para compatibilidade.

## Anti-padrões

- Acoplamento direto entre microfrontends.
- Estado compartilhado global sem controle.
- Deploy sincronizado de todos os microfrontends.