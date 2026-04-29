# Exemplos Práticos

Veja como agentes Copilot podem ajudar em cenários reais.

## Exemplo 1: Refatoração em Angular

**Cenário**: Migrar componente para Signals.

**Prompt**: "Refatore este componente para usar Signals do Angular 17."

**Antes**:
```typescript
@Component({...})
export class MyComponent {
  data$ = this.service.getData();
}
```

**Depois** (gerado pelo agente):
```typescript
@Component({...})
export class MyComponent {
  data = signal(this.service.getData());
}
```

**Lições**: Agente aplicou skills de Angular, focando em Signals.

## Exemplo 2: Testes em Spring Boot

**Cenário**: Gerar testes para controller.

**Prompt**: "Crie testes JUnit 5 para este controller."

**Resultado**: Agente gerou classe de teste completa com mocks.

**Lições**: Usou skills de Spring e JUnit, seguindo melhores práticas.

## Exemplo 3: Validação em Node.js

**Cenário**: Adicionar validação com Zod.

**Prompt**: "Valide entrada da API com Zod."

**Resultado**: Schema Zod gerado automaticamente.

**Lições**: Agente priorizou async/await e validação.

## Dicas para Usar Exemplos

- Adapte prompts para seu contexto
- Forneça código existente no prompt
- Teste iterativamente

Para mais, explore [Templates](../templates/).